# Comparing `tmp/prowler-3.7.0.tar.gz` & `tmp/prowler-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prowler-3.7.0.tar", max compression
+gzip compressed data, was "prowler-3.7.1.tar", max compression
```

## Comparing `prowler-3.7.0.tar` & `prowler-3.7.1.tar`

### file list

```diff
@@ -1,1463 +1,1466 @@
--rw-r--r--   0        0        0    11339 2023-07-06 15:19:30.298255 prowler-3.7.0/LICENSE
--rw-r--r--   0        0        0    13569 2023-07-06 15:19:30.298255 prowler-3.7.0/README.md
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.326255 prowler-3.7.0/prowler/__init__.py
--rw-r--r--   0        0        0     8955 2023-07-06 15:19:30.326255 prowler-3.7.0/prowler/__main__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.326255 prowler-3.7.0/prowler/compliance/aws/__init__.py
--rw-r--r--   0        0        0     6516 2023-07-06 15:19:30.326255 prowler-3.7.0/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json
--rw-r--r--   0        0        0    17475 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json
--rw-r--r--   0        0        0     4834 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/aws_well_architected_framework_reliability_pillar_aws.json
--rw-r--r--   0        0        0   165349 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/aws_well_architected_framework_security_pillar_aws.json
--rw-r--r--   0        0        0   260398 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/cis_1.4_aws.json
--rw-r--r--   0        0        0   287275 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/cis_1.5_aws.json
--rw-r--r--   0        0        0    15458 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/cisa_aws.json
--rw-r--r--   0        0        0   142312 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/ens_rd2022_aws.json
--rw-r--r--   0        0        0    18551 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/fedramp_low_revision_4_aws.json
--rw-r--r--   0        0        0    57257 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json
--rw-r--r--   0        0        0    31059 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/ffiec_aws.json
--rw-r--r--   0        0        0    10166 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/gdpr_aws.json
--rw-r--r--   0        0        0    18763 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json
--rw-r--r--   0        0        0    11774 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/gxp_eu_annex_11_aws.json
--rw-r--r--   0        0        0    31000 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/hipaa_aws.json
--rw-r--r--   0        0        0    41885 2023-07-06 15:19:30.330255 prowler-3.7.0/prowler/compliance/aws/iso27001_2013_aws.json
--rw-r--r--   0        0        0   132178 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/aws/mitre_attack_aws.json
--rw-r--r--   0        0        0    86208 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/aws/nist_800_171_revision_2_aws.json
--rw-r--r--   0        0        0    50559 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/aws/nist_800_53_revision_4_aws.json
--rw-r--r--   0        0        0   243911 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/aws/nist_800_53_revision_5_aws.json
--rw-r--r--   0        0        0    40042 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/aws/nist_csf_1.1_aws.json
--rw-r--r--   0        0        0     8722 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/aws/pci_3.2.1_aws.json
--rw-r--r--   0        0        0     8563 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/aws/rbi_cyber_security_framework_aws.json
--rw-r--r--   0        0        0    93913 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/aws/soc2_aws.json
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/azure/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/gcp/__init__.py
--rw-r--r--   0        0        0   385663 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/compliance/gcp/cis_2.0_gcp.json
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/config/__init__.py
--rw-r--r--   0        0        0     3459 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/config/allowlist.yaml
--rw-r--r--   0        0        0      165 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/config/checklist_example.json
--rw-r--r--   0        0        0     3300 2023-07-06 15:19:50.398453 prowler-3.7.0/prowler/config/config.py
--rw-r--r--   0        0        0     1942 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/config/config.yaml
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/lib/__init__.py
--rw-r--r--   0        0        0      854 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/lib/banner.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/lib/check/__init__.py
--rw-r--r--   0        0        0    22996 2023-07-06 15:19:30.334255 prowler-3.7.0/prowler/lib/check/check.py
--rw-r--r--   0        0        0     2973 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/check/checks_loader.py
--rw-r--r--   0        0        0     3864 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/check/compliance.py
--rw-r--r--   0        0        0     5225 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/check/compliance_models.py
--rw-r--r--   0        0        0     3835 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/check/models.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/cli/__init__.py
--rw-r--r--   0        0        0    18411 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/cli/parser.py
--rw-r--r--   0        0        0     1885 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/logger.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/outputs/__init__.py
--rw-r--r--   0        0        0    34169 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/outputs/compliance.py
--rw-r--r--   0        0        0    10181 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/outputs/file_descriptors.py
--rw-r--r--   0        0        0    20435 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/outputs/html.py
--rw-r--r--   0        0        0    12276 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/outputs/json.py
--rw-r--r--   0        0        0    25615 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/outputs/models.py
--rw-r--r--   0        0        0    11105 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/outputs/outputs.py
--rw-r--r--   0        0        0     5015 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/outputs/slack.py
--rw-r--r--   0        0        0     6592 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/outputs/summary_table.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/scan_filters/__init__.py
--rw-r--r--   0        0        0      552 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/scan_filters/scan_filters.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/utils/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/lib/utils/utils.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/__init__.py
--rw-r--r--   0        0        0    13384 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/aws_provider.py
--rw-r--r--   0        0        0   218667 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/aws_regions_by_service.json
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/allowlist/__init__.py
--rw-r--r--   0        0        0    10757 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/allowlist/allowlist.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/arn/__init__.py
--rw-r--r--   0        0        0     1871 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/arn/arn.py
--rw-r--r--   0        0        0     2193 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/arn/error.py
--rw-r--r--   0        0        0     1957 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/arn/models.py
--rw-r--r--   0        0        0     1152 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0     1251 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/credentials/__init__.py
--rw-r--r--   0        0        0     2459 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/credentials/credentials.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/organizations/__init__.py
--rw-r--r--   0        0        0     1657 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/organizations/organizations.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/quick_inventory/__init__.py
--rw-r--r--   0        0        0    15534 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/quick_inventory/quick_inventory.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/resource_api_tagging/__init__.py
--rw-r--r--   0        0        0     1585 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/security_hub/__init__.py
--rw-r--r--   0        0        0     5867 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/lib/security_hub/security_hub.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/__init__.py
--rw-r--r--   0        0        0      244 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/__init__.py
--rw-r--r--   0        0        0     1584 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json
--rw-r--r--   0        0        0     1478 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/__init__.py
--rw-r--r--   0        0        0     1635 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json
--rw-r--r--   0        0        0     2184 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py
--rw-r--r--   0        0        0     5375 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/__init__.py
--rw-r--r--   0        0        0      200 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/__init__.py
--rw-r--r--   0        0        0     1753 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json
--rw-r--r--   0        0        0      717 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/__init__.py
--rw-r--r--   0        0        0     1315 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json
--rw-r--r--   0        0        0      746 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/__init__.py
--rw-r--r--   0        0        0     1674 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json
--rw-r--r--   0        0        0      764 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py
--rw-r--r--   0        0        0      706 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/account/account_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/acm/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/__init__.py
--rw-r--r--   0        0        0     1368 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json
--rw-r--r--   0        0        0     1233 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/__init__.py
--rw-r--r--   0        0        0     1316 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json
--rw-r--r--   0        0        0     1636 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/acm/acm_client.py
--rw-r--r--   0        0        0     4752 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/acm/acm_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/apigateway/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/__init__.py
--rw-r--r--   0        0        0     1133 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json
--rw-r--r--   0        0        0      976 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py
--rw-r--r--   0        0        0      215 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/__init__.py
--rw-r--r--   0        0        0     1250 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json
--rw-r--r--   0        0        0     1126 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.338255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/__init__.py
--rw-r--r--   0        0        0     1087 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json
--rw-r--r--   0        0        0      994 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1676 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1079 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py
--rw-r--r--   0        0        0     5320 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/__init__.py
--rw-r--r--   0        0        0     1181 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json
--rw-r--r--   0        0        0     1093 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1504 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1123 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/__init__.py
--rw-r--r--   0        0        0      995 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json
--rw-r--r--   0        0        0      983 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py
--rw-r--r--   0        0        0      234 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_client.py
--rw-r--r--   0        0        0     4018 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/__init__.py
--rw-r--r--   0        0        0      210 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/__init__.py
--rw-r--r--   0        0        0     1346 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json
--rw-r--r--   0        0        0     1273 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/__init__.py
--rw-r--r--   0        0        0     1257 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json
--rw-r--r--   0        0        0     1408 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/__init__.py
--rw-r--r--   0        0        0     1269 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json
--rw-r--r--   0        0        0     1420 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/__init__.py
--rw-r--r--   0        0        0     1363 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json
--rw-r--r--   0        0        0     1583 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py
--rw-r--r--   0        0        0     3619 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/autoscaling/__init__.py
--rw-r--r--   0        0        0      220 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json
--rw-r--r--   0        0        0     1902 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py
--rw-r--r--   0        0        0       78 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/fixtures/fixture
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/__init__.py
--rw-r--r--   0        0        0     1285 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.metadata.json
--rw-r--r--   0        0        0     1002 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.py
--rw-r--r--   0        0        0     4192 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/__init__.py
--rw-r--r--   0        0        0      204 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1198 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2548 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/__init__.py
--rw-r--r--   0        0        0     1341 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json
--rw-r--r--   0        0        0     3352 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/__init__.py
--rw-r--r--   0        0        0     1536 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json
--rw-r--r--   0        0        0     2209 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1399 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1823 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/__init__.py
--rw-r--r--   0        0        0     1272 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json
--rw-r--r--   0        0        0     1058 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/__init__.py
--rw-r--r--   0        0        0     1120 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json
--rw-r--r--   0        0        0     1144 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/__init__.py
--rw-r--r--   0        0        0     1619 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json
--rw-r--r--   0        0        0     1169 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py
--rw-r--r--   0        0        0     8137 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/__init__.py
--rw-r--r--   0        0        0      195 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_plans_exist/__init__.py
--rw-r--r--   0        0        0     1350 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json
--rw-r--r--   0        0        0      999 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_reportplans_exist/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json
--rw-r--r--   0        0        0     1189 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py
--rw-r--r--   0        0        0     6981 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/__init__.py
--rw-r--r--   0        0        0     1397 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json
--rw-r--r--   0        0        0     1096 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_vaults_exist/__init__.py
--rw-r--r--   0        0        0     1264 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json
--rw-r--r--   0        0        0      976 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudformation/__init__.py
--rw-r--r--   0        0        0      244 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_client.py
--rw-r--r--   0        0        0     4466 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/__init__.py
--rw-r--r--   0        0        0     1367 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json
--rw-r--r--   0        0        0     1992 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/__init__.py
--rw-r--r--   0        0        0     1286 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json
--rw-r--r--   0        0        0     1249 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/__init__.py
--rw-r--r--   0        0        0      215 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1422 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/__init__.py
--rw-r--r--   0        0        0     1311 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json
--rw-r--r--   0        0        0     1164 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/__init__.py
--rw-r--r--   0        0        0     1385 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json
--rw-r--r--   0        0        0     1721 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1491 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1230 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/__init__.py
--rw-r--r--   0        0        0     1375 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json
--rw-r--r--   0        0        0     1781 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/__init__.py
--rw-r--r--   0        0        0     1479 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json
--rw-r--r--   0        0        0     1031 2023-07-06 15:19:30.342255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py
--rw-r--r--   0        0        0     6218 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/__init__.py
--rw-r--r--   0        0        0     1268 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json
--rw-r--r--   0        0        0     1707 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py
--rw-r--r--   0        0        0      215 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1575 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2245 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/__init__.py
--rw-r--r--   0        0        0     1287 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json
--rw-r--r--   0        0        0     1073 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1951 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1524 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/__init__.py
--rw-r--r--   0        0        0     1315 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json
--rw-r--r--   0        0        0     1457 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1380 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2232 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1393 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2755 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/__init__.py
--rw-r--r--   0        0        0     1730 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json
--rw-r--r--   0        0        0     2004 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/__init__.py
--rw-r--r--   0        0        0     1537 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json
--rw-r--r--   0        0        0     3014 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/__init__.py
--rw-r--r--   0        0        0     1565 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json
--rw-r--r--   0        0        0     3016 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py
--rw-r--r--   0        0        0     9527 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1496 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2519 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1462 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2525 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1450 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2543 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1418 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2728 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py
--rw-r--r--   0        0        0      215 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/__init__.py
--rw-r--r--   0        0        0     1179 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json
--rw-r--r--   0        0        0      922 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1249 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1002 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/__init__.py
--rw-r--r--   0        0        0     1345 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json
--rw-r--r--   0        0        0     5022 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json
--rw-r--r--   0        0        0     1569 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1498 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2519 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1498 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2465 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/__init__.py
--rw-r--r--   0        0        0     1495 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json
--rw-r--r--   0        0        0     2336 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/__init__.py
--rw-r--r--   0        0        0     1453 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json
--rw-r--r--   0        0        0     3174 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/__init__.py
--rw-r--r--   0        0        0     1560 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json
--rw-r--r--   0        0        0     2389 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/__init__.py
--rw-r--r--   0        0        0     1456 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json
--rw-r--r--   0        0        0     2671 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/__init__.py
--rw-r--r--   0        0        0     1430 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json
--rw-r--r--   0        0        0     2876 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/__init__.py
--rw-r--r--   0        0        0     1432 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json
--rw-r--r--   0        0        0     2356 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/__init__.py
--rw-r--r--   0        0        0     1448 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json
--rw-r--r--   0        0        0     2541 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/__init__.py
--rw-r--r--   0        0        0     1475 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json
--rw-r--r--   0        0        0     2331 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/__init__.py
--rw-r--r--   0        0        0     1446 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json
--rw-r--r--   0        0        0     2336 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py
--rw-r--r--   0        0        0    11386 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py
--rw-r--r--   0        0        0      197 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/cloudwatch/logs_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codeartifact/__init__.py
--rw-r--r--   0        0        0      234 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/__init__.py
--rw-r--r--   0        0        0     1540 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json
--rw-r--r--   0        0        0     1665 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py
--rw-r--r--   0        0        0    10588 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codebuild/__init__.py
--rw-r--r--   0        0        0      210 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/__init__.py
--rw-r--r--   0        0        0     1053 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json
--rw-r--r--   0        0        0     1250 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/__init__.py
--rw-r--r--   0        0        0     1018 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json
--rw-r--r--   0        0        0     1060 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py
--rw-r--r--   0        0        0     3858 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/config/__init__.py
--rw-r--r--   0        0        0      195 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/config/config_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/__init__.py
--rw-r--r--   0        0        0     1326 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json
--rw-r--r--   0        0        0     1682 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py
--rw-r--r--   0        0        0     3295 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/config/config_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/__init__.py
--rw-r--r--   0        0        0      254 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.346255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/__init__.py
--rw-r--r--   0        0        0     1191 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json
--rw-r--r--   0        0        0      997 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/__init__.py
--rw-r--r--   0        0        0     1187 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json
--rw-r--r--   0        0        0     1041 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/__init__.py
--rw-r--r--   0        0        0     1042 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json
--rw-r--r--   0        0        0     1872 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/__init__.py
--rw-r--r--   0        0        0     1098 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json
--rw-r--r--   0        0        0     1660 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/__init__.py
--rw-r--r--   0        0        0     1533 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json
--rw-r--r--   0        0        0     1373 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py
--rw-r--r--   0        0        0    13316 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/__init__.py
--rw-r--r--   0        0        0     1265 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json
--rw-r--r--   0        0        0     1269 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/drs/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/drs/drs_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/drs/drs_job_exist/__init__.py
--rw-r--r--   0        0        0      888 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json
--rw-r--r--   0        0        0      967 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py
--rw-r--r--   0        0        0     3504 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/drs/drs_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/__init__.py
--rw-r--r--   0        0        0      190 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dax_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1594 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      957 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py
--rw-r--r--   0        0        0      205 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_client.py
--rw-r--r--   0        0        0     8906 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1497 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      988 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/__init__.py
--rw-r--r--   0        0        0     1529 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json
--rw-r--r--   0        0        0      933 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ami_public/__init__.py
--rw-r--r--   0        0        0     1299 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json
--rw-r--r--   0        0        0      843 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/__init__.py
--rw-r--r--   0        0        0     1192 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json
--rw-r--r--   0        0        0      850 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/__init__.py
--rw-r--r--   0        0        0     1176 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json
--rw-r--r--   0        0        0      965 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/__init__.py
--rw-r--r--   0        0        0     1530 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json
--rw-r--r--   0        0        0      922 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/__init__.py
--rw-r--r--   0        0        0     1239 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json
--rw-r--r--   0        0        0      849 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/__init__.py
--rw-r--r--   0        0        0     1057 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json
--rw-r--r--   0        0        0     2037 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/__init__.py
--rw-r--r--   0        0        0     1107 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json
--rw-r--r--   0        0        0      971 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/__init__.py
--rw-r--r--   0        0        0     1461 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json
--rw-r--r--   0        0        0     1179 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/__init__.py
--rw-r--r--   0        0        0     1067 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json
--rw-r--r--   0        0        0     1111 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/__init__.py
--rw-r--r--   0        0        0     1174 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json
--rw-r--r--   0        0        0     1253 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/__init__.py
--rw-r--r--   0        0        0     1201 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json
--rw-r--r--   0        0        0     1491 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/__init__.py
--rw-r--r--   0        0        0     1543 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json
--rw-r--r--   0        0        0     1034 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json
--rw-r--r--   0        0        0     1118 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/__init__.py
--rw-r--r--   0        0        0     1292 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json
--rw-r--r--   0        0        0     2348 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py
--rw-r--r--   0        0        0       78 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/fixtures/fixture
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/__init__.py
--rw-r--r--   0        0        0     1378 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json
--rw-r--r--   0        0        0     1247 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json
--rw-r--r--   0        0        0     1268 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/__init__.py
--rw-r--r--   0        0        0     1513 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json
--rw-r--r--   0        0        0     1296 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/__init__.py
--rw-r--r--   0        0        0     1139 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json
--rw-r--r--   0        0        0     1028 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/__init__.py
--rw-r--r--   0        0        0     1197 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json
--rw-r--r--   0        0        0     1548 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/__init__.py
--rw-r--r--   0        0        0     1169 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json
--rw-r--r--   0        0        0     1516 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/__init__.py
--rw-r--r--   0        0        0     1429 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json
--rw-r--r--   0        0        0     1489 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/__init__.py
--rw-r--r--   0        0        0     1371 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json
--rw-r--r--   0        0        0     1517 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/__init__.py
--rw-r--r--   0        0        0     1220 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json
--rw-r--r--   0        0        0     1577 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/__init__.py
--rw-r--r--   0        0        0     1211 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json
--rw-r--r--   0        0        0     1612 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/__init__.py
--rw-r--r--   0        0        0     1164 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json
--rw-r--r--   0        0        0     1507 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/__init__.py
--rw-r--r--   0        0        0     1179 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json
--rw-r--r--   0        0        0     1523 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/__init__.py
--rw-r--r--   0        0        0     1165 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json
--rw-r--r--   0        0        0     1570 2023-07-06 15:19:30.350255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/__init__.py
--rw-r--r--   0        0        0     1190 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json
--rw-r--r--   0        0        0     1541 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/__init__.py
--rw-r--r--   0        0        0     1173 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json
--rw-r--r--   0        0        0     1516 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/__init__.py
--rw-r--r--   0        0        0     1164 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json
--rw-r--r--   0        0        0     1507 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/__init__.py
--rw-r--r--   0        0        0     1218 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json
--rw-r--r--   0        0        0     1579 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/__init__.py
--rw-r--r--   0        0        0     1161 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json
--rw-r--r--   0        0        0     1502 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/__init__.py
--rw-r--r--   0        0        0     1127 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json
--rw-r--r--   0        0        0     2440 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/__init__.py
--rw-r--r--   0        0        0     1374 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json
--rw-r--r--   0        0        0     1305 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/__init__.py
--rw-r--r--   0        0        0     1221 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json
--rw-r--r--   0        0        0     1029 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/__init__.py
--rw-r--r--   0        0        0     1043 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json
--rw-r--r--   0        0        0     1144 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/__init__.py
--rw-r--r--   0        0        0     1080 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json
--rw-r--r--   0        0        0     1219 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py
--rw-r--r--   0        0        0    21389 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/lib/__init__.py
--rw-r--r--   0        0        0     2581 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/lib/network_acls.py
--rw-r--r--   0        0        0     3966 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ec2/lib/security_groups.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/__init__.py
--rw-r--r--   0        0        0     1375 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json
--rw-r--r--   0        0        0     1568 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/__init__.py
--rw-r--r--   0        0        0     1123 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json
--rw-r--r--   0        0        0     1030 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1213 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1506 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json
--rw-r--r--   0        0        0     1108 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/__init__.py
--rw-r--r--   0        0        0     1268 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json
--rw-r--r--   0        0        0     2377 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py
--rw-r--r--   0        0        0    13675 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecs/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecs/ecs_client.py
--rw-r--r--   0        0        0     3857 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecs/ecs_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/__init__.py
--rw-r--r--   0        0        0     1625 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json
--rw-r--r--   0        0        0     2328 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1366 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0      857 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/__init__.py
--rw-r--r--   0        0        0     1099 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json
--rw-r--r--   0        0        0      847 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0      981 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1861 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py
--rw-r--r--   0        0        0     4240 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/efs/efs_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/__init__.py
--rw-r--r--   0        0        0     1362 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json
--rw-r--r--   0        0        0      992 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/__init__.py
--rw-r--r--   0        0        0     1559 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json
--rw-r--r--   0        0        0     1215 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/__init__.py
--rw-r--r--   0        0        0     1374 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json
--rw-r--r--   0        0        0     1489 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1533 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1020 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py
--rw-r--r--   0        0        0     4792 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/eks/eks_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/__init__.py
--rw-r--r--   0        0        0     1364 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json
--rw-r--r--   0        0        0     1115 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_internet_facing/__init__.py
--rw-r--r--   0        0        0     1111 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json
--rw-r--r--   0        0        0      823 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1392 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json
--rw-r--r--   0        0        0      817 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py
--rw-r--r--   0        0        0     4592 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_ssl_listeners/__init__.py
--rw-r--r--   0        0        0     1360 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json
--rw-r--r--   0        0        0      937 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/__init__.py
--rw-r--r--   0        0        0      190 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/__init__.py
--rw-r--r--   0        0        0     1347 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json
--rw-r--r--   0        0        0      892 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/__init__.py
--rw-r--r--   0        0        0     1718 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json
--rw-r--r--   0        0        0     1367 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/__init__.py
--rw-r--r--   0        0        0     1337 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json
--rw-r--r--   0        0        0     1646 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/__init__.py
--rw-r--r--   0        0        0     1162 2023-07-06 15:19:30.354255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json
--rw-r--r--   0        0        0      888 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/__init__.py
--rw-r--r--   0        0        0      996 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json
--rw-r--r--   0        0        0      836 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1435 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json
--rw-r--r--   0        0        0      924 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py
--rw-r--r--   0        0        0     7882 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/__init__.py
--rw-r--r--   0        0        0     1325 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json
--rw-r--r--   0        0        0     1664 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/__init__.py
--rw-r--r--   0        0        0     1004 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json
--rw-r--r--   0        0        0     1439 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/__init__.py
--rw-r--r--   0        0        0     1029 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json
--rw-r--r--   0        0        0      981 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/__init__.py
--rw-r--r--   0        0        0      897 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json
--rw-r--r--   0        0        0     1200 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/__init__.py
--rw-r--r--   0        0        0     1018 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json
--rw-r--r--   0        0        0     4444 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py
--rw-r--r--   0        0        0     8372 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/emr/emr_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/fms/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/fms/fms_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/fms/fms_policy_compliant/__init__.py
--rw-r--r--   0        0        0     1085 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.metadata.json
--rw-r--r--   0        0        0     1328 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.py
--rw-r--r--   0        0        0     4604 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/fms/fms_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glacier/__init__.py
--rw-r--r--   0        0        0      200 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glacier/glacier_client.py
--rw-r--r--   0        0        0     4080 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glacier/glacier_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/__init__.py
--rw-r--r--   0        0        0     1219 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json
--rw-r--r--   0        0        0     1940 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/globalaccelerator/__init__.py
--rw-r--r--   0        0        0      259 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_client.py
--rw-r--r--   0        0        0     2455 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/__init__.py
--rw-r--r--   0        0        0      185 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1464 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      994 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1539 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      986 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/__init__.py
--rw-r--r--   0        0        0     1222 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json
--rw-r--r--   0        0        0      927 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1632 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1408 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1623 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1399 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1644 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1369 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1574 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1664 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1600 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1335 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1591 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1326 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py
--rw-r--r--   0        0        0    10529 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/glue/glue_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/__init__.py
--rw-r--r--   0        0        0      998 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json
--rw-r--r--   0        0        0     1221 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py
--rw-r--r--   0        0        0      210 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/__init__.py
--rw-r--r--   0        0        0     1282 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json
--rw-r--r--   0        0        0     1130 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/__init__.py
--rw-r--r--   0        0        0     1179 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json
--rw-r--r--   0        0        0      961 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py
--rw-r--r--   0        0        0     7243 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/__init__.py
--rw-r--r--   0        0        0     1010 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json
--rw-r--r--   0        0        0     1933 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/__init__.py
--rw-r--r--   0        0        0     1112 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json
--rw-r--r--   0        0        0     2805 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2073 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2227 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/__init__.py
--rw-r--r--   0        0        0     1494 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json
--rw-r--r--   0        0        0      802 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2088 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2238 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2118 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2251 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/__init__.py
--rw-r--r--   0        0        0     1413 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json
--rw-r--r--   0        0        0     4192 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/__init__.py
--rw-r--r--   0        0        0     1413 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json
--rw-r--r--   0        0        0     4146 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/__init__.py
--rw-r--r--   0        0        0     1417 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json
--rw-r--r--   0        0        0     4192 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/__init__.py
--rw-r--r--   0        0        0     1089 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json
--rw-r--r--   0        0        0     2665 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/__init__.py
--rw-r--r--   0        0        0     1707 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json
--rw-r--r--   0        0        0     1090 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_root_access_key/__init__.py
--rw-r--r--   0        0        0     1453 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json
--rw-r--r--   0        0        0     1541 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-06 15:19:30.358255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json
--rw-r--r--   0        0        0     1414 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/__init__.py
--rw-r--r--   0        0        0     1299 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json
--rw-r--r--   0        0        0     1140 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/__init__.py
--rw-r--r--   0        0        0     1299 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json
--rw-r--r--   0        0        0     1239 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_number/__init__.py
--rw-r--r--   0        0        0     1254 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json
--rw-r--r--   0        0        0     1149 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/__init__.py
--rw-r--r--   0        0        0     1280 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json
--rw-r--r--   0        0        0     1285 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/__init__.py
--rw-r--r--   0        0        0     1294 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json
--rw-r--r--   0        0        0     1149 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/__init__.py
--rw-r--r--   0        0        0     1300 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json
--rw-r--r--   0        0        0     1137 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/__init__.py
--rw-r--r--   0        0        0     1223 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json
--rw-r--r--   0        0        0     6229 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/__init__.py
--rw-r--r--   0        0        0     1533 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json
--rw-r--r--   0        0        0     1925 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/__init__.py
--rw-r--r--   0        0        0     1384 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json
--rw-r--r--   0        0        0     1967 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/__init__.py
--rw-r--r--   0        0        0     1356 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json
--rw-r--r--   0        0        0     1954 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/__init__.py
--rw-r--r--   0        0        0     1539 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.metadata.json
--rw-r--r--   0        0        0     4380 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/__init__.py
--rw-r--r--   0        0        0     1172 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json
--rw-r--r--   0        0        0     4097 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1424 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1586 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1738 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1020 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/__init__.py
--rw-r--r--   0        0        0     1424 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json
--rw-r--r--   0        0        0     2832 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/__init__.py
--rw-r--r--   0        0        0     1335 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json
--rw-r--r--   0        0        0      901 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py
--rw-r--r--   0        0        0    23893 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_support_role_created/__init__.py
--rw-r--r--   0        0        0     1256 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json
--rw-r--r--   0        0        0      940 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1061 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1341 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json
--rw-r--r--   0        0        0     1698 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/__init__.py
--rw-r--r--   0        0        0     1671 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json
--rw-r--r--   0        0        0     2671 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/__init__.py
--rw-r--r--   0        0        0      998 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json
--rw-r--r--   0        0        0     1341 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/inspector2/__init__.py
--rw-r--r--   0        0        0      215 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/inspector2/inspector2_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/__init__.py
--rw-r--r--   0        0        0     1158 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json
--rw-r--r--   0        0        0     1498 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py
--rw-r--r--   0        0        0     4084 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/inspector2/inspector2_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_cmk_are_used/__init__.py
--rw-r--r--   0        0        0     1053 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json
--rw-r--r--   0        0        0     1194 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1294 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1354 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2525 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
--rw-r--r--   0        0        0     5417 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/kms/kms_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/macie/__init__.py
--rw-r--r--   0        0        0      190 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/macie/macie_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/macie/macie_is_enabled/__init__.py
--rw-r--r--   0        0        0     1065 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json
--rw-r--r--   0        0        0      982 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py
--rw-r--r--   0        0        0     1913 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/macie/macie_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/networkfirewall/__init__.py
--rw-r--r--   0        0        0      249 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/__init__.py
--rw-r--r--   0        0        0     1299 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.metadata.json
--rw-r--r--   0        0        0     1143 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.py
--rw-r--r--   0        0        0     3581 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/__init__.py
--rw-r--r--   0        0        0      238 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_client.py
--rw-r--r--   0        0        0     7580 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1124 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1102 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1478 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1871 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1555 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0     1003 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/__init__.py
--rw-r--r--   0        0        0     1281 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json
--rw-r--r--   0        0        0      991 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/__init__.py
--rw-r--r--   0        0        0     1128 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json
--rw-r--r--   0        0        0      983 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1766 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1023 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1281 2023-07-06 15:19:30.362255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2655 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/__init__.py
--rw-r--r--   0        0        0     1736 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json
--rw-r--r--   0        0        0     1046 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/__init__.py
--rw-r--r--   0        0        0     1242 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json
--rw-r--r--   0        0        0     1023 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/__init__.py
--rw-r--r--   0        0        0     1359 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json
--rw-r--r--   0        0        0      984 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py
--rw-r--r--   0        0        0      239 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/__init__.py
--rw-r--r--   0        0        0     1579 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json
--rw-r--r--   0        0        0     1816 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/__init__.py
--rw-r--r--   0        0        0     1548 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json
--rw-r--r--   0        0        0     5769 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py
--rw-r--r--   0        0        0     8762 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/__init__.py
--rw-r--r--   0        0        0     1047 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.metadata.json
--rw-r--r--   0        0        0     1432 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/__init__.py
--rw-r--r--   0        0        0     1473 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json
--rw-r--r--   0        0        0     1034 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/__init__.py
--rw-r--r--   0        0        0     1367 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json
--rw-r--r--   0        0        0     1789 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/__init__.py
--rw-r--r--   0        0        0     1111 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.metadata.json
--rw-r--r--   0        0        0     1215 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json
--rw-r--r--   0        0        0     1010 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/__init__.py
--rw-r--r--   0        0        0     1488 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json
--rw-r--r--   0        0        0      997 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/__init__.py
--rw-r--r--   0        0        0     1732 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json
--rw-r--r--   0        0        0     1019 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_multi_az/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json
--rw-r--r--   0        0        0     1730 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/__init__.py
--rw-r--r--   0        0        0     1426 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json
--rw-r--r--   0        0        0     1009 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/__init__.py
--rw-r--r--   0        0        0     1370 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json
--rw-r--r--   0        0        0      942 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/__init__.py
--rw-r--r--   0        0        0     1510 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json
--rw-r--r--   0        0        0     1469 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py
--rw-r--r--   0        0        0    16516 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/__init__.py
--rw-r--r--   0        0        0     1552 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json
--rw-r--r--   0        0        0     1635 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/__init__.py
--rw-r--r--   0        0        0      205 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/__init__.py
--rw-r--r--   0        0        0     1384 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json
--rw-r--r--   0        0        0      973 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/__init__.py
--rw-r--r--   0        0        0     1204 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json
--rw-r--r--   0        0        0      984 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/__init__.py
--rw-r--r--   0        0        0     1285 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json
--rw-r--r--   0        0        0      996 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/__init__.py
--rw-r--r--   0        0        0     1297 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json
--rw-r--r--   0        0        0      992 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py
--rw-r--r--   0        0        0     5144 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/resourceexplorer2/__init__.py
--rw-r--r--   0        0        0      261 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/__init__.py
--rw-r--r--   0        0        0      973 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json
--rw-r--r--   0        0        0     1089 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py
--rw-r--r--   0        0        0     2339 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/__init__.py
--rw-r--r--   0        0        0      200 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/__init__.py
--rw-r--r--   0        0        0     1426 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.metadata.json
--rw-r--r--   0        0        0     2927 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/__init__.py
--rw-r--r--   0        0        0     1188 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json
--rw-r--r--   0        0        0     1023 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/__init__.py
--rw-r--r--   0        0        0      998 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json
--rw-r--r--   0        0        0     1058 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1362 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1303 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0     8575 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53_service.py
--rw-r--r--   0        0        0      221 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/route53/route53domains_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/__init__.py
--rw-r--r--   0        0        0     1392 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json
--rw-r--r--   0        0        0     1128 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/__init__.py
--rw-r--r--   0        0        0     1266 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json
--rw-r--r--   0        0        0      957 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/__init__.py
--rw-r--r--   0        0        0     1459 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json
--rw-r--r--   0        0        0      917 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/__init__.py
--rw-r--r--   0        0        0     1496 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json
--rw-r--r--   0        0        0     1123 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/__init__.py
--rw-r--r--   0        0        0     1426 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json
--rw-r--r--   0        0        0      943 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/__init__.py
--rw-r--r--   0        0        0     1399 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.metadata.json
--rw-r--r--   0        0        0      944 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/__init__.py
--rw-r--r--   0        0        0     1212 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json
--rw-r--r--   0        0        0      947 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/__init__.py
--rw-r--r--   0        0        0     1080 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json
--rw-r--r--   0        0        0     1716 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_public_access/__init__.py
--rw-r--r--   0        0        0     1939 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json
--rw-r--r--   0        0        0     4078 2023-07-06 15:19:30.366255 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/__init__.py
--rw-r--r--   0        0        0     1190 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json
--rw-r--r--   0        0        0     2099 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1372 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0      978 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py
--rw-r--r--   0        0        0      175 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/s3/s3_client.py
--rw-r--r--   0        0        0    17497 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/s3/s3_service.py
--rw-r--r--   0        0        0      196 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/s3/s3control_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/__init__.py
--rw-r--r--   0        0        0      210 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/__init__.py
--rw-r--r--   0        0        0     1100 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json
--rw-r--r--   0        0        0      945 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1094 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0      966 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1412 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1046 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/__init__.py
--rw-r--r--   0        0        0     1227 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json
--rw-r--r--   0        0        0     1037 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1361 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0     1063 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/__init__.py
--rw-r--r--   0        0        0     1524 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json
--rw-r--r--   0        0        0     1091 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py
--rw-r--r--   0        0        0    11611 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1119 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1040 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/__init__.py
--rw-r--r--   0        0        0     1106 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json
--rw-r--r--   0        0        0     1005 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1179 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1042 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1100 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0     1072 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/secretsmanager/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1341 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1054 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py
--rw-r--r--   0        0        0      244 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_client.py
--rw-r--r--   0        0        0     2529 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/securityhub/__init__.py
--rw-r--r--   0        0        0      220 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/securityhub/securityhub_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/securityhub/securityhub_enabled/__init__.py
--rw-r--r--   0        0        0     1315 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json
--rw-r--r--   0        0        0     1296 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py
--rw-r--r--   0        0        0     4490 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/securityhub/securityhub_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/__init__.py
--rw-r--r--   0        0        0     1051 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json
--rw-r--r--   0        0        0     1259 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/__init__.py
--rw-r--r--   0        0        0     1045 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json
--rw-r--r--   0        0        0     1267 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/__init__.py
--rw-r--r--   0        0        0     1041 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json
--rw-r--r--   0        0        0     1316 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/__init__.py
--rw-r--r--   0        0        0     1021 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json
--rw-r--r--   0        0        0     1271 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/__init__.py
--rw-r--r--   0        0        0     1095 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json
--rw-r--r--   0        0        0     1353 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/__init__.py
--rw-r--r--   0        0        0     1020 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json
--rw-r--r--   0        0        0     1275 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py
--rw-r--r--   0        0        0      195 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_client.py
--rw-r--r--   0        0        0     2527 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/shield/shield_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sns/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sns/sns_client.py
--rw-r--r--   0        0        0     3814 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sns/sns_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1283 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0      841 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1340 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1938 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sqs/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1396 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1933 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1479 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      939 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py
--rw-r--r--   0        0        0     4417 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_document_secrets/__init__.py
--rw-r--r--   0        0        0     1225 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json
--rw-r--r--   0        0        0     1974 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/__init__.py
--rw-r--r--   0        0        0     1142 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json
--rw-r--r--   0        0        0      884 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/__init__.py
--rw-r--r--   0        0        0     1557 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json
--rw-r--r--   0        0        0      993 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py
--rw-r--r--   0        0        0     7698 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssmincidents/__init__.py
--rw-r--r--   0        0        0      234 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json
--rw-r--r--   0        0        0     1487 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py
--rw-r--r--   0        0        0     6856 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/trustedadvisor/__init__.py
--rw-r--r--   0        0        0      244 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/__init__.py
--rw-r--r--   0        0        0     1132 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json
--rw-r--r--   0        0        0     1478 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py
--rw-r--r--   0        0        0     3575 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/vpc/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_different_regions/__init__.py
--rw-r--r--   0        0        0      945 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json
--rw-r--r--   0        0        0     1010 2023-07-06 15:19:30.370256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/__init__.py
--rw-r--r--   0        0        0     1094 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json
--rw-r--r--   0        0        0     3410 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/__init__.py
--rw-r--r--   0        0        0     1173 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json
--rw-r--r--   0        0        0     2222 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/__init__.py
--rw-r--r--   0        0        0     1214 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json
--rw-r--r--   0        0        0      800 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/__init__.py
--rw-r--r--   0        0        0     1294 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json
--rw-r--r--   0        0        0     1497 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py
--rw-r--r--   0        0        0    16958 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/__init__.py
--rw-r--r--   0        0        0      988 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json
--rw-r--r--   0        0        0     1327 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/__init__.py
--rw-r--r--   0        0        0     1370 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.metadata.json
--rw-r--r--   0        0        0     1086 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/__init__.py
--rw-r--r--   0        0        0      967 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json
--rw-r--r--   0        0        0     1483 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/waf/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/waf/waf_client.py
--rw-r--r--   0        0        0     2645 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/waf/waf_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/wafv2/__init__.py
--rw-r--r--   0        0        0      190 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/wafv2/wafv2_client.py
--rw-r--r--   0        0        0     2724 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/wafv2/wafv2_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/wellarchitected/__init__.py
--rw-r--r--   0        0        0      249 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_client.py
--rw-r--r--   0        0        0     2972 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/__init__.py
--rw-r--r--   0        0        0     1680 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.metadata.json
--rw-r--r--   0        0        0     1090 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/workspaces/__init__.py
--rw-r--r--   0        0        0      215 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_client.py
--rw-r--r--   0        0        0     3821 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     2073 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1586 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/__init__.py
--rw-r--r--   0        0        0     1371 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.metadata.json
--rw-r--r--   0        0        0     2344 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/__init__.py
--rw-r--r--   0        0        0     8818 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/azure_provider.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/lib/audit_info/__init__.py
--rw-r--r--   0        0        0      258 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0      796 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/__init__.py
--rw-r--r--   0        0        0      205 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/__init__.py
--rw-r--r--   0        0        0     1496 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json
--rw-r--r--   0        0        0     1182 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/__init__.py
--rw-r--r--   0        0        0      926 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json
--rw-r--r--   0        0        0     1121 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/__init__.py
--rw-r--r--   0        0        0     1654 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1210 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/__init__.py
--rw-r--r--   0        0        0     1561 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json
--rw-r--r--   0        0        0     1181 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/__init__.py
--rw-r--r--   0        0        0     1306 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json
--rw-r--r--   0        0        0     1163 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/__init__.py
--rw-r--r--   0        0        0      906 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1638 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/__init__.py
--rw-r--r--   0        0        0     1254 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json
--rw-r--r--   0        0        0     1122 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/__init__.py
--rw-r--r--   0        0        0     1590 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json
--rw-r--r--   0        0        0     1163 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/__init__.py
--rw-r--r--   0        0        0     1187 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1346 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/__init__.py
--rw-r--r--   0        0        0     1509 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json
--rw-r--r--   0        0        0     1170 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/__init__.py
--rw-r--r--   0        0        0     1751 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json
--rw-r--r--   0        0        0     1227 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/__init__.py
--rw-r--r--   0        0        0     1693 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json
--rw-r--r--   0        0        0     1202 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py
--rw-r--r--   0        0        0     2326 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/defender/defender_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/iam/__init__.py
--rw-r--r--   0        0        0      180 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/iam/iam_client.py
--rw-r--r--   0        0        0     2696 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/__init__.py
--rw-r--r--   0        0        0      996 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json
--rw-r--r--   0        0        0     1330 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/__init__.py
--rw-r--r--   0        0        0     1470 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py
--rw-r--r--   0        0        0      200 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/__init__.py
--rw-r--r--   0        0        0     1354 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json
--rw-r--r--   0        0        0     1179 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/__init__.py
--rw-r--r--   0        0        0     1765 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json
--rw-r--r--   0        0        0     1265 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/__init__.py
--rw-r--r--   0        0        0     1399 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json
--rw-r--r--   0        0        0     1156 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/__init__.py
--rw-r--r--   0        0        0     1246 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json
--rw-r--r--   0        0        0     1151 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/__init__.py
--rw-r--r--   0        0        0     1093 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json
--rw-r--r--   0        0        0     1169 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/__init__.py
--rw-r--r--   0        0        0     1272 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py
--rw-r--r--   0        0        0     3651 2023-07-06 15:19:30.374256 prowler-3.7.0/prowler/providers/azure/services/storage/storage_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/common/__init__.py
--rw-r--r--   0        0        0     1212 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/common/allowlist.py
--rw-r--r--   0        0        0    15670 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/common/audit_info.py
--rw-r--r--   0        0        0      251 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/common/models.py
--rw-r--r--   0        0        0     4669 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/common/outputs.py
--rw-r--r--   0        0        0      837 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/common/quick_inventory.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/__init__.py
--rw-r--r--   0        0        0     3468 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/gcp_provider.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/lib/audit_info/__init__.py
--rw-r--r--   0        0        0      229 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0      683 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/__init__.py
--rw-r--r--   0        0        0     1751 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.metadata.json
--rw-r--r--   0        0        0     1135 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.py
--rw-r--r--   0        0        0      192 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_exists/__init__.py
--rw-r--r--   0        0        0     1446 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.metadata.json
--rw-r--r--   0        0        0      912 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/__init__.py
--rw-r--r--   0        0        0     1700 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.metadata.json
--rw-r--r--   0        0        0     1103 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.py
--rw-r--r--   0        0        0     2054 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/__init__.py
--rw-r--r--   0        0        0      197 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json
--rw-r--r--   0        0        0      988 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json
--rw-r--r--   0        0        0      968 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py
--rw-r--r--   0        0        0     4484 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/__init__.py
--rw-r--r--   0        0        0     1373 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json
--rw-r--r--   0        0        0      964 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudresourcemanager/__init__.py
--rw-r--r--   0        0        0      266 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_client.py
--rw-r--r--   0        0        0     2408 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/__init__.py
--rw-r--r--   0        0        0      197 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/__init__.py
--rw-r--r--   0        0        0     1408 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json
--rw-r--r--   0        0        0     1004 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/__init__.py
--rw-r--r--   0        0        0     1359 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json
--rw-r--r--   0        0        0     1175 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/__init__.py
--rw-r--r--   0        0        0     1216 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json
--rw-r--r--   0        0        0     1196 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/__init__.py
--rw-r--r--   0        0        0     2058 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json
--rw-r--r--   0        0        0     1295 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/__init__.py
--rw-r--r--   0        0        0     1587 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json
--rw-r--r--   0        0        0     1200 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/__init__.py
--rw-r--r--   0        0        0     1447 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json
--rw-r--r--   0        0        0     1212 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json
--rw-r--r--   0        0        0     1303 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/__init__.py
--rw-r--r--   0        0        0     1448 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json
--rw-r--r--   0        0        0     1316 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/__init__.py
--rw-r--r--   0        0        0     1955 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json
--rw-r--r--   0        0        0     1459 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json
--rw-r--r--   0        0        0     1403 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/__init__.py
--rw-r--r--   0        0        0     1326 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json
--rw-r--r--   0        0        0     1361 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/__init__.py
--rw-r--r--   0        0        0     1151 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json
--rw-r--r--   0        0        0     1097 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/__init__.py
--rw-r--r--   0        0        0     1492 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json
--rw-r--r--   0        0        0     1039 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1319 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json
--rw-r--r--   0        0        0      984 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/__init__.py
--rw-r--r--   0        0        0     2153 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json
--rw-r--r--   0        0        0     1343 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/__init__.py
--rw-r--r--   0        0        0     1702 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json
--rw-r--r--   0        0        0     1225 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/__init__.py
--rw-r--r--   0        0        0     1583 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json
--rw-r--r--   0        0        0     1312 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/__init__.py
--rw-r--r--   0        0        0     1860 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json
--rw-r--r--   0        0        0     1194 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/__init__.py
--rw-r--r--   0        0        0     2002 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json
--rw-r--r--   0        0        0     1183 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/__init__.py
--rw-r--r--   0        0        0     2238 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json
--rw-r--r--   0        0        0     1203 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/__init__.py
--rw-r--r--   0        0        0     1583 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json
--rw-r--r--   0        0        0     1172 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/__init__.py
--rw-r--r--   0        0        0     1428 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json
--rw-r--r--   0        0        0      970 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py
--rw-r--r--   0        0        0     2723 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/__init__.py
--rw-r--r--   0        0        0     1719 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.metadata.json
--rw-r--r--   0        0        0     1638 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json
--rw-r--r--   0        0        0      913 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/__init__.py
--rw-r--r--   0        0        0     1270 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json
--rw-r--r--   0        0        0     1054 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py
--rw-r--r--   0        0        0      226 2023-07-06 15:19:30.378255 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_client.py
--rw-r--r--   0        0        0     2493 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/__init__.py
--rw-r--r--   0        0        0      192 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/__init__.py
--rw-r--r--   0        0        0     2313 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.metadata.json
--rw-r--r--   0        0        0     1987 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/__init__.py
--rw-r--r--   0        0        0     2451 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.metadata.json
--rw-r--r--   0        0        0     1977 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/__init__.py
--rw-r--r--   0        0        0     1515 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.metadata.json
--rw-r--r--   0        0        0     1284 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/__init__.py
--rw-r--r--   0        0        0     2383 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.metadata.json
--rw-r--r--   0        0        0     1005 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/__init__.py
--rw-r--r--   0        0        0     1788 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.metadata.json
--rw-r--r--   0        0        0     1266 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/__init__.py
--rw-r--r--   0        0        0     2091 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.metadata.json
--rw-r--r--   0        0        0     1443 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/__init__.py
--rw-r--r--   0        0        0     2388 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.metadata.json
--rw-r--r--   0        0        0     1082 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/__init__.py
--rw-r--r--   0        0        0     2358 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.metadata.json
--rw-r--r--   0        0        0     1043 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1327 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json
--rw-r--r--   0        0        0      891 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/__init__.py
--rw-r--r--   0        0        0     2459 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.metadata.json
--rw-r--r--   0        0        0     1267 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/__init__.py
--rw-r--r--   0        0        0     2288 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.metadata.json
--rw-r--r--   0        0        0     1079 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1508 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.metadata.json
--rw-r--r--   0        0        0      930 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/__init__.py
--rw-r--r--   0        0        0     1132 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json
--rw-r--r--   0        0        0     1551 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1749 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1181 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_not_legacy/__init__.py
--rw-r--r--   0        0        0     2085 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.metadata.json
--rw-r--r--   0        0        0      889 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/__init__.py
--rw-r--r--   0        0        0     1897 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.metadata.json
--rw-r--r--   0        0        0      881 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.py
--rw-r--r--   0        0        0    12640 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/__init__.py
--rw-r--r--   0        0        0     2121 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.metadata.json
--rw-r--r--   0        0        0      949 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dataproc/__init__.py
--rw-r--r--   0        0        0      197 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/__init__.py
--rw-r--r--   0        0        0     2301 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.metadata.json
--rw-r--r--   0        0        0      975 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.py
--rw-r--r--   0        0        0     2316 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/__init__.py
--rw-r--r--   0        0        0      172 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_dnssec_disabled/__init__.py
--rw-r--r--   0        0        0     1818 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.metadata.json
--rw-r--r--   0        0        0      938 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/__init__.py
--rw-r--r--   0        0        0     1826 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.metadata.json
--rw-r--r--   0        0        0     1117 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/__init__.py
--rw-r--r--   0        0        0     1829 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.metadata.json
--rw-r--r--   0        0        0     1121 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.py
--rw-r--r--   0        0        0     3394 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/dns/dns_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/__init__.py
--rw-r--r--   0        0        0      205 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/accessapproval_client.py
--rw-r--r--   0        0        0      214 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/essentialcontacts_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/__init__.py
--rw-r--r--   0        0        0     2590 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.metadata.json
--rw-r--r--   0        0        0      972 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/__init__.py
--rw-r--r--   0        0        0     1997 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.metadata.json
--rw-r--r--   0        0        0      963 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.py
--rw-r--r--   0        0        0      172 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/__init__.py
--rw-r--r--   0        0        0     2294 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.metadata.json
--rw-r--r--   0        0        0     1605 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.metadata.json
--rw-r--r--   0        0        0     1040 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/__init__.py
--rw-r--r--   0        0        0     2135 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.metadata.json
--rw-r--r--   0        0        0     1857 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/__init__.py
--rw-r--r--   0        0        0     2235 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.metadata.json
--rw-r--r--   0        0        0     1469 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     1459 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     1392 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/__init__.py
--rw-r--r--   0        0        0     1363 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json
--rw-r--r--   0        0        0     1035 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/__init__.py
--rw-r--r--   0        0        0     1133 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json
--rw-r--r--   0        0        0     1314 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py
--rw-r--r--   0        0        0     6222 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/kms/__init__.py
--rw-r--r--   0        0        0      172 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/kms/kms_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1195 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0      993 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1233 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1128 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py
--rw-r--r--   0        0        0     5395 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/kms/kms_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/logging/__init__.py
--rw-r--r--   0        0        0      192 2023-07-06 15:19:30.382256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1438 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2234 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1243 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2209 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1239 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2328 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1589 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2526 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1212 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2145 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1233 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2324 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1113 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2426 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1157 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2257 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py
--rw-r--r--   0        0        0     3047 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_sink_created/__init__.py
--rw-r--r--   0        0        0     1235 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json
--rw-r--r--   0        0        0     1633 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/monitoring/__init__.py
--rw-r--r--   0        0        0      207 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/monitoring/monitoring_client.py
--rw-r--r--   0        0        0     2125 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/monitoring/monitoring_service.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/serviceusage/__init__.py
--rw-r--r--   0        0        0      226 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_client.py
--rw-r--r--   0        0        0        0 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/__init__.py
--rw-r--r--   0        0        0     1904 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.metadata.json
--rw-r--r--   0        0        0     1266 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.py
--rw-r--r--   0        0        0     1821 2023-07-06 15:19:30.386256 prowler-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_service.py
--rw-r--r--   0        0        0     2490 2023-07-06 15:19:50.374453 prowler-3.7.0/pyproject.toml
--rw-r--r--   0        0        0    15572 1970-01-01 00:00:00.000000 prowler-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-07-12 13:45:38.819553 prowler-3.7.1/LICENSE
+-rw-r--r--   0        0        0    13569 2023-07-12 13:45:38.819553 prowler-3.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.847553 prowler-3.7.1/prowler/__init__.py
+-rw-r--r--   0        0        0     8955 2023-07-12 13:45:38.847553 prowler-3.7.1/prowler/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.847553 prowler-3.7.1/prowler/compliance/aws/__init__.py
+-rw-r--r--   0        0        0     6516 2023-07-12 13:45:38.847553 prowler-3.7.1/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json
+-rw-r--r--   0        0        0    17475 2023-07-12 13:45:38.847553 prowler-3.7.1/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json
+-rw-r--r--   0        0        0     4834 2023-07-12 13:45:38.847553 prowler-3.7.1/prowler/compliance/aws/aws_well_architected_framework_reliability_pillar_aws.json
+-rw-r--r--   0        0        0   165349 2023-07-12 13:45:38.847553 prowler-3.7.1/prowler/compliance/aws/aws_well_architected_framework_security_pillar_aws.json
+-rw-r--r--   0        0        0   260398 2023-07-12 13:45:38.847553 prowler-3.7.1/prowler/compliance/aws/cis_1.4_aws.json
+-rw-r--r--   0        0        0   287275 2023-07-12 13:45:38.847553 prowler-3.7.1/prowler/compliance/aws/cis_1.5_aws.json
+-rw-r--r--   0        0        0   292304 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/cis_2.0_aws.json
+-rw-r--r--   0        0        0    15458 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/cisa_aws.json
+-rw-r--r--   0        0        0   142312 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/ens_rd2022_aws.json
+-rw-r--r--   0        0        0    18551 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/fedramp_low_revision_4_aws.json
+-rw-r--r--   0        0        0    57257 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json
+-rw-r--r--   0        0        0    31059 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/ffiec_aws.json
+-rw-r--r--   0        0        0    10166 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/gdpr_aws.json
+-rw-r--r--   0        0        0    18763 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json
+-rw-r--r--   0        0        0    11774 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/gxp_eu_annex_11_aws.json
+-rw-r--r--   0        0        0    31000 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/hipaa_aws.json
+-rw-r--r--   0        0        0    41885 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/iso27001_2013_aws.json
+-rw-r--r--   0        0        0   132178 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/mitre_attack_aws.json
+-rw-r--r--   0        0        0    86208 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/nist_800_171_revision_2_aws.json
+-rw-r--r--   0        0        0    50559 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/nist_800_53_revision_4_aws.json
+-rw-r--r--   0        0        0   243911 2023-07-12 13:45:38.851553 prowler-3.7.1/prowler/compliance/aws/nist_800_53_revision_5_aws.json
+-rw-r--r--   0        0        0    40042 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/compliance/aws/nist_csf_1.1_aws.json
+-rw-r--r--   0        0        0     8722 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/compliance/aws/pci_3.2.1_aws.json
+-rw-r--r--   0        0        0     8563 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/compliance/aws/rbi_cyber_security_framework_aws.json
+-rw-r--r--   0        0        0    93913 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/compliance/aws/soc2_aws.json
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/compliance/azure/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/compliance/gcp/__init__.py
+-rw-r--r--   0        0        0   385663 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/compliance/gcp/cis_2.0_gcp.json
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/config/__init__.py
+-rw-r--r--   0        0        0     3459 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/config/allowlist.yaml
+-rw-r--r--   0        0        0      165 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/config/checklist_example.json
+-rw-r--r--   0        0        0     3300 2023-07-12 13:45:55.116101 prowler-3.7.1/prowler/config/config.py
+-rw-r--r--   0        0        0     1942 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/config/config.yaml
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/__init__.py
+-rw-r--r--   0        0        0      854 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/banner.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/check/__init__.py
+-rw-r--r--   0        0        0    22996 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/check/check.py
+-rw-r--r--   0        0        0     2973 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/check/checks_loader.py
+-rw-r--r--   0        0        0     3864 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/check/compliance.py
+-rw-r--r--   0        0        0     5225 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/check/compliance_models.py
+-rw-r--r--   0        0        0     3835 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/check/models.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/cli/__init__.py
+-rw-r--r--   0        0        0    18411 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/cli/parser.py
+-rw-r--r--   0        0        0     1885 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/logger.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/outputs/__init__.py
+-rw-r--r--   0        0        0    34169 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/outputs/compliance.py
+-rw-r--r--   0        0        0    10181 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/outputs/file_descriptors.py
+-rw-r--r--   0        0        0    20435 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/outputs/html.py
+-rw-r--r--   0        0        0    12276 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/outputs/json.py
+-rw-r--r--   0        0        0    25615 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/outputs/models.py
+-rw-r--r--   0        0        0    11105 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/outputs/outputs.py
+-rw-r--r--   0        0        0     5015 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/outputs/slack.py
+-rw-r--r--   0        0        0     6592 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/outputs/summary_table.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/scan_filters/__init__.py
+-rw-r--r--   0        0        0      552 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/scan_filters/scan_filters.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/utils/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/lib/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/providers/aws/__init__.py
+-rw-r--r--   0        0        0    13384 2023-07-12 13:45:38.855553 prowler-3.7.1/prowler/providers/aws/aws_provider.py
+-rw-r--r--   0        0        0   219041 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/aws_regions_by_service.json
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/allowlist/__init__.py
+-rw-r--r--   0        0        0    11103 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/allowlist/allowlist.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/arn/__init__.py
+-rw-r--r--   0        0        0     1871 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/arn/arn.py
+-rw-r--r--   0        0        0     2193 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/arn/error.py
+-rw-r--r--   0        0        0     1957 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/arn/models.py
+-rw-r--r--   0        0        0     1152 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0     1251 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/credentials/__init__.py
+-rw-r--r--   0        0        0     2459 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/credentials/credentials.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/organizations/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/organizations/organizations.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/policy_condition_parser/__init__.py
+-rw-r--r--   0        0        0     1716 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/policy_condition_parser/policy_condition_parser.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/quick_inventory/__init__.py
+-rw-r--r--   0        0        0    15534 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/quick_inventory/quick_inventory.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/resource_api_tagging/__init__.py
+-rw-r--r--   0        0        0     1585 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/security_hub/__init__.py
+-rw-r--r--   0        0        0     5867 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/lib/security_hub/security_hub.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/__init__.py
+-rw-r--r--   0        0        0     1584 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json
+-rw-r--r--   0        0        0     1478 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/__init__.py
+-rw-r--r--   0        0        0     1635 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json
+-rw-r--r--   0        0        0     2184 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py
+-rw-r--r--   0        0        0     5375 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/__init__.py
+-rw-r--r--   0        0        0      200 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/__init__.py
+-rw-r--r--   0        0        0     1753 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json
+-rw-r--r--   0        0        0      717 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json
+-rw-r--r--   0        0        0      746 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/__init__.py
+-rw-r--r--   0        0        0     1674 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json
+-rw-r--r--   0        0        0      764 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py
+-rw-r--r--   0        0        0      706 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/account/account_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/acm/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/__init__.py
+-rw-r--r--   0        0        0     1368 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json
+-rw-r--r--   0        0        0     1233 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json
+-rw-r--r--   0        0        0     1636 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/acm/acm_client.py
+-rw-r--r--   0        0        0     4752 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/acm/acm_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/__init__.py
+-rw-r--r--   0        0        0     1133 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json
+-rw-r--r--   0        0        0      976 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py
+-rw-r--r--   0        0        0      215 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/__init__.py
+-rw-r--r--   0        0        0     1250 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json
+-rw-r--r--   0        0        0     1126 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/__init__.py
+-rw-r--r--   0        0        0     1087 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json
+-rw-r--r--   0        0        0      994 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1676 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1079 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py
+-rw-r--r--   0        0        0     5320 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/__init__.py
+-rw-r--r--   0        0        0     1181 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json
+-rw-r--r--   0        0        0     1093 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1504 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1123 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/__init__.py
+-rw-r--r--   0        0        0      995 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json
+-rw-r--r--   0        0        0      983 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py
+-rw-r--r--   0        0        0      234 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_client.py
+-rw-r--r--   0        0        0     4018 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/__init__.py
+-rw-r--r--   0        0        0      210 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/__init__.py
+-rw-r--r--   0        0        0     1346 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json
+-rw-r--r--   0        0        0     1273 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/__init__.py
+-rw-r--r--   0        0        0     1257 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json
+-rw-r--r--   0        0        0     1408 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/__init__.py
+-rw-r--r--   0        0        0     1269 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json
+-rw-r--r--   0        0        0     1420 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/__init__.py
+-rw-r--r--   0        0        0     1363 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json
+-rw-r--r--   0        0        0     1583 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py
+-rw-r--r--   0        0        0     3619 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/autoscaling/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.859554 prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/__init__.py
+-rw-r--r--   0        0        0     1182 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json
+-rw-r--r--   0        0        0     1902 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py
+-rw-r--r--   0        0        0       78 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/fixtures/fixture
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/__init__.py
+-rw-r--r--   0        0        0     1285 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.metadata.json
+-rw-r--r--   0        0        0     1002 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.py
+-rw-r--r--   0        0        0     4192 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1198 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2548 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/__init__.py
+-rw-r--r--   0        0        0     1341 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json
+-rw-r--r--   0        0        0     3352 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/__init__.py
+-rw-r--r--   0        0        0     1536 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json
+-rw-r--r--   0        0        0     2209 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1399 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1823 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json
+-rw-r--r--   0        0        0     1058 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/__init__.py
+-rw-r--r--   0        0        0     1120 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json
+-rw-r--r--   0        0        0     1144 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/__init__.py
+-rw-r--r--   0        0        0     1619 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json
+-rw-r--r--   0        0        0     1169 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py
+-rw-r--r--   0        0        0     8137 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_plans_exist/__init__.py
+-rw-r--r--   0        0        0     1350 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json
+-rw-r--r--   0        0        0      999 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_reportplans_exist/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json
+-rw-r--r--   0        0        0     1189 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py
+-rw-r--r--   0        0        0     6981 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/__init__.py
+-rw-r--r--   0        0        0     1397 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json
+-rw-r--r--   0        0        0     1096 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_vaults_exist/__init__.py
+-rw-r--r--   0        0        0     1264 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json
+-rw-r--r--   0        0        0      976 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudformation/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_client.py
+-rw-r--r--   0        0        0     4466 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/__init__.py
+-rw-r--r--   0        0        0     1367 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json
+-rw-r--r--   0        0        0     1992 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/__init__.py
+-rw-r--r--   0        0        0     1286 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json
+-rw-r--r--   0        0        0     1249 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/__init__.py
+-rw-r--r--   0        0        0      215 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1422 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/__init__.py
+-rw-r--r--   0        0        0     1311 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json
+-rw-r--r--   0        0        0     1164 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/__init__.py
+-rw-r--r--   0        0        0     1385 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json
+-rw-r--r--   0        0        0     1721 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1491 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1230 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/__init__.py
+-rw-r--r--   0        0        0     1375 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json
+-rw-r--r--   0        0        0     1781 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/__init__.py
+-rw-r--r--   0        0        0     1479 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json
+-rw-r--r--   0        0        0     1031 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py
+-rw-r--r--   0        0        0     6218 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/__init__.py
+-rw-r--r--   0        0        0     1268 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json
+-rw-r--r--   0        0        0     1707 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py
+-rw-r--r--   0        0        0      215 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1575 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2245 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/__init__.py
+-rw-r--r--   0        0        0     1287 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json
+-rw-r--r--   0        0        0     1073 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1951 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1524 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json
+-rw-r--r--   0        0        0     1457 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1380 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2232 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1393 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2755 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/__init__.py
+-rw-r--r--   0        0        0     1730 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json
+-rw-r--r--   0        0        0     2004 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/__init__.py
+-rw-r--r--   0        0        0     1537 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json
+-rw-r--r--   0        0        0     3014 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/__init__.py
+-rw-r--r--   0        0        0     1565 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json
+-rw-r--r--   0        0        0     3016 2023-07-12 13:45:38.863554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py
+-rw-r--r--   0        0        0     9527 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1496 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2519 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1462 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2525 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1450 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2543 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1418 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2728 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py
+-rw-r--r--   0        0        0      215 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json
+-rw-r--r--   0        0        0      922 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1249 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1002 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/__init__.py
+-rw-r--r--   0        0        0     1345 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json
+-rw-r--r--   0        0        0     5022 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json
+-rw-r--r--   0        0        0     1569 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1498 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2519 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1498 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2465 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/__init__.py
+-rw-r--r--   0        0        0     1495 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json
+-rw-r--r--   0        0        0     2336 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/__init__.py
+-rw-r--r--   0        0        0     1453 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json
+-rw-r--r--   0        0        0     3174 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/__init__.py
+-rw-r--r--   0        0        0     1560 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json
+-rw-r--r--   0        0        0     2389 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/__init__.py
+-rw-r--r--   0        0        0     1456 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json
+-rw-r--r--   0        0        0     2671 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/__init__.py
+-rw-r--r--   0        0        0     1430 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json
+-rw-r--r--   0        0        0     2876 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/__init__.py
+-rw-r--r--   0        0        0     1432 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json
+-rw-r--r--   0        0        0     2356 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/__init__.py
+-rw-r--r--   0        0        0     1448 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json
+-rw-r--r--   0        0        0     2541 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/__init__.py
+-rw-r--r--   0        0        0     1475 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json
+-rw-r--r--   0        0        0     2331 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/__init__.py
+-rw-r--r--   0        0        0     1446 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json
+-rw-r--r--   0        0        0     2336 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py
+-rw-r--r--   0        0        0    11386 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py
+-rw-r--r--   0        0        0      197 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/cloudwatch/logs_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codeartifact/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/__init__.py
+-rw-r--r--   0        0        0     1540 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json
+-rw-r--r--   0        0        0     1665 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py
+-rw-r--r--   0        0        0    10588 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codebuild/__init__.py
+-rw-r--r--   0        0        0      210 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/__init__.py
+-rw-r--r--   0        0        0     1053 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json
+-rw-r--r--   0        0        0     1250 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/__init__.py
+-rw-r--r--   0        0        0     1018 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json
+-rw-r--r--   0        0        0     1060 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py
+-rw-r--r--   0        0        0     3858 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/config/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/config/config_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json
+-rw-r--r--   0        0        0     1682 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py
+-rw-r--r--   0        0        0     3295 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/config/config_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/__init__.py
+-rw-r--r--   0        0        0      254 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/__init__.py
+-rw-r--r--   0        0        0     1191 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json
+-rw-r--r--   0        0        0      997 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/__init__.py
+-rw-r--r--   0        0        0     1187 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json
+-rw-r--r--   0        0        0     1041 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/__init__.py
+-rw-r--r--   0        0        0     1042 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json
+-rw-r--r--   0        0        0     1872 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/__init__.py
+-rw-r--r--   0        0        0     1098 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json
+-rw-r--r--   0        0        0     1660 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/__init__.py
+-rw-r--r--   0        0        0     1533 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json
+-rw-r--r--   0        0        0     1373 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py
+-rw-r--r--   0        0        0    13316 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/__init__.py
+-rw-r--r--   0        0        0     1265 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json
+-rw-r--r--   0        0        0     1269 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/drs/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/drs/drs_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/drs/drs_job_exist/__init__.py
+-rw-r--r--   0        0        0      888 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json
+-rw-r--r--   0        0        0      967 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py
+-rw-r--r--   0        0        0     3504 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/drs/drs_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dax_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1594 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      957 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py
+-rw-r--r--   0        0        0      205 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_client.py
+-rw-r--r--   0        0        0     8906 2023-07-12 13:45:38.867554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1497 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      988 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/__init__.py
+-rw-r--r--   0        0        0     1529 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json
+-rw-r--r--   0        0        0      933 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ami_public/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json
+-rw-r--r--   0        0        0      843 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/__init__.py
+-rw-r--r--   0        0        0     1192 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json
+-rw-r--r--   0        0        0      850 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/__init__.py
+-rw-r--r--   0        0        0     1176 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json
+-rw-r--r--   0        0        0      965 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/__init__.py
+-rw-r--r--   0        0        0     1530 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json
+-rw-r--r--   0        0        0      922 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json
+-rw-r--r--   0        0        0      849 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/__init__.py
+-rw-r--r--   0        0        0     1057 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json
+-rw-r--r--   0        0        0     2037 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/__init__.py
+-rw-r--r--   0        0        0     1107 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json
+-rw-r--r--   0        0        0      971 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/__init__.py
+-rw-r--r--   0        0        0     1461 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json
+-rw-r--r--   0        0        0     1179 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/__init__.py
+-rw-r--r--   0        0        0     1067 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json
+-rw-r--r--   0        0        0     1111 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/__init__.py
+-rw-r--r--   0        0        0     1174 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json
+-rw-r--r--   0        0        0     1253 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/__init__.py
+-rw-r--r--   0        0        0     1201 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json
+-rw-r--r--   0        0        0     1491 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/__init__.py
+-rw-r--r--   0        0        0     1543 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json
+-rw-r--r--   0        0        0     1034 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1141 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0     1118 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/__init__.py
+-rw-r--r--   0        0        0     1292 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json
+-rw-r--r--   0        0        0     2348 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py
+-rw-r--r--   0        0        0       78 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/fixtures/fixture
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/__init__.py
+-rw-r--r--   0        0        0     1378 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json
+-rw-r--r--   0        0        0     1247 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json
+-rw-r--r--   0        0        0     1268 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/__init__.py
+-rw-r--r--   0        0        0     1513 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json
+-rw-r--r--   0        0        0     1296 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/__init__.py
+-rw-r--r--   0        0        0     1139 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json
+-rw-r--r--   0        0        0     1028 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json
+-rw-r--r--   0        0        0     1548 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/__init__.py
+-rw-r--r--   0        0        0     1169 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json
+-rw-r--r--   0        0        0     1516 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/__init__.py
+-rw-r--r--   0        0        0     1429 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json
+-rw-r--r--   0        0        0     1489 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/__init__.py
+-rw-r--r--   0        0        0     1371 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json
+-rw-r--r--   0        0        0     1517 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json
+-rw-r--r--   0        0        0     1577 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json
+-rw-r--r--   0        0        0     1612 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json
+-rw-r--r--   0        0        0     1507 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json
+-rw-r--r--   0        0        0     1523 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/__init__.py
+-rw-r--r--   0        0        0     1165 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json
+-rw-r--r--   0        0        0     1570 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/__init__.py
+-rw-r--r--   0        0        0     1190 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json
+-rw-r--r--   0        0        0     1541 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/__init__.py
+-rw-r--r--   0        0        0     1173 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json
+-rw-r--r--   0        0        0     1516 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json
+-rw-r--r--   0        0        0     1507 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/__init__.py
+-rw-r--r--   0        0        0     1218 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json
+-rw-r--r--   0        0        0     1579 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/__init__.py
+-rw-r--r--   0        0        0     1161 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json
+-rw-r--r--   0        0        0     1502 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/__init__.py
+-rw-r--r--   0        0        0     1127 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json
+-rw-r--r--   0        0        0     2440 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/__init__.py
+-rw-r--r--   0        0        0     1374 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json
+-rw-r--r--   0        0        0     1305 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/__init__.py
+-rw-r--r--   0        0        0     1221 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json
+-rw-r--r--   0        0        0     1029 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/__init__.py
+-rw-r--r--   0        0        0     1043 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json
+-rw-r--r--   0        0        0     1144 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json
+-rw-r--r--   0        0        0     1219 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py
+-rw-r--r--   0        0        0    21389 2023-07-12 13:45:38.871554 prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ec2/lib/__init__.py
+-rw-r--r--   0        0        0     2581 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ec2/lib/network_acls.py
+-rw-r--r--   0        0        0     3966 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ec2/lib/security_groups.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/__init__.py
+-rw-r--r--   0        0        0     1375 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json
+-rw-r--r--   0        0        0     1568 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/__init__.py
+-rw-r--r--   0        0        0     1123 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json
+-rw-r--r--   0        0        0     1030 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1213 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1506 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json
+-rw-r--r--   0        0        0     1108 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/__init__.py
+-rw-r--r--   0        0        0     1268 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json
+-rw-r--r--   0        0        0     2377 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py
+-rw-r--r--   0        0        0    13675 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecs/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecs/ecs_client.py
+-rw-r--r--   0        0        0     3857 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecs/ecs_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/__init__.py
+-rw-r--r--   0        0        0     1625 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json
+-rw-r--r--   0        0        0     2328 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1366 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0      857 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/__init__.py
+-rw-r--r--   0        0        0     1099 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json
+-rw-r--r--   0        0        0      847 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0      981 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1861 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py
+-rw-r--r--   0        0        0     4240 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/efs/efs_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json
+-rw-r--r--   0        0        0      992 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json
+-rw-r--r--   0        0        0     1215 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/__init__.py
+-rw-r--r--   0        0        0     1374 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json
+-rw-r--r--   0        0        0     1489 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1533 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1020 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py
+-rw-r--r--   0        0        0     4792 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/eks/eks_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/__init__.py
+-rw-r--r--   0        0        0     1364 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json
+-rw-r--r--   0        0        0     1115 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_internet_facing/__init__.py
+-rw-r--r--   0        0        0     1111 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json
+-rw-r--r--   0        0        0      823 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1392 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      817 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py
+-rw-r--r--   0        0        0     4592 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_ssl_listeners/__init__.py
+-rw-r--r--   0        0        0     1360 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json
+-rw-r--r--   0        0        0      937 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/__init__.py
+-rw-r--r--   0        0        0     1347 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json
+-rw-r--r--   0        0        0      892 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/__init__.py
+-rw-r--r--   0        0        0     1718 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json
+-rw-r--r--   0        0        0     1367 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/__init__.py
+-rw-r--r--   0        0        0     1337 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json
+-rw-r--r--   0        0        0     1646 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/__init__.py
+-rw-r--r--   0        0        0     1162 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json
+-rw-r--r--   0        0        0      888 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/__init__.py
+-rw-r--r--   0        0        0      996 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json
+-rw-r--r--   0        0        0      836 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1435 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      924 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py
+-rw-r--r--   0        0        0     7882 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/__init__.py
+-rw-r--r--   0        0        0     1325 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json
+-rw-r--r--   0        0        0     1664 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/__init__.py
+-rw-r--r--   0        0        0     1004 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json
+-rw-r--r--   0        0        0     1439 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/__init__.py
+-rw-r--r--   0        0        0     1029 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json
+-rw-r--r--   0        0        0      981 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/__init__.py
+-rw-r--r--   0        0        0      897 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json
+-rw-r--r--   0        0        0     1200 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/__init__.py
+-rw-r--r--   0        0        0     1018 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json
+-rw-r--r--   0        0        0     4444 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py
+-rw-r--r--   0        0        0     8372 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/emr/emr_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/fms/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/fms/fms_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/fms/fms_policy_compliant/__init__.py
+-rw-r--r--   0        0        0     1085 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.metadata.json
+-rw-r--r--   0        0        0     1328 2023-07-12 13:45:38.875554 prowler-3.7.1/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.py
+-rw-r--r--   0        0        0     4604 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/fms/fms_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glacier/__init__.py
+-rw-r--r--   0        0        0      200 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glacier/glacier_client.py
+-rw-r--r--   0        0        0     4080 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glacier/glacier_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/__init__.py
+-rw-r--r--   0        0        0     1219 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json
+-rw-r--r--   0        0        0     1940 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/globalaccelerator/__init__.py
+-rw-r--r--   0        0        0      259 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_client.py
+-rw-r--r--   0        0        0     2455 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1464 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      994 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1539 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      986 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/__init__.py
+-rw-r--r--   0        0        0     1222 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json
+-rw-r--r--   0        0        0      927 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1632 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1408 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1623 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1399 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1644 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1369 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1574 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1664 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1600 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1335 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1591 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1326 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py
+-rw-r--r--   0        0        0    10529 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/glue/glue_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/__init__.py
+-rw-r--r--   0        0        0      998 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json
+-rw-r--r--   0        0        0     1221 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py
+-rw-r--r--   0        0        0      210 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1282 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1130 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json
+-rw-r--r--   0        0        0      961 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py
+-rw-r--r--   0        0        0     7243 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/__init__.py
+-rw-r--r--   0        0        0     1010 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json
+-rw-r--r--   0        0        0     1933 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/__init__.py
+-rw-r--r--   0        0        0     1112 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json
+-rw-r--r--   0        0        0     2805 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2073 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2227 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/__init__.py
+-rw-r--r--   0        0        0     1494 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json
+-rw-r--r--   0        0        0      802 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2088 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2238 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2118 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2251 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1413 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4192 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1413 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4146 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1417 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4192 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/__init__.py
+-rw-r--r--   0        0        0     1089 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json
+-rw-r--r--   0        0        0     2665 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/__init__.py
+-rw-r--r--   0        0        0     1707 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json
+-rw-r--r--   0        0        0     1090 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_root_access_key/__init__.py
+-rw-r--r--   0        0        0     1453 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json
+-rw-r--r--   0        0        0     1541 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json
+-rw-r--r--   0        0        0     1414 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json
+-rw-r--r--   0        0        0     1140 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json
+-rw-r--r--   0        0        0     1239 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_number/__init__.py
+-rw-r--r--   0        0        0     1254 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json
+-rw-r--r--   0        0        0     1149 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/__init__.py
+-rw-r--r--   0        0        0     1280 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json
+-rw-r--r--   0        0        0     1285 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/__init__.py
+-rw-r--r--   0        0        0     1294 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json
+-rw-r--r--   0        0        0     1149 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/__init__.py
+-rw-r--r--   0        0        0     1300 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json
+-rw-r--r--   0        0        0     1137 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json
+-rw-r--r--   0        0        0     6229 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/__init__.py
+-rw-r--r--   0        0        0     1533 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json
+-rw-r--r--   0        0        0     1925 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/__init__.py
+-rw-r--r--   0        0        0     1384 2023-07-12 13:45:38.879554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json
+-rw-r--r--   0        0        0     1967 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/__init__.py
+-rw-r--r--   0        0        0     1356 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json
+-rw-r--r--   0        0        0     1954 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/__init__.py
+-rw-r--r--   0        0        0     1539 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.metadata.json
+-rw-r--r--   0        0        0     4380 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/__init__.py
+-rw-r--r--   0        0        0     1172 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json
+-rw-r--r--   0        0        0     4097 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1424 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1586 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1738 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1020 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/__init__.py
+-rw-r--r--   0        0        0     1424 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json
+-rw-r--r--   0        0        0     2832 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/__init__.py
+-rw-r--r--   0        0        0     1335 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json
+-rw-r--r--   0        0        0      901 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py
+-rw-r--r--   0        0        0    24265 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_support_role_created/__init__.py
+-rw-r--r--   0        0        0     1256 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json
+-rw-r--r--   0        0        0      940 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1061 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1341 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json
+-rw-r--r--   0        0        0     1698 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json
+-rw-r--r--   0        0        0     2671 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/__init__.py
+-rw-r--r--   0        0        0      998 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json
+-rw-r--r--   0        0        0     1341 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/inspector2/__init__.py
+-rw-r--r--   0        0        0      215 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/inspector2/inspector2_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/__init__.py
+-rw-r--r--   0        0        0     1158 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json
+-rw-r--r--   0        0        0     1498 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py
+-rw-r--r--   0        0        0     4084 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/inspector2/inspector2_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_cmk_are_used/__init__.py
+-rw-r--r--   0        0        0     1053 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json
+-rw-r--r--   0        0        0     1194 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1294 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1354 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2525 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
+-rw-r--r--   0        0        0     5417 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/kms/kms_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/macie/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/macie/macie_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/macie/macie_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1065 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json
+-rw-r--r--   0        0        0      982 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py
+-rw-r--r--   0        0        0     1913 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/macie/macie_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/networkfirewall/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.metadata.json
+-rw-r--r--   0        0        0     1143 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.py
+-rw-r--r--   0        0        0     3581 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_client.py
+-rw-r--r--   0        0        0     7580 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1124 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1102 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1478 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1871 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1555 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0     1003 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/__init__.py
+-rw-r--r--   0        0        0     1281 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json
+-rw-r--r--   0        0        0      991 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/__init__.py
+-rw-r--r--   0        0        0     1128 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json
+-rw-r--r--   0        0        0      983 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1766 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1023 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1281 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2655 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/__init__.py
+-rw-r--r--   0        0        0     1736 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json
+-rw-r--r--   0        0        0     1046 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/__init__.py
+-rw-r--r--   0        0        0     1242 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json
+-rw-r--r--   0        0        0     1023 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/__init__.py
+-rw-r--r--   0        0        0     1359 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json
+-rw-r--r--   0        0        0      984 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py
+-rw-r--r--   0        0        0      239 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/__init__.py
+-rw-r--r--   0        0        0     1579 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json
+-rw-r--r--   0        0        0     1816 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json
+-rw-r--r--   0        0        0     5769 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py
+-rw-r--r--   0        0        0     8762 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/__init__.py
+-rw-r--r--   0        0        0     1047 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.metadata.json
+-rw-r--r--   0        0        0     1432 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.883554 prowler-3.7.1/prowler/providers/aws/services/rds/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/__init__.py
+-rw-r--r--   0        0        0     1473 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json
+-rw-r--r--   0        0        0     1034 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/__init__.py
+-rw-r--r--   0        0        0     1367 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json
+-rw-r--r--   0        0        0     1789 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/__init__.py
+-rw-r--r--   0        0        0     1111 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.metadata.json
+-rw-r--r--   0        0        0     1215 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json
+-rw-r--r--   0        0        0     1010 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/__init__.py
+-rw-r--r--   0        0        0     1488 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json
+-rw-r--r--   0        0        0      997 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/__init__.py
+-rw-r--r--   0        0        0     1732 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json
+-rw-r--r--   0        0        0     1019 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_multi_az/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json
+-rw-r--r--   0        0        0     1730 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json
+-rw-r--r--   0        0        0     1009 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/__init__.py
+-rw-r--r--   0        0        0     1370 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json
+-rw-r--r--   0        0        0      942 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/__init__.py
+-rw-r--r--   0        0        0     1510 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json
+-rw-r--r--   0        0        0     1469 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py
+-rw-r--r--   0        0        0    16516 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/__init__.py
+-rw-r--r--   0        0        0     1552 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json
+-rw-r--r--   0        0        0     1635 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/__init__.py
+-rw-r--r--   0        0        0      205 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/__init__.py
+-rw-r--r--   0        0        0     1384 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json
+-rw-r--r--   0        0        0      973 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/__init__.py
+-rw-r--r--   0        0        0     1204 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json
+-rw-r--r--   0        0        0      984 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/__init__.py
+-rw-r--r--   0        0        0     1285 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json
+-rw-r--r--   0        0        0      996 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/__init__.py
+-rw-r--r--   0        0        0     1297 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json
+-rw-r--r--   0        0        0      992 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py
+-rw-r--r--   0        0        0     5144 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/resourceexplorer2/__init__.py
+-rw-r--r--   0        0        0      261 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json
+-rw-r--r--   0        0        0     1089 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py
+-rw-r--r--   0        0        0     2339 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/__init__.py
+-rw-r--r--   0        0        0      200 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.metadata.json
+-rw-r--r--   0        0        0     2927 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/__init__.py
+-rw-r--r--   0        0        0     1188 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json
+-rw-r--r--   0        0        0     1023 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/__init__.py
+-rw-r--r--   0        0        0      998 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json
+-rw-r--r--   0        0        0     1058 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1303 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0     8575 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53_service.py
+-rw-r--r--   0        0        0      221 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/route53/route53domains_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/__init__.py
+-rw-r--r--   0        0        0     1392 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json
+-rw-r--r--   0        0        0     1128 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/__init__.py
+-rw-r--r--   0        0        0     1266 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json
+-rw-r--r--   0        0        0      957 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/__init__.py
+-rw-r--r--   0        0        0     1459 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json
+-rw-r--r--   0        0        0      917 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/__init__.py
+-rw-r--r--   0        0        0     1496 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json
+-rw-r--r--   0        0        0     1123 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json
+-rw-r--r--   0        0        0      943 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_lock/__init__.py
+-rw-r--r--   0        0        0     1399 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.metadata.json
+-rw-r--r--   0        0        0      944 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json
+-rw-r--r--   0        0        0      947 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json
+-rw-r--r--   0        0        0     1716 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_public_access/__init__.py
+-rw-r--r--   0        0        0     1939 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json
+-rw-r--r--   0        0        0     4078 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/__init__.py
+-rw-r--r--   0        0        0     1190 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json
+-rw-r--r--   0        0        0     2099 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1372 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      978 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py
+-rw-r--r--   0        0        0      175 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_client.py
+-rw-r--r--   0        0        0    17497 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3_service.py
+-rw-r--r--   0        0        0      196 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/s3/s3control_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/__init__.py
+-rw-r--r--   0        0        0      210 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/__init__.py
+-rw-r--r--   0        0        0     1100 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json
+-rw-r--r--   0        0        0      945 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1094 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0      966 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.887554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1412 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1046 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/__init__.py
+-rw-r--r--   0        0        0     1227 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json
+-rw-r--r--   0        0        0     1037 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1361 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0     1063 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/__init__.py
+-rw-r--r--   0        0        0     1524 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json
+-rw-r--r--   0        0        0     1091 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py
+-rw-r--r--   0        0        0    11611 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1119 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1040 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json
+-rw-r--r--   0        0        0     1005 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1042 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1100 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0     1072 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/secretsmanager/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1341 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1054 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py
+-rw-r--r--   0        0        0      244 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_client.py
+-rw-r--r--   0        0        0     2529 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/securityhub/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/securityhub/securityhub_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/securityhub/securityhub_enabled/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json
+-rw-r--r--   0        0        0     1296 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py
+-rw-r--r--   0        0        0     4490 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/securityhub/securityhub_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/__init__.py
+-rw-r--r--   0        0        0     1051 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json
+-rw-r--r--   0        0        0     1259 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/__init__.py
+-rw-r--r--   0        0        0     1045 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json
+-rw-r--r--   0        0        0     1267 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/__init__.py
+-rw-r--r--   0        0        0     1041 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json
+-rw-r--r--   0        0        0     1316 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/__init__.py
+-rw-r--r--   0        0        0     1021 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json
+-rw-r--r--   0        0        0     1271 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/__init__.py
+-rw-r--r--   0        0        0     1095 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json
+-rw-r--r--   0        0        0     1353 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/__init__.py
+-rw-r--r--   0        0        0     1020 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json
+-rw-r--r--   0        0        0     1275 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py
+-rw-r--r--   0        0        0      195 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_client.py
+-rw-r--r--   0        0        0     2527 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/shield/shield_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sns/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sns/sns_client.py
+-rw-r--r--   0        0        0     3814 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sns/sns_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1283 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0      841 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1340 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1938 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sqs/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1396 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2245 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1479 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      939 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py
+-rw-r--r--   0        0        0     4417 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_document_secrets/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json
+-rw-r--r--   0        0        0     1974 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/__init__.py
+-rw-r--r--   0        0        0     1142 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json
+-rw-r--r--   0        0        0      884 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/__init__.py
+-rw-r--r--   0        0        0     1557 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json
+-rw-r--r--   0        0        0      993 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py
+-rw-r--r--   0        0        0     7698 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssmincidents/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json
+-rw-r--r--   0        0        0     1487 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py
+-rw-r--r--   0        0        0     6856 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/trustedadvisor/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/__init__.py
+-rw-r--r--   0        0        0     1132 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json
+-rw-r--r--   0        0        0     1478 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py
+-rw-r--r--   0        0        0     3575 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_different_regions/__init__.py
+-rw-r--r--   0        0        0      945 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json
+-rw-r--r--   0        0        0     1010 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/__init__.py
+-rw-r--r--   0        0        0     1094 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json
+-rw-r--r--   0        0        0     3410 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/__init__.py
+-rw-r--r--   0        0        0     1173 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json
+-rw-r--r--   0        0        0     2222 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     1214 2023-07-12 13:45:38.891554 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json
+-rw-r--r--   0        0        0      800 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/__init__.py
+-rw-r--r--   0        0        0     1294 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json
+-rw-r--r--   0        0        0     1497 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py
+-rw-r--r--   0        0        0    16958 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/__init__.py
+-rw-r--r--   0        0        0      988 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json
+-rw-r--r--   0        0        0     1327 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/__init__.py
+-rw-r--r--   0        0        0     1370 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.metadata.json
+-rw-r--r--   0        0        0     1086 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/__init__.py
+-rw-r--r--   0        0        0      967 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json
+-rw-r--r--   0        0        0     1483 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/waf/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/waf/waf_client.py
+-rw-r--r--   0        0        0     2645 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/waf/waf_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/wafv2/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/wafv2/wafv2_client.py
+-rw-r--r--   0        0        0     2724 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/wafv2/wafv2_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/wellarchitected/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_client.py
+-rw-r--r--   0        0        0     2972 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/__init__.py
+-rw-r--r--   0        0        0     1680 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.metadata.json
+-rw-r--r--   0        0        0     1090 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/workspaces/__init__.py
+-rw-r--r--   0        0        0      215 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_client.py
+-rw-r--r--   0        0        0     3821 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     2073 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1586 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/__init__.py
+-rw-r--r--   0        0        0     1371 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.metadata.json
+-rw-r--r--   0        0        0     2344 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/__init__.py
+-rw-r--r--   0        0        0     8818 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/azure_provider.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/lib/audit_info/__init__.py
+-rw-r--r--   0        0        0      258 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0      796 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/__init__.py
+-rw-r--r--   0        0        0      205 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/__init__.py
+-rw-r--r--   0        0        0     1496 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json
+-rw-r--r--   0        0        0     1182 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/__init__.py
+-rw-r--r--   0        0        0      926 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json
+-rw-r--r--   0        0        0     1121 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/__init__.py
+-rw-r--r--   0        0        0     1654 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1210 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/__init__.py
+-rw-r--r--   0        0        0     1561 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json
+-rw-r--r--   0        0        0     1181 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/__init__.py
+-rw-r--r--   0        0        0     1306 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json
+-rw-r--r--   0        0        0     1163 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1638 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/__init__.py
+-rw-r--r--   0        0        0     1254 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json
+-rw-r--r--   0        0        0     1122 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/__init__.py
+-rw-r--r--   0        0        0     1590 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json
+-rw-r--r--   0        0        0     1163 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/__init__.py
+-rw-r--r--   0        0        0     1187 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1346 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/__init__.py
+-rw-r--r--   0        0        0     1509 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json
+-rw-r--r--   0        0        0     1170 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/__init__.py
+-rw-r--r--   0        0        0     1751 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json
+-rw-r--r--   0        0        0     1227 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/__init__.py
+-rw-r--r--   0        0        0     1693 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json
+-rw-r--r--   0        0        0     1202 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py
+-rw-r--r--   0        0        0     2326 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/defender/defender_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/iam/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/iam/iam_client.py
+-rw-r--r--   0        0        0     2696 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/__init__.py
+-rw-r--r--   0        0        0      996 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json
+-rw-r--r--   0        0        0     1330 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/storage/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/__init__.py
+-rw-r--r--   0        0        0     1470 2023-07-12 13:45:38.895555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py
+-rw-r--r--   0        0        0      200 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/__init__.py
+-rw-r--r--   0        0        0     1354 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json
+-rw-r--r--   0        0        0     1179 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1765 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1265 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/__init__.py
+-rw-r--r--   0        0        0     1399 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json
+-rw-r--r--   0        0        0     1156 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/__init__.py
+-rw-r--r--   0        0        0     1246 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json
+-rw-r--r--   0        0        0     1151 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1169 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py
+-rw-r--r--   0        0        0     3651 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/azure/services/storage/storage_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/common/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/common/allowlist.py
+-rw-r--r--   0        0        0    15670 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/common/audit_info.py
+-rw-r--r--   0        0        0      251 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/common/models.py
+-rw-r--r--   0        0        0     4669 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/common/outputs.py
+-rw-r--r--   0        0        0      837 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/common/quick_inventory.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/__init__.py
+-rw-r--r--   0        0        0     3468 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/gcp_provider.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/lib/audit_info/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0      683 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/__init__.py
+-rw-r--r--   0        0        0     1751 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.metadata.json
+-rw-r--r--   0        0        0     1135 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.py
+-rw-r--r--   0        0        0      192 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_exists/__init__.py
+-rw-r--r--   0        0        0     1446 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.metadata.json
+-rw-r--r--   0        0        0      912 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/__init__.py
+-rw-r--r--   0        0        0     1700 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.metadata.json
+-rw-r--r--   0        0        0     1103 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.py
+-rw-r--r--   0        0        0     2054 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json
+-rw-r--r--   0        0        0      988 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json
+-rw-r--r--   0        0        0      968 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py
+-rw-r--r--   0        0        0     4484 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/__init__.py
+-rw-r--r--   0        0        0     1373 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json
+-rw-r--r--   0        0        0      964 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudresourcemanager/__init__.py
+-rw-r--r--   0        0        0      266 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_client.py
+-rw-r--r--   0        0        0     2408 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/__init__.py
+-rw-r--r--   0        0        0     1408 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json
+-rw-r--r--   0        0        0     1004 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/__init__.py
+-rw-r--r--   0        0        0     1359 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json
+-rw-r--r--   0        0        0     1175 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/__init__.py
+-rw-r--r--   0        0        0     1216 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json
+-rw-r--r--   0        0        0     1196 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/__init__.py
+-rw-r--r--   0        0        0     2058 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json
+-rw-r--r--   0        0        0     1295 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/__init__.py
+-rw-r--r--   0        0        0     1587 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json
+-rw-r--r--   0        0        0     1200 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/__init__.py
+-rw-r--r--   0        0        0     1447 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json
+-rw-r--r--   0        0        0     1212 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json
+-rw-r--r--   0        0        0     1303 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1448 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1316 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1955 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1459 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json
+-rw-r--r--   0        0        0     1403 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1361 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/__init__.py
+-rw-r--r--   0        0        0     1151 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json
+-rw-r--r--   0        0        0     1097 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/__init__.py
+-rw-r--r--   0        0        0     1492 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json
+-rw-r--r--   0        0        0     1039 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1319 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0      984 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/__init__.py
+-rw-r--r--   0        0        0     2153 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json
+-rw-r--r--   0        0        0     1343 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/__init__.py
+-rw-r--r--   0        0        0     1702 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json
+-rw-r--r--   0        0        0     1225 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/__init__.py
+-rw-r--r--   0        0        0     1583 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json
+-rw-r--r--   0        0        0     1312 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/__init__.py
+-rw-r--r--   0        0        0     1860 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json
+-rw-r--r--   0        0        0     1194 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/__init__.py
+-rw-r--r--   0        0        0     2002 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json
+-rw-r--r--   0        0        0     1183 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/__init__.py
+-rw-r--r--   0        0        0     2238 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json
+-rw-r--r--   0        0        0     1203 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/__init__.py
+-rw-r--r--   0        0        0     1583 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json
+-rw-r--r--   0        0        0     1172 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/__init__.py
+-rw-r--r--   0        0        0     1428 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json
+-rw-r--r--   0        0        0      970 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py
+-rw-r--r--   0        0        0     2723 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/__init__.py
+-rw-r--r--   0        0        0     1719 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.metadata.json
+-rw-r--r--   0        0        0     1638 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json
+-rw-r--r--   0        0        0      913 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/__init__.py
+-rw-r--r--   0        0        0     1270 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json
+-rw-r--r--   0        0        0     1054 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py
+-rw-r--r--   0        0        0      226 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_client.py
+-rw-r--r--   0        0        0     2493 2023-07-12 13:45:38.899555 prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/__init__.py
+-rw-r--r--   0        0        0     2313 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.metadata.json
+-rw-r--r--   0        0        0     1987 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/__init__.py
+-rw-r--r--   0        0        0     2451 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.metadata.json
+-rw-r--r--   0        0        0     1977 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.metadata.json
+-rw-r--r--   0        0        0     1284 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/__init__.py
+-rw-r--r--   0        0        0     2383 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.metadata.json
+-rw-r--r--   0        0        0     1005 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/__init__.py
+-rw-r--r--   0        0        0     1788 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.metadata.json
+-rw-r--r--   0        0        0     1266 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/__init__.py
+-rw-r--r--   0        0        0     2091 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.metadata.json
+-rw-r--r--   0        0        0     1443 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/__init__.py
+-rw-r--r--   0        0        0     2388 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.metadata.json
+-rw-r--r--   0        0        0     1082 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/__init__.py
+-rw-r--r--   0        0        0     2358 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1043 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1327 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0      891 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/__init__.py
+-rw-r--r--   0        0        0     2459 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.metadata.json
+-rw-r--r--   0        0        0     1267 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/__init__.py
+-rw-r--r--   0        0        0     2288 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.metadata.json
+-rw-r--r--   0        0        0     1079 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1508 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      930 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/__init__.py
+-rw-r--r--   0        0        0     1132 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json
+-rw-r--r--   0        0        0     1551 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1749 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1181 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_not_legacy/__init__.py
+-rw-r--r--   0        0        0     2085 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.metadata.json
+-rw-r--r--   0        0        0      889 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/__init__.py
+-rw-r--r--   0        0        0     1897 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.metadata.json
+-rw-r--r--   0        0        0      881 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.py
+-rw-r--r--   0        0        0    12640 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     2121 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.metadata.json
+-rw-r--r--   0        0        0      949 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dataproc/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/__init__.py
+-rw-r--r--   0        0        0     2301 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.metadata.json
+-rw-r--r--   0        0        0      975 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.py
+-rw-r--r--   0        0        0     2316 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_dnssec_disabled/__init__.py
+-rw-r--r--   0        0        0     1818 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.metadata.json
+-rw-r--r--   0        0        0      938 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/__init__.py
+-rw-r--r--   0        0        0     1826 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.metadata.json
+-rw-r--r--   0        0        0     1117 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/__init__.py
+-rw-r--r--   0        0        0     1829 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.metadata.json
+-rw-r--r--   0        0        0     1121 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.py
+-rw-r--r--   0        0        0     3394 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/dns/dns_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/__init__.py
+-rw-r--r--   0        0        0      205 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/accessapproval_client.py
+-rw-r--r--   0        0        0      214 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/essentialcontacts_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/__init__.py
+-rw-r--r--   0        0        0     2590 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.metadata.json
+-rw-r--r--   0        0        0      972 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     1997 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.metadata.json
+-rw-r--r--   0        0        0      963 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.py
+-rw-r--r--   0        0        0      172 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/__init__.py
+-rw-r--r--   0        0        0     2294 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.metadata.json
+-rw-r--r--   0        0        0     1674 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.metadata.json
+-rw-r--r--   0        0        0     1040 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/__init__.py
+-rw-r--r--   0        0        0     2135 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.metadata.json
+-rw-r--r--   0        0        0     1857 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/__init__.py
+-rw-r--r--   0        0        0     2235 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.metadata.json
+-rw-r--r--   0        0        0     1469 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     1459 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     1392 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/__init__.py
+-rw-r--r--   0        0        0     1363 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json
+-rw-r--r--   0        0        0     1035 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/__init__.py
+-rw-r--r--   0        0        0     1133 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json
+-rw-r--r--   0        0        0     1314 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py
+-rw-r--r--   0        0        0     6222 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/kms/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/kms/kms_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1195 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0      993 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1233 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1128 2023-07-12 13:45:38.903555 prowler-3.7.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py
+-rw-r--r--   0        0        0     5395 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/kms/kms_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1438 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2234 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1243 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2209 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2328 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1589 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2526 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2145 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1233 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2324 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1113 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2426 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1157 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2257 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py
+-rw-r--r--   0        0        0     3047 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_sink_created/__init__.py
+-rw-r--r--   0        0        0     1235 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json
+-rw-r--r--   0        0        0     1633 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/monitoring/__init__.py
+-rw-r--r--   0        0        0      207 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/monitoring/monitoring_client.py
+-rw-r--r--   0        0        0     2125 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/monitoring/monitoring_service.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/serviceusage/__init__.py
+-rw-r--r--   0        0        0      226 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_client.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/__init__.py
+-rw-r--r--   0        0        0     1904 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.metadata.json
+-rw-r--r--   0        0        0     1266 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.py
+-rw-r--r--   0        0        0     1821 2023-07-12 13:45:38.907555 prowler-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_service.py
+-rw-r--r--   0        0        0     2491 2023-07-12 13:45:55.092100 prowler-3.7.1/pyproject.toml
+-rw-r--r--   0        0        0    15573 1970-01-01 00:00:00.000000 prowler-3.7.1/PKG-INFO
```

### Comparing `prowler-3.7.0/LICENSE` & `prowler-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/README.md` & `prowler-3.7.1/README.md`

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

### Comparing `prowler-3.7.0/prowler/__main__.py` & `prowler-3.7.1/prowler/__main__.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json` & `prowler-3.7.1/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json` & `prowler-3.7.1/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/aws_well_architected_framework_reliability_pillar_aws.json` & `prowler-3.7.1/prowler/compliance/aws/aws_well_architected_framework_reliability_pillar_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/aws_well_architected_framework_security_pillar_aws.json` & `prowler-3.7.1/prowler/compliance/aws/aws_well_architected_framework_security_pillar_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/cis_1.4_aws.json` & `prowler-3.7.1/prowler/compliance/aws/cis_1.4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/cis_1.5_aws.json` & `prowler-3.7.1/prowler/compliance/aws/cis_1.5_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/cisa_aws.json` & `prowler-3.7.1/prowler/compliance/aws/cisa_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/ens_rd2022_aws.json` & `prowler-3.7.1/prowler/compliance/aws/ens_rd2022_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/fedramp_low_revision_4_aws.json` & `prowler-3.7.1/prowler/compliance/aws/fedramp_low_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json` & `prowler-3.7.1/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/ffiec_aws.json` & `prowler-3.7.1/prowler/compliance/aws/ffiec_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/gdpr_aws.json` & `prowler-3.7.1/prowler/compliance/aws/gdpr_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json` & `prowler-3.7.1/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/gxp_eu_annex_11_aws.json` & `prowler-3.7.1/prowler/compliance/aws/gxp_eu_annex_11_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/hipaa_aws.json` & `prowler-3.7.1/prowler/compliance/aws/hipaa_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/iso27001_2013_aws.json` & `prowler-3.7.1/prowler/compliance/aws/iso27001_2013_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/mitre_attack_aws.json` & `prowler-3.7.1/prowler/compliance/aws/mitre_attack_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/nist_800_171_revision_2_aws.json` & `prowler-3.7.1/prowler/compliance/aws/nist_800_171_revision_2_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/nist_800_53_revision_4_aws.json` & `prowler-3.7.1/prowler/compliance/aws/nist_800_53_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/nist_800_53_revision_5_aws.json` & `prowler-3.7.1/prowler/compliance/aws/nist_800_53_revision_5_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/nist_csf_1.1_aws.json` & `prowler-3.7.1/prowler/compliance/aws/nist_csf_1.1_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/pci_3.2.1_aws.json` & `prowler-3.7.1/prowler/compliance/aws/pci_3.2.1_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/rbi_cyber_security_framework_aws.json` & `prowler-3.7.1/prowler/compliance/aws/rbi_cyber_security_framework_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/aws/soc2_aws.json` & `prowler-3.7.1/prowler/compliance/aws/soc2_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/compliance/gcp/cis_2.0_gcp.json` & `prowler-3.7.1/prowler/compliance/gcp/cis_2.0_gcp.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/config/allowlist.yaml` & `prowler-3.7.1/prowler/config/allowlist.yaml`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/config/config.py` & `prowler-3.7.1/prowler/config/config.py`

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

### Comparing `prowler-3.7.0/prowler/config/config.yaml` & `prowler-3.7.1/prowler/config/config.yaml`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/banner.py` & `prowler-3.7.1/prowler/lib/banner.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/check/check.py` & `prowler-3.7.1/prowler/lib/check/check.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/check/checks_loader.py` & `prowler-3.7.1/prowler/lib/check/checks_loader.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/check/compliance.py` & `prowler-3.7.1/prowler/lib/check/compliance.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/check/compliance_models.py` & `prowler-3.7.1/prowler/lib/check/compliance_models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/check/models.py` & `prowler-3.7.1/prowler/lib/check/models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/cli/parser.py` & `prowler-3.7.1/prowler/lib/cli/parser.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/logger.py` & `prowler-3.7.1/prowler/lib/logger.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/outputs/compliance.py` & `prowler-3.7.1/prowler/lib/outputs/compliance.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/outputs/file_descriptors.py` & `prowler-3.7.1/prowler/lib/outputs/file_descriptors.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/outputs/html.py` & `prowler-3.7.1/prowler/lib/outputs/html.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/outputs/json.py` & `prowler-3.7.1/prowler/lib/outputs/json.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/outputs/models.py` & `prowler-3.7.1/prowler/lib/outputs/models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/outputs/outputs.py` & `prowler-3.7.1/prowler/lib/outputs/outputs.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/outputs/slack.py` & `prowler-3.7.1/prowler/lib/outputs/slack.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/outputs/summary_table.py` & `prowler-3.7.1/prowler/lib/outputs/summary_table.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/scan_filters/scan_filters.py` & `prowler-3.7.1/prowler/lib/scan_filters/scan_filters.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/lib/utils/utils.py` & `prowler-3.7.1/prowler/lib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/aws_provider.py` & `prowler-3.7.1/prowler/providers/aws/aws_provider.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/aws_regions_by_service.json` & `prowler-3.7.1/prowler/providers/aws/aws_regions_by_service.json`

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

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/allowlist/allowlist.py` & `prowler-3.7.1/prowler/providers/aws/lib/allowlist/allowlist.py`

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

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/arn/arn.py` & `prowler-3.7.1/prowler/providers/aws/lib/arn/arn.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/arn/error.py` & `prowler-3.7.1/prowler/providers/aws/lib/arn/error.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/arn/models.py` & `prowler-3.7.1/prowler/providers/aws/lib/arn/models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/audit_info/audit_info.py` & `prowler-3.7.1/prowler/providers/aws/lib/audit_info/audit_info.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/audit_info/models.py` & `prowler-3.7.1/prowler/providers/aws/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/credentials/credentials.py` & `prowler-3.7.1/prowler/providers/aws/lib/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/organizations/organizations.py` & `prowler-3.7.1/prowler/providers/aws/lib/organizations/organizations.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/quick_inventory/quick_inventory.py` & `prowler-3.7.1/prowler/providers/aws/lib/quick_inventory/quick_inventory.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py` & `prowler-3.7.1/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/lib/security_hub/security_hub.py` & `prowler-3.7.1/prowler/providers/aws/lib/security_hub/security_hub.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py` & `prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py` & `prowler-3.7.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py` & `prowler-3.7.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py` & `prowler-3.7.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py` & `prowler-3.7.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/account/account_service.py` & `prowler-3.7.1/prowler/providers/aws/services/account/account_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py` & `prowler-3.7.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/acm/acm_service.py` & `prowler-3.7.1/prowler/providers/aws/services/acm/acm_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_service.py` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py` & `prowler-3.7.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py` & `prowler-3.7.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py` & `prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py` & `prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py` & `prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py` & `prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/appstream/appstream_service.py` & `prowler-3.7.1/prowler/providers/aws/services/appstream/appstream_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py` & `prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.py` & `prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/autoscaling/autoscaling_service.py` & `prowler-3.7.1/prowler/providers/aws/services/autoscaling/autoscaling_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/awslambda/awslambda_service.py` & `prowler-3.7.1/prowler/providers/aws/services/awslambda/awslambda_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py` & `prowler-3.7.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py` & `prowler-3.7.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/backup/backup_service.py` & `prowler-3.7.1/prowler/providers/aws/services/backup/backup_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py` & `prowler-3.7.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py` & `prowler-3.7.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_service.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudfront/cloudfront_service.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudfront/cloudfront_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py` & `prowler-3.7.1/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py` & `prowler-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/codeartifact/codeartifact_service.py` & `prowler-3.7.1/prowler/providers/aws/services/codeartifact/codeartifact_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py` & `prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py` & `prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/codebuild/codebuild_service.py` & `prowler-3.7.1/prowler/providers/aws/services/codebuild/codebuild_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/config/config_service.py` & `prowler-3.7.1/prowler/providers/aws/services/config/config_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_service.py` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py` & `prowler-3.7.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/drs/drs_service.py` & `prowler-3.7.1/prowler/providers/aws/services/drs/drs_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_service.py` & `prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/ec2_service.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/ec2_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/lib/network_acls.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/lib/network_acls.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ec2/lib/security_groups.py` & `prowler-3.7.1/prowler/providers/aws/services/ec2/lib/security_groups.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecr/ecr_service.py` & `prowler-3.7.1/prowler/providers/aws/services/ecr/ecr_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecs/ecs_service.py` & `prowler-3.7.1/prowler/providers/aws/services/ecs/ecs_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py` & `prowler-3.7.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py` & `prowler-3.7.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/efs/efs_service.py` & `prowler-3.7.1/prowler/providers/aws/services/efs/efs_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py` & `prowler-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py` & `prowler-3.7.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/eks/eks_service.py` & `prowler-3.7.1/prowler/providers/aws/services/eks/eks_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py` & `prowler-3.7.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py` & `prowler-3.7.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elb/elb_service.py` & `prowler-3.7.1/prowler/providers/aws/services/elb/elb_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py` & `prowler-3.7.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_service.py` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py` & `prowler-3.7.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py` & `prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py` & `prowler-3.7.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/emr/emr_service.py` & `prowler-3.7.1/prowler/providers/aws/services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.py` & `prowler-3.7.1/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/fms/fms_service.py` & `prowler-3.7.1/prowler/providers/aws/services/fms/fms_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glacier/glacier_service.py` & `prowler-3.7.1/prowler/providers/aws/services/glacier/glacier_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py` & `prowler-3.7.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py` & `prowler-3.7.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/glue/glue_service.py` & `prowler-3.7.1/prowler/providers/aws/services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py` & `prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py` & `prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/guardduty/guardduty_service.py` & `prowler-3.7.1/prowler/providers/aws/services/guardduty/guardduty_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_service.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_service.py`

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

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py` & `prowler-3.7.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py` & `prowler-3.7.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/inspector2/inspector2_service.py` & `prowler-3.7.1/prowler/providers/aws/services/inspector2/inspector2_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py` & `prowler-3.7.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py` & `prowler-3.7.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/kms/kms_service.py` & `prowler-3.7.1/prowler/providers/aws/services/kms/kms_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/macie/macie_service.py` & `prowler-3.7.1/prowler/providers/aws/services/macie/macie_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.py` & `prowler-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/networkfirewall/networkfirewall_service.py` & `prowler-3.7.1/prowler/providers/aws/services/networkfirewall/networkfirewall_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service.py` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py` & `prowler-3.7.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py` & `prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py` & `prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py` & `prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_service.py` & `prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.py` & `prowler-3.7.1/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_service.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py` & `prowler-3.7.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py` & `prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py` & `prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py` & `prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py` & `prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/redshift/redshift_service.py` & `prowler-3.7.1/prowler/providers/aws/services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py` & `prowler-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py` & `prowler-3.7.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.py` & `prowler-3.7.1/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/route53/route53_service.py` & `prowler-3.7.1/prowler/providers/aws/services/route53/route53_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/s3/s3_service.py` & `prowler-3.7.1/prowler/providers/aws/services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_service.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py` & `prowler-3.7.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py` & `prowler-3.7.1/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/securityhub/securityhub_service.py` & `prowler-3.7.1/prowler/providers/aws/services/securityhub/securityhub_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/shield/shield_service.py` & `prowler-3.7.1/prowler/providers/aws/services/shield/shield_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sns/sns_service.py` & `prowler-3.7.1/prowler/providers/aws/services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py` & `prowler-3.7.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py` & `prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py`

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

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/sqs/sqs_service.py` & `prowler-3.7.1/prowler/providers/aws/services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py` & `prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py` & `prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py` & `prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ssm/ssm_service.py` & `prowler-3.7.1/prowler/providers/aws/services/ssm/ssm_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py` & `prowler-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py` & `prowler-3.7.1/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py` & `prowler-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py` & `prowler-3.7.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_service.py` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.py` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_no_public_ip_by_default/vpc_subnet_no_public_ip_by_default.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py` & `prowler-3.7.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/waf/waf_service.py` & `prowler-3.7.1/prowler/providers/aws/services/waf/waf_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/wafv2/wafv2_service.py` & `prowler-3.7.1/prowler/providers/aws/services/wafv2/wafv2_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_service.py` & `prowler-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.py` & `prowler-3.7.1/prowler/providers/aws/services/wellarchitected/wellarchitected_workload_no_high_or_medium_risks/wellarchitected_workload_no_high_or_medium_risks.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_service.py` & `prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py` & `prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.metadata.json` & `prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.py` & `prowler-3.7.1/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/azure_provider.py` & `prowler-3.7.1/prowler/providers/azure/azure_provider.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/lib/audit_info/models.py` & `prowler-3.7.1/prowler/providers/azure/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/defender/defender_service.py` & `prowler-3.7.1/prowler/providers/azure/services/defender/defender_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/iam/iam_service.py` & `prowler-3.7.1/prowler/providers/azure/services/iam/iam_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py` & `prowler-3.7.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/azure/services/storage/storage_service.py` & `prowler-3.7.1/prowler/providers/azure/services/storage/storage_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/common/allowlist.py` & `prowler-3.7.1/prowler/providers/common/allowlist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/common/audit_info.py` & `prowler-3.7.1/prowler/providers/common/audit_info.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/common/outputs.py` & `prowler-3.7.1/prowler/providers/common/outputs.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/common/quick_inventory.py` & `prowler-3.7.1/prowler/providers/common/quick_inventory.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/gcp_provider.py` & `prowler-3.7.1/prowler/providers/gcp/gcp_provider.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/lib/audit_info/models.py` & `prowler-3.7.1/prowler/providers/gcp/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.py` & `prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_api_restrictions_configured/apikeys_api_restrictions_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.py` & `prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_exists/apikeys_key_exists.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.py` & `prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_key_rotated_in_90_days/apikeys_key_rotated_in_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/apikeys/apikeys_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/apikeys/apikeys_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py` & `prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py` & `prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py` & `prowler-3.7.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudsql/cloudsql_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudsql/cloudsql_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_log_retention_policy_lock/cloudstorage_bucket_log_retention_policy_lock.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_rdp_access_from_the_internet_allowed/compute_firewall_rdp_access_from_the_internet_allowed.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_firewall_ssh_access_from_the_internet_allowed/compute_firewall_ssh_access_from_the_internet_allowed.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_block_project_wide_ssh_keys_disabled/compute_instance_block_project_wide_ssh_keys_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_confidential_computing_enabled/compute_instance_confidential_computing_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use/compute_instance_default_service_account_in_use.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_default_service_account_in_use_with_full_api_access/compute_instance_default_service_account_in_use_with_full_api_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_encryption_with_csek_enabled/compute_instance_encryption_with_csek_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_ip_forwarding_is_enabled/compute_instance_ip_forwarding_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_serial_ports_in_use/compute_instance_serial_ports_in_use.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_instance_shielded_vm_enabled/compute_instance_shielded_vm_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_loadbalancer_logging_enabled/compute_loadbalancer_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_dns_logging_enabled/compute_network_dns_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_network_not_legacy/compute_network_not_legacy.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_project_os_login_enabled/compute_project_os_login_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/compute/compute_subnet_flow_logs_enabled/compute_subnet_flow_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_encrypted_with_cmks_disabled/dataproc_encrypted_with_cmks_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/dataproc/dataproc_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/dataproc/dataproc_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/dns/dns_dnssec_disabled/dns_dnssec_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.py` & `prowler-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_key_sign_in_dnssec/dns_rsasha1_in_use_to_key_sign_in_dnssec.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.py` & `prowler-3.7.1/prowler/providers/gcp/services/dns/dns_rsasha1_in_use_to_zone_sign_in_dnssec/dns_rsasha1_in_use_to_zone_sign_in_dnssec.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/dns/dns_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/dns/dns_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_account_access_approval_enabled/iam_account_access_approval_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_audit_logs_enabled/iam_audit_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.py` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_no_service_roles_at_project_level/iam_no_service_roles_at_project_level.py`

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

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.py` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_organization_essential_contacts_configured/iam_organization_essential_contacts_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.py` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_role_kms_enforce_separation_of_duties/iam_role_kms_enforce_separation_of_duties.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.py` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_role_sa_enforce_separation_of_duties/iam_role_sa_enforce_separation_of_duties.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/iam/iam_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/iam/iam_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py` & `prowler-3.7.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/kms/kms_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/kms/kms_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py` & `prowler-3.7.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/monitoring/monitoring_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/monitoring/monitoring_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.metadata.json` & `prowler-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.py` & `prowler-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_cloudasset_inventory_enabled/serviceusage_cloudasset_inventory_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/prowler/providers/gcp/services/serviceusage/serviceusage_service.py` & `prowler-3.7.1/prowler/providers/gcp/services/serviceusage/serviceusage_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.7.0/pyproject.toml` & `prowler-3.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,34 +18,34 @@
   "Pepe Fagoaga <pepe@verica.io>"
 ]
 name = "prowler"
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

### Comparing `prowler-3.7.0/PKG-INFO` & `prowler-3.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prowler
-Version: 3.7.0
+Version: 3.7.1
 Summary: Prowler is an Open Source security tool to perform Cloud Security best practices assessments, audits, incident response, continuous monitoring, hardening and forensics readiness. It contains more than 240 controls covering CIS, PCI-DSS, ISO27001, GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks.
 License: Apache-2.0
 Author: Toni de la Fuente
 Author-email: toni@blyx.com
 Maintainer: Sergio Garcia
 Maintainer-email: sergio@verica.io
 Requires-Python: >=3.9,<4.0
@@ -18,23 +18,23 @@
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
@@ -78,15 +78,15 @@
 
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
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: prowler Version: 3.7.0 Summary: Prowler is an Open
+Metadata-Version: 2.1 Name: prowler Version: 3.7.1 Summary: Prowler is an Open
 Source security tool to perform Cloud Security best practices assessments,
 audits, incident response, continuous monitoring, hardening and forensics
 readiness. It contains more than 240 controls covering CIS, PCI-DSS, ISO27001,
 GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks. License:
 Apache-2.0 Author: Toni de la Fuente Author-email: toni@blyx.com Maintainer:
 Sergio Garcia Maintainer-email: sergio@verica.io Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Provides-Extra: docs Requires-Dist:
 alive-progress (==3.1.4) Requires-Dist: awsipranges (==0.3.3) Requires-Dist:
 azure-identity (==1.13.0) Requires-Dist: azure-mgmt-authorization (==3.0.0)
 Requires-Dist: azure-mgmt-security (==5.0.0) Requires-Dist: azure-mgmt-storage
 (==21.0.0) Requires-Dist: azure-mgmt-subscription (==3.1.1) Requires-Dist:
-azure-storage-blob (==12.16.0) Requires-Dist: boto3 (==1.26.161) Requires-Dist:
+azure-storage-blob (==12.16.0) Requires-Dist: boto3 (==1.26.165) Requires-Dist:
 botocore (==1.29.165) Requires-Dist: colorama (==0.4.6) Requires-Dist: detect-
-secrets (==1.4.0) Requires-Dist: google-api-python-client (==2.91.0) Requires-
+secrets (==1.4.0) Requires-Dist: google-api-python-client (==2.92.0) Requires-
 Dist: mkdocs (==1.4.3) ; extra == "docs" Requires-Dist: mkdocs-material
 (==9.1.18) ; extra == "docs" Requires-Dist: msgraph-core (==0.2.2) Requires-
-Dist: pydantic (==1.10.9) Requires-Dist: schema (==0.7.5) Requires-Dist: shodan
-(==1.29.1) Requires-Dist: slack-sdk (==3.21.3) Requires-Dist: tabulate
+Dist: pydantic (==1.10.11) Requires-Dist: schema (==0.7.5) Requires-Dist:
+shodan (==1.29.1) Requires-Dist: slack-sdk (==3.21.3) Requires-Dist: tabulate
 (==0.9.0) Project-URL: Changelog, https://github.com/prowler-cloud/prowler/
 releases Project-URL: Documentation, https://docs.prowler.cloud Project-URL:
 Homepage, https://github.com/prowler-cloud/prowler Project-URL: Issue tracker,
 https://github.com/prowler-cloud/prowler/issues Description-Content-Type: text/
 markdown
                 [https://github.com/prowler-cloud/prowler/blob/
         62c1ce73bbcdd6b9e5ba03dfcae26dfd165defd9/docs/img/prowler-pro-
@@ -44,15 +44,15 @@
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

