# Comparing `tmp/fastly-3.0.0.tar.gz` & `tmp/fastly-3.0.1.tar.gz`

## Comparing `fastly-3.0.0.tar` & `fastly-3.0.1.tar`

### file list

```diff
@@ -1,1635 +1,1639 @@
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-3.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     8700 2020-02-02 00:00:00.000000 fastly-3.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fastly-3.0.0/MANIFEST.in
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-3.0.0/SECURITY.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastly-3.0.0/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastly-3.0.0/setup.cfg
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 fastly-3.0.0/setup.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastly-3.0.0/sig.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 fastly-3.0.0/test-requirements.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastly-3.0.0/tox.ini
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastly-3.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rwxr-xr-x   0        0        0      619 2020-02-02 00:00:00.000000 fastly-3.0.0/.github/scripts/pack.sh
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 fastly-3.0.0/.github/scripts/prepare.sh
--rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 fastly-3.0.0/.github/scripts/publish_env.sh
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 fastly-3.0.0/.github/scripts/release_body.sh
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fastly-3.0.0/.github/workflows/ci-release.yaml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Acl.md
--rw-r--r--   0        0        0    15695 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AclApi.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AclEntry.md
--rw-r--r--   0        0        0    20447 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AclEntryApi.md
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AclEntryResponse.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AclEntryResponseAllOf.md
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AclResponse.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AclResponseAllOf.md
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ApexRedirect.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ApexRedirectAllOf.md
--rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ApexRedirectApi.md
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AutomationToken.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AutomationTokenCreateRequest.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AutomationTokenCreateRequestAttributes.md
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AutomationTokenCreateResponse.md
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AutomationTokenCreateResponseAllOf.md
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AutomationTokenResponse.md
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AutomationTokenResponseAllOf.md
--rw-r--r--   0        0        0    15211 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AutomationTokensApi.md
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/AwsRegion.md
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Backend.md
--rw-r--r--   0        0        0    38268 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BackendApi.md
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BackendResponse.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BackendResponseAllOf.md
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Batch.md
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BatchErrors.md
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Billing.md
--rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingAddressApi.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingAddressAttributes.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingAddressRequest.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingAddressRequestData.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingAddressResponse.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingAddressResponseData.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingAddressVerificationErrorResponse.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingAddressVerificationErrorResponseErrors.md
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingApi.md
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingEstimateResponse.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingEstimateResponseAllOf.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingEstimateResponseAllOfLine.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingEstimateResponseAllOfLines.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingResponse.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingResponseAllOf.md
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingResponseLineItem.md
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingResponseLineItemAllOf.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingStatus.md
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingTotal.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BillingTotalExtras.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BulkUpdateAclEntriesRequest.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BulkUpdateAclEntry.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BulkUpdateAclEntryAllOf.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BulkUpdateConfigStoreItem.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BulkUpdateConfigStoreItemAllOf.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BulkUpdateConfigStoreListRequest.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BulkUpdateDictionaryItem.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BulkUpdateDictionaryListRequest.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BulkWafActiveRule.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/BulkWafActiveRules.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/CacheSetting.md
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/CacheSettingResponse.md
--rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/CacheSettingsApi.md
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ClientKey.md
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Condition.md
--rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConditionApi.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConditionResponse.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConditionsResponse.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConfigStore.md
--rw-r--r--   0        0        0    18464 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConfigStoreApi.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConfigStoreInfoResponse.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConfigStoreItem.md
--rw-r--r--   0        0        0    23504 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConfigStoreItemApi.md
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConfigStoreItemResponse.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConfigStoreItemResponseAllOf.md
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConfigStoreResponse.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ConfigStoreResponseAllOf.md
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Contact.md
--rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ContactApi.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ContactResponse.md
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ContactResponseAllOf.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Content.md
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ContentApi.md
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Customer.md
--rw-r--r--   0        0        0    18926 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/CustomerApi.md
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/CustomerResponse.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/CustomerResponseAllOf.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Dictionary.md
--rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DictionaryApi.md
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DictionaryInfoApi.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DictionaryInfoResponse.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DictionaryItem.md
--rw-r--r--   0        0        0    26138 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DictionaryItemApi.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DictionaryItemResponse.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DictionaryItemResponseAllOf.md
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DictionaryResponse.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DictionaryResponseAllOf.md
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DiffApi.md
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DiffResponse.md
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Director.md
--rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DirectorApi.md
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DirectorBackend.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DirectorBackendAllOf.md
--rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DirectorBackendApi.md
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DirectorResponse.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Domain.md
--rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainApi.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainCheckItem.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainCheckResponse.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainCheckResponseList.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainInspector.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainInspectorEntry.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainInspectorEntryDimensions.md
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainInspectorEntryValues.md
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainInspectorHistoricalApi.md
--rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainInspectorMeasurements.md
--rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainInspectorRealtimeApi.md
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainInspectorRealtimeEntry.md
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainOwnershipsApi.md
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainResponse.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/DomainsResponse.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EnabledProductResponse.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EnabledProductResponseLinks.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EnabledProductResponseProduct.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EnabledProductResponseService.md
--rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EnabledProductsApi.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ErrorResponse.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Event.md
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EventAttributes.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EventData.md
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EventDataItems.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EventResponse.md
--rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EventsApi.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/EventsResponse.md
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/GenericTokenError.md
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Gzip.md
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/GzipApi.md
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/GzipResponse.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Header.md
--rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HeaderApi.md
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HeaderResponse.md
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Healthcheck.md
--rw-r--r--   0        0        0    20120 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HealthcheckApi.md
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HealthcheckResponse.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Historical.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalAggregateResponse.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalAggregateResponseAllOf.md
--rw-r--r--   0        0        0    39081 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalApi.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalDomains.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalDomainsData.md
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalDomainsMeta.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalDomainsMetaFilters.md
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalDomainsResponse.md
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalDomainsResponseAllOf.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalFieldAggregateResponse.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalFieldAggregateResponseAllOf.md
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalFieldResponse.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalFieldResponseDataField.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalFieldResults.md
--rw-r--r--   0        0        0    27230 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalFieldResultsAttributes.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalFieldResultsAttributesAdditional.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalMeta.md
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalOriginsResponse.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalOriginsResponseAllOf.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalRegionsResponse.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalRegionsResponseAllOf.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalResponse.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalResponseDataField.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalResults.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalService.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalServices.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalUsageAggregateResponse.md
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalUsageMonthResponse.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalUsageMonthResponseAllOf.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalUsageMonthResponseData.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalUsageResults.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalUsageServiceResponse.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HistoricalUsageServiceResponseAllOf.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Http3.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Http3AllOf.md
--rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Http3Api.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HttpResponseFormat.md
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/HttpStreamFormat.md
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamPermission.md
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamPermissionsApi.md
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamRole.md
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamRoleAllOf.md
--rw-r--r--   0        0        0    21530 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamRolesApi.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamServiceGroup.md
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamServiceGroupAllOf.md
--rw-r--r--   0        0        0    23819 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamServiceGroupsApi.md
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamUserGroup.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamUserGroupAllOf.md
--rw-r--r--   0        0        0    42765 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IamUserGroupsApi.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IncludedWithWafActiveRule.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IncludedWithWafActiveRuleItem.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IncludedWithWafExclusion.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IncludedWithWafExclusionItem.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IncludedWithWafFirewall.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IncludedWithWafFirewallVersion.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IncludedWithWafFirewallVersionItem.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IncludedWithWafRule.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IncludedWithWafRuleItem.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/IncludedWithWafRuleRevision.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineObject.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineObject1.md
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse200.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse2001.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse2002.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse2003.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse2003Meta.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse2004.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse2004Meta.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse2005.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse2006.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse2007.md
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InlineResponse400.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Invitation.md
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InvitationData.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InvitationDataAttributes.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InvitationResponse.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InvitationResponseAllOf.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InvitationResponseData.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InvitationResponseDataAllOf.md
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InvitationsApi.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InvitationsResponse.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/InvitationsResponseAllOf.md
--rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/KvStoreApi.md
--rw-r--r--   0        0        0    12230 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/KvStoreItemApi.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafConfigurationSet.md
--rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafConfigurationSetsApi.md
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafFirewall.md
--rw-r--r--   0        0        0    28708 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafFirewallApi.md
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafOwasp.md
--rw-r--r--   0        0        0    10002 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafOwaspApi.md
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafRule.md
--rw-r--r--   0        0        0    13782 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafRuleApi.md
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafRuleStatus.md
--rw-r--r--   0        0        0    17124 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafRuleStatusApi.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafRuleset.md
--rw-r--r--   0        0        0     9577 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafRulesetApi.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafTag.md
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafTagApi.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafUpdateStatus.md
--rw-r--r--   0        0        0     7262 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LegacyWafUpdateStatusApi.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingAddressAndPort.md
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingAzureblob.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingAzureblobAllOf.md
--rw-r--r--   0        0        0    29125 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingAzureblobApi.md
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingAzureblobResponse.md
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingBigquery.md
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingBigqueryAllOf.md
--rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingBigqueryApi.md
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingBigqueryResponse.md
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingCloudfiles.md
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingCloudfilesAllOf.md
--rw-r--r--   0        0        0    27524 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingCloudfilesApi.md
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingCloudfilesResponse.md
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingCommon.md
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingDatadog.md
--rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingDatadogAllOf.md
--rw-r--r--   0        0        0    38955 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingDatadogApi.md
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingDatadogResponse.md
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingDigitalocean.md
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingDigitaloceanAllOf.md
--rw-r--r--   0        0        0    28174 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingDigitaloceanApi.md
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingDigitaloceanResponse.md
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingElasticsearch.md
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingElasticsearchAllOf.md
--rw-r--r--   0        0        0    30259 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingElasticsearchApi.md
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingElasticsearchResponse.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingFormatVersion.md
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingFtp.md
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingFtpAllOf.md
--rw-r--r--   0        0        0    27244 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingFtpApi.md
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingFtpResponse.md
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingGcs.md
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingGcsAllOf.md
--rw-r--r--   0        0        0    28487 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingGcsApi.md
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingGcsCommon.md
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingGcsResponse.md
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingGenericCommon.md
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingGooglePubsub.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingGooglePubsubAllOf.md
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingGooglePubsubResponse.md
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHeroku.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHerokuAllOf.md
--rw-r--r--   0        0        0    21127 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHerokuApi.md
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHerokuResponse.md
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHoneycomb.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHoneycombAllOf.md
--rw-r--r--   0        0        0    20986 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHoneycombApi.md
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHoneycombResponse.md
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHttps.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHttpsAllOf.md
--rw-r--r--   0        0        0    29036 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHttpsApi.md
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingHttpsResponse.md
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingKafka.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingKafkaAllOf.md
--rw-r--r--   0        0        0    21774 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingKafkaApi.md
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingKafkaResponse.md
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingKinesis.md
--rw-r--r--   0        0        0    20420 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingKinesisApi.md
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingKinesisResponse.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogentries.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogentriesAllOf.md
--rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogentriesApi.md
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogentriesResponse.md
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLoggly.md
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogglyAllOf.md
--rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogglyApi.md
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogglyResponse.md
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogshuttle.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogshuttleAllOf.md
--rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogshuttleApi.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingLogshuttleResponse.md
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingMessageType.md
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingNewrelic.md
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingNewrelicAllOf.md
--rw-r--r--   0        0        0    25794 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingNewrelicApi.md
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingNewrelicResponse.md
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingOpenstack.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingOpenstackAllOf.md
--rw-r--r--   0        0        0    27216 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingOpenstackApi.md
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingOpenstackResponse.md
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingPapertrail.md
--rw-r--r--   0        0        0    21189 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingPapertrailApi.md
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingPapertrailResponse.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingPlacement.md
--rw-r--r--   0        0        0    24358 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingPubsubApi.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingRequestCapsCommon.md
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingS3.md
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingS3AllOf.md
--rw-r--r--   0        0        0    31697 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingS3Api.md
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingS3Response.md
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingScalyr.md
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingScalyrAllOf.md
--rw-r--r--   0        0        0    21715 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingScalyrApi.md
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingScalyrResponse.md
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSftp.md
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSftpAllOf.md
--rw-r--r--   0        0        0    28475 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSftpApi.md
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSftpResponse.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSplunk.md
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSplunkAllOf.md
--rw-r--r--   0        0        0    26444 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSplunkApi.md
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSplunkResponse.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSumologic.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSumologicAllOf.md
--rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSumologicApi.md
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSumologicResponse.md
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSyslog.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSyslogAllOf.md
--rw-r--r--   0        0        0    26805 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSyslogApi.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingSyslogResponse.md
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingTlsCommon.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/LoggingUseTls.md
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Model403Forbidden.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthentication.md
--rw-r--r--   0        0        0    17143 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthenticationApi.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthenticationData.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthenticationDataAttributes.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthenticationResponse.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthenticationResponseAttributes.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthenticationResponseAttributesAllOf.md
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthenticationResponseData.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthenticationResponseDataAllOf.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthenticationsResponse.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/MutualAuthenticationsResponseAllOf.md
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/NumberVersion.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspector.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorDimensions.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorEntry.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorHistorical.md
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorHistoricalApi.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorHistoricalData.md
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorHistoricalMeta.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorHistoricalMetaFilters.md
--rw-r--r--   0        0        0    23594 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorMeasurements.md
--rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorRealtimeApi.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorRealtimeEntry.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorRealtimeEntryRecorded.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorSubsequentRequestTimestamp.md
--rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/OriginInspectorValues.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Package.md
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PackageApi.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PackageMetadata.md
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PackageResponse.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PackageResponseAllOf.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Pagination.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PaginationCursorMeta.md
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PaginationLinks.md
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PaginationMeta.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Permission.md
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Pool.md
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PoolAllOf.md
--rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PoolApi.md
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PoolResponse.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PoolResponseAllOf.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Pop.md
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PopApi.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PopCoordinates.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PublicIpList.md
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PublicIpListApi.md
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PublishApi.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PublishItem.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PublishItemFormats.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PublishRequest.md
--rw-r--r--   0        0        0    14751 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PurgeApi.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PurgeKeys.md
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PurgeKeysResponse.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/PurgeResponse.md
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RateLimiter.md
--rw-r--r--   0        0        0    21841 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RateLimiterApi.md
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RateLimiterResponse.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RateLimiterResponseAllOf.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ReadOnlyCustomerId.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ReadOnlyId.md
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ReadOnlyIdService.md
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ReadOnlyServiceId.md
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ReadOnlyUserId.md
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ReadOnlyVersion.md
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Realtime.md
--rw-r--r--   0        0        0     8759 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RealtimeApi.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RealtimeEntry.md
--rw-r--r--   0        0        0    27361 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RealtimeEntryAggregated.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RealtimeEntryDatacenter.md
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RealtimeEntryRecorded.md
--rw-r--r--   0        0        0    27336 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RealtimeMeasurements.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RecordedTimestamp.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipCommonName.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipCustomer.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipCustomerCustomer.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberCustomer.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberMutualAuthentication.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberService.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberServiceInvitation.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberTlsActivation.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberTlsBulkCertificate.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberTlsCertificate.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberTlsConfiguration.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberTlsDnsRecord.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberTlsDomain.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberTlsPrivateKey.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberTlsSubscription.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberWafActiveRule.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberWafFirewall.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberWafFirewallVersion.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberWafRule.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberWafRuleRevision.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMemberWafTag.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMutualAuthentication.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMutualAuthenticationMutualAuthentication.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMutualAuthentications.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipMutualAuthenticationsMutualAuthentications.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipService.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipServiceInvitations.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipServiceInvitationsCreate.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipServiceInvitationsCreateServiceInvitations.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipServiceInvitationsServiceInvitations.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipServices.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipServicesServices.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsActivation.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsActivationTlsActivation.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsActivations.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsBulkCertificate.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsBulkCertificates.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsCertificate.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsCertificateTlsCertificate.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsCertificates.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsCertificatesTlsCertificates.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsConfiguration.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsConfigurationForTlsSubscription.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsConfigurationTlsConfiguration.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsConfigurations.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsConfigurationsTlsConfigurations.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsDnsRecord.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsDnsRecordDnsRecord.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsDnsRecords.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsDomain.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsDomainTlsDomain.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsDomains.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsDomainsTlsDomains.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsPrivateKey.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsPrivateKeys.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsSubscription.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsSubscriptionTlsSubscription.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipTlsSubscriptions.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipUser.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipUserUser.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafActiveRules.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafActiveRulesWafActiveRules.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafFirewall.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafFirewallVersion.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafFirewallVersionWafFirewallVersion.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafFirewallVersions.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafFirewallWafFirewall.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafRule.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafRuleRevision.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafRuleRevisionWafRuleRevisions.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafRuleRevisions.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafRuleWafRule.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafRules.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafTags.md
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipWafTagsWafTags.md
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForInvitation.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForMutualAuthentication.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForStar.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForTlsActivation.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForTlsBulkCertificate.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForTlsConfiguration.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForTlsDomain.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForTlsPrivateKey.md
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForTlsSubscription.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForWafActiveRule.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForWafExclusion.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForWafFirewallVersion.md
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RelationshipsForWafRule.md
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RequestSettings.md
--rw-r--r--   0        0        0    18477 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RequestSettingsApi.md
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RequestSettingsResponse.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Resource.md
--rw-r--r--   0        0        0    15552 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ResourceApi.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ResourceResponse.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ResourceResponseAllOf.md
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ResponseObject.md
--rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ResponseObjectApi.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ResponseObjectResponse.md
--rw-r--r--   0        0        0    27224 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Results.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/RoleUser.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SchemasContactResponse.md
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SchemasSnippetResponse.md
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SchemasUserResponse.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SchemasVclResponse.md
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SchemasVersion.md
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SchemasVersionResponse.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SchemasWafFirewallVersion.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SchemasWafFirewallVersionData.md
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Secret.md
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SecretResponse.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SecretStore.md
--rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SecretStoreApi.md
--rw-r--r--   0        0        0    18545 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SecretStoreItemApi.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SecretStoreResponse.md
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Server.md
--rw-r--r--   0        0        0    19968 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServerApi.md
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServerResponse.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServerResponseAllOf.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Service.md
--rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceApi.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorization.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationData.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationDataAttributes.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationDataRelationships.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationDataRelationshipsUser.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationDataRelationshipsUserData.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationResponse.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationResponseData.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationResponseDataAllOf.md
--rw-r--r--   0        0        0    21776 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationsApi.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationsResponse.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceAuthorizationsResponseAllOf.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceCreate.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceCreateAllOf.md
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceDetail.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceDetailAllOf.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceIdAndVersion.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceInvitation.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceInvitationData.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceInvitationDataAttributes.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceInvitationDataRelationships.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceInvitationResponse.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceInvitationResponseAllOf.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceInvitationResponseAllOfData.md
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceListResponse.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceListResponseAllOf.md
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceResponse.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceResponseAllOf.md
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceVersionDetail.md
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ServiceVersionDetailOrNull.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Settings.md
--rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SettingsApi.md
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SettingsResponse.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SigningKey.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Snippet.md
--rw-r--r--   0        0        0    22311 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SnippetApi.md
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SnippetResponse.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SnippetResponseAllOf.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Star.md
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/StarApi.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/StarData.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/StarResponse.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/StarResponseAllOf.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Stats.md
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/StatsApi.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Store.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/StoreResponse.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SubsequentRequestTimestamp.md
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SudoApi.md
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SudoGenericTokenError.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SudoRequest.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/SudoResponse.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Timestamps.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TimestampsNoDelete.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsActivation.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsActivationData.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsActivationResponse.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsActivationResponseData.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsActivationResponseDataAllOf.md
--rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsActivationsApi.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsActivationsResponse.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsActivationsResponseAllOf.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificate.md
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificateData.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificateDataAttributes.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificateResponse.md
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificateResponseAttributes.md
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificateResponseAttributesAllOf.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificateResponseData.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificateResponseDataAllOf.md
--rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificatesApi.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificatesResponse.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsBulkCertificatesResponseAllOf.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificate.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificateData.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificateDataAttributes.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificateResponse.md
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificateResponseAttributes.md
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificateResponseAttributesAllOf.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificateResponseData.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificateResponseDataAllOf.md
--rw-r--r--   0        0        0    17205 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificatesApi.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificatesResponse.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCertificatesResponseAllOf.md
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsCommon.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfiguration.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfigurationData.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfigurationDataAttributes.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfigurationResponse.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfigurationResponseAttributes.md
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfigurationResponseAttributesAllOf.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfigurationResponseData.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfigurationResponseDataAllOf.md
--rw-r--r--   0        0        0    10339 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfigurationsApi.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfigurationsResponse.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsConfigurationsResponseAllOf.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsDnsRecord.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsDomainData.md
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsDomainsApi.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsDomainsResponse.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsDomainsResponseAllOf.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsPrivateKey.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsPrivateKeyData.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsPrivateKeyDataAttributes.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsPrivateKeyResponse.md
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsPrivateKeyResponseAttributes.md
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsPrivateKeyResponseAttributesAllOf.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsPrivateKeyResponseData.md
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsPrivateKeysApi.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsPrivateKeysResponse.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsPrivateKeysResponseAllOf.md
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscription.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscriptionData.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscriptionDataAttributes.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscriptionResponse.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscriptionResponseAttributes.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscriptionResponseAttributesAllOf.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscriptionResponseData.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscriptionResponseDataAllOf.md
--rw-r--r--   0        0        0    26148 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscriptionsApi.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscriptionsResponse.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TlsSubscriptionsResponseAllOf.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Token.md
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TokenCreatedResponse.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TokenCreatedResponseAllOf.md
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TokenResponse.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TokenResponseAllOf.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TokensAdditionalProps.md
--rw-r--r--   0        0        0    20100 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TokensApi.md
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TokensData.md
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeBillingAddress.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeContact.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeCustomer.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeEvent.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeInvitation.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeMutualAuthentication.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeResource.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeService.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeServiceAuthorization.md
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeServiceInvitation.md
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeStar.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeTlsActivation.md
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeTlsBulkCertificate.md
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeTlsCertificate.md
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeTlsConfiguration.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeTlsDnsRecord.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeTlsDomain.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeTlsPrivateKey.md
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeTlsSubscription.md
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeUser.md
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeWafActiveRule.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeWafExclusion.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeWafFirewall.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeWafFirewallVersion.md
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeWafRule.md
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeWafRuleRevision.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/TypeWafTag.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/UpdateBillingAddressRequest.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/UpdateBillingAddressRequestData.md
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/User.md
--rw-r--r--   0        0        0    20765 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/UserApi.md
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/UserResponse.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/UserResponseAllOf.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ValidatorResult.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ValidatorResultData.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ValidatorResultDataAttributes.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/ValidatorResultDataAttributesMessages.md
--rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Values.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Vcl.md
--rw-r--r--   0        0        0    38853 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VclApi.md
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VclDiff.md
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VclDiffApi.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VclResponse.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VclSyntaxHighlightingResponse.md
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/Version.md
--rw-r--r--   0        0        0    26131 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VersionApi.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VersionCreateResponse.md
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VersionDetail.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VersionDetailSettings.md
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VersionResponse.md
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/VersionResponseAllOf.md
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRule.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRuleCreationResponse.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRuleData.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRuleDataAttributes.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRuleResponse.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRuleResponseData.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRuleResponseDataAllOf.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRuleResponseDataAttributes.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRuleResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRuleResponseDataRelationships.md
--rw-r--r--   0        0        0    31218 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRulesApi.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRulesResponse.md
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafActiveRulesResponseAllOf.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusion.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionData.md
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionDataAttributes.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionResponse.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionResponseData.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionResponseDataAllOf.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionResponseDataAttributes.md
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionResponseDataRelationships.md
--rw-r--r--   0        0        0    19155 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionsApi.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionsResponse.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafExclusionsResponseAllOf.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewall.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallData.md
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallDataAttributes.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallResponse.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallResponseData.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallResponseDataAllOf.md
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallResponseDataAttributes.md
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersion.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersionData.md
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersionDataAttributes.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersionResponse.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersionResponseData.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersionResponseDataAllOf.md
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersionResponseDataAttributes.md
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersionResponseDataAttributesAllOf.md
--rw-r--r--   0        0        0    24852 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersionsApi.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersionsResponse.md
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallVersionsResponseAllOf.md
--rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallsApi.md
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallsResponse.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafFirewallsResponseAllOf.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRule.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleAttributes.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleResponse.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleResponseData.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleResponseDataAllOf.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleRevision.md
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleRevisionAttributes.md
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleRevisionOrLatest.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleRevisionResponse.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleRevisionResponseData.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleRevisionResponseDataAllOf.md
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleRevisionsApi.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleRevisionsResponse.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRuleRevisionsResponseAllOf.md
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRulesApi.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRulesResponse.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafRulesResponseAllOf.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafTag.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafTagAttributes.md
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafTagsApi.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafTagsResponse.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafTagsResponseAllOf.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WafTagsResponseDataItem.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-3.0.0/docs/WsMessageFormat.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/__init__.py
--rw-r--r--   0        0        0    39346 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api_client.py
--rw-r--r--   0        0        0    18987 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/configuration.py
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/exceptions.py
--rw-r--r--   0        0        0    82616 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model_utils.py
--rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/rest.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/__init__.py
--rw-r--r--   0        0        0    30565 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/acl_api.py
--rw-r--r--   0        0        0    37416 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/acl_entry_api.py
--rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/apex_redirect_api.py
--rw-r--r--   0        0        0    27130 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/automation_tokens_api.py
--rw-r--r--   0        0        0    54123 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/backend_api.py
--rw-r--r--   0        0        0    22509 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/billing_address_api.py
--rw-r--r--   0        0        0    18589 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/billing_api.py
--rw-r--r--   0        0        0    34253 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/cache_settings_api.py
--rw-r--r--   0        0        0    34233 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/condition_api.py
--rw-r--r--   0        0        0    36809 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/config_store_api.py
--rw-r--r--   0        0        0    42045 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/config_store_item_api.py
--rw-r--r--   0        0        0    19255 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/contact_api.py
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/content_api.py
--rw-r--r--   0        0        0    34431 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/customer_api.py
--rw-r--r--   0        0        0    31732 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/dictionary_api.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/dictionary_info_api.py
--rw-r--r--   0        0        0    46055 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/dictionary_item_api.py
--rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/diff_api.py
--rw-r--r--   0        0        0    32761 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/director_api.py
--rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/director_backend_api.py
--rw-r--r--   0        0        0    42736 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/domain_api.py
--rw-r--r--   0        0        0    10883 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/domain_inspector_historical_api.py
--rw-r--r--   0        0        0    18137 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/domain_inspector_realtime_api.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/domain_ownerships_api.py
--rw-r--r--   0        0        0    17704 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/enabled_products_api.py
--rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/events_api.py
--rw-r--r--   0        0        0    32656 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/gzip_api.py
--rw-r--r--   0        0        0    38546 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/header_api.py
--rw-r--r--   0        0        0    37114 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/healthcheck_api.py
--rw-r--r--   0        0        0    60468 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/historical_api.py
--rw-r--r--   0        0        0    19550 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/http3_api.py
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/iam_permissions_api.py
--rw-r--r--   0        0        0    42584 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/iam_roles_api.py
--rw-r--r--   0        0        0    44500 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/iam_service_groups_api.py
--rw-r--r--   0        0        0    77824 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/iam_user_groups_api.py
--rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/invitations_api.py
--rw-r--r--   0        0        0    21168 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/kv_store_api.py
--rw-r--r--   0        0        0    24533 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/kv_store_item_api.py
--rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/legacy_waf_configuration_sets_api.py
--rw-r--r--   0        0        0    50116 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/legacy_waf_firewall_api.py
--rw-r--r--   0        0        0    18781 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/legacy_waf_owasp_api.py
--rw-r--r--   0        0        0    25207 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/legacy_waf_rule_api.py
--rw-r--r--   0        0        0    29074 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/legacy_waf_rule_status_api.py
--rw-r--r--   0        0        0    18667 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/legacy_waf_ruleset_api.py
--rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/legacy_waf_tag_api.py
--rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/legacy_waf_update_status_api.py
--rw-r--r--   0        0        0    45445 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_azureblob_api.py
--rw-r--r--   0        0        0    40102 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_bigquery_api.py
--rw-r--r--   0        0        0    45152 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_cloudfiles_api.py
--rw-r--r--   0        0        0    42863 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_datadog_api.py
--rw-r--r--   0        0        0    44606 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_digitalocean_api.py
--rw-r--r--   0        0        0    45229 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_elasticsearch_api.py
--rw-r--r--   0        0        0    44432 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_ftp_api.py
--rw-r--r--   0        0        0    44765 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_gcs_api.py
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_heroku_api.py
--rw-r--r--   0        0        0    36624 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_honeycomb_api.py
--rw-r--r--   0        0        0    46115 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_https_api.py
--rw-r--r--   0        0        0    38597 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_kafka_api.py
--rw-r--r--   0        0        0    34377 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_kinesis_api.py
--rw-r--r--   0        0        0    38489 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_logentries_api.py
--rw-r--r--   0        0        0    36081 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_loggly_api.py
--rw-r--r--   0        0        0    36770 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_logshuttle_api.py
--rw-r--r--   0        0        0    38558 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_newrelic_api.py
--rw-r--r--   0        0        0    44042 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_openstack_api.py
--rw-r--r--   0        0        0    36635 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_papertrail_api.py
--rw-r--r--   0        0        0    39265 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_pubsub_api.py
--rw-r--r--   0        0        0    48777 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_s3_api.py
--rw-r--r--   0        0        0    37469 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_scalyr_api.py
--rw-r--r--   0        0        0    45357 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_sftp_api.py
--rw-r--r--   0        0        0    42255 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_splunk_api.py
--rw-r--r--   0        0        0    36567 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_sumologic_api.py
--rw-r--r--   0        0        0    43033 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/logging_syslog_api.py
--rw-r--r--   0        0        0    28852 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/mutual_authentication_api.py
--rw-r--r--   0        0        0    10862 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/origin_inspector_historical_api.py
--rw-r--r--   0        0        0    18138 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/origin_inspector_realtime_api.py
--rw-r--r--   0        0        0    12896 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/package_api.py
--rw-r--r--   0        0        0    47354 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/pool_api.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/pop_api.py
--rw-r--r--   0        0        0     5863 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/public_ip_list_api.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/publish_api.py
--rw-r--r--   0        0        0    24927 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/purge_api.py
--rw-r--r--   0        0        0    43466 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/rate_limiter_api.py
--rw-r--r--   0        0        0    17852 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/realtime_api.py
--rw-r--r--   0        0        0    34834 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/request_settings_api.py
--rw-r--r--   0        0        0    30490 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/resource_api.py
--rw-r--r--   0        0        0    30298 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/response_object_api.py
--rw-r--r--   0        0        0    30510 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/secret_store_api.py
--rw-r--r--   0        0        0    33761 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/secret_store_item_api.py
--rw-r--r--   0        0        0    35038 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/server_api.py
--rw-r--r--   0        0        0    44324 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/service_api.py
--rw-r--r--   0        0        0    38118 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/service_authorizations_api.py
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/settings_api.py
--rw-r--r--   0        0        0    44770 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/snippet_api.py
--rw-r--r--   0        0        0    20513 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/star_api.py
--rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/stats_api.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/sudo_api.py
--rw-r--r--   0        0        0    29279 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/tls_activations_api.py
--rw-r--r--   0        0        0    28695 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/tls_bulk_certificates_api.py
--rw-r--r--   0        0        0    29585 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/tls_certificates_api.py
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/tls_configurations_api.py
--rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/tls_domains_api.py
--rw-r--r--   0        0        0    22120 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/tls_private_keys_api.py
--rw-r--r--   0        0        0    43908 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/tls_subscriptions_api.py
--rw-r--r--   0        0        0    39861 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/tokens_api.py
--rw-r--r--   0        0        0    40392 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/user_api.py
--rw-r--r--   0        0        0    76536 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/vcl_api.py
--rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/vcl_diff_api.py
--rw-r--r--   0        0        0    51681 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/version_api.py
--rw-r--r--   0        0        0    51904 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/waf_active_rules_api.py
--rw-r--r--   0        0        0    33986 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/waf_exclusions_api.py
--rw-r--r--   0        0        0    36636 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/waf_firewall_versions_api.py
--rw-r--r--   0        0        0    29601 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/waf_firewalls_api.py
--rw-r--r--   0        0        0    13840 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/waf_rule_revisions_api.py
--rw-r--r--   0        0        0    13963 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/waf_rules_api.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/api/waf_tags_api.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/apis/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/__init__.py
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/acl.py
--rw-r--r--   0        0        0    13163 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/acl_entry.py
--rw-r--r--   0        0        0    17362 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/acl_entry_response.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/acl_entry_response_all_of.py
--rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/acl_response.py
--rw-r--r--   0        0        0    12025 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/acl_response_all_of.py
--rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/apex_redirect.py
--rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/apex_redirect_all_of.py
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/automation_token.py
--rw-r--r--   0        0        0    11840 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/automation_token_create_request.py
--rw-r--r--   0        0        0    13264 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/automation_token_create_request_attributes.py
--rw-r--r--   0        0        0    19202 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/automation_token_create_response.py
--rw-r--r--   0        0        0    13953 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/automation_token_create_response_all_of.py
--rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/automation_token_response.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/automation_token_response_all_of.py
--rw-r--r--   0        0        0    14660 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/aws_region.py
--rw-r--r--   0        0        0    26143 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/backend.py
--rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/backend_response.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/backend_response_all_of.py
--rw-r--r--   0        0        0    12338 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/batch.py
--rw-r--r--   0        0        0    12656 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/batch_errors.py
--rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing.py
--rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_address_attributes.py
--rw-r--r--   0        0        0    12075 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_address_request.py
--rw-r--r--   0        0        0    12080 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_address_request_data.py
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_address_response.py
--rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_address_response_data.py
--rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_address_verification_error_response.py
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_address_verification_error_response_errors.py
--rw-r--r--   0        0        0    16877 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_estimate_response.py
--rw-r--r--   0        0        0    11787 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_estimate_response_all_of.py
--rw-r--r--   0        0        0    13188 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_estimate_response_all_of_line.py
--rw-r--r--   0        0        0    11784 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_estimate_response_all_of_lines.py
--rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_response.py
--rw-r--r--   0        0        0    11716 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_response_all_of.py
--rw-r--r--   0        0        0    18617 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_response_line_item.py
--rw-r--r--   0        0        0    15190 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_response_line_item_all_of.py
--rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_status.py
--rw-r--r--   0        0        0    16362 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_total.py
--rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/billing_total_extras.py
--rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/bulk_update_acl_entries_request.py
--rw-r--r--   0        0        0    16005 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/bulk_update_acl_entry.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/bulk_update_acl_entry_all_of.py
--rw-r--r--   0        0        0    14518 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/bulk_update_config_store_item.py
--rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/bulk_update_config_store_item_all_of.py
--rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/bulk_update_config_store_list_request.py
--rw-r--r--   0        0        0    14509 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/bulk_update_dictionary_item.py
--rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/bulk_update_dictionary_list_request.py
--rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/bulk_waf_active_rule.py
--rw-r--r--   0        0        0    11638 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/bulk_waf_active_rules.py
--rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/cache_setting.py
--rw-r--r--   0        0        0    17524 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/cache_setting_response.py
--rw-r--r--   0        0        0    12661 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/client_key.py
--rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/condition.py
--rw-r--r--   0        0        0    16896 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/condition_response.py
--rw-r--r--   0        0        0    11911 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/conditions_response.py
--rw-r--r--   0        0        0    11444 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/config_store.py
--rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/config_store_info_response.py
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/config_store_item.py
--rw-r--r--   0        0        0    15611 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/config_store_item_response.py
--rw-r--r--   0        0        0    11487 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/config_store_item_response_all_of.py
--rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/config_store_response.py
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/config_store_response_all_of.py
--rw-r--r--   0        0        0    13577 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/contact.py
--rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/contact_response.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/contact_response_all_of.py
--rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/content.py
--rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/customer.py
--rw-r--r--   0        0        0    24131 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/customer_response.py
--rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/customer_response_all_of.py
--rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/dictionary.py
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/dictionary_info_response.py
--rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/dictionary_item.py
--rw-r--r--   0        0        0    15870 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/dictionary_item_response.py
--rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/dictionary_item_response_all_of.py
--rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/dictionary_response.py
--rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/dictionary_response_all_of.py
--rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/diff_response.py
--rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/director.py
--rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/director_backend.py
--rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/director_backend_all_of.py
--rw-r--r--   0        0        0    18553 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/director_response.py
--rw-r--r--   0        0        0    11783 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain.py
--rw-r--r--   0        0        0    13972 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain_check_item.py
--rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain_check_response.py
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain_check_response_list.py
--rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain_inspector.py
--rw-r--r--   0        0        0    12175 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain_inspector_entry.py
--rw-r--r--   0        0        0    12647 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain_inspector_entry_dimensions.py
--rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain_inspector_entry_values.py
--rw-r--r--   0        0        0    34374 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain_inspector_measurements.py
--rw-r--r--   0        0        0    13220 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain_inspector_realtime_entry.py
--rw-r--r--   0        0        0    15770 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domain_response.py
--rw-r--r--   0        0        0    11875 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/domains_response.py
--rw-r--r--   0        0        0    12604 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/enabled_product_response.py
--rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/enabled_product_response_links.py
--rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/enabled_product_response_product.py
--rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/enabled_product_response_service.py
--rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/error_response.py
--rw-r--r--   0        0        0    12088 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/event.py
--rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/event_attributes.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/event_data.py
--rw-r--r--   0        0        0    11790 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/event_data_items.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/event_response.py
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/events_response.py
--rw-r--r--   0        0        0    11395 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/generic_token_error.py
--rw-r--r--   0        0        0    12758 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/gzip.py
--rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/gzip_response.py
--rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/header.py
--rw-r--r--   0        0        0    19828 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/header_response.py
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/healthcheck.py
--rw-r--r--   0        0        0    18979 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/healthcheck_response.py
--rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical.py
--rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_aggregate_response.py
--rw-r--r--   0        0        0    11672 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_aggregate_response_all_of.py
--rw-r--r--   0        0        0    12972 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_domains.py
--rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_domains_data.py
--rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_domains_meta.py
--rw-r--r--   0        0        0    11839 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_domains_meta_filters.py
--rw-r--r--   0        0        0    15324 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_domains_response.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_domains_response_all_of.py
--rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_field_aggregate_response.py
--rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_field_aggregate_response_all_of.py
--rw-r--r--   0        0        0    15024 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_field_response.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_field_response_data_field.py
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_field_results.py
--rw-r--r--   0        0        0   100346 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_field_results_attributes.py
--rw-r--r--   0        0        0    11942 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_field_results_attributes_additional.py
--rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_meta.py
--rw-r--r--   0        0        0    15432 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_origins_response.py
--rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_origins_response_all_of.py
--rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_regions_response.py
--rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_regions_response_all_of.py
--rw-r--r--   0        0        0    15219 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_response.py
--rw-r--r--   0        0        0    11959 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_response_data_field.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_results.py
--rw-r--r--   0        0        0    11620 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_service.py
--rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_services.py
--rw-r--r--   0        0        0    15037 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_usage_aggregate_response.py
--rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_usage_month_response.py
--rw-r--r--   0        0        0    11783 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_usage_month_response_all_of.py
--rw-r--r--   0        0        0    12331 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_usage_month_response_data.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_usage_results.py
--rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_usage_service_response.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/historical_usage_service_response_all_of.py
--rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/http3.py
--rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/http3_all_of.py
--rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/http_response_format.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/http_stream_format.py
--rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/iam_permission.py
--rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/iam_role.py
--rw-r--r--   0        0        0    12962 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/iam_role_all_of.py
--rw-r--r--   0        0        0    15636 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/iam_service_group.py
--rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/iam_service_group_all_of.py
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/iam_user_group.py
--rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/iam_user_group_all_of.py
--rw-r--r--   0        0        0    12044 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/included_with_waf_active_rule.py
--rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/included_with_waf_active_rule_item.py
--rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/included_with_waf_exclusion.py
--rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/included_with_waf_exclusion_item.py
--rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/included_with_waf_firewall.py
--rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/included_with_waf_firewall_version.py
--rw-r--r--   0        0        0    13972 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/included_with_waf_firewall_version_item.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/included_with_waf_rule.py
--rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/included_with_waf_rule_item.py
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/included_with_waf_rule_revision.py
--rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_object.py
--rw-r--r--   0        0        0    11419 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_object1.py
--rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response200.py
--rw-r--r--   0        0        0    11607 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response2001.py
--rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response2002.py
--rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response2003.py
--rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response2003_meta.py
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response2004.py
--rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response2004_meta.py
--rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response2005.py
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response2006.py
--rw-r--r--   0        0        0    11743 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response2007.py
--rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/inline_response400.py
--rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/invitation.py
--rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/invitation_data.py
--rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/invitation_data_attributes.py
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/invitation_response.py
--rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/invitation_response_all_of.py
--rw-r--r--   0        0        0    14895 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/invitation_response_data.py
--rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/invitation_response_data_all_of.py
--rw-r--r--   0        0        0    14597 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/invitations_response.py
--rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/invitations_response_all_of.py
--rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/legacy_waf_configuration_set.py
--rw-r--r--   0        0        0    14430 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/legacy_waf_firewall.py
--rw-r--r--   0        0        0    23898 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/legacy_waf_owasp.py
--rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/legacy_waf_rule.py
--rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/legacy_waf_rule_status.py
--rw-r--r--   0        0        0    11777 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/legacy_waf_ruleset.py
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/legacy_waf_tag.py
--rw-r--r--   0        0        0    13049 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/legacy_waf_update_status.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_address_and_port.py
--rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_azureblob.py
--rw-r--r--   0        0        0    14206 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_azureblob_all_of.py
--rw-r--r--   0        0        0    24022 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_azureblob_response.py
--rw-r--r--   0        0        0    19390 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_bigquery.py
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_bigquery_all_of.py
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_bigquery_response.py
--rw-r--r--   0        0        0    21831 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_cloudfiles.py
--rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_cloudfiles_all_of.py
--rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_cloudfiles_response.py
--rw-r--r--   0        0        0    14144 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_common.py
--rw-r--r--   0        0        0    23211 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_datadog.py
--rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_datadog_all_of.py
--rw-r--r--   0        0        0    24914 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_datadog_response.py
--rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_digitalocean.py
--rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_digitalocean_all_of.py
--rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_digitalocean_response.py
--rw-r--r--   0        0        0    22734 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_elasticsearch.py
--rw-r--r--   0        0        0    14289 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_elasticsearch_all_of.py
--rw-r--r--   0        0        0    24096 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_elasticsearch_response.py
--rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_format_version.py
--rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_ftp.py
--rw-r--r--   0        0        0    13770 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_ftp_all_of.py
--rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_ftp_response.py
--rw-r--r--   0        0        0    22679 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_gcs.py
--rw-r--r--   0        0        0    12744 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_gcs_all_of.py
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_gcs_common.py
--rw-r--r--   0        0        0    24062 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_gcs_response.py
--rw-r--r--   0        0        0    14090 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_generic_common.py
--rw-r--r--   0        0        0    18898 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_google_pubsub.py
--rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_google_pubsub_all_of.py
--rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_google_pubsub_response.py
--rw-r--r--   0        0        0    17238 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_heroku.py
--rw-r--r--   0        0        0    11999 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_heroku_all_of.py
--rw-r--r--   0        0        0    18941 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_heroku_response.py
--rw-r--r--   0        0        0    17018 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_honeycomb.py
--rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_honeycomb_all_of.py
--rw-r--r--   0        0        0    18721 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_honeycomb_response.py
--rw-r--r--   0        0        0    23100 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_https.py
--rw-r--r--   0        0        0    15781 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_https_all_of.py
--rw-r--r--   0        0        0    24462 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_https_response.py
--rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_kafka.py
--rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_kafka_all_of.py
--rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_kafka_response.py
--rw-r--r--   0        0        0    16368 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_kinesis.py
--rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_kinesis_response.py
--rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_logentries.py
--rw-r--r--   0        0        0    12851 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_logentries_all_of.py
--rw-r--r--   0        0        0    19749 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_logentries_response.py
--rw-r--r--   0        0        0    16993 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_loggly.py
--rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_loggly_all_of.py
--rw-r--r--   0        0        0    18696 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_loggly_response.py
--rw-r--r--   0        0        0    17065 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_logshuttle.py
--rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_logshuttle_all_of.py
--rw-r--r--   0        0        0    18768 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_logshuttle_response.py
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_message_type.py
--rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_newrelic.py
--rw-r--r--   0        0        0    14066 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_newrelic_all_of.py
--rw-r--r--   0        0        0    20498 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_newrelic_response.py
--rw-r--r--   0        0        0    21509 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_openstack.py
--rw-r--r--   0        0        0    13226 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_openstack_all_of.py
--rw-r--r--   0        0        0    23042 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_openstack_response.py
--rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_papertrail.py
--rw-r--r--   0        0        0    18776 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_papertrail_response.py
--rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_placement.py
--rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_request_caps_common.py
--rw-r--r--   0        0        0    24622 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_s3.py
--rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_s3_all_of.py
--rw-r--r--   0        0        0    26155 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_s3_response.py
--rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_scalyr.py
--rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_scalyr_all_of.py
--rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_scalyr_response.py
--rw-r--r--   0        0        0    22808 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_sftp.py
--rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_sftp_all_of.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_sftp_response.py
--rw-r--r--   0        0        0    21030 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_splunk.py
--rw-r--r--   0        0        0    12164 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_splunk_all_of.py
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_splunk_response.py
--rw-r--r--   0        0        0    17102 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_sumologic.py
--rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_sumologic_all_of.py
--rw-r--r--   0        0        0    18805 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_sumologic_response.py
--rw-r--r--   0        0        0    21452 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_syslog.py
--rw-r--r--   0        0        0    13046 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_syslog_all_of.py
--rw-r--r--   0        0        0    22829 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_syslog_response.py
--rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_tls_common.py
--rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/logging_use_tls.py
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/model403_forbidden.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/mutual_authentication.py
--rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/mutual_authentication_data.py
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/mutual_authentication_data_attributes.py
--rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/mutual_authentication_response.py
--rw-r--r--   0        0        0    15149 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/mutual_authentication_response_attributes.py
--rw-r--r--   0        0        0    11647 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/mutual_authentication_response_attributes_all_of.py
--rw-r--r--   0        0        0    15368 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/mutual_authentication_response_data.py
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/mutual_authentication_response_data_all_of.py
--rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/mutual_authentications_response.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/mutual_authentications_response_all_of.py
--rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/number_version.py
--rw-r--r--   0        0        0    12795 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector.py
--rw-r--r--   0        0        0    12642 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_dimensions.py
--rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_entry.py
--rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_historical.py
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_historical_data.py
--rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_historical_meta.py
--rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_historical_meta_filters.py
--rw-r--r--   0        0        0    78482 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_measurements.py
--rw-r--r--   0        0        0    13076 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_realtime_entry.py
--rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_realtime_entry_recorded.py
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_subsequent_request_timestamp.py
--rw-r--r--   0        0        0    78464 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/origin_inspector_values.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/package.py
--rw-r--r--   0        0        0    13175 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/package_metadata.py
--rw-r--r--   0        0        0    15990 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/package_response.py
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/package_response_all_of.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/pagination.py
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/pagination_cursor_meta.py
--rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/pagination_links.py
--rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/pagination_meta.py
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/permission.py
--rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/pool.py
--rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/pool_all_of.py
--rw-r--r--   0        0        0    25586 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/pool_response.py
--rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/pool_response_all_of.py
--rw-r--r--   0        0        0    15216 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/pop.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/pop_coordinates.py
--rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/public_ip_list.py
--rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/publish_item.py
--rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/publish_item_formats.py
--rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/publish_request.py
--rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/purge_keys.py
--rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/purge_keys_response.py
--rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/purge_response.py
--rw-r--r--   0        0        0    19010 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/rate_limiter.py
--rw-r--r--   0        0        0    23485 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/rate_limiter_response.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/rate_limiter_response_all_of.py
--rw-r--r--   0        0        0    10950 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/read_only_customer_id.py
--rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/read_only_id.py
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/read_only_id_service.py
--rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/read_only_service_id.py
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/read_only_user_id.py
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/read_only_version.py
--rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/realtime.py
--rw-r--r--   0        0        0    12492 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/realtime_entry.py
--rw-r--r--   0        0        0   100248 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/realtime_entry_aggregated.py
--rw-r--r--   0        0        0    11397 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/realtime_entry_datacenter.py
--rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/realtime_entry_recorded.py
--rw-r--r--   0        0        0    98045 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/realtime_measurements.py
--rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/recorded_timestamp.py
--rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_common_name.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_customer.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_customer_customer.py
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_customer.py
--rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_mutual_authentication.py
--rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_service.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_service_invitation.py
--rw-r--r--   0        0        0    11866 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_tls_activation.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_tls_certificate.py
--rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_tls_configuration.py
--rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_tls_dns_record.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_tls_domain.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_tls_private_key.py
--rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_tls_subscription.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_waf_active_rule.py
--rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_waf_firewall.py
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_waf_firewall_version.py
--rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_waf_rule.py
--rw-r--r--   0        0        0    11995 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_waf_rule_revision.py
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_member_waf_tag.py
--rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_mutual_authentication.py
--rw-r--r--   0        0        0    11881 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_mutual_authentication_mutual_authentication.py
--rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_mutual_authentications.py
--rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_mutual_authentications_mutual_authentications.py
--rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_service.py
--rw-r--r--   0        0        0    11961 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_service_invitations.py
--rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_service_invitations_create.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_service_invitations_create_service_invitations.py
--rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_service_invitations_service_invitations.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_services.py
--rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_services_services.py
--rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_activation.py
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_activation_tls_activation.py
--rw-r--r--   0        0        0    11859 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_activations.py
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_bulk_certificates.py
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_certificate.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_certificate_tls_certificate.py
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_certificates.py
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_certificates_tls_certificates.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_configuration.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_configuration_for_tls_subscription.py
--rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_configuration_tls_configuration.py
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_configurations.py
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_configurations_tls_configurations.py
--rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_dns_record.py
--rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_dns_record_dns_record.py
--rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_dns_records.py
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_domain.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_domain_tls_domain.py
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_domains.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_domains_tls_domains.py
--rw-r--r--   0        0        0    11858 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_private_key.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_private_key_tls_private_key.py
--rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_private_keys.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_private_keys_tls_private_keys.py
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_subscription.py
--rw-r--r--   0        0        0    11822 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_subscription_tls_subscription.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_tls_subscriptions.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_user.py
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_user_user.py
--rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_active_rules.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_active_rules_waf_active_rules.py
--rw-r--r--   0        0        0    11807 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_firewall.py
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_firewall_version.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_firewall_versions.py
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_firewall_waf_firewall.py
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_rule.py
--rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_rule_revision.py
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_rule_revisions.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_rule_waf_rule.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_rules.py
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_tags.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationship_waf_tags_waf_tags.py
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_invitation.py
--rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_mutual_authentication.py
--rw-r--r--   0        0        0    14345 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_star.py
--rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_tls_activation.py
--rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_tls_configuration.py
--rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_tls_domain.py
--rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_tls_private_key.py
--rw-r--r--   0        0        0    16266 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_tls_subscription.py
--rw-r--r--   0        0        0    14951 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_waf_active_rule.py
--rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_waf_exclusion.py
--rw-r--r--   0        0        0    14940 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_waf_firewall_version.py
--rw-r--r--   0        0        0    14666 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/relationships_for_waf_rule.py
--rw-r--r--   0        0        0    15858 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/request_settings.py
--rw-r--r--   0        0        0    19891 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/request_settings_response.py
--rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/resource.py
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/resource_response.py
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/resource_response_all_of.py
--rw-r--r--   0        0        0    13673 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/response_object.py
--rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/response_object_response.py
--rw-r--r--   0        0        0    97280 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/results.py
--rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/role_user.py
--rw-r--r--   0        0        0    17321 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/schemas_contact_response.py
--rw-r--r--   0        0        0    17535 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/schemas_snippet_response.py
--rw-r--r--   0        0        0    18068 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/schemas_user_response.py
--rw-r--r--   0        0        0    15953 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/schemas_vcl_response.py
--rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/schemas_version.py
--rw-r--r--   0        0        0    17433 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/schemas_version_response.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/schemas_waf_firewall_version.py
--rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/schemas_waf_firewall_version_data.py
--rw-r--r--   0        0        0    12644 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/secret.py
--rw-r--r--   0        0        0    12598 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/secret_response.py
--rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/secret_store.py
--rw-r--r--   0        0        0    12048 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/secret_store_response.py
--rw-r--r--   0        0        0    14569 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/server.py
--rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/server_response.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/server_response_all_of.py
--rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorization.py
--rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorization_data.py
--rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorization_data_attributes.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorization_data_relationships.py
--rw-r--r--   0        0        0    11899 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorization_data_relationships_user.py
--rw-r--r--   0        0        0    11844 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorization_data_relationships_user_data.py
--rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorization_response.py
--rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorization_response_data.py
--rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorization_response_data_all_of.py
--rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorizations_response.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_authorizations_response_all_of.py
--rw-r--r--   0        0        0    14640 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_create.py
--rw-r--r--   0        0        0    11543 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_create_all_of.py
--rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_detail.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_detail_all_of.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_id_and_version.py
--rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_invitation.py
--rw-r--r--   0        0        0    12646 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_invitation_data.py
--rw-r--r--   0        0        0    11922 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_invitation_data_attributes.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_invitation_data_relationships.py
--rw-r--r--   0        0        0    14111 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_invitation_response.py
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_invitation_response_all_of.py
--rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_invitation_response_all_of_data.py
--rw-r--r--   0        0        0    17024 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_list_response.py
--rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_list_response_all_of.py
--rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_response.py
--rw-r--r--   0        0        0    12948 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_response_all_of.py
--rw-r--r--   0        0        0    23835 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_version_detail.py
--rw-r--r--   0        0        0    23852 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/service_version_detail_or_null.py
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/settings.py
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/settings_response.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/signing_key.py
--rw-r--r--   0        0        0    13181 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/snippet.py
--rw-r--r--   0        0        0    17514 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/snippet_response.py
--rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/snippet_response_all_of.py
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/star.py
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/star_data.py
--rw-r--r--   0        0        0    13825 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/star_response.py
--rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/star_response_all_of.py
--rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/stats.py
--rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/store.py
--rw-r--r--   0        0        0    11668 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/store_response.py
--rw-r--r--   0        0        0    11249 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/subsequent_request_timestamp.py
--rw-r--r--   0        0        0    11407 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/sudo_generic_token_error.py
--rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/sudo_request.py
--rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/sudo_response.py
--rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/timestamps.py
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/timestamps_no_delete.py
--rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_activation.py
--rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_activation_data.py
--rw-r--r--   0        0        0    11697 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_activation_response.py
--rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_activation_response_data.py
--rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_activation_response_data_all_of.py
--rw-r--r--   0        0        0    14644 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_activations_response.py
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_activations_response_all_of.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_bulk_certificate.py
--rw-r--r--   0        0        0    12666 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_bulk_certificate_data.py
--rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_bulk_certificate_data_attributes.py
--rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_bulk_certificate_response.py
--rw-r--r--   0        0        0    16192 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_bulk_certificate_response_attributes.py
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_bulk_certificate_response_attributes_all_of.py
--rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_bulk_certificate_response_data.py
--rw-r--r--   0        0        0    12043 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_bulk_certificate_response_data_all_of.py
--rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_bulk_certificates_response.py
--rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_bulk_certificates_response_all_of.py
--rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_certificate.py
--rw-r--r--   0        0        0    12510 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_certificate_data.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_certificate_data_attributes.py
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_certificate_response.py
--rw-r--r--   0        0        0    17609 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_certificate_response_attributes.py
--rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_certificate_response_attributes_all_of.py
--rw-r--r--   0        0        0    15107 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_certificate_response_data.py
--rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_certificate_response_data_all_of.py
--rw-r--r--   0        0        0    14659 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_certificates_response.py
--rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_certificates_response_all_of.py
--rw-r--r--   0        0        0    13892 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_common.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_configuration.py
--rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_configuration_data.py
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_configuration_data_attributes.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_configuration_response.py
--rw-r--r--   0        0        0    16408 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_configuration_response_attributes.py
--rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_configuration_response_attributes_all_of.py
--rw-r--r--   0        0        0    15232 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_configuration_response_data.py
--rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_configuration_response_data_all_of.py
--rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_configurations_response.py
--rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_configurations_response_all_of.py
--rw-r--r--   0        0        0    13196 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_dns_record.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_domain_data.py
--rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_domains_response.py
--rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_domains_response_all_of.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_private_key.py
--rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_private_key_data.py
--rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_private_key_data_attributes.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_private_key_response.py
--rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_private_key_response_attributes.py
--rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_private_key_response_attributes_all_of.py
--rw-r--r--   0        0        0    12321 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_private_key_response_data.py
--rw-r--r--   0        0        0    14646 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_private_keys_response.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_private_keys_response_all_of.py
--rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_subscription.py
--rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_subscription_data.py
--rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_subscription_data_attributes.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_subscription_response.py
--rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_subscription_response_attributes.py
--rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_subscription_response_attributes_all_of.py
--rw-r--r--   0        0        0    14191 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_subscription_response_data.py
--rw-r--r--   0        0        0    12012 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_subscription_response_data_all_of.py
--rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_subscriptions_response.py
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tls_subscriptions_response_all_of.py
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/token.py
--rw-r--r--   0        0        0    18055 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/token_created_response.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/token_created_response_all_of.py
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/token_response.py
--rw-r--r--   0        0        0    13237 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/token_response_all_of.py
--rw-r--r--   0        0        0    11233 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tokens_additional_props.py
--rw-r--r--   0        0        0    11974 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/tokens_data.py
--rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_billing_address.py
--rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_contact.py
--rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_customer.py
--rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_event.py
--rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_invitation.py
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_mutual_authentication.py
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_resource.py
--rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_service.py
--rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_service_authorization.py
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_service_invitation.py
--rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_star.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_tls_activation.py
--rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_tls_bulk_certificate.py
--rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_tls_certificate.py
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_tls_configuration.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_tls_dns_record.py
--rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_tls_domain.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_tls_private_key.py
--rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_tls_subscription.py
--rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_user.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_waf_active_rule.py
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_waf_exclusion.py
--rw-r--r--   0        0        0    11692 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_waf_firewall.py
--rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_waf_firewall_version.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_waf_rule.py
--rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_waf_rule_revision.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/type_waf_tag.py
--rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/update_billing_address_request.py
--rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/update_billing_address_request_data.py
--rw-r--r--   0        0        0    13820 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/user.py
--rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/user_response.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/user_response_all_of.py
--rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/validator_result.py
--rw-r--r--   0        0        0    12095 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/validator_result_data.py
--rw-r--r--   0        0        0    12712 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/validator_result_data_attributes.py
--rw-r--r--   0        0        0    12341 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/validator_result_data_attributes_messages.py
--rw-r--r--   0        0        0    34311 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/values.py
--rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/vcl.py
--rw-r--r--   0        0        0    12644 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/vcl_diff.py
--rw-r--r--   0        0        0    15932 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/vcl_response.py
--rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/vcl_syntax_highlighting_response.py
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/version.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/version_create_response.py
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/version_detail.py
--rw-r--r--   0        0        0    12978 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/version_detail_settings.py
--rw-r--r--   0        0        0    17376 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/version_response.py
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/version_response_all_of.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rule.py
--rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rule_creation_response.py
--rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rule_data.py
--rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rule_data_attributes.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rule_response.py
--rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rule_response_data.py
--rw-r--r--   0        0        0    12559 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rule_response_data_all_of.py
--rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rule_response_data_attributes.py
--rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rule_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rule_response_data_relationships.py
--rw-r--r--   0        0        0    15066 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rules_response.py
--rw-r--r--   0        0        0    12142 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_active_rules_response_all_of.py
--rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusion.py
--rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusion_data.py
--rw-r--r--   0        0        0    13837 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusion_data_attributes.py
--rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusion_response.py
--rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusion_response_data.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusion_response_data_all_of.py
--rw-r--r--   0        0        0    17359 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusion_response_data_attributes.py
--rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusion_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusion_response_data_relationships.py
--rw-r--r--   0        0        0    15041 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusions_response.py
--rw-r--r--   0        0        0    12123 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_exclusions_response_all_of.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall.py
--rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_data.py
--rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_data_attributes.py
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_response.py
--rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_response_data.py
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_response_data_all_of.py
--rw-r--r--   0        0        0    19383 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_response_data_attributes.py
--rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_version.py
--rw-r--r--   0        0        0    12158 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_version_data.py
--rw-r--r--   0        0        0    24857 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_version_data_attributes.py
--rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_version_response.py
--rw-r--r--   0        0        0    15440 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_version_response_data.py
--rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_version_response_data_all_of.py
--rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_version_response_data_attributes.py
--rw-r--r--   0        0        0    16832 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_version_response_data_attributes_all_of.py
--rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_versions_response.py
--rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewall_versions_response_all_of.py
--rw-r--r--   0        0        0    15019 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewalls_response.py
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_firewalls_response_all_of.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule.py
--rw-r--r--   0        0        0    12553 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_attributes.py
--rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_response.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_response_data.py
--rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_response_data_all_of.py
--rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_revision.py
--rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_revision_attributes.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_revision_or_latest.py
--rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_revision_response.py
--rw-r--r--   0        0        0    15147 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_revision_response_data.py
--rw-r--r--   0        0        0    11732 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_revision_response_data_all_of.py
--rw-r--r--   0        0        0    15110 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_revisions_response.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rule_revisions_response_all_of.py
--rw-r--r--   0        0        0    14931 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rules_response.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_rules_response_all_of.py
--rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_tag.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_tag_attributes.py
--rw-r--r--   0        0        0    14872 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_tags_response.py
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_tags_response_all_of.py
--rw-r--r--   0        0        0    14941 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/waf_tags_response_data_item.py
--rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/model/ws_message_format.py
--rw-r--r--   0        0        0    50550 2020-02-02 00:00:00.000000 fastly-3.0.0/fastly/models/__init__.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-3.0.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fastly-3.0.0/LICENSE
--rw-r--r--   0        0        0    97528 2020-02-02 00:00:00.000000 fastly-3.0.0/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastly-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    98020 2020-02-02 00:00:00.000000 fastly-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-3.0.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     9041 2020-02-02 00:00:00.000000 fastly-3.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fastly-3.0.1/MANIFEST.in
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-3.0.1/SECURITY.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastly-3.0.1/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastly-3.0.1/setup.cfg
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 fastly-3.0.1/setup.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastly-3.0.1/sig.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 fastly-3.0.1/test-requirements.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastly-3.0.1/tox.ini
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fastly-3.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxr-xr-x   0        0        0      619 2020-02-02 00:00:00.000000 fastly-3.0.1/.github/scripts/pack.sh
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 fastly-3.0.1/.github/scripts/prepare.sh
+-rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 fastly-3.0.1/.github/scripts/publish_env.sh
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 fastly-3.0.1/.github/scripts/release_body.sh
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fastly-3.0.1/.github/workflows/ci-release.yaml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Acl.md
+-rw-r--r--   0        0        0    15695 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AclApi.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AclEntry.md
+-rw-r--r--   0        0        0    20447 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AclEntryApi.md
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AclEntryResponse.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AclEntryResponseAllOf.md
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AclResponse.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AclResponseAllOf.md
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ApexRedirect.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ApexRedirectAllOf.md
+-rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ApexRedirectApi.md
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AutomationToken.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AutomationTokenCreateRequest.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AutomationTokenCreateRequestAttributes.md
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AutomationTokenCreateResponse.md
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AutomationTokenCreateResponseAllOf.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AutomationTokenResponse.md
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AutomationTokenResponseAllOf.md
+-rw-r--r--   0        0        0    15211 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AutomationTokensApi.md
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/AwsRegion.md
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Backend.md
+-rw-r--r--   0        0        0    38268 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BackendApi.md
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BackendResponse.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BackendResponseAllOf.md
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Batch.md
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BatchErrors.md
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Billing.md
+-rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingAddressApi.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingAddressAttributes.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingAddressRequest.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingAddressRequestData.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingAddressResponse.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingAddressResponseData.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingAddressVerificationErrorResponse.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingAddressVerificationErrorResponseErrors.md
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingApi.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingEstimateLines.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingEstimateLinesLineItems.md
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingEstimateResponse.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingResponse.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingResponseItemItemsData.md
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingResponseLineItem.md
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingResponseLineItems.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingStatus.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingTotal.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BillingTotalExtras.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BulkUpdateAclEntriesRequest.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BulkUpdateAclEntry.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BulkUpdateAclEntryAllOf.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BulkUpdateConfigStoreItem.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BulkUpdateConfigStoreItemAllOf.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BulkUpdateConfigStoreListRequest.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BulkUpdateDictionaryItem.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BulkUpdateDictionaryListRequest.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BulkWafActiveRule.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/BulkWafActiveRules.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/CacheSetting.md
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/CacheSettingResponse.md
+-rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/CacheSettingsApi.md
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ClientKey.md
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Condition.md
+-rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConditionApi.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConditionResponse.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConditionsResponse.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConfigStore.md
+-rw-r--r--   0        0        0    18464 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConfigStoreApi.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConfigStoreInfoResponse.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConfigStoreItem.md
+-rw-r--r--   0        0        0    23504 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConfigStoreItemApi.md
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConfigStoreItemResponse.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConfigStoreItemResponseAllOf.md
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConfigStoreResponse.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ConfigStoreResponseAllOf.md
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Contact.md
+-rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ContactApi.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ContactResponse.md
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ContactResponseAllOf.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Content.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ContentApi.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Customer.md
+-rw-r--r--   0        0        0    18926 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/CustomerApi.md
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/CustomerResponse.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/CustomerResponseAllOf.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Dictionary.md
+-rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DictionaryApi.md
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DictionaryInfoApi.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DictionaryInfoResponse.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DictionaryItem.md
+-rw-r--r--   0        0        0    26138 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DictionaryItemApi.md
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DictionaryItemResponse.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DictionaryItemResponseAllOf.md
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DictionaryResponse.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DictionaryResponseAllOf.md
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DiffApi.md
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DiffResponse.md
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Director.md
+-rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DirectorApi.md
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DirectorBackend.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DirectorBackendAllOf.md
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DirectorBackendApi.md
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DirectorResponse.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Domain.md
+-rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainApi.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainCheckItem.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainCheckResponse.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainCheckResponseList.md
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainInspector.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainInspectorEntry.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainInspectorEntryDimensions.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainInspectorEntryValues.md
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainInspectorHistoricalApi.md
+-rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainInspectorMeasurements.md
+-rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainInspectorRealtimeApi.md
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainInspectorRealtimeEntry.md
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainOwnershipsApi.md
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainResponse.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/DomainsResponse.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EnabledProductResponse.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EnabledProductResponseLinks.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EnabledProductResponseProduct.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EnabledProductResponseService.md
+-rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EnabledProductsApi.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ErrorResponse.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Event.md
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EventAttributes.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EventData.md
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EventDataItems.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EventResponse.md
+-rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EventsApi.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/EventsResponse.md
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/GenericTokenError.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Gzip.md
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/GzipApi.md
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/GzipResponse.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Header.md
+-rw-r--r--   0        0        0    20925 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HeaderApi.md
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HeaderResponse.md
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Healthcheck.md
+-rw-r--r--   0        0        0    20120 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HealthcheckApi.md
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HealthcheckResponse.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Historical.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalAggregateResponse.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalAggregateResponseAllOf.md
+-rw-r--r--   0        0        0    39081 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalApi.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalDomains.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalDomainsData.md
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalDomainsMeta.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalDomainsMetaFilters.md
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalDomainsResponse.md
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalDomainsResponseAllOf.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalFieldAggregateResponse.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalFieldAggregateResponseAllOf.md
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalFieldResponse.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalFieldResponseDataField.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalFieldResults.md
+-rw-r--r--   0        0        0    27230 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalFieldResultsAttributes.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalFieldResultsAttributesAdditional.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalMeta.md
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalOriginsResponse.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalOriginsResponseAllOf.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalRegionsResponse.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalRegionsResponseAllOf.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalResponse.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalResponseDataField.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalResults.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalService.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalServices.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalUsageAggregateResponse.md
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalUsageMonthResponse.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalUsageMonthResponseAllOf.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalUsageMonthResponseData.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalUsageResults.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalUsageServiceResponse.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HistoricalUsageServiceResponseAllOf.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Http3.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Http3AllOf.md
+-rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Http3Api.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HttpResponseFormat.md
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/HttpStreamFormat.md
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamPermission.md
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamPermissionsApi.md
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamRole.md
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamRoleAllOf.md
+-rw-r--r--   0        0        0    21530 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamRolesApi.md
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamServiceGroup.md
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamServiceGroupAllOf.md
+-rw-r--r--   0        0        0    23819 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamServiceGroupsApi.md
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamUserGroup.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamUserGroupAllOf.md
+-rw-r--r--   0        0        0    42765 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IamUserGroupsApi.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IncludedWithWafActiveRule.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IncludedWithWafActiveRuleItem.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IncludedWithWafExclusion.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IncludedWithWafExclusionItem.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IncludedWithWafFirewall.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IncludedWithWafFirewallVersion.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IncludedWithWafFirewallVersionItem.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IncludedWithWafRule.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IncludedWithWafRuleItem.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/IncludedWithWafRuleRevision.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineObject.md
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineObject1.md
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse200.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse2001.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse2002.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse2003.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse2003Meta.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse2004.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse2004Meta.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse2005.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse2006.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse2007.md
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InlineResponse400.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Invitation.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InvitationData.md
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InvitationDataAttributes.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InvitationResponse.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InvitationResponseAllOf.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InvitationResponseData.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InvitationResponseDataAllOf.md
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InvitationsApi.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InvitationsResponse.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/InvitationsResponseAllOf.md
+-rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/KvStoreApi.md
+-rw-r--r--   0        0        0    12230 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/KvStoreItemApi.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafConfigurationSet.md
+-rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafConfigurationSetsApi.md
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafFirewall.md
+-rw-r--r--   0        0        0    28708 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafFirewallApi.md
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafOwasp.md
+-rw-r--r--   0        0        0    10002 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafOwaspApi.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafRule.md
+-rw-r--r--   0        0        0    13782 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafRuleApi.md
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafRuleStatus.md
+-rw-r--r--   0        0        0    17124 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafRuleStatusApi.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafRuleset.md
+-rw-r--r--   0        0        0     9577 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafRulesetApi.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafTag.md
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafTagApi.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafUpdateStatus.md
+-rw-r--r--   0        0        0     7262 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LegacyWafUpdateStatusApi.md
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LineItemData.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LineItemDataReadOnlyInvoiceId.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingAddressAndPort.md
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingAzureblob.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingAzureblobAllOf.md
+-rw-r--r--   0        0        0    29125 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingAzureblobApi.md
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingAzureblobResponse.md
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingBigquery.md
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingBigqueryAllOf.md
+-rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingBigqueryApi.md
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingBigqueryResponse.md
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingCloudfiles.md
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingCloudfilesAllOf.md
+-rw-r--r--   0        0        0    27524 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingCloudfilesApi.md
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingCloudfilesResponse.md
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingCommon.md
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingDatadog.md
+-rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingDatadogAllOf.md
+-rw-r--r--   0        0        0    38955 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingDatadogApi.md
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingDatadogResponse.md
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingDigitalocean.md
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingDigitaloceanAllOf.md
+-rw-r--r--   0        0        0    28174 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingDigitaloceanApi.md
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingDigitaloceanResponse.md
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingElasticsearch.md
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingElasticsearchAllOf.md
+-rw-r--r--   0        0        0    30259 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingElasticsearchApi.md
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingElasticsearchResponse.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingFormatVersion.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingFtp.md
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingFtpAllOf.md
+-rw-r--r--   0        0        0    27244 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingFtpApi.md
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingFtpResponse.md
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingGcs.md
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingGcsAllOf.md
+-rw-r--r--   0        0        0    28487 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingGcsApi.md
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingGcsCommon.md
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingGcsResponse.md
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingGenericCommon.md
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingGooglePubsub.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingGooglePubsubAllOf.md
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingGooglePubsubResponse.md
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHeroku.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHerokuAllOf.md
+-rw-r--r--   0        0        0    21127 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHerokuApi.md
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHerokuResponse.md
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHoneycomb.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHoneycombAllOf.md
+-rw-r--r--   0        0        0    20986 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHoneycombApi.md
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHoneycombResponse.md
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHttps.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHttpsAllOf.md
+-rw-r--r--   0        0        0    29036 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHttpsApi.md
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingHttpsResponse.md
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingKafka.md
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingKafkaAllOf.md
+-rw-r--r--   0        0        0    21774 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingKafkaApi.md
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingKafkaResponse.md
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingKinesis.md
+-rw-r--r--   0        0        0    20420 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingKinesisApi.md
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingKinesisResponse.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogentries.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogentriesAllOf.md
+-rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogentriesApi.md
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogentriesResponse.md
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLoggly.md
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogglyAllOf.md
+-rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogglyApi.md
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogglyResponse.md
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogshuttle.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogshuttleAllOf.md
+-rw-r--r--   0        0        0    21288 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogshuttleApi.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingLogshuttleResponse.md
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingMessageType.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingNewrelic.md
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingNewrelicAllOf.md
+-rw-r--r--   0        0        0    25794 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingNewrelicApi.md
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingNewrelicResponse.md
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingOpenstack.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingOpenstackAllOf.md
+-rw-r--r--   0        0        0    27216 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingOpenstackApi.md
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingOpenstackResponse.md
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingPapertrail.md
+-rw-r--r--   0        0        0    21189 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingPapertrailApi.md
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingPapertrailResponse.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingPlacement.md
+-rw-r--r--   0        0        0    24358 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingPubsubApi.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingRequestCapsCommon.md
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingS3.md
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingS3AllOf.md
+-rw-r--r--   0        0        0    31697 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingS3Api.md
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingS3Response.md
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingScalyr.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingScalyrAllOf.md
+-rw-r--r--   0        0        0    21715 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingScalyrApi.md
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingScalyrResponse.md
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSftp.md
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSftpAllOf.md
+-rw-r--r--   0        0        0    28475 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSftpApi.md
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSftpResponse.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSplunk.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSplunkAllOf.md
+-rw-r--r--   0        0        0    26444 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSplunkApi.md
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSplunkResponse.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSumologic.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSumologicAllOf.md
+-rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSumologicApi.md
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSumologicResponse.md
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSyslog.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSyslogAllOf.md
+-rw-r--r--   0        0        0    26805 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSyslogApi.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingSyslogResponse.md
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingTlsCommon.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/LoggingUseTls.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Model403Forbidden.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthentication.md
+-rw-r--r--   0        0        0    17143 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthenticationApi.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthenticationData.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthenticationDataAttributes.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthenticationResponse.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthenticationResponseAttributes.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthenticationResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthenticationResponseData.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthenticationResponseDataAllOf.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthenticationsResponse.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/MutualAuthenticationsResponseAllOf.md
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/NumberVersion.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspector.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorDimensions.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorEntry.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorHistorical.md
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorHistoricalApi.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorHistoricalData.md
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorHistoricalMeta.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorHistoricalMetaFilters.md
+-rw-r--r--   0        0        0    23594 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorMeasurements.md
+-rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorRealtimeApi.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorRealtimeEntry.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorRealtimeEntryRecorded.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorSubsequentRequestTimestamp.md
+-rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/OriginInspectorValues.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Package.md
+-rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PackageApi.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PackageMetadata.md
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PackageResponse.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PackageResponseAllOf.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Pagination.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PaginationCursorMeta.md
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PaginationLinks.md
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PaginationMeta.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Permission.md
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Pool.md
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PoolAllOf.md
+-rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PoolApi.md
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PoolResponse.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PoolResponseAllOf.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Pop.md
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PopApi.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PopCoordinates.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PublicIpList.md
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PublicIpListApi.md
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PublishApi.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PublishItem.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PublishItemFormats.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PublishRequest.md
+-rw-r--r--   0        0        0    14751 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PurgeApi.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PurgeKeys.md
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PurgeKeysResponse.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/PurgeResponse.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RateLimiter.md
+-rw-r--r--   0        0        0    21841 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RateLimiterApi.md
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RateLimiterResponse.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RateLimiterResponseAllOf.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ReadOnlyCustomerId.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ReadOnlyId.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ReadOnlyIdService.md
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ReadOnlyServiceId.md
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ReadOnlyUserId.md
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ReadOnlyVersion.md
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Realtime.md
+-rw-r--r--   0        0        0     8759 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RealtimeApi.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RealtimeEntry.md
+-rw-r--r--   0        0        0    27361 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RealtimeEntryAggregated.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RealtimeEntryDatacenter.md
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RealtimeEntryRecorded.md
+-rw-r--r--   0        0        0    27336 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RealtimeMeasurements.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RecordedTimestamp.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipCommonName.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipCustomer.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipCustomerCustomer.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberCustomer.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberMutualAuthentication.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberService.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberServiceInvitation.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberTlsActivation.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberTlsBulkCertificate.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberTlsCertificate.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberTlsConfiguration.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberTlsDnsRecord.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberTlsDomain.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberTlsPrivateKey.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberTlsSubscription.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberWafActiveRule.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberWafFirewall.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberWafFirewallVersion.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberWafRule.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberWafRuleRevision.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMemberWafTag.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMutualAuthentication.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMutualAuthenticationMutualAuthentication.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMutualAuthentications.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipMutualAuthenticationsMutualAuthentications.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipService.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipServiceInvitations.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipServiceInvitationsCreate.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipServiceInvitationsCreateServiceInvitations.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipServiceInvitationsServiceInvitations.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipServices.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipServicesServices.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsActivation.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsActivationTlsActivation.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsActivations.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsBulkCertificate.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsBulkCertificates.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsCertificate.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsCertificateTlsCertificate.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsCertificates.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsCertificatesTlsCertificates.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsConfiguration.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsConfigurationForTlsSubscription.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsConfigurationTlsConfiguration.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsConfigurations.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsConfigurationsTlsConfigurations.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsDnsRecord.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsDnsRecordDnsRecord.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsDnsRecords.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsDomain.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsDomainTlsDomain.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsDomains.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsDomainsTlsDomains.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsPrivateKey.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsPrivateKeys.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsSubscription.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsSubscriptionTlsSubscription.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipTlsSubscriptions.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipUser.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipUserUser.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafActiveRules.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafActiveRulesWafActiveRules.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafFirewall.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafFirewallVersion.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafFirewallVersionWafFirewallVersion.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafFirewallVersions.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafFirewallWafFirewall.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafRule.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafRuleRevision.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafRuleRevisionWafRuleRevisions.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafRuleRevisions.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafRuleWafRule.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafRules.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafTags.md
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipWafTagsWafTags.md
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForInvitation.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForMutualAuthentication.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForStar.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForTlsActivation.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForTlsBulkCertificate.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForTlsConfiguration.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForTlsDomain.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForTlsPrivateKey.md
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForTlsSubscription.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForWafActiveRule.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForWafExclusion.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForWafFirewallVersion.md
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RelationshipsForWafRule.md
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RequestSettings.md
+-rw-r--r--   0        0        0    18477 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RequestSettingsApi.md
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RequestSettingsResponse.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Resource.md
+-rw-r--r--   0        0        0    15552 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ResourceApi.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ResourceResponse.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ResourceResponseAllOf.md
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ResponseObject.md
+-rw-r--r--   0        0        0    14712 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ResponseObjectApi.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ResponseObjectResponse.md
+-rw-r--r--   0        0        0    27224 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Results.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/RoleUser.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SchemasContactResponse.md
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SchemasSnippetResponse.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SchemasUserResponse.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SchemasUserResponseReadOnly.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SchemasVclResponse.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SchemasVersion.md
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SchemasVersionResponse.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SchemasWafFirewallVersion.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SchemasWafFirewallVersionData.md
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Secret.md
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SecretResponse.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SecretStore.md
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SecretStoreApi.md
+-rw-r--r--   0        0        0    18545 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SecretStoreItemApi.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SecretStoreResponse.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Server.md
+-rw-r--r--   0        0        0    19968 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServerApi.md
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServerResponse.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServerResponseAllOf.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Service.md
+-rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceApi.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorization.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationData.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationDataAttributes.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationDataRelationships.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationDataRelationshipsUser.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationDataRelationshipsUserData.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationResponse.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationResponseData.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationResponseDataAllOf.md
+-rw-r--r--   0        0        0    21776 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationsApi.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationsResponse.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceAuthorizationsResponseAllOf.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceCreate.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceCreateAllOf.md
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceDetail.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceDetailAllOf.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceIdAndVersion.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceInvitation.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceInvitationData.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceInvitationDataAttributes.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceInvitationDataRelationships.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceInvitationResponse.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceInvitationResponseAllOf.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceInvitationResponseAllOfData.md
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceListResponse.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceListResponseAllOf.md
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceResponse.md
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceResponseAllOf.md
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceVersionDetail.md
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ServiceVersionDetailOrNull.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Settings.md
+-rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SettingsApi.md
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SettingsResponse.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SigningKey.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Snippet.md
+-rw-r--r--   0        0        0    22311 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SnippetApi.md
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SnippetResponse.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SnippetResponseAllOf.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Star.md
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/StarApi.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/StarData.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/StarResponse.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/StarResponseAllOf.md
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Stats.md
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/StatsApi.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Store.md
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/StoreResponse.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SubsequentRequestTimestamp.md
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SudoApi.md
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SudoGenericTokenError.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SudoRequest.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/SudoResponse.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Timestamps.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TimestampsNoDelete.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsActivation.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsActivationData.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsActivationResponse.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsActivationResponseData.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsActivationResponseDataAllOf.md
+-rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsActivationsApi.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsActivationsResponse.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsActivationsResponseAllOf.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificate.md
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificateData.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificateDataAttributes.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificateResponse.md
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificateResponseAttributes.md
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificateResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificateResponseData.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificateResponseDataAllOf.md
+-rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificatesApi.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificatesResponse.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsBulkCertificatesResponseAllOf.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificate.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificateData.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificateDataAttributes.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificateResponse.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificateResponseAttributes.md
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificateResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificateResponseData.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificateResponseDataAllOf.md
+-rw-r--r--   0        0        0    17205 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificatesApi.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificatesResponse.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCertificatesResponseAllOf.md
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsCommon.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfiguration.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfigurationData.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfigurationDataAttributes.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfigurationResponse.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfigurationResponseAttributes.md
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfigurationResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfigurationResponseData.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfigurationResponseDataAllOf.md
+-rw-r--r--   0        0        0    10339 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfigurationsApi.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfigurationsResponse.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsConfigurationsResponseAllOf.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsDnsRecord.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsDomainData.md
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsDomainsApi.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsDomainsResponse.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsDomainsResponseAllOf.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsPrivateKey.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsPrivateKeyData.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsPrivateKeyDataAttributes.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsPrivateKeyResponse.md
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsPrivateKeyResponseAttributes.md
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsPrivateKeyResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsPrivateKeyResponseData.md
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsPrivateKeysApi.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsPrivateKeysResponse.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsPrivateKeysResponseAllOf.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscription.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscriptionData.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscriptionDataAttributes.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscriptionResponse.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscriptionResponseAttributes.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscriptionResponseAttributesAllOf.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscriptionResponseData.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscriptionResponseDataAllOf.md
+-rw-r--r--   0        0        0    26148 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscriptionsApi.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscriptionsResponse.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TlsSubscriptionsResponseAllOf.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Token.md
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TokenCreatedResponse.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TokenCreatedResponseAllOf.md
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TokenResponse.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TokenResponseAllOf.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TokensAdditionalProps.md
+-rw-r--r--   0        0        0    20100 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TokensApi.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TokensData.md
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeBillingAddress.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeContact.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeCustomer.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeEvent.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeInvitation.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeMutualAuthentication.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeResource.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeService.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeServiceAuthorization.md
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeServiceInvitation.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeStar.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeTlsActivation.md
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeTlsBulkCertificate.md
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeTlsCertificate.md
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeTlsConfiguration.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeTlsDnsRecord.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeTlsDomain.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeTlsPrivateKey.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeTlsSubscription.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeUser.md
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeWafActiveRule.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeWafExclusion.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeWafFirewall.md
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeWafFirewallVersion.md
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeWafRule.md
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeWafRuleRevision.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/TypeWafTag.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/UpdateBillingAddressRequest.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/UpdateBillingAddressRequestData.md
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/User.md
+-rw-r--r--   0        0        0    20897 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/UserApi.md
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/UserResponse.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/UserResponseReadOnly.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ValidatorResult.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ValidatorResultData.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ValidatorResultDataAttributes.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/ValidatorResultDataAttributesMessages.md
+-rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Values.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Vcl.md
+-rw-r--r--   0        0        0    38853 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VclApi.md
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VclDiff.md
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VclDiffApi.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VclResponse.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VclSyntaxHighlightingResponse.md
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/Version.md
+-rw-r--r--   0        0        0    26131 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VersionApi.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VersionCreateResponse.md
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VersionDetail.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VersionDetailSettings.md
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VersionResponse.md
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/VersionResponseAllOf.md
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRule.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRuleCreationResponse.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRuleData.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRuleDataAttributes.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRuleResponse.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRuleResponseData.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRuleResponseDataAllOf.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRuleResponseDataAttributes.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRuleResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRuleResponseDataRelationships.md
+-rw-r--r--   0        0        0    31218 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRulesApi.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRulesResponse.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafActiveRulesResponseAllOf.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusion.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionData.md
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionDataAttributes.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionResponse.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionResponseData.md
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionResponseDataAllOf.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionResponseDataAttributes.md
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionResponseDataRelationships.md
+-rw-r--r--   0        0        0    19155 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionsApi.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionsResponse.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafExclusionsResponseAllOf.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewall.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallData.md
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallDataAttributes.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallResponse.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallResponseData.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallResponseDataAllOf.md
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallResponseDataAttributes.md
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersion.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersionData.md
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersionDataAttributes.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersionResponse.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersionResponseData.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersionResponseDataAllOf.md
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersionResponseDataAttributes.md
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersionResponseDataAttributesAllOf.md
+-rw-r--r--   0        0        0    24852 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersionsApi.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersionsResponse.md
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallVersionsResponseAllOf.md
+-rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallsApi.md
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallsResponse.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafFirewallsResponseAllOf.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRule.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleAttributes.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleResponse.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleResponseData.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleResponseDataAllOf.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleRevision.md
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleRevisionAttributes.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleRevisionOrLatest.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleRevisionResponse.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleRevisionResponseData.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleRevisionResponseDataAllOf.md
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleRevisionsApi.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleRevisionsResponse.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRuleRevisionsResponseAllOf.md
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRulesApi.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRulesResponse.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafRulesResponseAllOf.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafTag.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafTagAttributes.md
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafTagsApi.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafTagsResponse.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafTagsResponseAllOf.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WafTagsResponseDataItem.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastly-3.0.1/docs/WsMessageFormat.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/__init__.py
+-rw-r--r--   0        0        0    39346 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api_client.py
+-rw-r--r--   0        0        0    18987 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/configuration.py
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/exceptions.py
+-rw-r--r--   0        0        0    82616 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model_utils.py
+-rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/rest.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/__init__.py
+-rw-r--r--   0        0        0    30565 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/acl_api.py
+-rw-r--r--   0        0        0    37416 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/acl_entry_api.py
+-rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/apex_redirect_api.py
+-rw-r--r--   0        0        0    27130 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/automation_tokens_api.py
+-rw-r--r--   0        0        0    54123 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/backend_api.py
+-rw-r--r--   0        0        0    22509 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/billing_address_api.py
+-rw-r--r--   0        0        0    18589 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/billing_api.py
+-rw-r--r--   0        0        0    34253 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/cache_settings_api.py
+-rw-r--r--   0        0        0    34233 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/condition_api.py
+-rw-r--r--   0        0        0    36809 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/config_store_api.py
+-rw-r--r--   0        0        0    42045 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/config_store_item_api.py
+-rw-r--r--   0        0        0    19255 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/contact_api.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/content_api.py
+-rw-r--r--   0        0        0    34431 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/customer_api.py
+-rw-r--r--   0        0        0    31732 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/dictionary_api.py
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/dictionary_info_api.py
+-rw-r--r--   0        0        0    46055 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/dictionary_item_api.py
+-rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/diff_api.py
+-rw-r--r--   0        0        0    32761 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/director_api.py
+-rw-r--r--   0        0        0    20598 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/director_backend_api.py
+-rw-r--r--   0        0        0    42736 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/domain_api.py
+-rw-r--r--   0        0        0    10883 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/domain_inspector_historical_api.py
+-rw-r--r--   0        0        0    18137 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/domain_inspector_realtime_api.py
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/domain_ownerships_api.py
+-rw-r--r--   0        0        0    17704 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/enabled_products_api.py
+-rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/events_api.py
+-rw-r--r--   0        0        0    32656 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/gzip_api.py
+-rw-r--r--   0        0        0    38546 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/header_api.py
+-rw-r--r--   0        0        0    37114 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/healthcheck_api.py
+-rw-r--r--   0        0        0    60468 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/historical_api.py
+-rw-r--r--   0        0        0    19550 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/http3_api.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/iam_permissions_api.py
+-rw-r--r--   0        0        0    42584 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/iam_roles_api.py
+-rw-r--r--   0        0        0    44500 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/iam_service_groups_api.py
+-rw-r--r--   0        0        0    77824 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/iam_user_groups_api.py
+-rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/invitations_api.py
+-rw-r--r--   0        0        0    21168 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/kv_store_api.py
+-rw-r--r--   0        0        0    24533 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/kv_store_item_api.py
+-rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/legacy_waf_configuration_sets_api.py
+-rw-r--r--   0        0        0    50116 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/legacy_waf_firewall_api.py
+-rw-r--r--   0        0        0    18781 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/legacy_waf_owasp_api.py
+-rw-r--r--   0        0        0    25207 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/legacy_waf_rule_api.py
+-rw-r--r--   0        0        0    29074 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/legacy_waf_rule_status_api.py
+-rw-r--r--   0        0        0    18667 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/legacy_waf_ruleset_api.py
+-rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/legacy_waf_tag_api.py
+-rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/legacy_waf_update_status_api.py
+-rw-r--r--   0        0        0    45445 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_azureblob_api.py
+-rw-r--r--   0        0        0    40102 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_bigquery_api.py
+-rw-r--r--   0        0        0    45152 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_cloudfiles_api.py
+-rw-r--r--   0        0        0    42863 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_datadog_api.py
+-rw-r--r--   0        0        0    44606 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_digitalocean_api.py
+-rw-r--r--   0        0        0    45229 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_elasticsearch_api.py
+-rw-r--r--   0        0        0    44432 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_ftp_api.py
+-rw-r--r--   0        0        0    44765 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_gcs_api.py
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_heroku_api.py
+-rw-r--r--   0        0        0    36624 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_honeycomb_api.py
+-rw-r--r--   0        0        0    46115 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_https_api.py
+-rw-r--r--   0        0        0    38597 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_kafka_api.py
+-rw-r--r--   0        0        0    34377 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_kinesis_api.py
+-rw-r--r--   0        0        0    38489 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_logentries_api.py
+-rw-r--r--   0        0        0    36081 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_loggly_api.py
+-rw-r--r--   0        0        0    36770 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_logshuttle_api.py
+-rw-r--r--   0        0        0    38558 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_newrelic_api.py
+-rw-r--r--   0        0        0    44042 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_openstack_api.py
+-rw-r--r--   0        0        0    36635 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_papertrail_api.py
+-rw-r--r--   0        0        0    39265 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_pubsub_api.py
+-rw-r--r--   0        0        0    48777 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_s3_api.py
+-rw-r--r--   0        0        0    37469 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_scalyr_api.py
+-rw-r--r--   0        0        0    45357 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_sftp_api.py
+-rw-r--r--   0        0        0    42255 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_splunk_api.py
+-rw-r--r--   0        0        0    36567 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_sumologic_api.py
+-rw-r--r--   0        0        0    43033 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/logging_syslog_api.py
+-rw-r--r--   0        0        0    28852 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/mutual_authentication_api.py
+-rw-r--r--   0        0        0    10862 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/origin_inspector_historical_api.py
+-rw-r--r--   0        0        0    18138 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/origin_inspector_realtime_api.py
+-rw-r--r--   0        0        0    12896 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/package_api.py
+-rw-r--r--   0        0        0    47354 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/pool_api.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/pop_api.py
+-rw-r--r--   0        0        0     5863 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/public_ip_list_api.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/publish_api.py
+-rw-r--r--   0        0        0    24927 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/purge_api.py
+-rw-r--r--   0        0        0    43466 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/rate_limiter_api.py
+-rw-r--r--   0        0        0    17852 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/realtime_api.py
+-rw-r--r--   0        0        0    34834 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/request_settings_api.py
+-rw-r--r--   0        0        0    30490 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/resource_api.py
+-rw-r--r--   0        0        0    30298 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/response_object_api.py
+-rw-r--r--   0        0        0    30510 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/secret_store_api.py
+-rw-r--r--   0        0        0    33761 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/secret_store_item_api.py
+-rw-r--r--   0        0        0    35038 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/server_api.py
+-rw-r--r--   0        0        0    44324 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/service_api.py
+-rw-r--r--   0        0        0    38118 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/service_authorizations_api.py
+-rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/settings_api.py
+-rw-r--r--   0        0        0    44770 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/snippet_api.py
+-rw-r--r--   0        0        0    20513 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/star_api.py
+-rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/stats_api.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/sudo_api.py
+-rw-r--r--   0        0        0    29279 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/tls_activations_api.py
+-rw-r--r--   0        0        0    28695 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/tls_bulk_certificates_api.py
+-rw-r--r--   0        0        0    29585 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/tls_certificates_api.py
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/tls_configurations_api.py
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/tls_domains_api.py
+-rw-r--r--   0        0        0    22120 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/tls_private_keys_api.py
+-rw-r--r--   0        0        0    43908 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/tls_subscriptions_api.py
+-rw-r--r--   0        0        0    39861 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/tokens_api.py
+-rw-r--r--   0        0        0    40766 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/user_api.py
+-rw-r--r--   0        0        0    76536 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/vcl_api.py
+-rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/vcl_diff_api.py
+-rw-r--r--   0        0        0    51681 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/version_api.py
+-rw-r--r--   0        0        0    51904 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/waf_active_rules_api.py
+-rw-r--r--   0        0        0    33986 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/waf_exclusions_api.py
+-rw-r--r--   0        0        0    36636 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/waf_firewall_versions_api.py
+-rw-r--r--   0        0        0    29601 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/waf_firewalls_api.py
+-rw-r--r--   0        0        0    13840 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/waf_rule_revisions_api.py
+-rw-r--r--   0        0        0    13963 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/waf_rules_api.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/api/waf_tags_api.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/apis/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/__init__.py
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/acl.py
+-rw-r--r--   0        0        0    13163 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/acl_entry.py
+-rw-r--r--   0        0        0    17362 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/acl_entry_response.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/acl_entry_response_all_of.py
+-rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/acl_response.py
+-rw-r--r--   0        0        0    12025 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/acl_response_all_of.py
+-rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/apex_redirect.py
+-rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/apex_redirect_all_of.py
+-rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/automation_token.py
+-rw-r--r--   0        0        0    11840 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/automation_token_create_request.py
+-rw-r--r--   0        0        0    13264 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/automation_token_create_request_attributes.py
+-rw-r--r--   0        0        0    19202 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/automation_token_create_response.py
+-rw-r--r--   0        0        0    13953 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/automation_token_create_response_all_of.py
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/automation_token_response.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/automation_token_response_all_of.py
+-rw-r--r--   0        0        0    14660 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/aws_region.py
+-rw-r--r--   0        0        0    26143 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/backend.py
+-rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/backend_response.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/backend_response_all_of.py
+-rw-r--r--   0        0        0    12338 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/batch.py
+-rw-r--r--   0        0        0    12656 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/batch_errors.py
+-rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing.py
+-rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_address_attributes.py
+-rw-r--r--   0        0        0    12075 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_address_request.py
+-rw-r--r--   0        0        0    12080 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_address_request_data.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_address_response.py
+-rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_address_response_data.py
+-rw-r--r--   0        0        0    11909 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_address_verification_error_response.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_address_verification_error_response_errors.py
+-rw-r--r--   0        0        0    11759 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_estimate_lines.py
+-rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_estimate_lines_line_items.py
+-rw-r--r--   0        0        0    16831 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_estimate_response.py
+-rw-r--r--   0        0        0    16807 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_response.py
+-rw-r--r--   0        0        0    11741 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_response_item_items_data.py
+-rw-r--r--   0        0        0    18745 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_response_line_item.py
+-rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_response_line_items.py
+-rw-r--r--   0        0        0    12004 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_status.py
+-rw-r--r--   0        0        0    16362 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_total.py
+-rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/billing_total_extras.py
+-rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/bulk_update_acl_entries_request.py
+-rw-r--r--   0        0        0    16005 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/bulk_update_acl_entry.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/bulk_update_acl_entry_all_of.py
+-rw-r--r--   0        0        0    14518 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/bulk_update_config_store_item.py
+-rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/bulk_update_config_store_item_all_of.py
+-rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/bulk_update_config_store_list_request.py
+-rw-r--r--   0        0        0    14509 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/bulk_update_dictionary_item.py
+-rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/bulk_update_dictionary_list_request.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/bulk_waf_active_rule.py
+-rw-r--r--   0        0        0    11638 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/bulk_waf_active_rules.py
+-rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/cache_setting.py
+-rw-r--r--   0        0        0    17524 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/cache_setting_response.py
+-rw-r--r--   0        0        0    12661 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/client_key.py
+-rw-r--r--   0        0        0    13530 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/condition.py
+-rw-r--r--   0        0        0    16896 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/condition_response.py
+-rw-r--r--   0        0        0    11911 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/conditions_response.py
+-rw-r--r--   0        0        0    11444 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/config_store.py
+-rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/config_store_info_response.py
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/config_store_item.py
+-rw-r--r--   0        0        0    15611 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/config_store_item_response.py
+-rw-r--r--   0        0        0    11487 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/config_store_item_response_all_of.py
+-rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/config_store_response.py
+-rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/config_store_response_all_of.py
+-rw-r--r--   0        0        0    13577 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/contact.py
+-rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/contact_response.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/contact_response_all_of.py
+-rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/content.py
+-rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/customer.py
+-rw-r--r--   0        0        0    24131 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/customer_response.py
+-rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/customer_response_all_of.py
+-rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/dictionary.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/dictionary_info_response.py
+-rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/dictionary_item.py
+-rw-r--r--   0        0        0    15870 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/dictionary_item_response.py
+-rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/dictionary_item_response_all_of.py
+-rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/dictionary_response.py
+-rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/dictionary_response_all_of.py
+-rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/diff_response.py
+-rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/director.py
+-rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/director_backend.py
+-rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/director_backend_all_of.py
+-rw-r--r--   0        0        0    18553 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/director_response.py
+-rw-r--r--   0        0        0    11783 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain.py
+-rw-r--r--   0        0        0    13972 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain_check_item.py
+-rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain_check_response.py
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain_check_response_list.py
+-rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain_inspector.py
+-rw-r--r--   0        0        0    12175 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain_inspector_entry.py
+-rw-r--r--   0        0        0    12647 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain_inspector_entry_dimensions.py
+-rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain_inspector_entry_values.py
+-rw-r--r--   0        0        0    34374 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain_inspector_measurements.py
+-rw-r--r--   0        0        0    13220 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain_inspector_realtime_entry.py
+-rw-r--r--   0        0        0    15770 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domain_response.py
+-rw-r--r--   0        0        0    11875 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/domains_response.py
+-rw-r--r--   0        0        0    12604 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/enabled_product_response.py
+-rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/enabled_product_response_links.py
+-rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/enabled_product_response_product.py
+-rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/enabled_product_response_service.py
+-rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/error_response.py
+-rw-r--r--   0        0        0    12088 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/event.py
+-rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/event_attributes.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/event_data.py
+-rw-r--r--   0        0        0    11790 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/event_data_items.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/event_response.py
+-rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/events_response.py
+-rw-r--r--   0        0        0    11395 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/generic_token_error.py
+-rw-r--r--   0        0        0    12758 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/gzip.py
+-rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/gzip_response.py
+-rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/header.py
+-rw-r--r--   0        0        0    19828 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/header_response.py
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/healthcheck.py
+-rw-r--r--   0        0        0    18979 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/healthcheck_response.py
+-rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical.py
+-rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_aggregate_response.py
+-rw-r--r--   0        0        0    11672 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_aggregate_response_all_of.py
+-rw-r--r--   0        0        0    12972 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_domains.py
+-rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_domains_data.py
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_domains_meta.py
+-rw-r--r--   0        0        0    11839 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_domains_meta_filters.py
+-rw-r--r--   0        0        0    15324 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_domains_response.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_domains_response_all_of.py
+-rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_field_aggregate_response.py
+-rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_field_aggregate_response_all_of.py
+-rw-r--r--   0        0        0    15024 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_field_response.py
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_field_response_data_field.py
+-rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_field_results.py
+-rw-r--r--   0        0        0   100346 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_field_results_attributes.py
+-rw-r--r--   0        0        0    11942 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_field_results_attributes_additional.py
+-rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_meta.py
+-rw-r--r--   0        0        0    15432 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_origins_response.py
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_origins_response_all_of.py
+-rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_regions_response.py
+-rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_regions_response_all_of.py
+-rw-r--r--   0        0        0    15219 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_response.py
+-rw-r--r--   0        0        0    11959 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_response_data_field.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_results.py
+-rw-r--r--   0        0        0    11620 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_service.py
+-rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_services.py
+-rw-r--r--   0        0        0    15037 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_usage_aggregate_response.py
+-rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_usage_month_response.py
+-rw-r--r--   0        0        0    11783 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_usage_month_response_all_of.py
+-rw-r--r--   0        0        0    12331 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_usage_month_response_data.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_usage_results.py
+-rw-r--r--   0        0        0    15031 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_usage_service_response.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/historical_usage_service_response_all_of.py
+-rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/http3.py
+-rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/http3_all_of.py
+-rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/http_response_format.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/http_stream_format.py
+-rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/iam_permission.py
+-rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/iam_role.py
+-rw-r--r--   0        0        0    12962 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/iam_role_all_of.py
+-rw-r--r--   0        0        0    15636 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/iam_service_group.py
+-rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/iam_service_group_all_of.py
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/iam_user_group.py
+-rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/iam_user_group_all_of.py
+-rw-r--r--   0        0        0    12044 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/included_with_waf_active_rule.py
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/included_with_waf_active_rule_item.py
+-rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/included_with_waf_exclusion.py
+-rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/included_with_waf_exclusion_item.py
+-rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/included_with_waf_firewall.py
+-rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/included_with_waf_firewall_version.py
+-rw-r--r--   0        0        0    13972 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/included_with_waf_firewall_version_item.py
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/included_with_waf_rule.py
+-rw-r--r--   0        0        0    14599 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/included_with_waf_rule_item.py
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/included_with_waf_rule_revision.py
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_object.py
+-rw-r--r--   0        0        0    11419 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_object1.py
+-rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response200.py
+-rw-r--r--   0        0        0    11607 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response2001.py
+-rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response2002.py
+-rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response2003.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response2003_meta.py
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response2004.py
+-rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response2004_meta.py
+-rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response2005.py
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response2006.py
+-rw-r--r--   0        0        0    11743 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response2007.py
+-rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/inline_response400.py
+-rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/invitation.py
+-rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/invitation_data.py
+-rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/invitation_data_attributes.py
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/invitation_response.py
+-rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/invitation_response_all_of.py
+-rw-r--r--   0        0        0    14895 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/invitation_response_data.py
+-rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/invitation_response_data_all_of.py
+-rw-r--r--   0        0        0    14597 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/invitations_response.py
+-rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/invitations_response_all_of.py
+-rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/legacy_waf_configuration_set.py
+-rw-r--r--   0        0        0    14430 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/legacy_waf_firewall.py
+-rw-r--r--   0        0        0    23898 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/legacy_waf_owasp.py
+-rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/legacy_waf_rule.py
+-rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/legacy_waf_rule_status.py
+-rw-r--r--   0        0        0    11777 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/legacy_waf_ruleset.py
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/legacy_waf_tag.py
+-rw-r--r--   0        0        0    13049 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/legacy_waf_update_status.py
+-rw-r--r--   0        0        0    15417 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/line_item_data.py
+-rw-r--r--   0        0        0    10983 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/line_item_data_read_only_invoice_id.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_address_and_port.py
+-rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_azureblob.py
+-rw-r--r--   0        0        0    14206 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_azureblob_all_of.py
+-rw-r--r--   0        0        0    24022 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_azureblob_response.py
+-rw-r--r--   0        0        0    19390 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_bigquery.py
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_bigquery_all_of.py
+-rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_bigquery_response.py
+-rw-r--r--   0        0        0    21831 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_cloudfiles.py
+-rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_cloudfiles_all_of.py
+-rw-r--r--   0        0        0    23364 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_cloudfiles_response.py
+-rw-r--r--   0        0        0    14144 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_common.py
+-rw-r--r--   0        0        0    23211 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_datadog.py
+-rw-r--r--   0        0        0    18487 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_datadog_all_of.py
+-rw-r--r--   0        0        0    24914 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_datadog_response.py
+-rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_digitalocean.py
+-rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_digitalocean_all_of.py
+-rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_digitalocean_response.py
+-rw-r--r--   0        0        0    22734 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_elasticsearch.py
+-rw-r--r--   0        0        0    14289 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_elasticsearch_all_of.py
+-rw-r--r--   0        0        0    24096 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_elasticsearch_response.py
+-rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_format_version.py
+-rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_ftp.py
+-rw-r--r--   0        0        0    13770 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_ftp_all_of.py
+-rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_ftp_response.py
+-rw-r--r--   0        0        0    22679 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_gcs.py
+-rw-r--r--   0        0        0    12744 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_gcs_all_of.py
+-rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_gcs_common.py
+-rw-r--r--   0        0        0    24062 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_gcs_response.py
+-rw-r--r--   0        0        0    14090 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_generic_common.py
+-rw-r--r--   0        0        0    18898 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_google_pubsub.py
+-rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_google_pubsub_all_of.py
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_google_pubsub_response.py
+-rw-r--r--   0        0        0    17238 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_heroku.py
+-rw-r--r--   0        0        0    11999 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_heroku_all_of.py
+-rw-r--r--   0        0        0    18941 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_heroku_response.py
+-rw-r--r--   0        0        0    17018 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_honeycomb.py
+-rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_honeycomb_all_of.py
+-rw-r--r--   0        0        0    18721 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_honeycomb_response.py
+-rw-r--r--   0        0        0    23100 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_https.py
+-rw-r--r--   0        0        0    15781 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_https_all_of.py
+-rw-r--r--   0        0        0    24462 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_https_response.py
+-rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_kafka.py
+-rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_kafka_all_of.py
+-rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_kafka_response.py
+-rw-r--r--   0        0        0    16368 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_kinesis.py
+-rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_kinesis_response.py
+-rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_logentries.py
+-rw-r--r--   0        0        0    12851 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_logentries_all_of.py
+-rw-r--r--   0        0        0    19749 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_logentries_response.py
+-rw-r--r--   0        0        0    16993 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_loggly.py
+-rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_loggly_all_of.py
+-rw-r--r--   0        0        0    18696 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_loggly_response.py
+-rw-r--r--   0        0        0    17065 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_logshuttle.py
+-rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_logshuttle_all_of.py
+-rw-r--r--   0        0        0    18768 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_logshuttle_response.py
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_message_type.py
+-rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_newrelic.py
+-rw-r--r--   0        0        0    14066 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_newrelic_all_of.py
+-rw-r--r--   0        0        0    20498 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_newrelic_response.py
+-rw-r--r--   0        0        0    21509 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_openstack.py
+-rw-r--r--   0        0        0    13226 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_openstack_all_of.py
+-rw-r--r--   0        0        0    23042 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_openstack_response.py
+-rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_papertrail.py
+-rw-r--r--   0        0        0    18776 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_papertrail_response.py
+-rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_placement.py
+-rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_request_caps_common.py
+-rw-r--r--   0        0        0    24622 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_s3.py
+-rw-r--r--   0        0        0    16374 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_s3_all_of.py
+-rw-r--r--   0        0        0    26155 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_s3_response.py
+-rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_scalyr.py
+-rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_scalyr_all_of.py
+-rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_scalyr_response.py
+-rw-r--r--   0        0        0    22808 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_sftp.py
+-rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_sftp_all_of.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_sftp_response.py
+-rw-r--r--   0        0        0    21030 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_splunk.py
+-rw-r--r--   0        0        0    12164 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_splunk_all_of.py
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_splunk_response.py
+-rw-r--r--   0        0        0    17102 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_sumologic.py
+-rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_sumologic_all_of.py
+-rw-r--r--   0        0        0    18805 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_sumologic_response.py
+-rw-r--r--   0        0        0    21452 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_syslog.py
+-rw-r--r--   0        0        0    13046 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_syslog_all_of.py
+-rw-r--r--   0        0        0    22829 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_syslog_response.py
+-rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_tls_common.py
+-rw-r--r--   0        0        0    11595 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/logging_use_tls.py
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/model403_forbidden.py
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/mutual_authentication.py
+-rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/mutual_authentication_data.py
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/mutual_authentication_data_attributes.py
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/mutual_authentication_response.py
+-rw-r--r--   0        0        0    15149 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/mutual_authentication_response_attributes.py
+-rw-r--r--   0        0        0    11647 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/mutual_authentication_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15368 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/mutual_authentication_response_data.py
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/mutual_authentication_response_data_all_of.py
+-rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/mutual_authentications_response.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/mutual_authentications_response_all_of.py
+-rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/number_version.py
+-rw-r--r--   0        0        0    12795 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector.py
+-rw-r--r--   0        0        0    12642 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_dimensions.py
+-rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_entry.py
+-rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_historical.py
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_historical_data.py
+-rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_historical_meta.py
+-rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_historical_meta_filters.py
+-rw-r--r--   0        0        0    78482 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_measurements.py
+-rw-r--r--   0        0        0    13076 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_realtime_entry.py
+-rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_realtime_entry_recorded.py
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_subsequent_request_timestamp.py
+-rw-r--r--   0        0        0    78464 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/origin_inspector_values.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/package.py
+-rw-r--r--   0        0        0    13175 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/package_metadata.py
+-rw-r--r--   0        0        0    15990 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/package_response.py
+-rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/package_response_all_of.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/pagination.py
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/pagination_cursor_meta.py
+-rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/pagination_links.py
+-rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/pagination_meta.py
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/permission.py
+-rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/pool.py
+-rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/pool_all_of.py
+-rw-r--r--   0        0        0    25586 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/pool_response.py
+-rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/pool_response_all_of.py
+-rw-r--r--   0        0        0    15216 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/pop.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/pop_coordinates.py
+-rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/public_ip_list.py
+-rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/publish_item.py
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/publish_item_formats.py
+-rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/publish_request.py
+-rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/purge_keys.py
+-rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/purge_keys_response.py
+-rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/purge_response.py
+-rw-r--r--   0        0        0    19010 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/rate_limiter.py
+-rw-r--r--   0        0        0    23485 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/rate_limiter_response.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/rate_limiter_response_all_of.py
+-rw-r--r--   0        0        0    10950 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/read_only_customer_id.py
+-rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/read_only_id.py
+-rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/read_only_id_service.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/read_only_service_id.py
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/read_only_user_id.py
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/read_only_version.py
+-rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/realtime.py
+-rw-r--r--   0        0        0    12492 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/realtime_entry.py
+-rw-r--r--   0        0        0   100248 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/realtime_entry_aggregated.py
+-rw-r--r--   0        0        0    11397 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/realtime_entry_datacenter.py
+-rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/realtime_entry_recorded.py
+-rw-r--r--   0        0        0    98045 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/realtime_measurements.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/recorded_timestamp.py
+-rw-r--r--   0        0        0    11749 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_common_name.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_customer.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_customer_customer.py
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_customer.py
+-rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_mutual_authentication.py
+-rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_service.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_service_invitation.py
+-rw-r--r--   0        0        0    11866 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_tls_activation.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_tls_certificate.py
+-rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_tls_configuration.py
+-rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_tls_dns_record.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_tls_domain.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_tls_private_key.py
+-rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_tls_subscription.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_waf_active_rule.py
+-rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_waf_firewall.py
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_waf_firewall_version.py
+-rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_waf_rule.py
+-rw-r--r--   0        0        0    11995 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_waf_rule_revision.py
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_member_waf_tag.py
+-rw-r--r--   0        0        0    12005 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_mutual_authentication.py
+-rw-r--r--   0        0        0    11881 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_mutual_authentication_mutual_authentication.py
+-rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_mutual_authentications.py
+-rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_mutual_authentications_mutual_authentications.py
+-rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_service.py
+-rw-r--r--   0        0        0    11961 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_service_invitations.py
+-rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_service_invitations_create.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_service_invitations_create_service_invitations.py
+-rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_service_invitations_service_invitations.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_services.py
+-rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_services_services.py
+-rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_activation.py
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_activation_tls_activation.py
+-rw-r--r--   0        0        0    11859 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_activations.py
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_bulk_certificates.py
+-rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_certificate.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_certificate_tls_certificate.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_certificates.py
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_certificates_tls_certificates.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_configuration.py
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_configuration_for_tls_subscription.py
+-rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_configuration_tls_configuration.py
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_configurations.py
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_configurations_tls_configurations.py
+-rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_dns_record.py
+-rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_dns_record_dns_record.py
+-rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_dns_records.py
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_domain.py
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_domain_tls_domain.py
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_domains.py
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_domains_tls_domains.py
+-rw-r--r--   0        0        0    11858 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_private_key.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_private_key_tls_private_key.py
+-rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_private_keys.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_private_keys_tls_private_keys.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_subscription.py
+-rw-r--r--   0        0        0    11822 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_subscription_tls_subscription.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_tls_subscriptions.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_user.py
+-rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_user_user.py
+-rw-r--r--   0        0        0    11880 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_active_rules.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_active_rules_waf_active_rules.py
+-rw-r--r--   0        0        0    11807 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_firewall.py
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_firewall_version.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_firewall_versions.py
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_firewall_waf_firewall.py
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_rule.py
+-rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_rule_revision.py
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_rule_revisions.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_rule_waf_rule.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_rules.py
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_tags.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationship_waf_tags_waf_tags.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_invitation.py
+-rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_mutual_authentication.py
+-rw-r--r--   0        0        0    14345 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_star.py
+-rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_tls_activation.py
+-rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_tls_configuration.py
+-rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_tls_domain.py
+-rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_tls_private_key.py
+-rw-r--r--   0        0        0    16266 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_tls_subscription.py
+-rw-r--r--   0        0        0    14951 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_waf_active_rule.py
+-rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_waf_exclusion.py
+-rw-r--r--   0        0        0    14940 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_waf_firewall_version.py
+-rw-r--r--   0        0        0    14666 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/relationships_for_waf_rule.py
+-rw-r--r--   0        0        0    15858 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/request_settings.py
+-rw-r--r--   0        0        0    19891 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/request_settings_response.py
+-rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/resource.py
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/resource_response.py
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/resource_response_all_of.py
+-rw-r--r--   0        0        0    13673 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/response_object.py
+-rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/response_object_response.py
+-rw-r--r--   0        0        0    97280 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/results.py
+-rw-r--r--   0        0        0    12451 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/role_user.py
+-rw-r--r--   0        0        0    17321 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/schemas_contact_response.py
+-rw-r--r--   0        0        0    17535 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/schemas_snippet_response.py
+-rw-r--r--   0        0        0    18218 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/schemas_user_response.py
+-rw-r--r--   0        0        0    12046 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/schemas_user_response_read_only.py
+-rw-r--r--   0        0        0    15953 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/schemas_vcl_response.py
+-rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/schemas_version.py
+-rw-r--r--   0        0        0    17433 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/schemas_version_response.py
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/schemas_waf_firewall_version.py
+-rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/schemas_waf_firewall_version_data.py
+-rw-r--r--   0        0        0    12644 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/secret.py
+-rw-r--r--   0        0        0    12598 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/secret_response.py
+-rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/secret_store.py
+-rw-r--r--   0        0        0    12048 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/secret_store_response.py
+-rw-r--r--   0        0        0    14569 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/server.py
+-rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/server_response.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/server_response_all_of.py
+-rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service.py
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorization.py
+-rw-r--r--   0        0        0    12718 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorization_data.py
+-rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorization_data_attributes.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorization_data_relationships.py
+-rw-r--r--   0        0        0    11899 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorization_data_relationships_user.py
+-rw-r--r--   0        0        0    11844 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorization_data_relationships_user_data.py
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorization_response.py
+-rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorization_response_data.py
+-rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorization_response_data_all_of.py
+-rw-r--r--   0        0        0    14749 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorizations_response.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_authorizations_response_all_of.py
+-rw-r--r--   0        0        0    14640 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_create.py
+-rw-r--r--   0        0        0    11543 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_create_all_of.py
+-rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_detail.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_detail_all_of.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_id_and_version.py
+-rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_invitation.py
+-rw-r--r--   0        0        0    12646 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_invitation_data.py
+-rw-r--r--   0        0        0    11922 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_invitation_data_attributes.py
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_invitation_data_relationships.py
+-rw-r--r--   0        0        0    14111 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_invitation_response.py
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_invitation_response_all_of.py
+-rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_invitation_response_all_of_data.py
+-rw-r--r--   0        0        0    17024 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_list_response.py
+-rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_list_response_all_of.py
+-rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_response.py
+-rw-r--r--   0        0        0    12948 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_response_all_of.py
+-rw-r--r--   0        0        0    23835 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_version_detail.py
+-rw-r--r--   0        0        0    23852 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/service_version_detail_or_null.py
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/settings.py
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/settings_response.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/signing_key.py
+-rw-r--r--   0        0        0    13181 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/snippet.py
+-rw-r--r--   0        0        0    17514 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/snippet_response.py
+-rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/snippet_response_all_of.py
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/star.py
+-rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/star_data.py
+-rw-r--r--   0        0        0    13825 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/star_response.py
+-rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/star_response_all_of.py
+-rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/stats.py
+-rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/store.py
+-rw-r--r--   0        0        0    11668 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/store_response.py
+-rw-r--r--   0        0        0    11249 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/subsequent_request_timestamp.py
+-rw-r--r--   0        0        0    11407 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/sudo_generic_token_error.py
+-rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/sudo_request.py
+-rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/sudo_response.py
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/timestamps.py
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/timestamps_no_delete.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_activation.py
+-rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_activation_data.py
+-rw-r--r--   0        0        0    11697 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_activation_response.py
+-rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_activation_response_data.py
+-rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_activation_response_data_all_of.py
+-rw-r--r--   0        0        0    14644 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_activations_response.py
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_activations_response_all_of.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_bulk_certificate.py
+-rw-r--r--   0        0        0    12666 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_bulk_certificate_data.py
+-rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_bulk_certificate_data_attributes.py
+-rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_bulk_certificate_response.py
+-rw-r--r--   0        0        0    16192 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_bulk_certificate_response_attributes.py
+-rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_bulk_certificate_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_bulk_certificate_response_data.py
+-rw-r--r--   0        0        0    12043 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_bulk_certificate_response_data_all_of.py
+-rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_bulk_certificates_response.py
+-rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_bulk_certificates_response_all_of.py
+-rw-r--r--   0        0        0    11626 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_certificate.py
+-rw-r--r--   0        0        0    12510 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_certificate_data.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_certificate_data_attributes.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_certificate_response.py
+-rw-r--r--   0        0        0    17609 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_certificate_response_attributes.py
+-rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_certificate_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15107 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_certificate_response_data.py
+-rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_certificate_response_data_all_of.py
+-rw-r--r--   0        0        0    14659 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_certificates_response.py
+-rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_certificates_response_all_of.py
+-rw-r--r--   0        0        0    13892 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_common.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_configuration.py
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_configuration_data.py
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_configuration_data_attributes.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_configuration_response.py
+-rw-r--r--   0        0        0    16408 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_configuration_response_attributes.py
+-rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_configuration_response_attributes_all_of.py
+-rw-r--r--   0        0        0    15232 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_configuration_response_data.py
+-rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_configuration_response_data_all_of.py
+-rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_configurations_response.py
+-rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_configurations_response_all_of.py
+-rw-r--r--   0        0        0    13196 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_dns_record.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_domain_data.py
+-rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_domains_response.py
+-rw-r--r--   0        0        0    11624 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_domains_response_all_of.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_private_key.py
+-rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_private_key_data.py
+-rw-r--r--   0        0        0    11917 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_private_key_data_attributes.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_private_key_response.py
+-rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_private_key_response_attributes.py
+-rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_private_key_response_attributes_all_of.py
+-rw-r--r--   0        0        0    12321 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_private_key_response_data.py
+-rw-r--r--   0        0        0    14646 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_private_keys_response.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_private_keys_response_all_of.py
+-rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_subscription.py
+-rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_subscription_data.py
+-rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_subscription_data_attributes.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_subscription_response.py
+-rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_subscription_response_attributes.py
+-rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_subscription_response_attributes_all_of.py
+-rw-r--r--   0        0        0    14191 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_subscription_response_data.py
+-rw-r--r--   0        0        0    12012 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_subscription_response_data_all_of.py
+-rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_subscriptions_response.py
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tls_subscriptions_response_all_of.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/token.py
+-rw-r--r--   0        0        0    18055 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/token_created_response.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/token_created_response_all_of.py
+-rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/token_response.py
+-rw-r--r--   0        0        0    13237 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/token_response_all_of.py
+-rw-r--r--   0        0        0    11233 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tokens_additional_props.py
+-rw-r--r--   0        0        0    11974 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/tokens_data.py
+-rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_billing_address.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_contact.py
+-rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_customer.py
+-rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_event.py
+-rw-r--r--   0        0        0    11661 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_invitation.py
+-rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_mutual_authentication.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_resource.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_service.py
+-rw-r--r--   0        0        0    11823 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_service_authorization.py
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_service_invitation.py
+-rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_star.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_tls_activation.py
+-rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_tls_bulk_certificate.py
+-rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_tls_certificate.py
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_tls_configuration.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_tls_dns_record.py
+-rw-r--r--   0        0        0    11658 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_tls_domain.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_tls_private_key.py
+-rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_tls_subscription.py
+-rw-r--r--   0        0        0    11571 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_user.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_waf_active_rule.py
+-rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_waf_exclusion.py
+-rw-r--r--   0        0        0    11692 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_waf_firewall.py
+-rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_waf_firewall_version.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_waf_rule.py
+-rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_waf_rule_revision.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/type_waf_tag.py
+-rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/update_billing_address_request.py
+-rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/update_billing_address_request_data.py
+-rw-r--r--   0        0        0    13919 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/user.py
+-rw-r--r--   0        0        0    18161 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/user_response.py
+-rw-r--r--   0        0        0    12025 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/user_response_read_only.py
+-rw-r--r--   0        0        0    11636 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/validator_result.py
+-rw-r--r--   0        0        0    12095 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/validator_result_data.py
+-rw-r--r--   0        0        0    12712 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/validator_result_data_attributes.py
+-rw-r--r--   0        0        0    12341 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/validator_result_data_attributes_messages.py
+-rw-r--r--   0        0        0    34311 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/values.py
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/vcl.py
+-rw-r--r--   0        0        0    12644 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/vcl_diff.py
+-rw-r--r--   0        0        0    15932 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/vcl_response.py
+-rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/vcl_syntax_highlighting_response.py
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/version.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/version_create_response.py
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/version_detail.py
+-rw-r--r--   0        0        0    12978 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/version_detail_settings.py
+-rw-r--r--   0        0        0    17376 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/version_response.py
+-rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/version_response_all_of.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rule.py
+-rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rule_creation_response.py
+-rw-r--r--   0        0        0    12546 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rule_data.py
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rule_data_attributes.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rule_response.py
+-rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rule_response_data.py
+-rw-r--r--   0        0        0    12559 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rule_response_data_all_of.py
+-rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rule_response_data_attributes.py
+-rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rule_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rule_response_data_relationships.py
+-rw-r--r--   0        0        0    15066 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rules_response.py
+-rw-r--r--   0        0        0    12142 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_active_rules_response_all_of.py
+-rw-r--r--   0        0        0    11606 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusion.py
+-rw-r--r--   0        0        0    12519 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusion_data.py
+-rw-r--r--   0        0        0    13837 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusion_data_attributes.py
+-rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusion_response.py
+-rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusion_response_data.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusion_response_data_all_of.py
+-rw-r--r--   0        0        0    17359 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusion_response_data_attributes.py
+-rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusion_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusion_response_data_relationships.py
+-rw-r--r--   0        0        0    15041 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusions_response.py
+-rw-r--r--   0        0        0    12123 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_exclusions_response_all_of.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall.py
+-rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_data.py
+-rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_data_attributes.py
+-rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_response.py
+-rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_response_data.py
+-rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_response_data_all_of.py
+-rw-r--r--   0        0        0    19383 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_response_data_attributes.py
+-rw-r--r--   0        0        0    15905 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_version.py
+-rw-r--r--   0        0        0    12158 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_version_data.py
+-rw-r--r--   0        0        0    24857 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_version_data_attributes.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_version_response.py
+-rw-r--r--   0        0        0    15440 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_version_response_data.py
+-rw-r--r--   0        0        0    12686 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_version_response_data_all_of.py
+-rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_version_response_data_attributes.py
+-rw-r--r--   0        0        0    16832 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_version_response_data_attributes_all_of.py
+-rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_versions_response.py
+-rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewall_versions_response_all_of.py
+-rw-r--r--   0        0        0    15019 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewalls_response.py
+-rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_firewalls_response_all_of.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule.py
+-rw-r--r--   0        0        0    12553 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_attributes.py
+-rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_response.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_response_data.py
+-rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_response_data_all_of.py
+-rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_revision.py
+-rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_revision_attributes.py
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_revision_or_latest.py
+-rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_revision_response.py
+-rw-r--r--   0        0        0    15147 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_revision_response_data.py
+-rw-r--r--   0        0        0    11732 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_revision_response_data_all_of.py
+-rw-r--r--   0        0        0    15110 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_revisions_response.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rule_revisions_response_all_of.py
+-rw-r--r--   0        0        0    14931 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rules_response.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_rules_response_all_of.py
+-rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_tag.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_tag_attributes.py
+-rw-r--r--   0        0        0    14872 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_tags_response.py
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_tags_response_all_of.py
+-rw-r--r--   0        0        0    14941 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/waf_tags_response_data_item.py
+-rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/model/ws_message_format.py
+-rw-r--r--   0        0        0    50669 2020-02-02 00:00:00.000000 fastly-3.0.1/fastly/models/__init__.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastly-3.0.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fastly-3.0.1/LICENSE
+-rw-r--r--   0        0        0    97528 2020-02-02 00:00:00.000000 fastly-3.0.1/README.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastly-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    98020 2020-02-02 00:00:00.000000 fastly-3.0.1/PKG-INFO
```

### Comparing `fastly-3.0.0/CHANGELOG.md` & `fastly-3.0.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [v3.0.1](https://github.com/fastly/fastly-py/releases/tag/release/v3.0.1) (2023-07-12)
+
+**Bug fixes:**
+
+- fix(billing): rename response field 'lines' to 'line_items'.
+- fix(billing): restructure response models like 'aria_invoice_id'.
+- fix(billing): make 'sent_at', 'locked', 'require_new_password', 'two_factor_auth_enabled' nullable.
+
 ## [v3.0.0](https://github.com/fastly/fastly-py/releases/tag/release/v3.0.0) (2023-07-06)
 
 Substantial changes were made to the underlying OpenAPI specification that produces this API client. These changes have resulted in multiple new endpoints being supported as well as multiple breaking type changes and so we're publishing these changes as a new major release.
 
 **Enhancements:**
 
 - feat(apex_redirect): support all endpoints.
```

### Comparing `fastly-3.0.0/SECURITY.md` & `fastly-3.0.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/setup.py` & `fastly-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 from pathlib import Path
 
 NAME = "fastly"
-VERSION = "3.0.0"
+VERSION = "3.0.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `fastly-3.0.0/.github/scripts/pack.sh` & `fastly-3.0.1/.github/scripts/pack.sh`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/.github/scripts/publish_env.sh` & `fastly-3.0.1/.github/scripts/publish_env.sh`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/.github/scripts/release_body.sh` & `fastly-3.0.1/.github/scripts/release_body.sh`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/.github/workflows/ci-release.yaml` & `fastly-3.0.1/.github/workflows/ci-release.yaml`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Acl.md` & `fastly-3.0.1/docs/Acl.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AclApi.md` & `fastly-3.0.1/docs/AclApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AclEntry.md` & `fastly-3.0.1/docs/AclEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AclEntryApi.md` & `fastly-3.0.1/docs/AclEntryApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AclEntryResponse.md` & `fastly-3.0.1/docs/AclEntryResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AclEntryResponseAllOf.md` & `fastly-3.0.1/docs/AclEntryResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AclResponse.md` & `fastly-3.0.1/docs/AclResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AclResponseAllOf.md` & `fastly-3.0.1/docs/AclResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ApexRedirect.md` & `fastly-3.0.1/docs/ApexRedirect.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ApexRedirectAllOf.md` & `fastly-3.0.1/docs/ApexRedirectAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ApexRedirectApi.md` & `fastly-3.0.1/docs/ApexRedirectApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AutomationToken.md` & `fastly-3.0.1/docs/AutomationToken.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AutomationTokenCreateRequest.md` & `fastly-3.0.1/docs/AutomationTokenCreateRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AutomationTokenCreateRequestAttributes.md` & `fastly-3.0.1/docs/AutomationTokenCreateRequestAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AutomationTokenCreateResponse.md` & `fastly-3.0.1/docs/AutomationTokenCreateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AutomationTokenCreateResponseAllOf.md` & `fastly-3.0.1/docs/AutomationTokenCreateResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AutomationTokenResponse.md` & `fastly-3.0.1/docs/AutomationTokenResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AutomationTokenResponseAllOf.md` & `fastly-3.0.1/docs/AutomationTokenResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AutomationTokensApi.md` & `fastly-3.0.1/docs/AutomationTokensApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/AwsRegion.md` & `fastly-3.0.1/docs/AwsRegion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Backend.md` & `fastly-3.0.1/docs/Backend.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BackendApi.md` & `fastly-3.0.1/docs/BackendApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BackendResponse.md` & `fastly-3.0.1/docs/BackendResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BackendResponseAllOf.md` & `fastly-3.0.1/docs/BackendResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Batch.md` & `fastly-3.0.1/docs/Batch.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BatchErrors.md` & `fastly-3.0.1/docs/BatchErrors.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Billing.md` & `fastly-3.0.1/docs/Billing.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingAddressApi.md` & `fastly-3.0.1/docs/BillingAddressApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingAddressAttributes.md` & `fastly-3.0.1/docs/BillingAddressAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingAddressRequest.md` & `fastly-3.0.1/docs/BillingAddressRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingAddressRequestData.md` & `fastly-3.0.1/docs/BillingAddressRequestData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingAddressResponse.md` & `fastly-3.0.1/docs/BillingAddressResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingAddressResponseData.md` & `fastly-3.0.1/docs/BillingAddressResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingAddressVerificationErrorResponse.md` & `fastly-3.0.1/docs/BillingAddressVerificationErrorResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingAddressVerificationErrorResponseErrors.md` & `fastly-3.0.1/docs/BillingAddressVerificationErrorResponseErrors.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingApi.md` & `fastly-3.0.1/docs/BillingApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingEstimateResponse.md` & `fastly-3.0.1/docs/BillingResponse.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# BillingEstimateResponse
+# BillingResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **end_time** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **start_time** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **invoice_id** | **str** |  | [optional] [readonly] 
 **customer_id** | **str** |  | [optional] [readonly] 
 **vendor_state** | **str** | The current state of our third-party billing vendor. One of `up` or `down`. | [optional] [readonly] 
 **status** | [**BillingStatus**](BillingStatus.md) |  | [optional] 
 **total** | [**BillingTotal**](BillingTotal.md) |  | [optional] 
 **regions** | **{str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}** | Breakdown of regional data for products that are region based. | [optional] 
-**lines** | [**[BillingEstimateResponseAllOfLines]**](BillingEstimateResponseAllOfLines.md) |  | [optional] 
+**line_items** | [**BillingResponseLineItems**](BillingResponseLineItems.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/BillingEstimateResponseAllOf.md` & `fastly-3.0.1/docs/ServiceInvitationResponse.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# BillingEstimateResponseAllOf
+# ServiceInvitationResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**lines** | [**[BillingEstimateResponseAllOfLines]**](BillingEstimateResponseAllOfLines.md) |  | [optional] 
+**data** | [**ServiceInvitationResponseAllOfData**](ServiceInvitationResponseAllOfData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/BillingEstimateResponseAllOfLine.md` & `fastly-3.0.1/docs/BillingEstimateLinesLineItems.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# BillingEstimateResponseAllOfLine
+# BillingEstimateLinesLineItems
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **plan_no** | **int** |  | [optional] 
 **description** | **str** |  | [optional]
```

### Comparing `fastly-3.0.0/docs/BillingEstimateResponseAllOfLines.md` & `fastly-3.0.1/docs/RelationshipServiceInvitationsCreateServiceInvitations.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# BillingEstimateResponseAllOfLines
+# RelationshipServiceInvitationsCreateServiceInvitations
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**line** | [**BillingEstimateResponseAllOfLine**](BillingEstimateResponseAllOfLine.md) |  | [optional] 
+**data** | [**[ServiceInvitation]**](ServiceInvitation.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/BillingResponse.md` & `fastly-3.0.1/docs/BillingEstimateResponse.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# BillingResponse
+# BillingEstimateResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **end_time** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **start_time** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **invoice_id** | **str** |  | [optional] [readonly] 
 **customer_id** | **str** |  | [optional] [readonly] 
 **vendor_state** | **str** | The current state of our third-party billing vendor. One of `up` or `down`. | [optional] [readonly] 
 **status** | [**BillingStatus**](BillingStatus.md) |  | [optional] 
 **total** | [**BillingTotal**](BillingTotal.md) |  | [optional] 
 **regions** | **{str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}** | Breakdown of regional data for products that are region based. | [optional] 
-**line_items** | [**[BillingResponseLineItem]**](BillingResponseLineItem.md) |  | [optional] 
+**line_items** | [**[BillingEstimateLinesLineItems]**](BillingEstimateLinesLineItems.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/BillingResponseAllOf.md` & `fastly-3.0.1/docs/TlsSubscriptionsResponseAllOf.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# BillingResponseAllOf
+# TlsSubscriptionsResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**line_items** | [**[BillingResponseLineItem]**](BillingResponseLineItem.md) |  | [optional] 
+**data** | [**[TlsSubscriptionResponse]**](TlsSubscriptionResponse.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/BillingResponseLineItem.md` & `fastly-3.0.1/docs/BillingResponseLineItem.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **created_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **deleted_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **updated_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **amount** | **float** |  | [optional] 
-**aria_invoice_id** | **str** |  | [optional] [readonly] 
+**aria_invoice_id** | [**LineItemDataReadOnlyInvoiceId**](LineItemDataReadOnlyInvoiceId.md) |  | [optional] 
 **client_service_id** | **str** |  | [optional] 
 **credit_coupon_code** | **str, none_type** |  | [optional] 
 **description** | **str** |  | [optional] 
 **id** | **str** |  | [optional] 
 **line_number** | **int** |  | [optional] 
 **plan_name** | **str** |  | [optional] 
 **plan_no** | **float** |  | [optional]
```

### Comparing `fastly-3.0.0/docs/BillingResponseLineItemAllOf.md` & `fastly-3.0.1/docs/LineItemData.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# BillingResponseLineItemAllOf
+# LineItemData
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **amount** | **float** |  | [optional] 
-**aria_invoice_id** | **str** |  | [optional] [readonly] 
+**aria_invoice_id** | [**LineItemDataReadOnlyInvoiceId**](LineItemDataReadOnlyInvoiceId.md) |  | [optional] 
 **client_service_id** | **str** |  | [optional] 
 **credit_coupon_code** | **str, none_type** |  | [optional] 
 **description** | **str** |  | [optional] 
 **id** | **str** |  | [optional] 
 **line_number** | **int** |  | [optional] 
 **plan_name** | **str** |  | [optional] 
 **plan_no** | **float** |  | [optional]
```

### Comparing `fastly-3.0.0/docs/BillingStatus.md` & `fastly-3.0.1/docs/EnabledProductResponseService.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# BillingStatus
+# EnabledProductResponseService
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**status** | **str** | What the current status of this invoice can be. | [optional] 
-**sent_at** | **str** |  | [optional] 
+**id** | **str** | Service identifier | [optional] 
+**object** | **str** | Name of the object | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/BillingTotal.md` & `fastly-3.0.1/docs/BillingTotal.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BillingTotalExtras.md` & `fastly-3.0.1/docs/BillingTotalExtras.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BulkUpdateAclEntriesRequest.md` & `fastly-3.0.1/docs/BulkUpdateAclEntriesRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BulkUpdateAclEntry.md` & `fastly-3.0.1/docs/BulkUpdateAclEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BulkUpdateAclEntryAllOf.md` & `fastly-3.0.1/docs/BulkUpdateAclEntryAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BulkUpdateConfigStoreItem.md` & `fastly-3.0.1/docs/BulkUpdateConfigStoreItem.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BulkUpdateConfigStoreItemAllOf.md` & `fastly-3.0.1/docs/BulkUpdateConfigStoreItemAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BulkUpdateConfigStoreListRequest.md` & `fastly-3.0.1/docs/BulkUpdateConfigStoreListRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BulkUpdateDictionaryItem.md` & `fastly-3.0.1/docs/BulkUpdateDictionaryItem.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BulkUpdateDictionaryListRequest.md` & `fastly-3.0.1/docs/BulkUpdateDictionaryListRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/BulkWafActiveRules.md` & `fastly-3.0.1/docs/BulkWafActiveRules.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/CacheSetting.md` & `fastly-3.0.1/docs/CacheSetting.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/CacheSettingResponse.md` & `fastly-3.0.1/docs/CacheSettingResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/CacheSettingsApi.md` & `fastly-3.0.1/docs/CacheSettingsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ClientKey.md` & `fastly-3.0.1/docs/ClientKey.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Condition.md` & `fastly-3.0.1/docs/Condition.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConditionApi.md` & `fastly-3.0.1/docs/ConditionApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConditionResponse.md` & `fastly-3.0.1/docs/ConditionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConfigStore.md` & `fastly-3.0.1/docs/ConfigStore.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConfigStoreApi.md` & `fastly-3.0.1/docs/ConfigStoreApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConfigStoreInfoResponse.md` & `fastly-3.0.1/docs/ConfigStoreInfoResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConfigStoreItem.md` & `fastly-3.0.1/docs/ConfigStoreItem.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConfigStoreItemApi.md` & `fastly-3.0.1/docs/ConfigStoreItemApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConfigStoreItemResponse.md` & `fastly-3.0.1/docs/ConfigStoreItemResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConfigStoreItemResponseAllOf.md` & `fastly-3.0.1/docs/ConfigStoreItemResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConfigStoreResponse.md` & `fastly-3.0.1/docs/ConfigStoreResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ConfigStoreResponseAllOf.md` & `fastly-3.0.1/docs/ConfigStoreResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Contact.md` & `fastly-3.0.1/docs/Contact.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ContactApi.md` & `fastly-3.0.1/docs/ContactApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ContactResponse.md` & `fastly-3.0.1/docs/ContactResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ContactResponseAllOf.md` & `fastly-3.0.1/docs/ContactResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Content.md` & `fastly-3.0.1/docs/Content.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ContentApi.md` & `fastly-3.0.1/docs/ContentApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Customer.md` & `fastly-3.0.1/docs/Customer.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/CustomerApi.md` & `fastly-3.0.1/docs/CustomerApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/CustomerResponse.md` & `fastly-3.0.1/docs/CustomerResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/CustomerResponseAllOf.md` & `fastly-3.0.1/docs/CustomerResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Dictionary.md` & `fastly-3.0.1/docs/Dictionary.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DictionaryApi.md` & `fastly-3.0.1/docs/DictionaryApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DictionaryInfoApi.md` & `fastly-3.0.1/docs/DictionaryInfoApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DictionaryInfoResponse.md` & `fastly-3.0.1/docs/DictionaryInfoResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DictionaryItem.md` & `fastly-3.0.1/docs/DictionaryItem.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DictionaryItemApi.md` & `fastly-3.0.1/docs/DictionaryItemApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DictionaryItemResponse.md` & `fastly-3.0.1/docs/DictionaryItemResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DictionaryItemResponseAllOf.md` & `fastly-3.0.1/docs/DictionaryItemResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DictionaryResponse.md` & `fastly-3.0.1/docs/DictionaryResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DictionaryResponseAllOf.md` & `fastly-3.0.1/docs/DictionaryResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DiffApi.md` & `fastly-3.0.1/docs/DiffApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DiffResponse.md` & `fastly-3.0.1/docs/DiffResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Director.md` & `fastly-3.0.1/docs/Director.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DirectorApi.md` & `fastly-3.0.1/docs/DirectorApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DirectorBackend.md` & `fastly-3.0.1/docs/DirectorBackend.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DirectorBackendAllOf.md` & `fastly-3.0.1/docs/DirectorBackendAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DirectorBackendApi.md` & `fastly-3.0.1/docs/DirectorBackendApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DirectorResponse.md` & `fastly-3.0.1/docs/DirectorResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Domain.md` & `fastly-3.0.1/docs/Domain.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainApi.md` & `fastly-3.0.1/docs/DomainApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainCheckItem.md` & `fastly-3.0.1/docs/DomainCheckItem.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainInspector.md` & `fastly-3.0.1/docs/DomainInspector.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainInspectorEntry.md` & `fastly-3.0.1/docs/DomainInspectorEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainInspectorEntryDimensions.md` & `fastly-3.0.1/docs/DomainInspectorEntryDimensions.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainInspectorEntryValues.md` & `fastly-3.0.1/docs/DomainInspectorEntryValues.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainInspectorHistoricalApi.md` & `fastly-3.0.1/docs/DomainInspectorHistoricalApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainInspectorMeasurements.md` & `fastly-3.0.1/docs/DomainInspectorMeasurements.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainInspectorRealtimeApi.md` & `fastly-3.0.1/docs/DomainInspectorRealtimeApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainInspectorRealtimeEntry.md` & `fastly-3.0.1/docs/DomainInspectorRealtimeEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainOwnershipsApi.md` & `fastly-3.0.1/docs/DomainOwnershipsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/DomainResponse.md` & `fastly-3.0.1/docs/DomainResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/EnabledProductResponse.md` & `fastly-3.0.1/docs/EnabledProductResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/EnabledProductResponseLinks.md` & `fastly-3.0.1/docs/EnabledProductResponseLinks.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/EnabledProductResponseProduct.md` & `fastly-3.0.1/docs/EnabledProductResponseProduct.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/EnabledProductResponseService.md` & `fastly-3.0.1/docs/StoreResponse.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# EnabledProductResponseService
+# StoreResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**id** | **str** | Service identifier | [optional] 
-**object** | **str** | Name of the object | [optional] 
+**id** | **str** | ID of the store. | [optional] 
+**name** | **str** | A human-readable name for the store. | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/EnabledProductsApi.md` & `fastly-3.0.1/docs/EnabledProductsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ErrorResponse.md` & `fastly-3.0.1/docs/ErrorResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Event.md` & `fastly-3.0.1/docs/Event.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/EventAttributes.md` & `fastly-3.0.1/docs/EventAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/EventData.md` & `fastly-3.0.1/docs/EventData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/EventsApi.md` & `fastly-3.0.1/docs/EventsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/EventsResponse.md` & `fastly-3.0.1/docs/EventsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Gzip.md` & `fastly-3.0.1/docs/Gzip.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/GzipApi.md` & `fastly-3.0.1/docs/GzipApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/GzipResponse.md` & `fastly-3.0.1/docs/GzipResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Header.md` & `fastly-3.0.1/docs/Header.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HeaderApi.md` & `fastly-3.0.1/docs/HeaderApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HeaderResponse.md` & `fastly-3.0.1/docs/HeaderResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Healthcheck.md` & `fastly-3.0.1/docs/Healthcheck.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HealthcheckApi.md` & `fastly-3.0.1/docs/HealthcheckApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HealthcheckResponse.md` & `fastly-3.0.1/docs/HealthcheckResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Historical.md` & `fastly-3.0.1/docs/Historical.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalAggregateResponse.md` & `fastly-3.0.1/docs/HistoricalAggregateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalAggregateResponseAllOf.md` & `fastly-3.0.1/docs/HistoricalAggregateResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalApi.md` & `fastly-3.0.1/docs/HistoricalApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalDomains.md` & `fastly-3.0.1/docs/HistoricalDomains.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalDomainsData.md` & `fastly-3.0.1/docs/HistoricalDomainsData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalDomainsMeta.md` & `fastly-3.0.1/docs/HistoricalDomainsMeta.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalDomainsMetaFilters.md` & `fastly-3.0.1/docs/HistoricalDomainsMetaFilters.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalDomainsResponse.md` & `fastly-3.0.1/docs/HistoricalDomainsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalDomainsResponseAllOf.md` & `fastly-3.0.1/docs/HistoricalDomainsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalFieldAggregateResponse.md` & `fastly-3.0.1/docs/HistoricalFieldAggregateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalFieldAggregateResponseAllOf.md` & `fastly-3.0.1/docs/HistoricalFieldAggregateResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalFieldResponse.md` & `fastly-3.0.1/docs/HistoricalFieldResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalFieldResponseDataField.md` & `fastly-3.0.1/docs/HistoricalFieldResponseDataField.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalFieldResultsAttributes.md` & `fastly-3.0.1/docs/HistoricalFieldResultsAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalFieldResultsAttributesAdditional.md` & `fastly-3.0.1/docs/HistoricalFieldResultsAttributesAdditional.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalMeta.md` & `fastly-3.0.1/docs/HistoricalMeta.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalOriginsResponse.md` & `fastly-3.0.1/docs/HistoricalOriginsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalOriginsResponseAllOf.md` & `fastly-3.0.1/docs/HistoricalOriginsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalRegionsResponse.md` & `fastly-3.0.1/docs/HistoricalRegionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalRegionsResponseAllOf.md` & `fastly-3.0.1/docs/HistoricalRegionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalResponse.md` & `fastly-3.0.1/docs/HistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalResponseDataField.md` & `fastly-3.0.1/docs/HistoricalResponseDataField.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalService.md` & `fastly-3.0.1/docs/HistoricalService.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalUsageAggregateResponse.md` & `fastly-3.0.1/docs/HistoricalUsageAggregateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalUsageMonthResponse.md` & `fastly-3.0.1/docs/HistoricalUsageMonthResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalUsageMonthResponseAllOf.md` & `fastly-3.0.1/docs/HistoricalUsageMonthResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalUsageMonthResponseData.md` & `fastly-3.0.1/docs/HistoricalUsageMonthResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalUsageResults.md` & `fastly-3.0.1/docs/HistoricalUsageResults.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalUsageServiceResponse.md` & `fastly-3.0.1/docs/HistoricalUsageServiceResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HistoricalUsageServiceResponseAllOf.md` & `fastly-3.0.1/docs/HistoricalUsageServiceResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Http3.md` & `fastly-3.0.1/docs/Http3.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Http3AllOf.md` & `fastly-3.0.1/docs/Http3AllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Http3Api.md` & `fastly-3.0.1/docs/Http3Api.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HttpResponseFormat.md` & `fastly-3.0.1/docs/HttpResponseFormat.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/HttpStreamFormat.md` & `fastly-3.0.1/docs/HttpStreamFormat.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamPermission.md` & `fastly-3.0.1/docs/IamPermission.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamPermissionsApi.md` & `fastly-3.0.1/docs/IamPermissionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamRole.md` & `fastly-3.0.1/docs/IamRole.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamRoleAllOf.md` & `fastly-3.0.1/docs/IamRoleAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamRolesApi.md` & `fastly-3.0.1/docs/IamRolesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamServiceGroup.md` & `fastly-3.0.1/docs/IamServiceGroup.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamServiceGroupAllOf.md` & `fastly-3.0.1/docs/IamServiceGroupAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamServiceGroupsApi.md` & `fastly-3.0.1/docs/IamServiceGroupsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamUserGroup.md` & `fastly-3.0.1/docs/IamUserGroup.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamUserGroupAllOf.md` & `fastly-3.0.1/docs/IamUserGroupAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IamUserGroupsApi.md` & `fastly-3.0.1/docs/IamUserGroupsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IncludedWithWafActiveRuleItem.md` & `fastly-3.0.1/docs/IncludedWithWafActiveRuleItem.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IncludedWithWafExclusionItem.md` & `fastly-3.0.1/docs/IncludedWithWafExclusionItem.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IncludedWithWafFirewallVersionItem.md` & `fastly-3.0.1/docs/IncludedWithWafFirewallVersionItem.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/IncludedWithWafRuleItem.md` & `fastly-3.0.1/docs/IncludedWithWafRuleItem.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InlineResponse2001.md` & `fastly-3.0.1/docs/InlineResponse2001.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InlineResponse2002.md` & `fastly-3.0.1/docs/InlineResponse2002.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InlineResponse2003.md` & `fastly-3.0.1/docs/InlineResponse2003.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InlineResponse2003Meta.md` & `fastly-3.0.1/docs/InlineResponse2003Meta.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InlineResponse2004.md` & `fastly-3.0.1/docs/InlineResponse2004.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InlineResponse2004Meta.md` & `fastly-3.0.1/docs/InlineResponse2004Meta.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InlineResponse2005.md` & `fastly-3.0.1/docs/InlineResponse2005.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InlineResponse2006.md` & `fastly-3.0.1/docs/InlineResponse2006.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InlineResponse2007.md` & `fastly-3.0.1/docs/InlineResponse2007.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Invitation.md` & `fastly-3.0.1/docs/Invitation.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InvitationData.md` & `fastly-3.0.1/docs/InvitationData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InvitationDataAttributes.md` & `fastly-3.0.1/docs/InvitationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InvitationResponse.md` & `fastly-3.0.1/docs/InvitationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InvitationResponseAllOf.md` & `fastly-3.0.1/docs/InvitationResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InvitationResponseData.md` & `fastly-3.0.1/docs/InvitationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InvitationResponseDataAllOf.md` & `fastly-3.0.1/docs/InvitationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InvitationsApi.md` & `fastly-3.0.1/docs/InvitationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InvitationsResponse.md` & `fastly-3.0.1/docs/InvitationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/InvitationsResponseAllOf.md` & `fastly-3.0.1/docs/InvitationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/KvStoreApi.md` & `fastly-3.0.1/docs/KvStoreApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/KvStoreItemApi.md` & `fastly-3.0.1/docs/KvStoreItemApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafConfigurationSet.md` & `fastly-3.0.1/docs/LegacyWafConfigurationSet.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafConfigurationSetsApi.md` & `fastly-3.0.1/docs/LegacyWafConfigurationSetsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafFirewall.md` & `fastly-3.0.1/docs/LegacyWafFirewall.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafFirewallApi.md` & `fastly-3.0.1/docs/LegacyWafFirewallApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafOwasp.md` & `fastly-3.0.1/docs/LegacyWafOwasp.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafOwaspApi.md` & `fastly-3.0.1/docs/LegacyWafOwaspApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafRule.md` & `fastly-3.0.1/docs/LegacyWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafRuleApi.md` & `fastly-3.0.1/docs/LegacyWafRuleApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafRuleStatus.md` & `fastly-3.0.1/docs/LegacyWafRuleStatus.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafRuleStatusApi.md` & `fastly-3.0.1/docs/LegacyWafRuleStatusApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafRuleset.md` & `fastly-3.0.1/docs/LegacyWafRuleset.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafRulesetApi.md` & `fastly-3.0.1/docs/LegacyWafRulesetApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafTag.md` & `fastly-3.0.1/docs/LegacyWafTag.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafTagApi.md` & `fastly-3.0.1/docs/LegacyWafTagApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafUpdateStatus.md` & `fastly-3.0.1/docs/LegacyWafUpdateStatus.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LegacyWafUpdateStatusApi.md` & `fastly-3.0.1/docs/LegacyWafUpdateStatusApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingAddressAndPort.md` & `fastly-3.0.1/docs/LoggingAddressAndPort.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingAzureblob.md` & `fastly-3.0.1/docs/LoggingAzureblob.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingAzureblobAllOf.md` & `fastly-3.0.1/docs/LoggingAzureblobAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingAzureblobApi.md` & `fastly-3.0.1/docs/LoggingAzureblobApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingAzureblobResponse.md` & `fastly-3.0.1/docs/LoggingAzureblobResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingBigquery.md` & `fastly-3.0.1/docs/LoggingBigquery.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingBigqueryAllOf.md` & `fastly-3.0.1/docs/LoggingBigqueryAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingBigqueryApi.md` & `fastly-3.0.1/docs/LoggingBigqueryApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingBigqueryResponse.md` & `fastly-3.0.1/docs/LoggingBigqueryResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingCloudfiles.md` & `fastly-3.0.1/docs/LoggingCloudfiles.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingCloudfilesAllOf.md` & `fastly-3.0.1/docs/LoggingCloudfilesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingCloudfilesApi.md` & `fastly-3.0.1/docs/LoggingCloudfilesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingCloudfilesResponse.md` & `fastly-3.0.1/docs/LoggingCloudfilesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingCommon.md` & `fastly-3.0.1/docs/LoggingCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingDatadog.md` & `fastly-3.0.1/docs/LoggingDatadog.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingDatadogAllOf.md` & `fastly-3.0.1/docs/LoggingDatadogAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingDatadogApi.md` & `fastly-3.0.1/docs/LoggingDatadogApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingDatadogResponse.md` & `fastly-3.0.1/docs/LoggingDatadogResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingDigitalocean.md` & `fastly-3.0.1/docs/LoggingDigitalocean.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingDigitaloceanAllOf.md` & `fastly-3.0.1/docs/LoggingDigitaloceanAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingDigitaloceanApi.md` & `fastly-3.0.1/docs/LoggingDigitaloceanApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingDigitaloceanResponse.md` & `fastly-3.0.1/docs/LoggingDigitaloceanResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingElasticsearch.md` & `fastly-3.0.1/docs/LoggingElasticsearch.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingElasticsearchAllOf.md` & `fastly-3.0.1/docs/LoggingElasticsearchAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingElasticsearchApi.md` & `fastly-3.0.1/docs/LoggingElasticsearchApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingElasticsearchResponse.md` & `fastly-3.0.1/docs/LoggingElasticsearchResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingFormatVersion.md` & `fastly-3.0.1/docs/LoggingFormatVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingFtp.md` & `fastly-3.0.1/docs/LoggingFtp.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingFtpAllOf.md` & `fastly-3.0.1/docs/LoggingFtpAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingFtpApi.md` & `fastly-3.0.1/docs/LoggingFtpApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingFtpResponse.md` & `fastly-3.0.1/docs/LoggingFtpResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingGcs.md` & `fastly-3.0.1/docs/LoggingGcs.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingGcsAllOf.md` & `fastly-3.0.1/docs/LoggingGcsAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingGcsApi.md` & `fastly-3.0.1/docs/LoggingGcsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingGcsCommon.md` & `fastly-3.0.1/docs/LoggingGcsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingGcsResponse.md` & `fastly-3.0.1/docs/LoggingGcsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingGenericCommon.md` & `fastly-3.0.1/docs/LoggingGenericCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingGooglePubsub.md` & `fastly-3.0.1/docs/LoggingGooglePubsub.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingGooglePubsubAllOf.md` & `fastly-3.0.1/docs/LoggingGooglePubsubAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingGooglePubsubResponse.md` & `fastly-3.0.1/docs/LoggingGooglePubsubResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHeroku.md` & `fastly-3.0.1/docs/LoggingHeroku.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHerokuAllOf.md` & `fastly-3.0.1/docs/LoggingHerokuAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHerokuApi.md` & `fastly-3.0.1/docs/LoggingHerokuApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHerokuResponse.md` & `fastly-3.0.1/docs/LoggingHerokuResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHoneycomb.md` & `fastly-3.0.1/docs/LoggingHoneycomb.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHoneycombAllOf.md` & `fastly-3.0.1/docs/LoggingHoneycombAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHoneycombApi.md` & `fastly-3.0.1/docs/LoggingHoneycombApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHoneycombResponse.md` & `fastly-3.0.1/docs/LoggingHoneycombResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHttps.md` & `fastly-3.0.1/docs/LoggingHttps.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHttpsAllOf.md` & `fastly-3.0.1/docs/LoggingHttpsAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHttpsApi.md` & `fastly-3.0.1/docs/LoggingHttpsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingHttpsResponse.md` & `fastly-3.0.1/docs/LoggingHttpsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingKafka.md` & `fastly-3.0.1/docs/LoggingKafka.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingKafkaAllOf.md` & `fastly-3.0.1/docs/LoggingKafkaAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingKafkaApi.md` & `fastly-3.0.1/docs/LoggingKafkaApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingKafkaResponse.md` & `fastly-3.0.1/docs/LoggingKafkaResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingKinesis.md` & `fastly-3.0.1/docs/LoggingKinesis.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingKinesisApi.md` & `fastly-3.0.1/docs/LoggingKinesisApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingKinesisResponse.md` & `fastly-3.0.1/docs/LoggingKinesisResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogentries.md` & `fastly-3.0.1/docs/LoggingLogentries.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogentriesAllOf.md` & `fastly-3.0.1/docs/LoggingLogentriesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogentriesApi.md` & `fastly-3.0.1/docs/LoggingLogentriesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogentriesResponse.md` & `fastly-3.0.1/docs/LoggingLogentriesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLoggly.md` & `fastly-3.0.1/docs/LoggingLoggly.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogglyAllOf.md` & `fastly-3.0.1/docs/LoggingLogglyAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogglyApi.md` & `fastly-3.0.1/docs/LoggingLogglyApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogglyResponse.md` & `fastly-3.0.1/docs/LoggingLogglyResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogshuttle.md` & `fastly-3.0.1/docs/LoggingLogshuttle.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogshuttleAllOf.md` & `fastly-3.0.1/docs/LoggingLogshuttleAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogshuttleApi.md` & `fastly-3.0.1/docs/LoggingLogshuttleApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingLogshuttleResponse.md` & `fastly-3.0.1/docs/LoggingLogshuttleResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingNewrelic.md` & `fastly-3.0.1/docs/LoggingNewrelic.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingNewrelicAllOf.md` & `fastly-3.0.1/docs/LoggingNewrelicAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingNewrelicApi.md` & `fastly-3.0.1/docs/LoggingNewrelicApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingNewrelicResponse.md` & `fastly-3.0.1/docs/LoggingNewrelicResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingOpenstack.md` & `fastly-3.0.1/docs/LoggingOpenstack.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingOpenstackAllOf.md` & `fastly-3.0.1/docs/LoggingOpenstackAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingOpenstackApi.md` & `fastly-3.0.1/docs/LoggingOpenstackApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingOpenstackResponse.md` & `fastly-3.0.1/docs/LoggingOpenstackResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingPapertrail.md` & `fastly-3.0.1/docs/LoggingPapertrail.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingPapertrailApi.md` & `fastly-3.0.1/docs/LoggingPapertrailApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingPapertrailResponse.md` & `fastly-3.0.1/docs/LoggingPapertrailResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingPlacement.md` & `fastly-3.0.1/docs/LoggingPlacement.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingPubsubApi.md` & `fastly-3.0.1/docs/LoggingPubsubApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingRequestCapsCommon.md` & `fastly-3.0.1/docs/LoggingRequestCapsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingS3.md` & `fastly-3.0.1/docs/LoggingS3.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingS3AllOf.md` & `fastly-3.0.1/docs/LoggingS3AllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingS3Api.md` & `fastly-3.0.1/docs/LoggingS3Api.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingS3Response.md` & `fastly-3.0.1/docs/LoggingS3Response.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingScalyr.md` & `fastly-3.0.1/docs/LoggingScalyr.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingScalyrAllOf.md` & `fastly-3.0.1/docs/LoggingScalyrAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingScalyrApi.md` & `fastly-3.0.1/docs/LoggingScalyrApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingScalyrResponse.md` & `fastly-3.0.1/docs/LoggingScalyrResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSftp.md` & `fastly-3.0.1/docs/LoggingSftp.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSftpAllOf.md` & `fastly-3.0.1/docs/LoggingSftpAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSftpApi.md` & `fastly-3.0.1/docs/LoggingSftpApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSftpResponse.md` & `fastly-3.0.1/docs/LoggingSftpResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSplunk.md` & `fastly-3.0.1/docs/LoggingSplunk.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSplunkAllOf.md` & `fastly-3.0.1/docs/LoggingSplunkAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSplunkApi.md` & `fastly-3.0.1/docs/LoggingSplunkApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSplunkResponse.md` & `fastly-3.0.1/docs/LoggingSplunkResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSumologic.md` & `fastly-3.0.1/docs/LoggingSumologic.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSumologicAllOf.md` & `fastly-3.0.1/docs/LoggingSumologicAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSumologicApi.md` & `fastly-3.0.1/docs/LoggingSumologicApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSumologicResponse.md` & `fastly-3.0.1/docs/LoggingSumologicResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSyslog.md` & `fastly-3.0.1/docs/LoggingSyslog.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSyslogAllOf.md` & `fastly-3.0.1/docs/LoggingSyslogAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSyslogApi.md` & `fastly-3.0.1/docs/LoggingSyslogApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingSyslogResponse.md` & `fastly-3.0.1/docs/LoggingSyslogResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/LoggingTlsCommon.md` & `fastly-3.0.1/docs/LoggingTlsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthentication.md` & `fastly-3.0.1/docs/MutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthenticationApi.md` & `fastly-3.0.1/docs/MutualAuthenticationApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthenticationData.md` & `fastly-3.0.1/docs/MutualAuthenticationData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthenticationDataAttributes.md` & `fastly-3.0.1/docs/MutualAuthenticationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthenticationResponse.md` & `fastly-3.0.1/docs/MutualAuthenticationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthenticationResponseAttributes.md` & `fastly-3.0.1/docs/MutualAuthenticationResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthenticationResponseAttributesAllOf.md` & `fastly-3.0.1/docs/MutualAuthenticationResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthenticationResponseData.md` & `fastly-3.0.1/docs/MutualAuthenticationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthenticationResponseDataAllOf.md` & `fastly-3.0.1/docs/MutualAuthenticationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthenticationsResponse.md` & `fastly-3.0.1/docs/MutualAuthenticationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/MutualAuthenticationsResponseAllOf.md` & `fastly-3.0.1/docs/MutualAuthenticationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspector.md` & `fastly-3.0.1/docs/OriginInspector.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorDimensions.md` & `fastly-3.0.1/docs/OriginInspectorDimensions.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorEntry.md` & `fastly-3.0.1/docs/OriginInspectorEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorHistorical.md` & `fastly-3.0.1/docs/OriginInspectorHistorical.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorHistoricalApi.md` & `fastly-3.0.1/docs/OriginInspectorHistoricalApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorHistoricalData.md` & `fastly-3.0.1/docs/OriginInspectorHistoricalData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorHistoricalMeta.md` & `fastly-3.0.1/docs/OriginInspectorHistoricalMeta.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorHistoricalMetaFilters.md` & `fastly-3.0.1/docs/OriginInspectorHistoricalMetaFilters.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorMeasurements.md` & `fastly-3.0.1/docs/OriginInspectorMeasurements.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorRealtimeApi.md` & `fastly-3.0.1/docs/OriginInspectorRealtimeApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorRealtimeEntry.md` & `fastly-3.0.1/docs/OriginInspectorRealtimeEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorRealtimeEntryRecorded.md` & `fastly-3.0.1/docs/OriginInspectorRealtimeEntryRecorded.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorSubsequentRequestTimestamp.md` & `fastly-3.0.1/docs/OriginInspectorSubsequentRequestTimestamp.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/OriginInspectorValues.md` & `fastly-3.0.1/docs/OriginInspectorValues.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Package.md` & `fastly-3.0.1/docs/Package.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PackageApi.md` & `fastly-3.0.1/docs/PackageApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PackageMetadata.md` & `fastly-3.0.1/docs/PackageMetadata.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PackageResponse.md` & `fastly-3.0.1/docs/PackageResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PackageResponseAllOf.md` & `fastly-3.0.1/docs/PackageResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Pagination.md` & `fastly-3.0.1/docs/Pagination.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PaginationCursorMeta.md` & `fastly-3.0.1/docs/PaginationCursorMeta.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PaginationLinks.md` & `fastly-3.0.1/docs/PaginationLinks.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PaginationMeta.md` & `fastly-3.0.1/docs/PaginationMeta.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Permission.md` & `fastly-3.0.1/docs/Permission.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Pool.md` & `fastly-3.0.1/docs/Pool.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PoolAllOf.md` & `fastly-3.0.1/docs/PoolAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PoolApi.md` & `fastly-3.0.1/docs/PoolApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PoolResponse.md` & `fastly-3.0.1/docs/PoolResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Pop.md` & `fastly-3.0.1/docs/Pop.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PopApi.md` & `fastly-3.0.1/docs/PopApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PopCoordinates.md` & `fastly-3.0.1/docs/PopCoordinates.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PublicIpList.md` & `fastly-3.0.1/docs/PublicIpList.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PublicIpListApi.md` & `fastly-3.0.1/docs/PublicIpListApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PublishApi.md` & `fastly-3.0.1/docs/PublishApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PublishItem.md` & `fastly-3.0.1/docs/PublishItem.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PublishItemFormats.md` & `fastly-3.0.1/docs/PublishItemFormats.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PublishRequest.md` & `fastly-3.0.1/docs/PublishRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PurgeApi.md` & `fastly-3.0.1/docs/PurgeApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PurgeKeys.md` & `fastly-3.0.1/docs/PurgeKeys.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/PurgeResponse.md` & `fastly-3.0.1/docs/PurgeResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RateLimiter.md` & `fastly-3.0.1/docs/RateLimiter.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RateLimiterApi.md` & `fastly-3.0.1/docs/RateLimiterApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RateLimiterResponse.md` & `fastly-3.0.1/docs/RateLimiterResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RateLimiterResponseAllOf.md` & `fastly-3.0.1/docs/RateLimiterResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Realtime.md` & `fastly-3.0.1/docs/Realtime.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RealtimeApi.md` & `fastly-3.0.1/docs/RealtimeApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RealtimeEntry.md` & `fastly-3.0.1/docs/RealtimeEntry.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RealtimeEntryAggregated.md` & `fastly-3.0.1/docs/RealtimeEntryAggregated.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RealtimeEntryDatacenter.md` & `fastly-3.0.1/docs/RealtimeEntryDatacenter.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RealtimeMeasurements.md` & `fastly-3.0.1/docs/RealtimeMeasurements.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RecordedTimestamp.md` & `fastly-3.0.1/docs/RecordedTimestamp.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipCommonName.md` & `fastly-3.0.1/docs/RelationshipCommonName.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipCustomer.md` & `fastly-3.0.1/docs/RelationshipCustomer.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipCustomerCustomer.md` & `fastly-3.0.1/docs/RelationshipCustomerCustomer.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberCustomer.md` & `fastly-3.0.1/docs/RelationshipMemberCustomer.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberMutualAuthentication.md` & `fastly-3.0.1/docs/RelationshipMemberMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberService.md` & `fastly-3.0.1/docs/RelationshipMemberService.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberServiceInvitation.md` & `fastly-3.0.1/docs/RelationshipMemberServiceInvitation.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberTlsActivation.md` & `fastly-3.0.1/docs/RelationshipMemberTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberTlsBulkCertificate.md` & `fastly-3.0.1/docs/RelationshipMemberTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberTlsCertificate.md` & `fastly-3.0.1/docs/RelationshipMemberTlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberTlsConfiguration.md` & `fastly-3.0.1/docs/RelationshipMemberTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberTlsDnsRecord.md` & `fastly-3.0.1/docs/RelationshipMemberTlsDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberTlsDomain.md` & `fastly-3.0.1/docs/RelationshipMemberTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberTlsPrivateKey.md` & `fastly-3.0.1/docs/RelationshipMemberTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberTlsSubscription.md` & `fastly-3.0.1/docs/RelationshipMemberTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberWafActiveRule.md` & `fastly-3.0.1/docs/RelationshipMemberWafActiveRule.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberWafFirewall.md` & `fastly-3.0.1/docs/RelationshipMemberWafFirewall.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberWafFirewallVersion.md` & `fastly-3.0.1/docs/RelationshipMemberWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberWafRule.md` & `fastly-3.0.1/docs/RelationshipMemberWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberWafRuleRevision.md` & `fastly-3.0.1/docs/RelationshipMemberWafRuleRevision.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMemberWafTag.md` & `fastly-3.0.1/docs/RelationshipMemberWafTag.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMutualAuthentication.md` & `fastly-3.0.1/docs/RelationshipMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMutualAuthenticationMutualAuthentication.md` & `fastly-3.0.1/docs/RelationshipMutualAuthenticationMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMutualAuthentications.md` & `fastly-3.0.1/docs/RelationshipMutualAuthentications.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipMutualAuthenticationsMutualAuthentications.md` & `fastly-3.0.1/docs/RelationshipMutualAuthenticationsMutualAuthentications.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipService.md` & `fastly-3.0.1/docs/RelationshipService.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipServiceInvitations.md` & `fastly-3.0.1/docs/RelationshipServiceInvitations.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipServiceInvitationsCreate.md` & `fastly-3.0.1/docs/RelationshipServiceInvitationsCreate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipServiceInvitationsCreateServiceInvitations.md` & `fastly-3.0.1/docs/ServiceAuthorizationsResponse.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# RelationshipServiceInvitationsCreateServiceInvitations
+# ServiceAuthorizationsResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[ServiceInvitation]**](ServiceInvitation.md) |  | [optional] 
+**links** | [**PaginationLinks**](PaginationLinks.md) |  | [optional] 
+**meta** | [**PaginationMeta**](PaginationMeta.md) |  | [optional] 
+**data** | [**[ServiceAuthorizationResponseData]**](ServiceAuthorizationResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/RelationshipServiceInvitationsServiceInvitations.md` & `fastly-3.0.1/docs/RelationshipServiceInvitationsServiceInvitations.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipServices.md` & `fastly-3.0.1/docs/RelationshipServices.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipServicesServices.md` & `fastly-3.0.1/docs/RelationshipServicesServices.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsActivation.md` & `fastly-3.0.1/docs/RelationshipTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsActivationTlsActivation.md` & `fastly-3.0.1/docs/RelationshipTlsActivationTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsActivations.md` & `fastly-3.0.1/docs/RelationshipTlsActivations.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsBulkCertificate.md` & `fastly-3.0.1/docs/RelationshipTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md` & `fastly-3.0.1/docs/RelationshipTlsBulkCertificateTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsBulkCertificates.md` & `fastly-3.0.1/docs/RelationshipTlsBulkCertificates.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsCertificate.md` & `fastly-3.0.1/docs/RelationshipTlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsCertificateTlsCertificate.md` & `fastly-3.0.1/docs/RelationshipTlsCertificateTlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsCertificates.md` & `fastly-3.0.1/docs/RelationshipTlsCertificates.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsCertificatesTlsCertificates.md` & `fastly-3.0.1/docs/RelationshipTlsCertificatesTlsCertificates.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsConfiguration.md` & `fastly-3.0.1/docs/RelationshipTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsConfigurationForTlsSubscription.md` & `fastly-3.0.1/docs/RelationshipTlsConfigurationForTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsConfigurationTlsConfiguration.md` & `fastly-3.0.1/docs/RelationshipTlsConfigurationTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsConfigurations.md` & `fastly-3.0.1/docs/RelationshipTlsConfigurations.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsConfigurationsTlsConfigurations.md` & `fastly-3.0.1/docs/RelationshipTlsConfigurationsTlsConfigurations.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsDnsRecord.md` & `fastly-3.0.1/docs/RelationshipTlsDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsDnsRecordDnsRecord.md` & `fastly-3.0.1/docs/RelationshipTlsDnsRecordDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsDnsRecords.md` & `fastly-3.0.1/docs/RelationshipTlsDnsRecords.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsDomain.md` & `fastly-3.0.1/docs/RelationshipTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsDomainTlsDomain.md` & `fastly-3.0.1/docs/RelationshipTlsDomainTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsDomains.md` & `fastly-3.0.1/docs/RelationshipTlsDomains.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsDomainsTlsDomains.md` & `fastly-3.0.1/docs/RelationshipTlsDomainsTlsDomains.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsPrivateKey.md` & `fastly-3.0.1/docs/RelationshipTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md` & `fastly-3.0.1/docs/RelationshipTlsPrivateKeyTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsPrivateKeys.md` & `fastly-3.0.1/docs/RelationshipTlsPrivateKeys.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md` & `fastly-3.0.1/docs/RelationshipTlsPrivateKeysTlsPrivateKeys.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsSubscription.md` & `fastly-3.0.1/docs/RelationshipTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsSubscriptionTlsSubscription.md` & `fastly-3.0.1/docs/RelationshipTlsSubscriptionTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipTlsSubscriptions.md` & `fastly-3.0.1/docs/RelationshipTlsSubscriptions.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipUser.md` & `fastly-3.0.1/docs/RelationshipUser.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipUserUser.md` & `fastly-3.0.1/docs/RelationshipUserUser.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafActiveRules.md` & `fastly-3.0.1/docs/RelationshipWafActiveRules.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafActiveRulesWafActiveRules.md` & `fastly-3.0.1/docs/RelationshipWafActiveRulesWafActiveRules.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafFirewall.md` & `fastly-3.0.1/docs/RelationshipWafFirewall.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafFirewallVersion.md` & `fastly-3.0.1/docs/RelationshipWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafFirewallVersionWafFirewallVersion.md` & `fastly-3.0.1/docs/RelationshipWafFirewallVersionWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafFirewallVersions.md` & `fastly-3.0.1/docs/RelationshipWafFirewallVersions.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafFirewallWafFirewall.md` & `fastly-3.0.1/docs/RelationshipWafFirewallWafFirewall.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafRule.md` & `fastly-3.0.1/docs/RelationshipWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafRuleRevision.md` & `fastly-3.0.1/docs/RelationshipWafRuleRevision.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafRuleRevisionWafRuleRevisions.md` & `fastly-3.0.1/docs/RelationshipWafRuleRevisionWafRuleRevisions.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafRuleRevisions.md` & `fastly-3.0.1/docs/RelationshipWafRuleRevisions.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafRuleWafRule.md` & `fastly-3.0.1/docs/RelationshipWafRuleWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafRules.md` & `fastly-3.0.1/docs/RelationshipWafRules.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafTags.md` & `fastly-3.0.1/docs/RelationshipWafTags.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipWafTagsWafTags.md` & `fastly-3.0.1/docs/RelationshipWafTagsWafTags.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForInvitation.md` & `fastly-3.0.1/docs/RelationshipsForInvitation.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForMutualAuthentication.md` & `fastly-3.0.1/docs/RelationshipsForMutualAuthentication.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForStar.md` & `fastly-3.0.1/docs/RelationshipsForStar.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForTlsActivation.md` & `fastly-3.0.1/docs/RelationshipsForTlsActivation.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForTlsBulkCertificate.md` & `fastly-3.0.1/docs/RelationshipsForTlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForTlsConfiguration.md` & `fastly-3.0.1/docs/RelationshipsForTlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForTlsDomain.md` & `fastly-3.0.1/docs/RelationshipsForTlsDomain.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForTlsPrivateKey.md` & `fastly-3.0.1/docs/RelationshipsForTlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForTlsSubscription.md` & `fastly-3.0.1/docs/RelationshipsForTlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForWafActiveRule.md` & `fastly-3.0.1/docs/RelationshipsForWafActiveRule.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForWafExclusion.md` & `fastly-3.0.1/docs/RelationshipsForWafExclusion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForWafFirewallVersion.md` & `fastly-3.0.1/docs/RelationshipsForWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RelationshipsForWafRule.md` & `fastly-3.0.1/docs/RelationshipsForWafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RequestSettings.md` & `fastly-3.0.1/docs/RequestSettings.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RequestSettingsApi.md` & `fastly-3.0.1/docs/RequestSettingsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RequestSettingsResponse.md` & `fastly-3.0.1/docs/RequestSettingsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Resource.md` & `fastly-3.0.1/docs/Resource.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ResourceApi.md` & `fastly-3.0.1/docs/ResourceApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ResourceResponse.md` & `fastly-3.0.1/docs/ResourceResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ResourceResponseAllOf.md` & `fastly-3.0.1/docs/ResourceResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ResponseObject.md` & `fastly-3.0.1/docs/ResponseObject.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ResponseObjectApi.md` & `fastly-3.0.1/docs/ResponseObjectApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ResponseObjectResponse.md` & `fastly-3.0.1/docs/ResponseObjectResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Results.md` & `fastly-3.0.1/docs/Results.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/RoleUser.md` & `fastly-3.0.1/docs/RoleUser.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SchemasContactResponse.md` & `fastly-3.0.1/docs/SchemasContactResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SchemasSnippetResponse.md` & `fastly-3.0.1/docs/SchemasSnippetResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SchemasUserResponse.md` & `fastly-3.0.1/docs/SchemasUserResponse.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **login** | **str** |  | [optional] [readonly] 
 **name** | **str** | The real life name of the user. | [optional] 
 **limit_services** | **bool** | Indicates that the user has limited access to the customer&#39;s services. | [optional] 
-**locked** | **bool** | Indicates whether the is account is locked for editing or not. | [optional] 
-**require_new_password** | **bool** | Indicates if a new password is required at next login. | [optional] 
+**locked** | **bool, none_type** | Indicates whether the is account is locked for editing or not. | [optional] 
+**require_new_password** | **bool, none_type** | Indicates if a new password is required at next login. | [optional] 
 **role** | [**RoleUser**](RoleUser.md) |  | [optional] 
-**two_factor_auth_enabled** | **bool** | Indicates if 2FA is enabled on the user. | [optional] 
+**two_factor_auth_enabled** | **bool, none_type** | Indicates if 2FA is enabled on the user. | [optional] 
 **two_factor_setup_required** | **bool** | Indicates if 2FA is required by the user&#39;s customer account. | [optional] 
 **created_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **deleted_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **updated_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **id** | **str** |  | [optional] [readonly] 
 **email_hash** | **str** | The alphanumeric string identifying a email login. | [optional] [readonly] 
 **customer_id** | **str** |  | [optional] [readonly]
```

### Comparing `fastly-3.0.0/docs/SchemasVclResponse.md` & `fastly-3.0.1/docs/SchemasVclResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SchemasVersion.md` & `fastly-3.0.1/docs/SchemasVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SchemasVersionResponse.md` & `fastly-3.0.1/docs/SchemasVersionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SchemasWafFirewallVersion.md` & `fastly-3.0.1/docs/SchemasWafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SchemasWafFirewallVersionData.md` & `fastly-3.0.1/docs/SchemasWafFirewallVersionData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Secret.md` & `fastly-3.0.1/docs/Secret.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SecretResponse.md` & `fastly-3.0.1/docs/SecretResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SecretStore.md` & `fastly-3.0.1/docs/SecretStore.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SecretStoreApi.md` & `fastly-3.0.1/docs/SecretStoreApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SecretStoreItemApi.md` & `fastly-3.0.1/docs/SecretStoreItemApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SecretStoreResponse.md` & `fastly-3.0.1/docs/SecretStoreResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Server.md` & `fastly-3.0.1/docs/Server.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServerApi.md` & `fastly-3.0.1/docs/ServerApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServerResponse.md` & `fastly-3.0.1/docs/ServerResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServerResponseAllOf.md` & `fastly-3.0.1/docs/ServerResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Service.md` & `fastly-3.0.1/docs/Service.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceApi.md` & `fastly-3.0.1/docs/ServiceApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorization.md` & `fastly-3.0.1/docs/ServiceAuthorization.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationData.md` & `fastly-3.0.1/docs/ServiceAuthorizationData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationDataAttributes.md` & `fastly-3.0.1/docs/ServiceAuthorizationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationDataRelationships.md` & `fastly-3.0.1/docs/ServiceAuthorizationDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationDataRelationshipsUser.md` & `fastly-3.0.1/docs/ServiceAuthorizationDataRelationshipsUser.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationDataRelationshipsUserData.md` & `fastly-3.0.1/docs/ServiceAuthorizationDataRelationshipsUserData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationResponse.md` & `fastly-3.0.1/docs/ServiceAuthorizationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationResponseData.md` & `fastly-3.0.1/docs/ServiceAuthorizationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationResponseDataAllOf.md` & `fastly-3.0.1/docs/ServiceAuthorizationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationsApi.md` & `fastly-3.0.1/docs/ServiceAuthorizationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationsResponse.md` & `fastly-3.0.1/docs/TlsActivation.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# ServiceAuthorizationsResponse
+# TlsActivation
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**links** | [**PaginationLinks**](PaginationLinks.md) |  | [optional] 
-**meta** | [**PaginationMeta**](PaginationMeta.md) |  | [optional] 
-**data** | [**[ServiceAuthorizationResponseData]**](ServiceAuthorizationResponseData.md) |  | [optional] 
+**data** | [**TlsActivationData**](TlsActivationData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/ServiceAuthorizationsResponseAllOf.md` & `fastly-3.0.1/docs/ServiceAuthorizationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceCreate.md` & `fastly-3.0.1/docs/ServiceCreate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceCreateAllOf.md` & `fastly-3.0.1/docs/ServiceCreateAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceDetail.md` & `fastly-3.0.1/docs/ServiceDetail.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceDetailAllOf.md` & `fastly-3.0.1/docs/ServiceDetailAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceIdAndVersion.md` & `fastly-3.0.1/docs/ServiceIdAndVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceInvitation.md` & `fastly-3.0.1/docs/ServiceInvitation.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceInvitationData.md` & `fastly-3.0.1/docs/ServiceInvitationData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceInvitationDataAttributes.md` & `fastly-3.0.1/docs/ServiceInvitationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceInvitationDataRelationships.md` & `fastly-3.0.1/docs/ServiceInvitationDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceInvitationResponse.md` & `fastly-3.0.1/docs/ServiceInvitationResponseAllOf.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ServiceInvitationResponse
+# ServiceInvitationResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **data** | [**ServiceInvitationResponseAllOfData**](ServiceInvitationResponseAllOfData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
```

### Comparing `fastly-3.0.0/docs/ServiceInvitationResponseAllOf.md` & `fastly-3.0.1/docs/TlsActivationsResponseAllOf.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# ServiceInvitationResponseAllOf
+# TlsActivationsResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**ServiceInvitationResponseAllOfData**](ServiceInvitationResponseAllOfData.md) |  | [optional] 
+**data** | [**[TlsActivationResponseData]**](TlsActivationResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/ServiceInvitationResponseAllOfData.md` & `fastly-3.0.1/docs/ServiceInvitationResponseAllOfData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceListResponse.md` & `fastly-3.0.1/docs/ServiceListResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceListResponseAllOf.md` & `fastly-3.0.1/docs/ServiceListResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceResponse.md` & `fastly-3.0.1/docs/ServiceResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceResponseAllOf.md` & `fastly-3.0.1/docs/ServiceResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceVersionDetail.md` & `fastly-3.0.1/docs/ServiceVersionDetail.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ServiceVersionDetailOrNull.md` & `fastly-3.0.1/docs/ServiceVersionDetailOrNull.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Settings.md` & `fastly-3.0.1/docs/Settings.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SettingsApi.md` & `fastly-3.0.1/docs/SettingsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SettingsResponse.md` & `fastly-3.0.1/docs/SettingsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SigningKey.md` & `fastly-3.0.1/docs/SigningKey.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Snippet.md` & `fastly-3.0.1/docs/Snippet.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SnippetApi.md` & `fastly-3.0.1/docs/SnippetApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SnippetResponse.md` & `fastly-3.0.1/docs/SnippetResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SnippetResponseAllOf.md` & `fastly-3.0.1/docs/SnippetResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/StarApi.md` & `fastly-3.0.1/docs/StarApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/StarData.md` & `fastly-3.0.1/docs/StarData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/StarResponse.md` & `fastly-3.0.1/docs/StarResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/StarResponseAllOf.md` & `fastly-3.0.1/docs/StarResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Stats.md` & `fastly-3.0.1/docs/Stats.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/StatsApi.md` & `fastly-3.0.1/docs/StatsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Store.md` & `fastly-3.0.1/docs/Store.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/StoreResponse.md` & `fastly-3.0.1/docs/TlsActivationResponseDataAllOf.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# StoreResponse
+# TlsActivationResponseDataAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**id** | **str** | ID of the store. | [optional] 
-**name** | **str** | A human-readable name for the store. | [optional] 
+**id** | **str** |  | [optional] [readonly] 
+**attributes** | [**Timestamps**](Timestamps.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/SubsequentRequestTimestamp.md` & `fastly-3.0.1/docs/SubsequentRequestTimestamp.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SudoApi.md` & `fastly-3.0.1/docs/SudoApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SudoRequest.md` & `fastly-3.0.1/docs/SudoRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/SudoResponse.md` & `fastly-3.0.1/docs/SudoResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Timestamps.md` & `fastly-3.0.1/docs/Timestamps.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TimestampsNoDelete.md` & `fastly-3.0.1/docs/TimestampsNoDelete.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsActivation.md` & `fastly-3.0.1/docs/WafActiveRuleResponse.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TlsActivation
+# WafActiveRuleResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**TlsActivationData**](TlsActivationData.md) |  | [optional] 
+**data** | [**WafActiveRuleResponseData**](WafActiveRuleResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/TlsActivationData.md` & `fastly-3.0.1/docs/TlsActivationData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsActivationResponse.md` & `fastly-3.0.1/docs/TlsActivationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsActivationResponseData.md` & `fastly-3.0.1/docs/TlsActivationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsActivationResponseDataAllOf.md` & `fastly-3.0.1/docs/BillingResponseItemItemsData.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# TlsActivationResponseDataAllOf
+# BillingResponseItemItemsData
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**id** | **str** |  | [optional] [readonly] 
-**attributes** | [**Timestamps**](Timestamps.md) |  | [optional] 
+**line_items** | [**BillingResponseLineItems**](BillingResponseLineItems.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/TlsActivationsApi.md` & `fastly-3.0.1/docs/TlsActivationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsActivationsResponse.md` & `fastly-3.0.1/docs/TlsActivationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsActivationsResponseAllOf.md` & `fastly-3.0.1/docs/TlsCertificatesResponseAllOf.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TlsActivationsResponseAllOf
+# TlsCertificatesResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[TlsActivationResponseData]**](TlsActivationResponseData.md) |  | [optional] 
+**data** | [**[TlsCertificateResponseData]**](TlsCertificateResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/TlsBulkCertificate.md` & `fastly-3.0.1/docs/TlsBulkCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsBulkCertificateData.md` & `fastly-3.0.1/docs/TlsBulkCertificateData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsBulkCertificateDataAttributes.md` & `fastly-3.0.1/docs/TlsBulkCertificateDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsBulkCertificateResponse.md` & `fastly-3.0.1/docs/TlsBulkCertificateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsBulkCertificateResponseAttributes.md` & `fastly-3.0.1/docs/TlsBulkCertificateResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsBulkCertificateResponseAttributesAllOf.md` & `fastly-3.0.1/docs/TlsBulkCertificateResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsBulkCertificateResponseData.md` & `fastly-3.0.1/docs/TlsBulkCertificateResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsBulkCertificateResponseDataAllOf.md` & `fastly-3.0.1/docs/TlsBulkCertificateResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsBulkCertificatesApi.md` & `fastly-3.0.1/docs/TlsBulkCertificatesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsBulkCertificatesResponse.md` & `fastly-3.0.1/docs/TlsBulkCertificatesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsBulkCertificatesResponseAllOf.md` & `fastly-3.0.1/docs/TlsBulkCertificatesResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificate.md` & `fastly-3.0.1/docs/TlsCertificate.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificateData.md` & `fastly-3.0.1/docs/TlsCertificateData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificateDataAttributes.md` & `fastly-3.0.1/docs/TlsCertificateDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificateResponse.md` & `fastly-3.0.1/docs/TlsCertificateResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificateResponseAttributes.md` & `fastly-3.0.1/docs/TlsCertificateResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificateResponseAttributesAllOf.md` & `fastly-3.0.1/docs/TlsCertificateResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificateResponseData.md` & `fastly-3.0.1/docs/TlsCertificateResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificateResponseDataAllOf.md` & `fastly-3.0.1/docs/TlsCertificateResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificatesApi.md` & `fastly-3.0.1/docs/TlsCertificatesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificatesResponse.md` & `fastly-3.0.1/docs/TlsCertificatesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsCertificatesResponseAllOf.md` & `fastly-3.0.1/docs/TlsPrivateKeysResponseAllOf.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TlsCertificatesResponseAllOf
+# TlsPrivateKeysResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[TlsCertificateResponseData]**](TlsCertificateResponseData.md) |  | [optional] 
+**data** | [**[TlsPrivateKeyResponseData]**](TlsPrivateKeyResponseData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/TlsCommon.md` & `fastly-3.0.1/docs/TlsCommon.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfiguration.md` & `fastly-3.0.1/docs/TlsConfiguration.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfigurationData.md` & `fastly-3.0.1/docs/TlsConfigurationData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfigurationDataAttributes.md` & `fastly-3.0.1/docs/TlsConfigurationDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfigurationResponse.md` & `fastly-3.0.1/docs/TlsConfigurationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfigurationResponseAttributes.md` & `fastly-3.0.1/docs/TlsConfigurationResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfigurationResponseAttributesAllOf.md` & `fastly-3.0.1/docs/TlsConfigurationResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfigurationResponseData.md` & `fastly-3.0.1/docs/TlsConfigurationResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfigurationResponseDataAllOf.md` & `fastly-3.0.1/docs/TlsConfigurationResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfigurationsApi.md` & `fastly-3.0.1/docs/TlsConfigurationsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfigurationsResponse.md` & `fastly-3.0.1/docs/TlsConfigurationsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsConfigurationsResponseAllOf.md` & `fastly-3.0.1/docs/TlsConfigurationsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsDnsRecord.md` & `fastly-3.0.1/docs/TlsDnsRecord.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsDomainData.md` & `fastly-3.0.1/docs/TlsDomainData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsDomainsApi.md` & `fastly-3.0.1/docs/TlsDomainsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsDomainsResponse.md` & `fastly-3.0.1/docs/TlsDomainsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsDomainsResponseAllOf.md` & `fastly-3.0.1/docs/TlsDomainsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsPrivateKey.md` & `fastly-3.0.1/docs/TlsPrivateKey.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsPrivateKeyData.md` & `fastly-3.0.1/docs/TlsPrivateKeyData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsPrivateKeyDataAttributes.md` & `fastly-3.0.1/docs/TlsPrivateKeyDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsPrivateKeyResponse.md` & `fastly-3.0.1/docs/TlsPrivateKeyResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsPrivateKeyResponseAttributes.md` & `fastly-3.0.1/docs/TlsPrivateKeyResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsPrivateKeyResponseAttributesAllOf.md` & `fastly-3.0.1/docs/TlsPrivateKeyResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsPrivateKeyResponseData.md` & `fastly-3.0.1/docs/TlsPrivateKeyResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsPrivateKeysApi.md` & `fastly-3.0.1/docs/TlsPrivateKeysApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsPrivateKeysResponse.md` & `fastly-3.0.1/docs/TlsPrivateKeysResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsPrivateKeysResponseAllOf.md` & `fastly-3.0.1/docs/BillingEstimateLines.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TlsPrivateKeysResponseAllOf
+# BillingEstimateLines
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[TlsPrivateKeyResponseData]**](TlsPrivateKeyResponseData.md) |  | [optional] 
+**line_items** | [**[BillingEstimateLinesLineItems]**](BillingEstimateLinesLineItems.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/TlsSubscription.md` & `fastly-3.0.1/docs/TlsSubscription.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsSubscriptionData.md` & `fastly-3.0.1/docs/TlsSubscriptionData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsSubscriptionDataAttributes.md` & `fastly-3.0.1/docs/TlsSubscriptionDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsSubscriptionResponse.md` & `fastly-3.0.1/docs/TlsSubscriptionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsSubscriptionResponseAttributes.md` & `fastly-3.0.1/docs/TlsSubscriptionResponseAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsSubscriptionResponseAttributesAllOf.md` & `fastly-3.0.1/docs/TlsSubscriptionResponseAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsSubscriptionResponseData.md` & `fastly-3.0.1/docs/TlsSubscriptionResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsSubscriptionResponseDataAllOf.md` & `fastly-3.0.1/docs/TlsSubscriptionResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsSubscriptionsApi.md` & `fastly-3.0.1/docs/TlsSubscriptionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsSubscriptionsResponse.md` & `fastly-3.0.1/docs/TlsSubscriptionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TlsSubscriptionsResponseAllOf.md` & `fastly-3.0.1/docs/VersionCreateResponse.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# TlsSubscriptionsResponseAllOf
+# VersionCreateResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[TlsSubscriptionResponse]**](TlsSubscriptionResponse.md) |  | [optional] 
+**number** | **int** |  | [optional] [readonly] 
+**service_id** | **str** |  | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/Token.md` & `fastly-3.0.1/docs/Token.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TokenCreatedResponse.md` & `fastly-3.0.1/docs/TokenCreatedResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TokenCreatedResponseAllOf.md` & `fastly-3.0.1/docs/TokenCreatedResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TokenResponse.md` & `fastly-3.0.1/docs/TokenResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TokenResponseAllOf.md` & `fastly-3.0.1/docs/TokenResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/TokensApi.md` & `fastly-3.0.1/docs/TokensApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/UpdateBillingAddressRequest.md` & `fastly-3.0.1/docs/UpdateBillingAddressRequest.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/UpdateBillingAddressRequestData.md` & `fastly-3.0.1/docs/UpdateBillingAddressRequestData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/User.md` & `fastly-3.0.1/docs/User.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **login** | **str** |  | [optional] [readonly] 
 **name** | **str** | The real life name of the user. | [optional] 
 **limit_services** | **bool** | Indicates that the user has limited access to the customer&#39;s services. | [optional] 
-**locked** | **bool** | Indicates whether the is account is locked for editing or not. | [optional] 
-**require_new_password** | **bool** | Indicates if a new password is required at next login. | [optional] 
+**locked** | **bool, none_type** | Indicates whether the is account is locked for editing or not. | [optional] 
+**require_new_password** | **bool, none_type** | Indicates if a new password is required at next login. | [optional] 
 **role** | [**RoleUser**](RoleUser.md) |  | [optional] 
-**two_factor_auth_enabled** | **bool** | Indicates if 2FA is enabled on the user. | [optional] 
+**two_factor_auth_enabled** | **bool, none_type** | Indicates if 2FA is enabled on the user. | [optional] 
 **two_factor_setup_required** | **bool** | Indicates if 2FA is required by the user&#39;s customer account. | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/UserApi.md` & `fastly-3.0.1/docs/UserApi.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
 # Enter a context with an instance of the API client
 with fastly.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = user_api.UserApi(api_client)
     login = "login_example" # str |  (optional)
     name = "name_example" # str | The real life name of the user. (optional)
     limit_services = True # bool | Indicates that the user has limited access to the customer's services. (optional)
-    locked = True # bool | Indicates whether the is account is locked for editing or not. (optional)
-    require_new_password = True # bool | Indicates if a new password is required at next login. (optional)
+    locked = True # bool, none_type | Indicates whether the is account is locked for editing or not. (optional)
+    require_new_password = True # bool, none_type | Indicates if a new password is required at next login. (optional)
     role = RoleUser("user") # RoleUser |  (optional)
-    two_factor_auth_enabled = True # bool | Indicates if 2FA is enabled on the user. (optional)
+    two_factor_auth_enabled = True # bool, none_type | Indicates if 2FA is enabled on the user. (optional)
     two_factor_setup_required = True # bool | Indicates if 2FA is required by the user's customer account. (optional)
 
     # example passing only required values which don't have defaults set
     # and optional values
     try:
         # Create a user
         api_response = api_instance.create_user(login=login, name=name, limit_services=limit_services, locked=locked, require_new_password=require_new_password, role=role, two_factor_auth_enabled=two_factor_auth_enabled, two_factor_setup_required=two_factor_setup_required)
@@ -75,18 +75,18 @@
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **login** | **str**|  | [optional]
  **name** | **str**| The real life name of the user. | [optional]
  **limit_services** | **bool**| Indicates that the user has limited access to the customer&#39;s services. | [optional]
- **locked** | **bool**| Indicates whether the is account is locked for editing or not. | [optional]
- **require_new_password** | **bool**| Indicates if a new password is required at next login. | [optional]
+ **locked** | **bool, none_type**| Indicates whether the is account is locked for editing or not. | [optional]
+ **require_new_password** | **bool, none_type**| Indicates if a new password is required at next login. | [optional]
  **role** | [**RoleUser**](RoleUser.md)|  | [optional]
- **two_factor_auth_enabled** | **bool**| Indicates if 2FA is enabled on the user. | [optional]
+ **two_factor_auth_enabled** | **bool, none_type**| Indicates if 2FA is enabled on the user. | [optional]
  **two_factor_setup_required** | **bool**| Indicates if 2FA is required by the user&#39;s customer account. | [optional]
 
 ### Return type
 
 [**UserResponse**](UserResponse.md)
 
 ### Authorization
@@ -454,18 +454,18 @@
 with fastly.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = user_api.UserApi(api_client)
     user_id = "x9KzsrACXZv8tPwlEDsKb6" # str | Alphanumeric string identifying the user.
     login = "login_example" # str |  (optional)
     name = "name_example" # str | The real life name of the user. (optional)
     limit_services = True # bool | Indicates that the user has limited access to the customer's services. (optional)
-    locked = True # bool | Indicates whether the is account is locked for editing or not. (optional)
-    require_new_password = True # bool | Indicates if a new password is required at next login. (optional)
+    locked = True # bool, none_type | Indicates whether the is account is locked for editing or not. (optional)
+    require_new_password = True # bool, none_type | Indicates if a new password is required at next login. (optional)
     role = RoleUser("user") # RoleUser |  (optional)
-    two_factor_auth_enabled = True # bool | Indicates if 2FA is enabled on the user. (optional)
+    two_factor_auth_enabled = True # bool, none_type | Indicates if 2FA is enabled on the user. (optional)
     two_factor_setup_required = True # bool | Indicates if 2FA is required by the user's customer account. (optional)
 
     # example passing only required values which don't have defaults set
     try:
         # Update a user
         api_response = api_instance.update_user(user_id)
         pprint(api_response)
@@ -487,18 +487,18 @@
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **user_id** | **str**| Alphanumeric string identifying the user. |
  **login** | **str**|  | [optional]
  **name** | **str**| The real life name of the user. | [optional]
  **limit_services** | **bool**| Indicates that the user has limited access to the customer&#39;s services. | [optional]
- **locked** | **bool**| Indicates whether the is account is locked for editing or not. | [optional]
- **require_new_password** | **bool**| Indicates if a new password is required at next login. | [optional]
+ **locked** | **bool, none_type**| Indicates whether the is account is locked for editing or not. | [optional]
+ **require_new_password** | **bool, none_type**| Indicates if a new password is required at next login. | [optional]
  **role** | [**RoleUser**](RoleUser.md)|  | [optional]
- **two_factor_auth_enabled** | **bool**| Indicates if 2FA is enabled on the user. | [optional]
+ **two_factor_auth_enabled** | **bool, none_type**| Indicates if 2FA is enabled on the user. | [optional]
  **two_factor_setup_required** | **bool**| Indicates if 2FA is required by the user&#39;s customer account. | [optional]
 
 ### Return type
 
 [**UserResponse**](UserResponse.md)
 
 ### Authorization
```

### Comparing `fastly-3.0.0/docs/UserResponse.md` & `fastly-3.0.1/docs/UserResponse.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **login** | **str** |  | [optional] [readonly] 
 **name** | **str** | The real life name of the user. | [optional] 
 **limit_services** | **bool** | Indicates that the user has limited access to the customer&#39;s services. | [optional] 
-**locked** | **bool** | Indicates whether the is account is locked for editing or not. | [optional] 
-**require_new_password** | **bool** | Indicates if a new password is required at next login. | [optional] 
+**locked** | **bool, none_type** | Indicates whether the is account is locked for editing or not. | [optional] 
+**require_new_password** | **bool, none_type** | Indicates if a new password is required at next login. | [optional] 
 **role** | [**RoleUser**](RoleUser.md) |  | [optional] 
-**two_factor_auth_enabled** | **bool** | Indicates if 2FA is enabled on the user. | [optional] 
+**two_factor_auth_enabled** | **bool, none_type** | Indicates if 2FA is enabled on the user. | [optional] 
 **two_factor_setup_required** | **bool** | Indicates if 2FA is required by the user&#39;s customer account. | [optional] 
 **created_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **deleted_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **updated_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **id** | **str** |  | [optional] [readonly] 
 **email_hash** | **str** | The alphanumeric string identifying a email login. | [optional] [readonly] 
 **customer_id** | **str** |  | [optional] [readonly]
```

### Comparing `fastly-3.0.0/docs/UserResponseAllOf.md` & `fastly-3.0.1/docs/WafRuleAttributes.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# UserResponseAllOf
+# WafRuleAttributes
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**id** | **str** |  | [optional] [readonly] 
-**email_hash** | **str** | The alphanumeric string identifying a email login. | [optional] [readonly] 
-**customer_id** | **str** |  | [optional] [readonly] 
+**modsec_rule_id** | **int** | Corresponding ModSecurity rule ID. | [optional] [readonly] 
+**publisher** | **str** | Rule publisher. | [optional] [readonly] 
+**type** | **str** | The rule&#39;s [type](https://docs.fastly.com/en/guides/managing-rules-on-the-fastly-waf#understanding-the-types-of-rules). | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/ValidatorResult.md` & `fastly-3.0.1/docs/ValidatorResult.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ValidatorResultData.md` & `fastly-3.0.1/docs/ValidatorResultData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ValidatorResultDataAttributes.md` & `fastly-3.0.1/docs/ValidatorResultDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/ValidatorResultDataAttributesMessages.md` & `fastly-3.0.1/docs/ValidatorResultDataAttributesMessages.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Values.md` & `fastly-3.0.1/docs/Values.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Vcl.md` & `fastly-3.0.1/docs/Vcl.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/VclApi.md` & `fastly-3.0.1/docs/VclApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/VclDiff.md` & `fastly-3.0.1/docs/VclDiff.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/VclDiffApi.md` & `fastly-3.0.1/docs/VclDiffApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/VclResponse.md` & `fastly-3.0.1/docs/VclResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/VclSyntaxHighlightingResponse.md` & `fastly-3.0.1/docs/VclSyntaxHighlightingResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/Version.md` & `fastly-3.0.1/docs/Version.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/VersionApi.md` & `fastly-3.0.1/docs/VersionApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/VersionCreateResponse.md` & `fastly-3.0.1/docs/VersionResponseAllOf.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# VersionCreateResponse
+# VersionResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**number** | **int** |  | [optional] [readonly] 
 **service_id** | **str** |  | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/VersionDetail.md` & `fastly-3.0.1/docs/VersionDetail.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/VersionDetailSettings.md` & `fastly-3.0.1/docs/VersionDetailSettings.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/VersionResponse.md` & `fastly-3.0.1/docs/VersionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/VersionResponseAllOf.md` & `fastly-3.0.1/docs/WafFirewall.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# VersionResponseAllOf
+# WafFirewall
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**service_id** | **str** |  | [optional] [readonly] 
+**data** | [**WafFirewallData**](WafFirewallData.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/WafActiveRule.md` & `fastly-3.0.1/docs/WafActiveRule.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRuleCreationResponse.md` & `fastly-3.0.1/docs/WafActiveRuleCreationResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRuleData.md` & `fastly-3.0.1/docs/WafActiveRuleData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRuleDataAttributes.md` & `fastly-3.0.1/docs/WafActiveRuleDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRuleResponse.md` & `fastly-3.0.1/docs/WafRuleRevisionResponse.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# WafActiveRuleResponse
+# WafRuleRevisionResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**WafActiveRuleResponseData**](WafActiveRuleResponseData.md) |  | [optional] 
+**data** | [**WafRuleRevisionResponseData**](WafRuleRevisionResponseData.md) |  | [optional] 
+**included** | [**IncludedWithWafRuleRevision**](IncludedWithWafRuleRevision.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/WafActiveRuleResponseData.md` & `fastly-3.0.1/docs/WafActiveRuleResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRuleResponseDataAllOf.md` & `fastly-3.0.1/docs/WafActiveRuleResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRuleResponseDataAttributes.md` & `fastly-3.0.1/docs/WafActiveRuleResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRuleResponseDataAttributesAllOf.md` & `fastly-3.0.1/docs/WafActiveRuleResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRuleResponseDataRelationships.md` & `fastly-3.0.1/docs/WafActiveRuleResponseDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRulesApi.md` & `fastly-3.0.1/docs/WafActiveRulesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRulesResponse.md` & `fastly-3.0.1/docs/WafActiveRulesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafActiveRulesResponseAllOf.md` & `fastly-3.0.1/docs/WafActiveRulesResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusion.md` & `fastly-3.0.1/docs/WafExclusion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionData.md` & `fastly-3.0.1/docs/WafExclusionData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionDataAttributes.md` & `fastly-3.0.1/docs/WafExclusionDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionResponse.md` & `fastly-3.0.1/docs/WafExclusionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionResponseData.md` & `fastly-3.0.1/docs/WafExclusionResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionResponseDataAllOf.md` & `fastly-3.0.1/docs/WafExclusionResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionResponseDataAttributes.md` & `fastly-3.0.1/docs/WafExclusionResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionResponseDataAttributesAllOf.md` & `fastly-3.0.1/docs/WafExclusionResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionResponseDataRelationships.md` & `fastly-3.0.1/docs/WafExclusionResponseDataRelationships.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionsApi.md` & `fastly-3.0.1/docs/WafExclusionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionsResponse.md` & `fastly-3.0.1/docs/WafExclusionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafExclusionsResponseAllOf.md` & `fastly-3.0.1/docs/WafExclusionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewall.md` & `fastly-3.0.1/docs/WafFirewallData.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# WafFirewall
+# WafFirewallData
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**WafFirewallData**](WafFirewallData.md) |  | [optional] 
+**type** | [**TypeWafFirewall**](TypeWafFirewall.md) |  | [optional] 
+**attributes** | [**WafFirewallDataAttributes**](WafFirewallDataAttributes.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/WafFirewallData.md` & `fastly-3.0.1/docs/WafTagsResponseAllOf.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# WafFirewallData
+# WafTagsResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | [**TypeWafFirewall**](TypeWafFirewall.md) |  | [optional] 
-**attributes** | [**WafFirewallDataAttributes**](WafFirewallDataAttributes.md) |  | [optional] 
+**data** | [**[WafTagsResponseDataItem]**](WafTagsResponseDataItem.md) |  | [optional] 
+**included** | [**[WafRule]**](WafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/WafFirewallDataAttributes.md` & `fastly-3.0.1/docs/WafFirewallDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallResponse.md` & `fastly-3.0.1/docs/WafFirewallResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallResponseData.md` & `fastly-3.0.1/docs/WafFirewallResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallResponseDataAllOf.md` & `fastly-3.0.1/docs/WafFirewallResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallResponseDataAttributes.md` & `fastly-3.0.1/docs/WafFirewallResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallResponseDataAttributesAllOf.md` & `fastly-3.0.1/docs/WafFirewallResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersion.md` & `fastly-3.0.1/docs/WafFirewallVersion.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersionData.md` & `fastly-3.0.1/docs/WafFirewallVersionData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersionDataAttributes.md` & `fastly-3.0.1/docs/WafFirewallVersionDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersionResponse.md` & `fastly-3.0.1/docs/WafFirewallVersionResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersionResponseData.md` & `fastly-3.0.1/docs/WafFirewallVersionResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersionResponseDataAllOf.md` & `fastly-3.0.1/docs/WafFirewallVersionResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersionResponseDataAttributes.md` & `fastly-3.0.1/docs/WafFirewallVersionResponseDataAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersionResponseDataAttributesAllOf.md` & `fastly-3.0.1/docs/WafFirewallVersionResponseDataAttributesAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersionsApi.md` & `fastly-3.0.1/docs/WafFirewallVersionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersionsResponse.md` & `fastly-3.0.1/docs/WafFirewallVersionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallVersionsResponseAllOf.md` & `fastly-3.0.1/docs/WafFirewallVersionsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallsApi.md` & `fastly-3.0.1/docs/WafFirewallsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallsResponse.md` & `fastly-3.0.1/docs/WafFirewallsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafFirewallsResponseAllOf.md` & `fastly-3.0.1/docs/WafFirewallsResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRule.md` & `fastly-3.0.1/docs/WafRule.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRuleAttributes.md` & `fastly-3.0.1/docs/WafTagsResponse.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# WafRuleAttributes
+# WafTagsResponse
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**modsec_rule_id** | **int** | Corresponding ModSecurity rule ID. | [optional] [readonly] 
-**publisher** | **str** | Rule publisher. | [optional] [readonly] 
-**type** | **str** | The rule&#39;s [type](https://docs.fastly.com/en/guides/managing-rules-on-the-fastly-waf#understanding-the-types-of-rules). | [optional] [readonly] 
+**links** | [**PaginationLinks**](PaginationLinks.md) |  | [optional] 
+**meta** | [**PaginationMeta**](PaginationMeta.md) |  | [optional] 
+**data** | [**[WafTagsResponseDataItem]**](WafTagsResponseDataItem.md) |  | [optional] 
+**included** | [**[WafRule]**](WafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/WafRuleResponse.md` & `fastly-3.0.1/docs/WafRuleResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRuleResponseData.md` & `fastly-3.0.1/docs/WafRuleResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRuleResponseDataAllOf.md` & `fastly-3.0.1/docs/WafRuleResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRuleRevision.md` & `fastly-3.0.1/docs/WafRuleRevision.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRuleRevisionAttributes.md` & `fastly-3.0.1/docs/WafRuleRevisionAttributes.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRuleRevisionResponse.md` & `fastly-3.0.1/docs/WafRuleRevisionsResponseAllOf.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# WafRuleRevisionResponse
+# WafRuleRevisionsResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**WafRuleRevisionResponseData**](WafRuleRevisionResponseData.md) |  | [optional] 
+**data** | [**[WafRuleRevisionResponseData]**](WafRuleRevisionResponseData.md) |  | [optional] 
 **included** | [**IncludedWithWafRuleRevision**](IncludedWithWafRuleRevision.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/WafRuleRevisionResponseData.md` & `fastly-3.0.1/docs/WafRuleRevisionResponseData.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRuleRevisionResponseDataAllOf.md` & `fastly-3.0.1/docs/WafRuleRevisionResponseDataAllOf.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRuleRevisionsApi.md` & `fastly-3.0.1/docs/WafRuleRevisionsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRuleRevisionsResponse.md` & `fastly-3.0.1/docs/WafRuleRevisionsResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRuleRevisionsResponseAllOf.md` & `fastly-3.0.1/docs/WafRulesResponseAllOf.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# WafRuleRevisionsResponseAllOf
+# WafRulesResponseAllOf
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**data** | [**[WafRuleRevisionResponseData]**](WafRuleRevisionResponseData.md) |  | [optional] 
-**included** | [**IncludedWithWafRuleRevision**](IncludedWithWafRuleRevision.md) |  | [optional] 
+**data** | [**[WafRuleResponseData]**](WafRuleResponseData.md) |  | [optional] 
+**included** | [**IncludedWithWafRule**](IncludedWithWafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/WafRulesApi.md` & `fastly-3.0.1/docs/WafRulesApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafRulesResponse.md` & `fastly-3.0.1/docs/WafRulesResponse.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafTag.md` & `fastly-3.0.1/docs/WafTag.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafTagsApi.md` & `fastly-3.0.1/docs/WafTagsApi.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/docs/WafTagsResponse.md` & `fastly-3.0.1/docs/WafTagsResponseDataItem.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# WafTagsResponse
+# WafTagsResponseDataItem
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**links** | [**PaginationLinks**](PaginationLinks.md) |  | [optional] 
-**meta** | [**PaginationMeta**](PaginationMeta.md) |  | [optional] 
-**data** | [**[WafTagsResponseDataItem]**](WafTagsResponseDataItem.md) |  | [optional] 
-**included** | [**[WafRule]**](WafRule.md) |  | [optional] 
+**type** | [**TypeWafTag**](TypeWafTag.md) |  | [optional] 
+**id** | **str** | Alphanumeric string identifying a WAF tag. | [optional] [readonly] 
+**attributes** | [**WafTagAttributes**](WafTagAttributes.md) |  | [optional] 
+**relationships** | [**RelationshipWafRule**](RelationshipWafRule.md) |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/WafTagsResponseDataItem.md` & `fastly-3.0.1/docs/BillingStatus.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# WafTagsResponseDataItem
+# BillingStatus
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**type** | [**TypeWafTag**](TypeWafTag.md) |  | [optional] 
-**id** | **str** | Alphanumeric string identifying a WAF tag. | [optional] [readonly] 
-**attributes** | [**WafTagAttributes**](WafTagAttributes.md) |  | [optional] 
-**relationships** | [**RelationshipWafRule**](RelationshipWafRule.md) |  | [optional] 
+**status** | **str** | What the current status of this invoice can be. | [optional] 
+**sent_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `fastly-3.0.0/docs/WsMessageFormat.md` & `fastly-3.0.1/docs/WsMessageFormat.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/__init__.py` & `fastly-3.0.1/fastly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Via the Fastly API you can perform any of the operations that are possible within the management console,  including creating services, domains, and backends, configuring rules or uploading your own application code, as well as account operations such as user administration and billing reports. The API is organized into collections of endpoints that allow manipulation of objects related to Fastly services and accounts. For the most accurate and up-to-date API reference content, visit our [Developer Hub](https://developer.fastly.com/reference/api/)   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: oss@fastly.com
 """
 
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 
 # import ApiClient
 from fastly.api_client import ApiClient
 
 # import Configuration
 from fastly.configuration import Configuration
```

### Comparing `fastly-3.0.0/fastly/api_client.py` & `fastly-3.0.1/fastly/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'fastly-py/3.0.0'
+        self.user_agent = 'fastly-py/3.0.1'
 
         # The last observed value of http header Fastly-RateLimit-Remaining
         self.rate_limit_remaining = DEFAULT_RATELIMIT
 
         # The last observed value of http header Fastly-RateLimit-Reset
         self.rate_limit_reset = 0
```

### Comparing `fastly-3.0.0/fastly/configuration.py` & `fastly-3.0.1/fastly/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 3.0.0".\
+               "SDK Package Version: 3.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `fastly-3.0.0/fastly/exceptions.py` & `fastly-3.0.1/fastly/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model_utils.py` & `fastly-3.0.1/fastly/model_utils.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/rest.py` & `fastly-3.0.1/fastly/rest.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/acl_api.py` & `fastly-3.0.1/fastly/api/acl_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/acl_entry_api.py` & `fastly-3.0.1/fastly/api/acl_entry_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/apex_redirect_api.py` & `fastly-3.0.1/fastly/api/apex_redirect_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/automation_tokens_api.py` & `fastly-3.0.1/fastly/api/automation_tokens_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/backend_api.py` & `fastly-3.0.1/fastly/api/backend_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/billing_address_api.py` & `fastly-3.0.1/fastly/api/billing_address_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/billing_api.py` & `fastly-3.0.1/fastly/api/billing_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/cache_settings_api.py` & `fastly-3.0.1/fastly/api/cache_settings_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/condition_api.py` & `fastly-3.0.1/fastly/api/condition_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/config_store_api.py` & `fastly-3.0.1/fastly/api/config_store_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/config_store_item_api.py` & `fastly-3.0.1/fastly/api/config_store_item_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/contact_api.py` & `fastly-3.0.1/fastly/api/contact_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/content_api.py` & `fastly-3.0.1/fastly/api/content_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/customer_api.py` & `fastly-3.0.1/fastly/api/customer_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/dictionary_api.py` & `fastly-3.0.1/fastly/api/dictionary_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/dictionary_info_api.py` & `fastly-3.0.1/fastly/api/dictionary_info_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/dictionary_item_api.py` & `fastly-3.0.1/fastly/api/dictionary_item_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/diff_api.py` & `fastly-3.0.1/fastly/api/diff_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/director_api.py` & `fastly-3.0.1/fastly/api/director_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/director_backend_api.py` & `fastly-3.0.1/fastly/api/director_backend_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/domain_api.py` & `fastly-3.0.1/fastly/api/domain_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/domain_inspector_historical_api.py` & `fastly-3.0.1/fastly/api/domain_inspector_historical_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/domain_inspector_realtime_api.py` & `fastly-3.0.1/fastly/api/domain_inspector_realtime_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/domain_ownerships_api.py` & `fastly-3.0.1/fastly/api/domain_ownerships_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/enabled_products_api.py` & `fastly-3.0.1/fastly/api/enabled_products_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/events_api.py` & `fastly-3.0.1/fastly/api/events_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/gzip_api.py` & `fastly-3.0.1/fastly/api/gzip_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/header_api.py` & `fastly-3.0.1/fastly/api/header_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/healthcheck_api.py` & `fastly-3.0.1/fastly/api/healthcheck_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/historical_api.py` & `fastly-3.0.1/fastly/api/historical_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/http3_api.py` & `fastly-3.0.1/fastly/api/http3_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/iam_permissions_api.py` & `fastly-3.0.1/fastly/api/iam_permissions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/iam_roles_api.py` & `fastly-3.0.1/fastly/api/iam_roles_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/iam_service_groups_api.py` & `fastly-3.0.1/fastly/api/iam_service_groups_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/iam_user_groups_api.py` & `fastly-3.0.1/fastly/api/iam_user_groups_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/invitations_api.py` & `fastly-3.0.1/fastly/api/invitations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/kv_store_api.py` & `fastly-3.0.1/fastly/api/kv_store_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/kv_store_item_api.py` & `fastly-3.0.1/fastly/api/kv_store_item_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/legacy_waf_configuration_sets_api.py` & `fastly-3.0.1/fastly/api/legacy_waf_configuration_sets_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/legacy_waf_firewall_api.py` & `fastly-3.0.1/fastly/api/legacy_waf_firewall_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/legacy_waf_owasp_api.py` & `fastly-3.0.1/fastly/api/legacy_waf_owasp_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/legacy_waf_rule_api.py` & `fastly-3.0.1/fastly/api/legacy_waf_rule_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/legacy_waf_rule_status_api.py` & `fastly-3.0.1/fastly/api/legacy_waf_rule_status_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/legacy_waf_ruleset_api.py` & `fastly-3.0.1/fastly/api/legacy_waf_ruleset_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/legacy_waf_tag_api.py` & `fastly-3.0.1/fastly/api/legacy_waf_tag_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/legacy_waf_update_status_api.py` & `fastly-3.0.1/fastly/api/legacy_waf_update_status_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_azureblob_api.py` & `fastly-3.0.1/fastly/api/logging_azureblob_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_bigquery_api.py` & `fastly-3.0.1/fastly/api/logging_bigquery_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_cloudfiles_api.py` & `fastly-3.0.1/fastly/api/logging_cloudfiles_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_datadog_api.py` & `fastly-3.0.1/fastly/api/logging_datadog_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_digitalocean_api.py` & `fastly-3.0.1/fastly/api/logging_digitalocean_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_elasticsearch_api.py` & `fastly-3.0.1/fastly/api/logging_elasticsearch_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_ftp_api.py` & `fastly-3.0.1/fastly/api/logging_ftp_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_gcs_api.py` & `fastly-3.0.1/fastly/api/logging_gcs_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_heroku_api.py` & `fastly-3.0.1/fastly/api/logging_heroku_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_honeycomb_api.py` & `fastly-3.0.1/fastly/api/logging_honeycomb_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_https_api.py` & `fastly-3.0.1/fastly/api/logging_https_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_kafka_api.py` & `fastly-3.0.1/fastly/api/logging_kafka_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_kinesis_api.py` & `fastly-3.0.1/fastly/api/logging_kinesis_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_logentries_api.py` & `fastly-3.0.1/fastly/api/logging_logentries_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_loggly_api.py` & `fastly-3.0.1/fastly/api/logging_loggly_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_logshuttle_api.py` & `fastly-3.0.1/fastly/api/logging_logshuttle_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_newrelic_api.py` & `fastly-3.0.1/fastly/api/logging_newrelic_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_openstack_api.py` & `fastly-3.0.1/fastly/api/logging_openstack_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_papertrail_api.py` & `fastly-3.0.1/fastly/api/logging_papertrail_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_pubsub_api.py` & `fastly-3.0.1/fastly/api/logging_pubsub_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_s3_api.py` & `fastly-3.0.1/fastly/api/logging_s3_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_scalyr_api.py` & `fastly-3.0.1/fastly/api/logging_scalyr_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_sftp_api.py` & `fastly-3.0.1/fastly/api/logging_sftp_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_splunk_api.py` & `fastly-3.0.1/fastly/api/logging_splunk_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_sumologic_api.py` & `fastly-3.0.1/fastly/api/logging_sumologic_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/logging_syslog_api.py` & `fastly-3.0.1/fastly/api/logging_syslog_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/mutual_authentication_api.py` & `fastly-3.0.1/fastly/api/mutual_authentication_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/origin_inspector_historical_api.py` & `fastly-3.0.1/fastly/api/origin_inspector_historical_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/origin_inspector_realtime_api.py` & `fastly-3.0.1/fastly/api/origin_inspector_realtime_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/package_api.py` & `fastly-3.0.1/fastly/api/package_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/pool_api.py` & `fastly-3.0.1/fastly/api/pool_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/pop_api.py` & `fastly-3.0.1/fastly/api/pop_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/public_ip_list_api.py` & `fastly-3.0.1/fastly/api/public_ip_list_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/publish_api.py` & `fastly-3.0.1/fastly/api/publish_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/purge_api.py` & `fastly-3.0.1/fastly/api/purge_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/rate_limiter_api.py` & `fastly-3.0.1/fastly/api/rate_limiter_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/realtime_api.py` & `fastly-3.0.1/fastly/api/realtime_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/request_settings_api.py` & `fastly-3.0.1/fastly/api/request_settings_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/resource_api.py` & `fastly-3.0.1/fastly/api/resource_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/response_object_api.py` & `fastly-3.0.1/fastly/api/response_object_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/secret_store_api.py` & `fastly-3.0.1/fastly/api/secret_store_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/secret_store_item_api.py` & `fastly-3.0.1/fastly/api/secret_store_item_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/server_api.py` & `fastly-3.0.1/fastly/api/server_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/service_api.py` & `fastly-3.0.1/fastly/api/service_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/service_authorizations_api.py` & `fastly-3.0.1/fastly/api/service_authorizations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/settings_api.py` & `fastly-3.0.1/fastly/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/snippet_api.py` & `fastly-3.0.1/fastly/api/snippet_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/star_api.py` & `fastly-3.0.1/fastly/api/star_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/stats_api.py` & `fastly-3.0.1/fastly/api/stats_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/sudo_api.py` & `fastly-3.0.1/fastly/api/sudo_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/tls_activations_api.py` & `fastly-3.0.1/fastly/api/tls_activations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/tls_bulk_certificates_api.py` & `fastly-3.0.1/fastly/api/tls_bulk_certificates_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/tls_certificates_api.py` & `fastly-3.0.1/fastly/api/tls_certificates_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/tls_configurations_api.py` & `fastly-3.0.1/fastly/api/tls_configurations_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/tls_domains_api.py` & `fastly-3.0.1/fastly/api/tls_domains_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/tls_private_keys_api.py` & `fastly-3.0.1/fastly/api/tls_private_keys_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/tls_subscriptions_api.py` & `fastly-3.0.1/fastly/api/tls_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/tokens_api.py` & `fastly-3.0.1/fastly/api/tokens_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/user_api.py` & `fastly-3.0.1/fastly/api/user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,17 @@
                     'require_new_password',
                     'role',
                     'two_factor_auth_enabled',
                     'two_factor_setup_required',
                 ],
                 'required': [],
                 'nullable': [
+                    'locked',
+                    'require_new_password',
+                    'two_factor_auth_enabled',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -79,21 +82,21 @@
                     'login':
                         (str,),
                     'name':
                         (str,),
                     'limit_services':
                         (bool,),
                     'locked':
-                        (bool,),
+                        (bool, none_type,),
                     'require_new_password':
-                        (bool,),
+                        (bool, none_type,),
                     'role':
                         (RoleUser,),
                     'two_factor_auth_enabled':
-                        (bool,),
+                        (bool, none_type,),
                     'two_factor_setup_required':
                         (bool,),
                 },
                 'attribute_map': {
                     'login': 'login',
                     'name': 'name',
                     'limit_services': 'limit_services',
@@ -381,14 +384,17 @@
                     'two_factor_auth_enabled',
                     'two_factor_setup_required',
                 ],
                 'required': [
                     'user_id',
                 ],
                 'nullable': [
+                    'locked',
+                    'require_new_password',
+                    'two_factor_auth_enabled',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -402,21 +408,21 @@
                     'login':
                         (str,),
                     'name':
                         (str,),
                     'limit_services':
                         (bool,),
                     'locked':
-                        (bool,),
+                        (bool, none_type,),
                     'require_new_password':
-                        (bool,),
+                        (bool, none_type,),
                     'role':
                         (RoleUser,),
                     'two_factor_auth_enabled':
-                        (bool,),
+                        (bool, none_type,),
                     'two_factor_setup_required':
                         (bool,),
                 },
                 'attribute_map': {
                     'user_id': 'user_id',
                     'login': 'login',
                     'name': 'name',
@@ -531,18 +537,18 @@
         >>> result = thread.get()
 
 
         Keyword Args:
             login (str): [optional]
             name (str): The real life name of the user.. [optional]
             limit_services (bool): Indicates that the user has limited access to the customer's services.. [optional]
-            locked (bool): Indicates whether the is account is locked for editing or not.. [optional]
-            require_new_password (bool): Indicates if a new password is required at next login.. [optional]
+            locked (bool, none_type): Indicates whether the is account is locked for editing or not.. [optional]
+            require_new_password (bool, none_type): Indicates if a new password is required at next login.. [optional]
             role (RoleUser): [optional]
-            two_factor_auth_enabled (bool): Indicates if 2FA is enabled on the user.. [optional]
+            two_factor_auth_enabled (bool, none_type): Indicates if 2FA is enabled on the user.. [optional]
             two_factor_setup_required (bool): Indicates if 2FA is required by the user's customer account.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -922,18 +928,18 @@
         Args:
             user_id (str): Alphanumeric string identifying the user.
 
         Keyword Args:
             login (str): [optional]
             name (str): The real life name of the user.. [optional]
             limit_services (bool): Indicates that the user has limited access to the customer's services.. [optional]
-            locked (bool): Indicates whether the is account is locked for editing or not.. [optional]
-            require_new_password (bool): Indicates if a new password is required at next login.. [optional]
+            locked (bool, none_type): Indicates whether the is account is locked for editing or not.. [optional]
+            require_new_password (bool, none_type): Indicates if a new password is required at next login.. [optional]
             role (RoleUser): [optional]
-            two_factor_auth_enabled (bool): Indicates if 2FA is enabled on the user.. [optional]
+            two_factor_auth_enabled (bool, none_type): Indicates if 2FA is enabled on the user.. [optional]
             two_factor_setup_required (bool): Indicates if 2FA is required by the user's customer account.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
```

### Comparing `fastly-3.0.0/fastly/api/vcl_api.py` & `fastly-3.0.1/fastly/api/vcl_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/vcl_diff_api.py` & `fastly-3.0.1/fastly/api/vcl_diff_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/version_api.py` & `fastly-3.0.1/fastly/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/waf_active_rules_api.py` & `fastly-3.0.1/fastly/api/waf_active_rules_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/waf_exclusions_api.py` & `fastly-3.0.1/fastly/api/waf_exclusions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/waf_firewall_versions_api.py` & `fastly-3.0.1/fastly/api/waf_firewall_versions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/waf_firewalls_api.py` & `fastly-3.0.1/fastly/api/waf_firewalls_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/waf_rule_revisions_api.py` & `fastly-3.0.1/fastly/api/waf_rule_revisions_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/waf_rules_api.py` & `fastly-3.0.1/fastly/api/waf_rules_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/api/waf_tags_api.py` & `fastly-3.0.1/fastly/api/waf_tags_api.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/apis/__init__.py` & `fastly-3.0.1/fastly/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/acl.py` & `fastly-3.0.1/fastly/model/acl.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/acl_entry.py` & `fastly-3.0.1/fastly/model/acl_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/acl_entry_response.py` & `fastly-3.0.1/fastly/model/acl_entry_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/acl_entry_response_all_of.py` & `fastly-3.0.1/fastly/model/acl_entry_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/acl_response.py` & `fastly-3.0.1/fastly/model/acl_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/acl_response_all_of.py` & `fastly-3.0.1/fastly/model/acl_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/apex_redirect.py` & `fastly-3.0.1/fastly/model/apex_redirect.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/apex_redirect_all_of.py` & `fastly-3.0.1/fastly/model/apex_redirect_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/automation_token.py` & `fastly-3.0.1/fastly/model/automation_token.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/automation_token_create_request.py` & `fastly-3.0.1/fastly/model/automation_token_create_request.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/automation_token_create_request_attributes.py` & `fastly-3.0.1/fastly/model/automation_token_create_request_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/automation_token_create_response.py` & `fastly-3.0.1/fastly/model/automation_token_create_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/automation_token_create_response_all_of.py` & `fastly-3.0.1/fastly/model/automation_token_create_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/automation_token_response.py` & `fastly-3.0.1/fastly/model/automation_token_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/automation_token_response_all_of.py` & `fastly-3.0.1/fastly/model/automation_token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/aws_region.py` & `fastly-3.0.1/fastly/model/aws_region.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/backend.py` & `fastly-3.0.1/fastly/model/backend.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/backend_response.py` & `fastly-3.0.1/fastly/model/backend_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/backend_response_all_of.py` & `fastly-3.0.1/fastly/model/backend_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/batch.py` & `fastly-3.0.1/fastly/model/batch.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/batch_errors.py` & `fastly-3.0.1/fastly/model/batch_errors.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/billing.py` & `fastly-3.0.1/fastly/model/billing.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/billing_address_attributes.py` & `fastly-3.0.1/fastly/model/billing_address_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/billing_address_request.py` & `fastly-3.0.1/fastly/model/billing_address_request.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/billing_address_request_data.py` & `fastly-3.0.1/fastly/model/billing_address_request_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/billing_address_response.py` & `fastly-3.0.1/fastly/model/billing_address_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/billing_address_response_data.py` & `fastly-3.0.1/fastly/model/billing_address_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/billing_address_verification_error_response.py` & `fastly-3.0.1/fastly/model/billing_address_verification_error_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/billing_address_verification_error_response_errors.py` & `fastly-3.0.1/fastly/model/billing_address_verification_error_response_errors.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/billing_estimate_response.py` & `fastly-3.0.1/fastly/model/billing_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,26 +27,26 @@
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from fastly.model.billing import Billing
-    from fastly.model.billing_estimate_response_all_of import BillingEstimateResponseAllOf
-    from fastly.model.billing_estimate_response_all_of_lines import BillingEstimateResponseAllOfLines
+    from fastly.model.billing_response_item_items_data import BillingResponseItemItemsData
+    from fastly.model.billing_response_line_items import BillingResponseLineItems
     from fastly.model.billing_status import BillingStatus
     from fastly.model.billing_total import BillingTotal
     globals()['Billing'] = Billing
-    globals()['BillingEstimateResponseAllOf'] = BillingEstimateResponseAllOf
-    globals()['BillingEstimateResponseAllOfLines'] = BillingEstimateResponseAllOfLines
+    globals()['BillingResponseItemItemsData'] = BillingResponseItemItemsData
+    globals()['BillingResponseLineItems'] = BillingResponseLineItems
     globals()['BillingStatus'] = BillingStatus
     globals()['BillingTotal'] = BillingTotal
 
 
-class BillingEstimateResponse(ModelComposed):
+class BillingResponse(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -97,15 +97,15 @@
             'start_time': (datetime, none_type,),  # noqa: E501
             'invoice_id': (str,),  # noqa: E501
             'customer_id': (str,),  # noqa: E501
             'vendor_state': (str,),  # noqa: E501
             'status': (BillingStatus,),  # noqa: E501
             'total': (BillingTotal,),  # noqa: E501
             'regions': ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)},),  # noqa: E501
-            'lines': ([BillingEstimateResponseAllOfLines],),  # noqa: E501
+            'line_items': (BillingResponseLineItems,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -114,29 +114,29 @@
         'start_time': 'start_time',  # noqa: E501
         'invoice_id': 'invoice_id',  # noqa: E501
         'customer_id': 'customer_id',  # noqa: E501
         'vendor_state': 'vendor_state',  # noqa: E501
         'status': 'status',  # noqa: E501
         'total': 'total',  # noqa: E501
         'regions': 'regions',  # noqa: E501
-        'lines': 'lines',  # noqa: E501
+        'line_items': 'line_items',  # noqa: E501
     }
 
     read_only_vars = {
         'end_time',  # noqa: E501
         'start_time',  # noqa: E501
         'invoice_id',  # noqa: E501
         'customer_id',  # noqa: E501
         'vendor_state',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BillingEstimateResponse - a model defined in OpenAPI
+        """BillingResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -169,15 +169,15 @@
             start_time (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             invoice_id (str): [optional]  # noqa: E501
             customer_id (str): [optional]  # noqa: E501
             vendor_state (str): The current state of our third-party billing vendor. One of `up` or `down`.. [optional]  # noqa: E501
             status (BillingStatus): [optional]  # noqa: E501
             total (BillingTotal): [optional]  # noqa: E501
             regions ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}): Breakdown of regional data for products that are region based.. [optional]  # noqa: E501
-            lines ([BillingEstimateResponseAllOfLines]): [optional]  # noqa: E501
+            line_items (BillingResponseLineItems): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -236,15 +236,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """BillingEstimateResponse - a model defined in OpenAPI
+        """BillingResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -277,15 +277,15 @@
             start_time (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             invoice_id (str): [optional]  # noqa: E501
             customer_id (str): [optional]  # noqa: E501
             vendor_state (str): The current state of our third-party billing vendor. One of `up` or `down`.. [optional]  # noqa: E501
             status (BillingStatus): [optional]  # noqa: E501
             total (BillingTotal): [optional]  # noqa: E501
             regions ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}): Breakdown of regional data for products that are region based.. [optional]  # noqa: E501
-            lines ([BillingEstimateResponseAllOfLines]): [optional]  # noqa: E501
+            line_items (BillingResponseLineItems): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -344,12 +344,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               Billing,
-              BillingEstimateResponseAllOf,
+              BillingResponseItemItemsData,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-3.0.0/fastly/model/billing_estimate_response_all_of.py` & `fastly-3.0.1/fastly/model/billing_response_item_items_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.billing_estimate_response_all_of_lines import BillingEstimateResponseAllOfLines
-    globals()['BillingEstimateResponseAllOfLines'] = BillingEstimateResponseAllOfLines
+    from fastly.model.billing_response_line_items import BillingResponseLineItems
+    globals()['BillingResponseLineItems'] = BillingResponseLineItems
 
 
-class BillingEstimateResponseAllOf(ModelNormal):
+class BillingResponseItemItemsData(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,35 +81,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'lines': ([BillingEstimateResponseAllOfLines],),  # noqa: E501
+            'line_items': (BillingResponseLineItems,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'lines': 'lines',  # noqa: E501
+        'line_items': 'line_items',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BillingEstimateResponseAllOf - a model defined in OpenAPI
+        """BillingResponseItemItemsData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            lines ([BillingEstimateResponseAllOfLines]): [optional]  # noqa: E501
+            line_items (BillingResponseLineItems): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """BillingEstimateResponseAllOf - a model defined in OpenAPI
+        """BillingResponseItemItemsData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            lines ([BillingEstimateResponseAllOfLines]): [optional]  # noqa: E501
+            line_items (BillingResponseLineItems): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/billing_estimate_response_all_of_line.py` & `fastly-3.0.1/fastly/model/billing_estimate_lines_line_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class BillingEstimateResponseAllOfLine(ModelNormal):
+class BillingEstimateLinesLineItems(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -111,15 +111,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BillingEstimateResponseAllOfLine - a model defined in OpenAPI
+        """BillingEstimateLinesLineItems - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -201,15 +201,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """BillingEstimateResponseAllOfLine - a model defined in OpenAPI
+        """BillingEstimateLinesLineItems - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `fastly-3.0.0/fastly/model/billing_estimate_response_all_of_lines.py` & `fastly-3.0.1/fastly/model/event_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.billing_estimate_response_all_of_line import BillingEstimateResponseAllOfLine
-    globals()['BillingEstimateResponseAllOfLine'] = BillingEstimateResponseAllOfLine
+    from fastly.model.event import Event
+    globals()['Event'] = Event
 
 
-class BillingEstimateResponseAllOfLines(ModelNormal):
+class EventResponse(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,35 +81,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'line': (BillingEstimateResponseAllOfLine,),  # noqa: E501
+            'data': (Event,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'line': 'line',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BillingEstimateResponseAllOfLines - a model defined in OpenAPI
+        """EventResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            line (BillingEstimateResponseAllOfLine): [optional]  # noqa: E501
+            data (Event): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """BillingEstimateResponseAllOfLines - a model defined in OpenAPI
+        """EventResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            line (BillingEstimateResponseAllOfLine): [optional]  # noqa: E501
+            data (Event): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/billing_response.py` & `fastly-3.0.1/fastly/model/billing_estimate_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,26 +27,26 @@
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from fastly.model.billing import Billing
-    from fastly.model.billing_response_all_of import BillingResponseAllOf
-    from fastly.model.billing_response_line_item import BillingResponseLineItem
+    from fastly.model.billing_estimate_lines import BillingEstimateLines
+    from fastly.model.billing_estimate_lines_line_items import BillingEstimateLinesLineItems
     from fastly.model.billing_status import BillingStatus
     from fastly.model.billing_total import BillingTotal
     globals()['Billing'] = Billing
-    globals()['BillingResponseAllOf'] = BillingResponseAllOf
-    globals()['BillingResponseLineItem'] = BillingResponseLineItem
+    globals()['BillingEstimateLines'] = BillingEstimateLines
+    globals()['BillingEstimateLinesLineItems'] = BillingEstimateLinesLineItems
     globals()['BillingStatus'] = BillingStatus
     globals()['BillingTotal'] = BillingTotal
 
 
-class BillingResponse(ModelComposed):
+class BillingEstimateResponse(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -97,15 +97,15 @@
             'start_time': (datetime, none_type,),  # noqa: E501
             'invoice_id': (str,),  # noqa: E501
             'customer_id': (str,),  # noqa: E501
             'vendor_state': (str,),  # noqa: E501
             'status': (BillingStatus,),  # noqa: E501
             'total': (BillingTotal,),  # noqa: E501
             'regions': ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)},),  # noqa: E501
-            'line_items': ([BillingResponseLineItem],),  # noqa: E501
+            'line_items': ([BillingEstimateLinesLineItems],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -128,15 +128,15 @@
         'customer_id',  # noqa: E501
         'vendor_state',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BillingResponse - a model defined in OpenAPI
+        """BillingEstimateResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -169,15 +169,15 @@
             start_time (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             invoice_id (str): [optional]  # noqa: E501
             customer_id (str): [optional]  # noqa: E501
             vendor_state (str): The current state of our third-party billing vendor. One of `up` or `down`.. [optional]  # noqa: E501
             status (BillingStatus): [optional]  # noqa: E501
             total (BillingTotal): [optional]  # noqa: E501
             regions ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}): Breakdown of regional data for products that are region based.. [optional]  # noqa: E501
-            line_items ([BillingResponseLineItem]): [optional]  # noqa: E501
+            line_items ([BillingEstimateLinesLineItems]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -236,15 +236,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """BillingResponse - a model defined in OpenAPI
+        """BillingEstimateResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -277,15 +277,15 @@
             start_time (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             invoice_id (str): [optional]  # noqa: E501
             customer_id (str): [optional]  # noqa: E501
             vendor_state (str): The current state of our third-party billing vendor. One of `up` or `down`.. [optional]  # noqa: E501
             status (BillingStatus): [optional]  # noqa: E501
             total (BillingTotal): [optional]  # noqa: E501
             regions ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}): Breakdown of regional data for products that are region based.. [optional]  # noqa: E501
-            line_items ([BillingResponseLineItem]): [optional]  # noqa: E501
+            line_items ([BillingEstimateLinesLineItems]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -344,12 +344,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               Billing,
-              BillingResponseAllOf,
+              BillingEstimateLines,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-3.0.0/fastly/model/billing_response_all_of.py` & `fastly-3.0.1/fastly/model/config_store_response_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.billing_response_line_item import BillingResponseLineItem
-    globals()['BillingResponseLineItem'] = BillingResponseLineItem
 
-
-class BillingResponseAllOf(ModelNormal):
+class ConfigStoreResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -64,52 +60,50 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'line_items': ([BillingResponseLineItem],),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'line_items': 'line_items',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BillingResponseAllOf - a model defined in OpenAPI
+        """ConfigStoreResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +128,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            line_items ([BillingResponseLineItem]): [optional]  # noqa: E501
+            id (str): An alphanumeric string identifying the config store.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +177,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """BillingResponseAllOf - a model defined in OpenAPI
+        """ConfigStoreResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +210,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            line_items ([BillingResponseLineItem]): [optional]  # noqa: E501
+            id (str): An alphanumeric string identifying the config store.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/billing_response_line_item.py` & `fastly-3.0.1/fastly/model/billing_response_line_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.billing_response_line_item_all_of import BillingResponseLineItemAllOf
+    from fastly.model.line_item_data import LineItemData
+    from fastly.model.line_item_data_read_only_invoice_id import LineItemDataReadOnlyInvoiceId
     from fastly.model.timestamps import Timestamps
-    globals()['BillingResponseLineItemAllOf'] = BillingResponseLineItemAllOf
+    globals()['LineItemData'] = LineItemData
+    globals()['LineItemDataReadOnlyInvoiceId'] = LineItemDataReadOnlyInvoiceId
     globals()['Timestamps'] = Timestamps
 
 
 class BillingResponseLineItem(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
@@ -87,15 +89,15 @@
         """
         lazy_import()
         return {
             'created_at': (datetime, none_type,),  # noqa: E501
             'deleted_at': (datetime, none_type,),  # noqa: E501
             'updated_at': (datetime, none_type,),  # noqa: E501
             'amount': (float,),  # noqa: E501
-            'aria_invoice_id': (str,),  # noqa: E501
+            'aria_invoice_id': (LineItemDataReadOnlyInvoiceId,),  # noqa: E501
             'client_service_id': (str,),  # noqa: E501
             'credit_coupon_code': (str, none_type,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'line_number': (int,),  # noqa: E501
             'plan_name': (str,),  # noqa: E501
             'plan_no': (float,),  # noqa: E501
@@ -137,15 +139,14 @@
         'usage_type_no': 'usage_type_no',  # noqa: E501
     }
 
     read_only_vars = {
         'created_at',  # noqa: E501
         'deleted_at',  # noqa: E501
         'updated_at',  # noqa: E501
-        'aria_invoice_id',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """BillingResponseLineItem - a model defined in OpenAPI
 
@@ -180,15 +181,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             created_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             deleted_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             updated_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             amount (float): [optional]  # noqa: E501
-            aria_invoice_id (str): [optional]  # noqa: E501
+            aria_invoice_id (LineItemDataReadOnlyInvoiceId): [optional]  # noqa: E501
             client_service_id (str): [optional]  # noqa: E501
             credit_coupon_code (str, none_type): [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             line_number (int): [optional]  # noqa: E501
             plan_name (str): [optional]  # noqa: E501
             plan_no (float): [optional]  # noqa: E501
@@ -299,15 +300,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             created_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             deleted_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             updated_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             amount (float): [optional]  # noqa: E501
-            aria_invoice_id (str): [optional]  # noqa: E501
+            aria_invoice_id (LineItemDataReadOnlyInvoiceId): [optional]  # noqa: E501
             client_service_id (str): [optional]  # noqa: E501
             credit_coupon_code (str, none_type): [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             line_number (int): [optional]  # noqa: E501
             plan_name (str): [optional]  # noqa: E501
             plan_no (float): [optional]  # noqa: E501
@@ -380,13 +381,13 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              BillingResponseLineItemAllOf,
+              LineItemData,
               Timestamps,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-3.0.0/fastly/model/billing_response_line_item_all_of.py` & `fastly-3.0.1/fastly/model/line_item_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.line_item_data_read_only_invoice_id import LineItemDataReadOnlyInvoiceId
+    globals()['LineItemDataReadOnlyInvoiceId'] = LineItemDataReadOnlyInvoiceId
 
-class BillingResponseLineItemAllOf(ModelNormal):
+
+class LineItemData(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,31 +64,33 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'amount': (float,),  # noqa: E501
-            'aria_invoice_id': (str,),  # noqa: E501
+            'aria_invoice_id': (LineItemDataReadOnlyInvoiceId,),  # noqa: E501
             'client_service_id': (str,),  # noqa: E501
             'credit_coupon_code': (str, none_type,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'line_number': (int,),  # noqa: E501
             'plan_name': (str,),  # noqa: E501
             'plan_no': (float,),  # noqa: E501
@@ -120,23 +126,22 @@
         'service_no': 'service_no',  # noqa: E501
         'units': 'units',  # noqa: E501
         'usage_type_cd': 'usage_type_cd',  # noqa: E501
         'usage_type_no': 'usage_type_no',  # noqa: E501
     }
 
     read_only_vars = {
-        'aria_invoice_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BillingResponseLineItemAllOf - a model defined in OpenAPI
+        """LineItemData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -162,15 +167,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             amount (float): [optional]  # noqa: E501
-            aria_invoice_id (str): [optional]  # noqa: E501
+            aria_invoice_id (LineItemDataReadOnlyInvoiceId): [optional]  # noqa: E501
             client_service_id (str): [optional]  # noqa: E501
             credit_coupon_code (str, none_type): [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             line_number (int): [optional]  # noqa: E501
             plan_name (str): [optional]  # noqa: E501
             plan_no (float): [optional]  # noqa: E501
@@ -226,15 +231,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """BillingResponseLineItemAllOf - a model defined in OpenAPI
+        """LineItemData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -260,15 +265,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             amount (float): [optional]  # noqa: E501
-            aria_invoice_id (str): [optional]  # noqa: E501
+            aria_invoice_id (LineItemDataReadOnlyInvoiceId): [optional]  # noqa: E501
             client_service_id (str): [optional]  # noqa: E501
             credit_coupon_code (str, none_type): [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             line_number (int): [optional]  # noqa: E501
             plan_name (str): [optional]  # noqa: E501
             plan_no (float): [optional]  # noqa: E501
```

### Comparing `fastly-3.0.0/fastly/model/billing_status.py` & `fastly-3.0.1/fastly/model/billing_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,14 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.datetime_none_type import DatetimeNoneType
-    globals()['datetime, none_type'] = datetime, none_type
-
 
 class BillingStatus(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -70,46 +66,45 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'status': (str,),  # noqa: E501
-            'sent_at': (str,),  # noqa: E501
+            'sent_at': (datetime, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'status': 'status',  # noqa: E501
         'sent_at': 'sent_at',  # noqa: E501
     }
 
     read_only_vars = {
+        'sent_at',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -143,15 +138,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             status (str): What the current status of this invoice can be.. [optional]  # noqa: E501
-            sent_at (str): [optional]  # noqa: E501
+            sent_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -226,15 +221,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             status (str): What the current status of this invoice can be.. [optional]  # noqa: E501
-            sent_at (str): [optional]  # noqa: E501
+            sent_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/billing_total.py` & `fastly-3.0.1/fastly/model/billing_total.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/billing_total_extras.py` & `fastly-3.0.1/fastly/model/billing_total_extras.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/bulk_update_acl_entries_request.py` & `fastly-3.0.1/fastly/model/bulk_update_acl_entries_request.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/bulk_update_acl_entry.py` & `fastly-3.0.1/fastly/model/bulk_update_acl_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/bulk_update_acl_entry_all_of.py` & `fastly-3.0.1/fastly/model/bulk_update_acl_entry_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/bulk_update_config_store_item.py` & `fastly-3.0.1/fastly/model/bulk_update_config_store_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/bulk_update_config_store_item_all_of.py` & `fastly-3.0.1/fastly/model/bulk_update_config_store_item_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/bulk_update_config_store_list_request.py` & `fastly-3.0.1/fastly/model/bulk_update_config_store_list_request.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/bulk_update_dictionary_item.py` & `fastly-3.0.1/fastly/model/bulk_update_dictionary_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/bulk_update_dictionary_list_request.py` & `fastly-3.0.1/fastly/model/bulk_update_dictionary_list_request.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/bulk_waf_active_rule.py` & `fastly-3.0.1/fastly/model/bulk_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/bulk_waf_active_rules.py` & `fastly-3.0.1/fastly/model/bulk_waf_active_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/cache_setting.py` & `fastly-3.0.1/fastly/model/cache_setting.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/cache_setting_response.py` & `fastly-3.0.1/fastly/model/cache_setting_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/client_key.py` & `fastly-3.0.1/fastly/model/client_key.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/condition.py` & `fastly-3.0.1/fastly/model/condition.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/condition_response.py` & `fastly-3.0.1/fastly/model/condition_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/conditions_response.py` & `fastly-3.0.1/fastly/model/conditions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/config_store.py` & `fastly-3.0.1/fastly/model/config_store.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/config_store_info_response.py` & `fastly-3.0.1/fastly/model/config_store_info_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/config_store_item.py` & `fastly-3.0.1/fastly/model/config_store_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/config_store_item_response.py` & `fastly-3.0.1/fastly/model/config_store_item_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/config_store_item_response_all_of.py` & `fastly-3.0.1/fastly/model/config_store_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/config_store_response.py` & `fastly-3.0.1/fastly/model/config_store_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/config_store_response_all_of.py` & `fastly-3.0.1/fastly/model/tls_configurations_response_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.tls_configuration_response_data import TlsConfigurationResponseData
+    globals()['TlsConfigurationResponseData'] = TlsConfigurationResponseData
 
-class ConfigStoreResponseAllOf(ModelNormal):
+
+class TlsConfigurationsResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,50 +64,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (str,),  # noqa: E501
+            'data': ([TlsConfigurationResponseData],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ConfigStoreResponseAllOf - a model defined in OpenAPI
+        """TlsConfigurationsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -128,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): An alphanumeric string identifying the config store.. [optional]  # noqa: E501
+            data ([TlsConfigurationResponseData]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -177,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ConfigStoreResponseAllOf - a model defined in OpenAPI
+        """TlsConfigurationsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -210,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): An alphanumeric string identifying the config store.. [optional]  # noqa: E501
+            data ([TlsConfigurationResponseData]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/contact.py` & `fastly-3.0.1/fastly/model/contact.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/contact_response.py` & `fastly-3.0.1/fastly/model/contact_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/contact_response_all_of.py` & `fastly-3.0.1/fastly/model/contact_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/content.py` & `fastly-3.0.1/fastly/model/content.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/customer.py` & `fastly-3.0.1/fastly/model/customer.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/customer_response.py` & `fastly-3.0.1/fastly/model/customer_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/customer_response_all_of.py` & `fastly-3.0.1/fastly/model/customer_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/dictionary.py` & `fastly-3.0.1/fastly/model/dictionary.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/dictionary_info_response.py` & `fastly-3.0.1/fastly/model/dictionary_info_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/dictionary_item.py` & `fastly-3.0.1/fastly/model/dictionary_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/dictionary_item_response.py` & `fastly-3.0.1/fastly/model/dictionary_item_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/dictionary_item_response_all_of.py` & `fastly-3.0.1/fastly/model/dictionary_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/dictionary_response.py` & `fastly-3.0.1/fastly/model/dictionary_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/dictionary_response_all_of.py` & `fastly-3.0.1/fastly/model/dictionary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/diff_response.py` & `fastly-3.0.1/fastly/model/diff_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/director.py` & `fastly-3.0.1/fastly/model/director.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/director_backend.py` & `fastly-3.0.1/fastly/model/director_backend.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/director_backend_all_of.py` & `fastly-3.0.1/fastly/model/director_backend_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/director_response.py` & `fastly-3.0.1/fastly/model/director_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain.py` & `fastly-3.0.1/fastly/model/domain.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain_check_item.py` & `fastly-3.0.1/fastly/model/domain_check_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain_check_response.py` & `fastly-3.0.1/fastly/model/domain_check_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain_check_response_list.py` & `fastly-3.0.1/fastly/model/domain_check_response_list.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain_inspector.py` & `fastly-3.0.1/fastly/model/domain_inspector.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain_inspector_entry.py` & `fastly-3.0.1/fastly/model/domain_inspector_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain_inspector_entry_dimensions.py` & `fastly-3.0.1/fastly/model/domain_inspector_entry_dimensions.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain_inspector_entry_values.py` & `fastly-3.0.1/fastly/model/domain_inspector_entry_values.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain_inspector_measurements.py` & `fastly-3.0.1/fastly/model/domain_inspector_measurements.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain_inspector_realtime_entry.py` & `fastly-3.0.1/fastly/model/domain_inspector_realtime_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domain_response.py` & `fastly-3.0.1/fastly/model/domain_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/domains_response.py` & `fastly-3.0.1/fastly/model/domains_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/enabled_product_response.py` & `fastly-3.0.1/fastly/model/enabled_product_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/enabled_product_response_links.py` & `fastly-3.0.1/fastly/model/enabled_product_response_links.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/enabled_product_response_product.py` & `fastly-3.0.1/fastly/model/enabled_product_response_product.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/enabled_product_response_service.py` & `fastly-3.0.1/fastly/model/enabled_product_response_service.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/error_response.py` & `fastly-3.0.1/fastly/model/error_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/event.py` & `fastly-3.0.1/fastly/model/event.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/event_attributes.py` & `fastly-3.0.1/fastly/model/event_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/event_data.py` & `fastly-3.0.1/fastly/model/event_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/event_data_items.py` & `fastly-3.0.1/fastly/model/event_data_items.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/event_response.py` & `fastly-3.0.1/fastly/model/waf_exclusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.event import Event
-    globals()['Event'] = Event
+    from fastly.model.waf_exclusion_data import WafExclusionData
+    globals()['WafExclusionData'] = WafExclusionData
 
 
-class EventResponse(ModelNormal):
+class WafExclusion(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (Event,),  # noqa: E501
+            'data': (WafExclusionData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """EventResponse - a model defined in OpenAPI
+        """WafExclusion - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (Event): [optional]  # noqa: E501
+            data (WafExclusionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """EventResponse - a model defined in OpenAPI
+        """WafExclusion - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (Event): [optional]  # noqa: E501
+            data (WafExclusionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/events_response.py` & `fastly-3.0.1/fastly/model/events_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/generic_token_error.py` & `fastly-3.0.1/fastly/model/generic_token_error.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/gzip.py` & `fastly-3.0.1/fastly/model/gzip.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/gzip_response.py` & `fastly-3.0.1/fastly/model/gzip_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/header.py` & `fastly-3.0.1/fastly/model/header.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/header_response.py` & `fastly-3.0.1/fastly/model/header_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/healthcheck.py` & `fastly-3.0.1/fastly/model/healthcheck.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/healthcheck_response.py` & `fastly-3.0.1/fastly/model/healthcheck_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical.py` & `fastly-3.0.1/fastly/model/historical.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_aggregate_response.py` & `fastly-3.0.1/fastly/model/historical_aggregate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_aggregate_response_all_of.py` & `fastly-3.0.1/fastly/model/historical_aggregate_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_domains.py` & `fastly-3.0.1/fastly/model/historical_domains.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_domains_data.py` & `fastly-3.0.1/fastly/model/historical_domains_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_domains_meta.py` & `fastly-3.0.1/fastly/model/historical_domains_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_domains_meta_filters.py` & `fastly-3.0.1/fastly/model/historical_domains_meta_filters.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_domains_response.py` & `fastly-3.0.1/fastly/model/historical_domains_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_domains_response_all_of.py` & `fastly-3.0.1/fastly/model/historical_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_field_aggregate_response.py` & `fastly-3.0.1/fastly/model/historical_field_aggregate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_field_aggregate_response_all_of.py` & `fastly-3.0.1/fastly/model/historical_field_aggregate_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_field_response.py` & `fastly-3.0.1/fastly/model/historical_field_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_field_response_data_field.py` & `fastly-3.0.1/fastly/model/historical_field_response_data_field.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_field_results.py` & `fastly-3.0.1/fastly/model/historical_field_results.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_field_results_attributes.py` & `fastly-3.0.1/fastly/model/historical_field_results_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_field_results_attributes_additional.py` & `fastly-3.0.1/fastly/model/historical_field_results_attributes_additional.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_meta.py` & `fastly-3.0.1/fastly/model/historical_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_origins_response.py` & `fastly-3.0.1/fastly/model/historical_origins_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_origins_response_all_of.py` & `fastly-3.0.1/fastly/model/historical_origins_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_regions_response.py` & `fastly-3.0.1/fastly/model/historical_regions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_regions_response_all_of.py` & `fastly-3.0.1/fastly/model/historical_regions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_response.py` & `fastly-3.0.1/fastly/model/historical_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_response_data_field.py` & `fastly-3.0.1/fastly/model/historical_response_data_field.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_results.py` & `fastly-3.0.1/fastly/model/historical_results.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_service.py` & `fastly-3.0.1/fastly/model/historical_service.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_services.py` & `fastly-3.0.1/fastly/model/historical_services.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_usage_aggregate_response.py` & `fastly-3.0.1/fastly/model/historical_usage_aggregate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_usage_month_response.py` & `fastly-3.0.1/fastly/model/historical_usage_month_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_usage_month_response_all_of.py` & `fastly-3.0.1/fastly/model/historical_usage_month_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_usage_month_response_data.py` & `fastly-3.0.1/fastly/model/historical_usage_month_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_usage_results.py` & `fastly-3.0.1/fastly/model/historical_usage_results.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_usage_service_response.py` & `fastly-3.0.1/fastly/model/historical_usage_service_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/historical_usage_service_response_all_of.py` & `fastly-3.0.1/fastly/model/historical_usage_service_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/http3.py` & `fastly-3.0.1/fastly/model/http3.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/http3_all_of.py` & `fastly-3.0.1/fastly/model/http3_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/http_response_format.py` & `fastly-3.0.1/fastly/model/http_response_format.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/http_stream_format.py` & `fastly-3.0.1/fastly/model/http_stream_format.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/iam_permission.py` & `fastly-3.0.1/fastly/model/iam_permission.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/iam_role.py` & `fastly-3.0.1/fastly/model/iam_role.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/iam_role_all_of.py` & `fastly-3.0.1/fastly/model/iam_role_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/iam_service_group.py` & `fastly-3.0.1/fastly/model/iam_service_group.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/iam_service_group_all_of.py` & `fastly-3.0.1/fastly/model/iam_service_group_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/iam_user_group.py` & `fastly-3.0.1/fastly/model/iam_user_group.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/iam_user_group_all_of.py` & `fastly-3.0.1/fastly/model/iam_user_group_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/included_with_waf_active_rule.py` & `fastly-3.0.1/fastly/model/included_with_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/included_with_waf_active_rule_item.py` & `fastly-3.0.1/fastly/model/included_with_waf_active_rule_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/included_with_waf_exclusion.py` & `fastly-3.0.1/fastly/model/included_with_waf_exclusion.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/included_with_waf_exclusion_item.py` & `fastly-3.0.1/fastly/model/included_with_waf_exclusion_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/included_with_waf_firewall.py` & `fastly-3.0.1/fastly/model/included_with_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/included_with_waf_firewall_version.py` & `fastly-3.0.1/fastly/model/included_with_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/included_with_waf_firewall_version_item.py` & `fastly-3.0.1/fastly/model/included_with_waf_firewall_version_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/included_with_waf_rule.py` & `fastly-3.0.1/fastly/model/included_with_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/included_with_waf_rule_item.py` & `fastly-3.0.1/fastly/model/included_with_waf_rule_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/included_with_waf_rule_revision.py` & `fastly-3.0.1/fastly/model/included_with_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_object.py` & `fastly-3.0.1/fastly/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_object1.py` & `fastly-3.0.1/fastly/model/inline_object1.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response200.py` & `fastly-3.0.1/fastly/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response2001.py` & `fastly-3.0.1/fastly/model/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response2002.py` & `fastly-3.0.1/fastly/model/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response2003.py` & `fastly-3.0.1/fastly/model/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response2003_meta.py` & `fastly-3.0.1/fastly/model/inline_response2003_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response2004.py` & `fastly-3.0.1/fastly/model/inline_response2004.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response2004_meta.py` & `fastly-3.0.1/fastly/model/inline_response2004_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response2005.py` & `fastly-3.0.1/fastly/model/inline_response2005.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response2006.py` & `fastly-3.0.1/fastly/model/inline_response2006.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response2007.py` & `fastly-3.0.1/fastly/model/inline_response2007.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/inline_response400.py` & `fastly-3.0.1/fastly/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/invitation.py` & `fastly-3.0.1/fastly/model/invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/invitation_data.py` & `fastly-3.0.1/fastly/model/invitation_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/invitation_data_attributes.py` & `fastly-3.0.1/fastly/model/invitation_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/invitation_response.py` & `fastly-3.0.1/fastly/model/invitation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/invitation_response_all_of.py` & `fastly-3.0.1/fastly/model/invitation_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/invitation_response_data.py` & `fastly-3.0.1/fastly/model/invitation_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/invitation_response_data_all_of.py` & `fastly-3.0.1/fastly/model/invitation_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/invitations_response.py` & `fastly-3.0.1/fastly/model/invitations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/invitations_response_all_of.py` & `fastly-3.0.1/fastly/model/invitations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/legacy_waf_configuration_set.py` & `fastly-3.0.1/fastly/model/legacy_waf_configuration_set.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/legacy_waf_firewall.py` & `fastly-3.0.1/fastly/model/legacy_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/legacy_waf_owasp.py` & `fastly-3.0.1/fastly/model/legacy_waf_owasp.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/legacy_waf_rule.py` & `fastly-3.0.1/fastly/model/legacy_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/legacy_waf_rule_status.py` & `fastly-3.0.1/fastly/model/legacy_waf_rule_status.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/legacy_waf_ruleset.py` & `fastly-3.0.1/fastly/model/legacy_waf_ruleset.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/legacy_waf_tag.py` & `fastly-3.0.1/fastly/model/legacy_waf_tag.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/legacy_waf_update_status.py` & `fastly-3.0.1/fastly/model/legacy_waf_update_status.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_address_and_port.py` & `fastly-3.0.1/fastly/model/logging_address_and_port.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_azureblob.py` & `fastly-3.0.1/fastly/model/logging_azureblob.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_azureblob_all_of.py` & `fastly-3.0.1/fastly/model/logging_azureblob_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_azureblob_response.py` & `fastly-3.0.1/fastly/model/logging_azureblob_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_bigquery.py` & `fastly-3.0.1/fastly/model/logging_bigquery.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_bigquery_all_of.py` & `fastly-3.0.1/fastly/model/logging_bigquery_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_bigquery_response.py` & `fastly-3.0.1/fastly/model/logging_bigquery_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_cloudfiles.py` & `fastly-3.0.1/fastly/model/logging_cloudfiles.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_cloudfiles_all_of.py` & `fastly-3.0.1/fastly/model/logging_cloudfiles_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_cloudfiles_response.py` & `fastly-3.0.1/fastly/model/logging_cloudfiles_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_common.py` & `fastly-3.0.1/fastly/model/logging_common.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_datadog.py` & `fastly-3.0.1/fastly/model/logging_datadog.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_datadog_all_of.py` & `fastly-3.0.1/fastly/model/logging_datadog_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_datadog_response.py` & `fastly-3.0.1/fastly/model/logging_datadog_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_digitalocean.py` & `fastly-3.0.1/fastly/model/logging_digitalocean.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_digitalocean_all_of.py` & `fastly-3.0.1/fastly/model/logging_digitalocean_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_digitalocean_response.py` & `fastly-3.0.1/fastly/model/logging_digitalocean_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_elasticsearch.py` & `fastly-3.0.1/fastly/model/logging_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_elasticsearch_all_of.py` & `fastly-3.0.1/fastly/model/logging_elasticsearch_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_elasticsearch_response.py` & `fastly-3.0.1/fastly/model/logging_elasticsearch_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_format_version.py` & `fastly-3.0.1/fastly/model/logging_format_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_ftp.py` & `fastly-3.0.1/fastly/model/logging_ftp.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_ftp_all_of.py` & `fastly-3.0.1/fastly/model/logging_ftp_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_ftp_response.py` & `fastly-3.0.1/fastly/model/logging_ftp_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_gcs.py` & `fastly-3.0.1/fastly/model/logging_gcs.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_gcs_all_of.py` & `fastly-3.0.1/fastly/model/logging_gcs_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_gcs_common.py` & `fastly-3.0.1/fastly/model/logging_gcs_common.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_gcs_response.py` & `fastly-3.0.1/fastly/model/logging_gcs_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_generic_common.py` & `fastly-3.0.1/fastly/model/logging_generic_common.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_google_pubsub.py` & `fastly-3.0.1/fastly/model/logging_google_pubsub.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_google_pubsub_all_of.py` & `fastly-3.0.1/fastly/model/logging_google_pubsub_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_google_pubsub_response.py` & `fastly-3.0.1/fastly/model/logging_google_pubsub_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_heroku.py` & `fastly-3.0.1/fastly/model/logging_heroku.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_heroku_all_of.py` & `fastly-3.0.1/fastly/model/logging_heroku_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_heroku_response.py` & `fastly-3.0.1/fastly/model/logging_heroku_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_honeycomb.py` & `fastly-3.0.1/fastly/model/logging_honeycomb.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_honeycomb_all_of.py` & `fastly-3.0.1/fastly/model/logging_honeycomb_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_honeycomb_response.py` & `fastly-3.0.1/fastly/model/logging_honeycomb_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_https.py` & `fastly-3.0.1/fastly/model/logging_https.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_https_all_of.py` & `fastly-3.0.1/fastly/model/logging_https_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_https_response.py` & `fastly-3.0.1/fastly/model/logging_https_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_kafka.py` & `fastly-3.0.1/fastly/model/logging_kafka.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_kafka_all_of.py` & `fastly-3.0.1/fastly/model/logging_kafka_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_kafka_response.py` & `fastly-3.0.1/fastly/model/logging_kafka_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_kinesis.py` & `fastly-3.0.1/fastly/model/logging_kinesis.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_kinesis_response.py` & `fastly-3.0.1/fastly/model/logging_kinesis_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_logentries.py` & `fastly-3.0.1/fastly/model/logging_logentries.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_logentries_all_of.py` & `fastly-3.0.1/fastly/model/logging_logentries_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_logentries_response.py` & `fastly-3.0.1/fastly/model/logging_logentries_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_loggly.py` & `fastly-3.0.1/fastly/model/logging_loggly.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_loggly_all_of.py` & `fastly-3.0.1/fastly/model/logging_loggly_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_loggly_response.py` & `fastly-3.0.1/fastly/model/logging_loggly_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_logshuttle.py` & `fastly-3.0.1/fastly/model/logging_logshuttle.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_logshuttle_all_of.py` & `fastly-3.0.1/fastly/model/logging_logshuttle_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_logshuttle_response.py` & `fastly-3.0.1/fastly/model/logging_logshuttle_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_message_type.py` & `fastly-3.0.1/fastly/model/logging_message_type.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_newrelic.py` & `fastly-3.0.1/fastly/model/logging_newrelic.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_newrelic_all_of.py` & `fastly-3.0.1/fastly/model/logging_newrelic_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_newrelic_response.py` & `fastly-3.0.1/fastly/model/logging_newrelic_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_openstack.py` & `fastly-3.0.1/fastly/model/logging_openstack.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_openstack_all_of.py` & `fastly-3.0.1/fastly/model/logging_openstack_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_openstack_response.py` & `fastly-3.0.1/fastly/model/logging_openstack_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_papertrail.py` & `fastly-3.0.1/fastly/model/logging_papertrail.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_papertrail_response.py` & `fastly-3.0.1/fastly/model/logging_papertrail_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_placement.py` & `fastly-3.0.1/fastly/model/logging_placement.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_request_caps_common.py` & `fastly-3.0.1/fastly/model/logging_request_caps_common.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_s3.py` & `fastly-3.0.1/fastly/model/logging_s3.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_s3_all_of.py` & `fastly-3.0.1/fastly/model/logging_s3_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_s3_response.py` & `fastly-3.0.1/fastly/model/logging_s3_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_scalyr.py` & `fastly-3.0.1/fastly/model/logging_scalyr.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_scalyr_all_of.py` & `fastly-3.0.1/fastly/model/logging_scalyr_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_scalyr_response.py` & `fastly-3.0.1/fastly/model/logging_scalyr_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_sftp.py` & `fastly-3.0.1/fastly/model/logging_sftp.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_sftp_all_of.py` & `fastly-3.0.1/fastly/model/logging_sftp_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_sftp_response.py` & `fastly-3.0.1/fastly/model/logging_sftp_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_splunk.py` & `fastly-3.0.1/fastly/model/logging_splunk.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_splunk_all_of.py` & `fastly-3.0.1/fastly/model/logging_splunk_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_splunk_response.py` & `fastly-3.0.1/fastly/model/logging_splunk_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_sumologic.py` & `fastly-3.0.1/fastly/model/logging_sumologic.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_sumologic_all_of.py` & `fastly-3.0.1/fastly/model/logging_sumologic_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_sumologic_response.py` & `fastly-3.0.1/fastly/model/logging_sumologic_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_syslog.py` & `fastly-3.0.1/fastly/model/logging_syslog.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_syslog_all_of.py` & `fastly-3.0.1/fastly/model/logging_syslog_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_syslog_response.py` & `fastly-3.0.1/fastly/model/logging_syslog_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_tls_common.py` & `fastly-3.0.1/fastly/model/logging_tls_common.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/logging_use_tls.py` & `fastly-3.0.1/fastly/model/logging_use_tls.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/model403_forbidden.py` & `fastly-3.0.1/fastly/model/model403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/mutual_authentication.py` & `fastly-3.0.1/fastly/model/mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/mutual_authentication_data.py` & `fastly-3.0.1/fastly/model/mutual_authentication_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/mutual_authentication_data_attributes.py` & `fastly-3.0.1/fastly/model/mutual_authentication_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/mutual_authentication_response.py` & `fastly-3.0.1/fastly/model/mutual_authentication_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/mutual_authentication_response_attributes.py` & `fastly-3.0.1/fastly/model/mutual_authentication_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/mutual_authentication_response_attributes_all_of.py` & `fastly-3.0.1/fastly/model/mutual_authentication_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/mutual_authentication_response_data.py` & `fastly-3.0.1/fastly/model/mutual_authentication_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/mutual_authentication_response_data_all_of.py` & `fastly-3.0.1/fastly/model/mutual_authentication_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/mutual_authentications_response.py` & `fastly-3.0.1/fastly/model/mutual_authentications_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/mutual_authentications_response_all_of.py` & `fastly-3.0.1/fastly/model/mutual_authentications_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/number_version.py` & `fastly-3.0.1/fastly/model/number_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector.py` & `fastly-3.0.1/fastly/model/origin_inspector.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_dimensions.py` & `fastly-3.0.1/fastly/model/origin_inspector_dimensions.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_entry.py` & `fastly-3.0.1/fastly/model/origin_inspector_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_historical.py` & `fastly-3.0.1/fastly/model/origin_inspector_historical.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_historical_data.py` & `fastly-3.0.1/fastly/model/origin_inspector_historical_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_historical_meta.py` & `fastly-3.0.1/fastly/model/origin_inspector_historical_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_historical_meta_filters.py` & `fastly-3.0.1/fastly/model/origin_inspector_historical_meta_filters.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_measurements.py` & `fastly-3.0.1/fastly/model/origin_inspector_measurements.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_realtime_entry.py` & `fastly-3.0.1/fastly/model/origin_inspector_realtime_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_realtime_entry_recorded.py` & `fastly-3.0.1/fastly/model/origin_inspector_realtime_entry_recorded.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_subsequent_request_timestamp.py` & `fastly-3.0.1/fastly/model/origin_inspector_subsequent_request_timestamp.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/origin_inspector_values.py` & `fastly-3.0.1/fastly/model/origin_inspector_values.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/package.py` & `fastly-3.0.1/fastly/model/package.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/package_metadata.py` & `fastly-3.0.1/fastly/model/package_metadata.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/package_response.py` & `fastly-3.0.1/fastly/model/package_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/package_response_all_of.py` & `fastly-3.0.1/fastly/model/package_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/pagination.py` & `fastly-3.0.1/fastly/model/pagination.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/pagination_cursor_meta.py` & `fastly-3.0.1/fastly/model/pagination_cursor_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/pagination_links.py` & `fastly-3.0.1/fastly/model/pagination_links.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/pagination_meta.py` & `fastly-3.0.1/fastly/model/pagination_meta.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/permission.py` & `fastly-3.0.1/fastly/model/permission.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/pool.py` & `fastly-3.0.1/fastly/model/pool.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/pool_all_of.py` & `fastly-3.0.1/fastly/model/pool_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/pool_response.py` & `fastly-3.0.1/fastly/model/pool_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/pool_response_all_of.py` & `fastly-3.0.1/fastly/model/pool_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/pop.py` & `fastly-3.0.1/fastly/model/pop.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/pop_coordinates.py` & `fastly-3.0.1/fastly/model/pop_coordinates.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/public_ip_list.py` & `fastly-3.0.1/fastly/model/public_ip_list.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/publish_item.py` & `fastly-3.0.1/fastly/model/publish_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/publish_item_formats.py` & `fastly-3.0.1/fastly/model/publish_item_formats.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/publish_request.py` & `fastly-3.0.1/fastly/model/publish_request.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/purge_keys.py` & `fastly-3.0.1/fastly/model/purge_keys.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/purge_keys_response.py` & `fastly-3.0.1/fastly/model/purge_keys_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/purge_response.py` & `fastly-3.0.1/fastly/model/purge_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/rate_limiter.py` & `fastly-3.0.1/fastly/model/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/rate_limiter_response.py` & `fastly-3.0.1/fastly/model/rate_limiter_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/rate_limiter_response_all_of.py` & `fastly-3.0.1/fastly/model/rate_limiter_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/read_only_customer_id.py` & `fastly-3.0.1/fastly/model/read_only_customer_id.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/read_only_id.py` & `fastly-3.0.1/fastly/model/read_only_id.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/read_only_id_service.py` & `fastly-3.0.1/fastly/model/read_only_id_service.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/read_only_service_id.py` & `fastly-3.0.1/fastly/model/read_only_service_id.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/read_only_user_id.py` & `fastly-3.0.1/fastly/model/read_only_user_id.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/read_only_version.py` & `fastly-3.0.1/fastly/model/read_only_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/realtime.py` & `fastly-3.0.1/fastly/model/realtime.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/realtime_entry.py` & `fastly-3.0.1/fastly/model/realtime_entry.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/realtime_entry_aggregated.py` & `fastly-3.0.1/fastly/model/realtime_entry_aggregated.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/realtime_entry_datacenter.py` & `fastly-3.0.1/fastly/model/realtime_entry_datacenter.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/realtime_entry_recorded.py` & `fastly-3.0.1/fastly/model/realtime_entry_recorded.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/realtime_measurements.py` & `fastly-3.0.1/fastly/model/realtime_measurements.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/recorded_timestamp.py` & `fastly-3.0.1/fastly/model/recorded_timestamp.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_common_name.py` & `fastly-3.0.1/fastly/model/relationship_common_name.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_customer.py` & `fastly-3.0.1/fastly/model/relationship_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_customer_customer.py` & `fastly-3.0.1/fastly/model/relationship_customer_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_customer.py` & `fastly-3.0.1/fastly/model/relationship_member_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_mutual_authentication.py` & `fastly-3.0.1/fastly/model/relationship_member_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_service.py` & `fastly-3.0.1/fastly/model/relationship_member_service.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_service_invitation.py` & `fastly-3.0.1/fastly/model/relationship_member_service_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_tls_activation.py` & `fastly-3.0.1/fastly/model/relationship_member_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_tls_bulk_certificate.py` & `fastly-3.0.1/fastly/model/relationship_member_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_tls_certificate.py` & `fastly-3.0.1/fastly/model/relationship_member_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_tls_configuration.py` & `fastly-3.0.1/fastly/model/relationship_member_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_tls_dns_record.py` & `fastly-3.0.1/fastly/model/relationship_member_tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_tls_domain.py` & `fastly-3.0.1/fastly/model/relationship_member_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_tls_private_key.py` & `fastly-3.0.1/fastly/model/relationship_member_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_tls_subscription.py` & `fastly-3.0.1/fastly/model/relationship_member_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_waf_active_rule.py` & `fastly-3.0.1/fastly/model/relationship_member_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_waf_firewall.py` & `fastly-3.0.1/fastly/model/relationship_member_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_waf_firewall_version.py` & `fastly-3.0.1/fastly/model/relationship_member_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_waf_rule.py` & `fastly-3.0.1/fastly/model/relationship_member_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_waf_rule_revision.py` & `fastly-3.0.1/fastly/model/relationship_member_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_member_waf_tag.py` & `fastly-3.0.1/fastly/model/relationship_member_waf_tag.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_mutual_authentication.py` & `fastly-3.0.1/fastly/model/relationship_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_mutual_authentication_mutual_authentication.py` & `fastly-3.0.1/fastly/model/relationship_mutual_authentication_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_mutual_authentications.py` & `fastly-3.0.1/fastly/model/relationship_mutual_authentications.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_mutual_authentications_mutual_authentications.py` & `fastly-3.0.1/fastly/model/relationship_mutual_authentications_mutual_authentications.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_service.py` & `fastly-3.0.1/fastly/model/relationship_service.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_service_invitations.py` & `fastly-3.0.1/fastly/model/relationship_service_invitations.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_service_invitations_create.py` & `fastly-3.0.1/fastly/model/relationship_service_invitations_create.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_service_invitations_create_service_invitations.py` & `fastly-3.0.1/fastly/model/relationship_service_invitations_create_service_invitations.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_service_invitations_service_invitations.py` & `fastly-3.0.1/fastly/model/relationship_service_invitations_service_invitations.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_services.py` & `fastly-3.0.1/fastly/model/relationship_services.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_services_services.py` & `fastly-3.0.1/fastly/model/relationship_services_services.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_activation.py` & `fastly-3.0.1/fastly/model/relationship_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_activation_tls_activation.py` & `fastly-3.0.1/fastly/model/relationship_tls_activation_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_activations.py` & `fastly-3.0.1/fastly/model/relationship_tls_activations.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_bulk_certificate.py` & `fastly-3.0.1/fastly/model/relationship_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py` & `fastly-3.0.1/fastly/model/relationship_tls_bulk_certificate_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_bulk_certificates.py` & `fastly-3.0.1/fastly/model/relationship_tls_bulk_certificates.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_certificate.py` & `fastly-3.0.1/fastly/model/relationship_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_certificate_tls_certificate.py` & `fastly-3.0.1/fastly/model/relationship_tls_certificate_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_certificates.py` & `fastly-3.0.1/fastly/model/relationship_tls_certificates.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_certificates_tls_certificates.py` & `fastly-3.0.1/fastly/model/relationship_tls_certificates_tls_certificates.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_configuration.py` & `fastly-3.0.1/fastly/model/relationship_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_configuration_for_tls_subscription.py` & `fastly-3.0.1/fastly/model/relationship_tls_configuration_for_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_configuration_tls_configuration.py` & `fastly-3.0.1/fastly/model/relationship_tls_configuration_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_configurations.py` & `fastly-3.0.1/fastly/model/relationship_tls_configurations.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_configurations_tls_configurations.py` & `fastly-3.0.1/fastly/model/relationship_tls_configurations_tls_configurations.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_dns_record.py` & `fastly-3.0.1/fastly/model/relationship_tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_dns_record_dns_record.py` & `fastly-3.0.1/fastly/model/relationship_tls_dns_record_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_dns_records.py` & `fastly-3.0.1/fastly/model/relationship_tls_dns_records.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_domain.py` & `fastly-3.0.1/fastly/model/relationship_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_domain_tls_domain.py` & `fastly-3.0.1/fastly/model/relationship_tls_domain_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_domains.py` & `fastly-3.0.1/fastly/model/relationship_tls_domains.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_domains_tls_domains.py` & `fastly-3.0.1/fastly/model/relationship_tls_domains_tls_domains.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_private_key.py` & `fastly-3.0.1/fastly/model/relationship_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_private_key_tls_private_key.py` & `fastly-3.0.1/fastly/model/relationship_tls_private_key_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_private_keys.py` & `fastly-3.0.1/fastly/model/relationship_tls_private_keys.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_private_keys_tls_private_keys.py` & `fastly-3.0.1/fastly/model/relationship_tls_private_keys_tls_private_keys.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_subscription.py` & `fastly-3.0.1/fastly/model/relationship_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_subscription_tls_subscription.py` & `fastly-3.0.1/fastly/model/relationship_tls_subscription_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_tls_subscriptions.py` & `fastly-3.0.1/fastly/model/relationship_tls_subscriptions.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_user.py` & `fastly-3.0.1/fastly/model/relationship_user.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_user_user.py` & `fastly-3.0.1/fastly/model/relationship_user_user.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_active_rules.py` & `fastly-3.0.1/fastly/model/relationship_waf_active_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_active_rules_waf_active_rules.py` & `fastly-3.0.1/fastly/model/relationship_waf_active_rules_waf_active_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_firewall.py` & `fastly-3.0.1/fastly/model/relationship_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_firewall_version.py` & `fastly-3.0.1/fastly/model/relationship_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py` & `fastly-3.0.1/fastly/model/relationship_waf_firewall_version_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_firewall_versions.py` & `fastly-3.0.1/fastly/model/relationship_waf_firewall_versions.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_firewall_waf_firewall.py` & `fastly-3.0.1/fastly/model/relationship_waf_firewall_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_rule.py` & `fastly-3.0.1/fastly/model/relationship_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_rule_revision.py` & `fastly-3.0.1/fastly/model/relationship_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py` & `fastly-3.0.1/fastly/model/relationship_waf_rule_revision_waf_rule_revisions.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_rule_revisions.py` & `fastly-3.0.1/fastly/model/relationship_waf_rule_revisions.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_rule_waf_rule.py` & `fastly-3.0.1/fastly/model/relationship_waf_rule_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_rules.py` & `fastly-3.0.1/fastly/model/relationship_waf_rules.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_tags.py` & `fastly-3.0.1/fastly/model/relationship_waf_tags.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationship_waf_tags_waf_tags.py` & `fastly-3.0.1/fastly/model/relationship_waf_tags_waf_tags.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_invitation.py` & `fastly-3.0.1/fastly/model/relationships_for_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_mutual_authentication.py` & `fastly-3.0.1/fastly/model/relationships_for_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_star.py` & `fastly-3.0.1/fastly/model/relationships_for_star.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_tls_activation.py` & `fastly-3.0.1/fastly/model/relationships_for_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_tls_bulk_certificate.py` & `fastly-3.0.1/fastly/model/relationships_for_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_tls_configuration.py` & `fastly-3.0.1/fastly/model/relationships_for_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_tls_domain.py` & `fastly-3.0.1/fastly/model/relationships_for_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_tls_private_key.py` & `fastly-3.0.1/fastly/model/relationships_for_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_tls_subscription.py` & `fastly-3.0.1/fastly/model/relationships_for_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_waf_active_rule.py` & `fastly-3.0.1/fastly/model/relationships_for_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_waf_exclusion.py` & `fastly-3.0.1/fastly/model/relationships_for_waf_exclusion.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_waf_firewall_version.py` & `fastly-3.0.1/fastly/model/relationships_for_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/relationships_for_waf_rule.py` & `fastly-3.0.1/fastly/model/relationships_for_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/request_settings.py` & `fastly-3.0.1/fastly/model/request_settings.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/request_settings_response.py` & `fastly-3.0.1/fastly/model/request_settings_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/resource.py` & `fastly-3.0.1/fastly/model/resource.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/resource_response.py` & `fastly-3.0.1/fastly/model/resource_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/resource_response_all_of.py` & `fastly-3.0.1/fastly/model/resource_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/response_object.py` & `fastly-3.0.1/fastly/model/response_object.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/response_object_response.py` & `fastly-3.0.1/fastly/model/response_object_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/results.py` & `fastly-3.0.1/fastly/model/results.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/role_user.py` & `fastly-3.0.1/fastly/model/role_user.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/schemas_contact_response.py` & `fastly-3.0.1/fastly/model/schemas_contact_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/schemas_snippet_response.py` & `fastly-3.0.1/fastly/model/schemas_snippet_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/schemas_user_response.py` & `fastly-3.0.1/fastly/model/user_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,22 +29,22 @@
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from fastly.model.role_user import RoleUser
     from fastly.model.timestamps import Timestamps
     from fastly.model.user import User
-    from fastly.model.user_response_all_of import UserResponseAllOf
+    from fastly.model.user_response_read_only import UserResponseReadOnly
     globals()['RoleUser'] = RoleUser
     globals()['Timestamps'] = Timestamps
     globals()['User'] = User
-    globals()['UserResponseAllOf'] = UserResponseAllOf
+    globals()['UserResponseReadOnly'] = UserResponseReadOnly
 
 
-class SchemasUserResponse(ModelComposed):
+class UserResponse(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -90,18 +90,18 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'login': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'limit_services': (bool,),  # noqa: E501
-            'locked': (bool,),  # noqa: E501
-            'require_new_password': (bool,),  # noqa: E501
+            'locked': (bool, none_type,),  # noqa: E501
+            'require_new_password': (bool, none_type,),  # noqa: E501
             'role': (RoleUser,),  # noqa: E501
-            'two_factor_auth_enabled': (bool,),  # noqa: E501
+            'two_factor_auth_enabled': (bool, none_type,),  # noqa: E501
             'two_factor_setup_required': (bool,),  # noqa: E501
             'created_at': (datetime, none_type,),  # noqa: E501
             'deleted_at': (datetime, none_type,),  # noqa: E501
             'updated_at': (datetime, none_type,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'email_hash': (str,),  # noqa: E501
             'customer_id': (str,),  # noqa: E501
@@ -138,15 +138,15 @@
         'email_hash',  # noqa: E501
         'customer_id',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SchemasUserResponse - a model defined in OpenAPI
+        """UserResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -174,18 +174,18 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             login (str): [optional]  # noqa: E501
             name (str): The real life name of the user.. [optional]  # noqa: E501
             limit_services (bool): Indicates that the user has limited access to the customer's services.. [optional]  # noqa: E501
-            locked (bool): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
-            require_new_password (bool): Indicates if a new password is required at next login.. [optional]  # noqa: E501
+            locked (bool, none_type): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
+            require_new_password (bool, none_type): Indicates if a new password is required at next login.. [optional]  # noqa: E501
             role (RoleUser): [optional]  # noqa: E501
-            two_factor_auth_enabled (bool): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
+            two_factor_auth_enabled (bool, none_type): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
             two_factor_setup_required (bool): Indicates if 2FA is required by the user's customer account.. [optional]  # noqa: E501
             created_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             deleted_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             updated_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             email_hash (str): The alphanumeric string identifying a email login.. [optional]  # noqa: E501
             customer_id (str): [optional]  # noqa: E501
@@ -251,15 +251,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SchemasUserResponse - a model defined in OpenAPI
+        """UserResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -287,18 +287,18 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             login (str): [optional]  # noqa: E501
             name (str): The real life name of the user.. [optional]  # noqa: E501
             limit_services (bool): Indicates that the user has limited access to the customer's services.. [optional]  # noqa: E501
-            locked (bool): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
-            require_new_password (bool): Indicates if a new password is required at next login.. [optional]  # noqa: E501
+            locked (bool, none_type): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
+            require_new_password (bool, none_type): Indicates if a new password is required at next login.. [optional]  # noqa: E501
             role (RoleUser): [optional]  # noqa: E501
-            two_factor_auth_enabled (bool): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
+            two_factor_auth_enabled (bool, none_type): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
             two_factor_setup_required (bool): Indicates if 2FA is required by the user's customer account.. [optional]  # noqa: E501
             created_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             deleted_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             updated_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             email_hash (str): The alphanumeric string identifying a email login.. [optional]  # noqa: E501
             customer_id (str): [optional]  # noqa: E501
@@ -365,12 +365,12 @@
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               Timestamps,
               User,
-              UserResponseAllOf,
+              UserResponseReadOnly,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-3.0.0/fastly/model/schemas_vcl_response.py` & `fastly-3.0.1/fastly/model/schemas_vcl_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/schemas_version.py` & `fastly-3.0.1/fastly/model/schemas_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/schemas_version_response.py` & `fastly-3.0.1/fastly/model/schemas_version_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/schemas_waf_firewall_version.py` & `fastly-3.0.1/fastly/model/schemas_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/schemas_waf_firewall_version_data.py` & `fastly-3.0.1/fastly/model/schemas_waf_firewall_version_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/secret.py` & `fastly-3.0.1/fastly/model/secret.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/secret_response.py` & `fastly-3.0.1/fastly/model/secret_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/secret_store.py` & `fastly-3.0.1/fastly/model/secret_store.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/secret_store_response.py` & `fastly-3.0.1/fastly/model/secret_store_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/server.py` & `fastly-3.0.1/fastly/model/server.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/server_response.py` & `fastly-3.0.1/fastly/model/server_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/server_response_all_of.py` & `fastly-3.0.1/fastly/model/server_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service.py` & `fastly-3.0.1/fastly/model/service.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorization.py` & `fastly-3.0.1/fastly/model/service_authorization.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorization_data.py` & `fastly-3.0.1/fastly/model/service_authorization_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorization_data_attributes.py` & `fastly-3.0.1/fastly/model/service_authorization_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorization_data_relationships.py` & `fastly-3.0.1/fastly/model/service_authorization_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorization_data_relationships_user.py` & `fastly-3.0.1/fastly/model/service_authorization_data_relationships_user.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorization_data_relationships_user_data.py` & `fastly-3.0.1/fastly/model/service_authorization_data_relationships_user_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorization_response.py` & `fastly-3.0.1/fastly/model/service_authorization_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorization_response_data.py` & `fastly-3.0.1/fastly/model/service_authorization_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorization_response_data_all_of.py` & `fastly-3.0.1/fastly/model/service_authorization_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorizations_response.py` & `fastly-3.0.1/fastly/model/service_authorizations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_authorizations_response_all_of.py` & `fastly-3.0.1/fastly/model/service_authorizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_create.py` & `fastly-3.0.1/fastly/model/service_create.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_create_all_of.py` & `fastly-3.0.1/fastly/model/service_create_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_detail.py` & `fastly-3.0.1/fastly/model/service_detail.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_detail_all_of.py` & `fastly-3.0.1/fastly/model/service_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_id_and_version.py` & `fastly-3.0.1/fastly/model/service_id_and_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_invitation.py` & `fastly-3.0.1/fastly/model/service_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_invitation_data.py` & `fastly-3.0.1/fastly/model/service_invitation_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_invitation_data_attributes.py` & `fastly-3.0.1/fastly/model/service_invitation_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_invitation_data_relationships.py` & `fastly-3.0.1/fastly/model/service_invitation_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_invitation_response.py` & `fastly-3.0.1/fastly/model/service_invitation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_invitation_response_all_of.py` & `fastly-3.0.1/fastly/model/service_invitation_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_invitation_response_all_of_data.py` & `fastly-3.0.1/fastly/model/service_invitation_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_list_response.py` & `fastly-3.0.1/fastly/model/service_list_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_list_response_all_of.py` & `fastly-3.0.1/fastly/model/service_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_response.py` & `fastly-3.0.1/fastly/model/service_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_response_all_of.py` & `fastly-3.0.1/fastly/model/service_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_version_detail.py` & `fastly-3.0.1/fastly/model/service_version_detail.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/service_version_detail_or_null.py` & `fastly-3.0.1/fastly/model/service_version_detail_or_null.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/settings.py` & `fastly-3.0.1/fastly/model/settings.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/settings_response.py` & `fastly-3.0.1/fastly/model/settings_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/signing_key.py` & `fastly-3.0.1/fastly/model/signing_key.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/snippet.py` & `fastly-3.0.1/fastly/model/snippet.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/snippet_response.py` & `fastly-3.0.1/fastly/model/snippet_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/snippet_response_all_of.py` & `fastly-3.0.1/fastly/model/snippet_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/star.py` & `fastly-3.0.1/fastly/model/star.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/star_data.py` & `fastly-3.0.1/fastly/model/star_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/star_response.py` & `fastly-3.0.1/fastly/model/star_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/star_response_all_of.py` & `fastly-3.0.1/fastly/model/star_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/stats.py` & `fastly-3.0.1/fastly/model/stats.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/store.py` & `fastly-3.0.1/fastly/model/store.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/store_response.py` & `fastly-3.0.1/fastly/model/store_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/subsequent_request_timestamp.py` & `fastly-3.0.1/fastly/model/subsequent_request_timestamp.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/sudo_generic_token_error.py` & `fastly-3.0.1/fastly/model/sudo_generic_token_error.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/sudo_request.py` & `fastly-3.0.1/fastly/model/sudo_request.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/sudo_response.py` & `fastly-3.0.1/fastly/model/sudo_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/timestamps.py` & `fastly-3.0.1/fastly/model/timestamps.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/timestamps_no_delete.py` & `fastly-3.0.1/fastly/model/timestamps_no_delete.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_activation.py` & `fastly-3.0.1/fastly/model/tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_activation_data.py` & `fastly-3.0.1/fastly/model/tls_activation_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_activation_response.py` & `fastly-3.0.1/fastly/model/tls_activation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_activation_response_data.py` & `fastly-3.0.1/fastly/model/tls_activation_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_activation_response_data_all_of.py` & `fastly-3.0.1/fastly/model/tls_activation_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_activations_response.py` & `fastly-3.0.1/fastly/model/tls_activations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_activations_response_all_of.py` & `fastly-3.0.1/fastly/model/tls_activations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_bulk_certificate.py` & `fastly-3.0.1/fastly/model/tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_bulk_certificate_data.py` & `fastly-3.0.1/fastly/model/tls_bulk_certificate_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_bulk_certificate_data_attributes.py` & `fastly-3.0.1/fastly/model/tls_bulk_certificate_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_bulk_certificate_response.py` & `fastly-3.0.1/fastly/model/tls_bulk_certificate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_bulk_certificate_response_attributes.py` & `fastly-3.0.1/fastly/model/tls_bulk_certificate_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_bulk_certificate_response_attributes_all_of.py` & `fastly-3.0.1/fastly/model/tls_bulk_certificate_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_bulk_certificate_response_data.py` & `fastly-3.0.1/fastly/model/tls_bulk_certificate_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_bulk_certificate_response_data_all_of.py` & `fastly-3.0.1/fastly/model/tls_bulk_certificate_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_bulk_certificates_response.py` & `fastly-3.0.1/fastly/model/tls_bulk_certificates_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_bulk_certificates_response_all_of.py` & `fastly-3.0.1/fastly/model/tls_bulk_certificates_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_certificate.py` & `fastly-3.0.1/fastly/model/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_certificate_data.py` & `fastly-3.0.1/fastly/model/tls_certificate_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_certificate_data_attributes.py` & `fastly-3.0.1/fastly/model/tls_certificate_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_certificate_response.py` & `fastly-3.0.1/fastly/model/tls_certificate_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_certificate_response_attributes.py` & `fastly-3.0.1/fastly/model/tls_certificate_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_certificate_response_attributes_all_of.py` & `fastly-3.0.1/fastly/model/tls_certificate_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_certificate_response_data.py` & `fastly-3.0.1/fastly/model/tls_certificate_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_certificate_response_data_all_of.py` & `fastly-3.0.1/fastly/model/tls_certificate_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_certificates_response.py` & `fastly-3.0.1/fastly/model/tls_certificates_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_certificates_response_all_of.py` & `fastly-3.0.1/fastly/model/tls_certificates_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_common.py` & `fastly-3.0.1/fastly/model/tls_common.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_configuration.py` & `fastly-3.0.1/fastly/model/tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_configuration_data.py` & `fastly-3.0.1/fastly/model/tls_configuration_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_configuration_data_attributes.py` & `fastly-3.0.1/fastly/model/tls_configuration_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_configuration_response.py` & `fastly-3.0.1/fastly/model/tls_configuration_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_configuration_response_attributes.py` & `fastly-3.0.1/fastly/model/tls_configuration_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_configuration_response_attributes_all_of.py` & `fastly-3.0.1/fastly/model/tls_configuration_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_configuration_response_data.py` & `fastly-3.0.1/fastly/model/tls_configuration_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_configuration_response_data_all_of.py` & `fastly-3.0.1/fastly/model/tls_configuration_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_configurations_response.py` & `fastly-3.0.1/fastly/model/tls_configurations_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_configurations_response_all_of.py` & `fastly-3.0.1/fastly/model/version_response_all_of.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.tls_configuration_response_data import TlsConfigurationResponseData
-    globals()['TlsConfigurationResponseData'] = TlsConfigurationResponseData
 
-
-class TlsConfigurationsResponseAllOf(ModelNormal):
+class VersionResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -64,52 +60,51 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': ([TlsConfigurationResponseData],),  # noqa: E501
+            'service_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'service_id': 'service_id',  # noqa: E501
     }
 
     read_only_vars = {
+        'service_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TlsConfigurationsResponseAllOf - a model defined in OpenAPI
+        """VersionResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +129,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([TlsConfigurationResponseData]): [optional]  # noqa: E501
+            service_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +178,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TlsConfigurationsResponseAllOf - a model defined in OpenAPI
+        """VersionResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +211,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([TlsConfigurationResponseData]): [optional]  # noqa: E501
+            service_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/tls_dns_record.py` & `fastly-3.0.1/fastly/model/tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_domain_data.py` & `fastly-3.0.1/fastly/model/tls_domain_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_domains_response.py` & `fastly-3.0.1/fastly/model/tls_domains_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_domains_response_all_of.py` & `fastly-3.0.1/fastly/model/tls_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_private_key.py` & `fastly-3.0.1/fastly/model/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_private_key_data.py` & `fastly-3.0.1/fastly/model/tls_private_key_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_private_key_data_attributes.py` & `fastly-3.0.1/fastly/model/tls_private_key_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_private_key_response.py` & `fastly-3.0.1/fastly/model/tls_private_key_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_private_key_response_attributes.py` & `fastly-3.0.1/fastly/model/tls_private_key_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_private_key_response_attributes_all_of.py` & `fastly-3.0.1/fastly/model/tls_private_key_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_private_key_response_data.py` & `fastly-3.0.1/fastly/model/tls_private_key_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_private_keys_response.py` & `fastly-3.0.1/fastly/model/tls_private_keys_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_private_keys_response_all_of.py` & `fastly-3.0.1/fastly/model/tls_private_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_subscription.py` & `fastly-3.0.1/fastly/model/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_subscription_data.py` & `fastly-3.0.1/fastly/model/tls_subscription_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_subscription_data_attributes.py` & `fastly-3.0.1/fastly/model/tls_subscription_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_subscription_response.py` & `fastly-3.0.1/fastly/model/tls_subscription_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_subscription_response_attributes.py` & `fastly-3.0.1/fastly/model/tls_subscription_response_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_subscription_response_attributes_all_of.py` & `fastly-3.0.1/fastly/model/tls_subscription_response_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_subscription_response_data.py` & `fastly-3.0.1/fastly/model/tls_subscription_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_subscription_response_data_all_of.py` & `fastly-3.0.1/fastly/model/tls_subscription_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_subscriptions_response.py` & `fastly-3.0.1/fastly/model/tls_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tls_subscriptions_response_all_of.py` & `fastly-3.0.1/fastly/model/tls_subscriptions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/token.py` & `fastly-3.0.1/fastly/model/token.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/token_created_response.py` & `fastly-3.0.1/fastly/model/token_created_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/token_created_response_all_of.py` & `fastly-3.0.1/fastly/model/token_created_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/token_response.py` & `fastly-3.0.1/fastly/model/token_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/token_response_all_of.py` & `fastly-3.0.1/fastly/model/token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tokens_additional_props.py` & `fastly-3.0.1/fastly/model/tokens_additional_props.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/tokens_data.py` & `fastly-3.0.1/fastly/model/tokens_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_billing_address.py` & `fastly-3.0.1/fastly/model/type_billing_address.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_contact.py` & `fastly-3.0.1/fastly/model/type_contact.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_customer.py` & `fastly-3.0.1/fastly/model/type_customer.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_event.py` & `fastly-3.0.1/fastly/model/type_event.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_invitation.py` & `fastly-3.0.1/fastly/model/type_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_mutual_authentication.py` & `fastly-3.0.1/fastly/model/type_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_resource.py` & `fastly-3.0.1/fastly/model/type_resource.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_service.py` & `fastly-3.0.1/fastly/model/type_service.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_service_authorization.py` & `fastly-3.0.1/fastly/model/type_service_authorization.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_service_invitation.py` & `fastly-3.0.1/fastly/model/type_service_invitation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_star.py` & `fastly-3.0.1/fastly/model/type_star.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_tls_activation.py` & `fastly-3.0.1/fastly/model/type_tls_activation.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_tls_bulk_certificate.py` & `fastly-3.0.1/fastly/model/type_tls_bulk_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_tls_certificate.py` & `fastly-3.0.1/fastly/model/type_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_tls_configuration.py` & `fastly-3.0.1/fastly/model/type_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_tls_dns_record.py` & `fastly-3.0.1/fastly/model/type_tls_dns_record.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_tls_domain.py` & `fastly-3.0.1/fastly/model/type_tls_domain.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_tls_private_key.py` & `fastly-3.0.1/fastly/model/type_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_tls_subscription.py` & `fastly-3.0.1/fastly/model/type_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_user.py` & `fastly-3.0.1/fastly/model/type_user.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_waf_active_rule.py` & `fastly-3.0.1/fastly/model/type_waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_waf_exclusion.py` & `fastly-3.0.1/fastly/model/type_waf_exclusion.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_waf_firewall.py` & `fastly-3.0.1/fastly/model/type_waf_firewall.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_waf_firewall_version.py` & `fastly-3.0.1/fastly/model/type_waf_firewall_version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_waf_rule.py` & `fastly-3.0.1/fastly/model/type_waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_waf_rule_revision.py` & `fastly-3.0.1/fastly/model/type_waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/type_waf_tag.py` & `fastly-3.0.1/fastly/model/type_waf_tag.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/update_billing_address_request.py` & `fastly-3.0.1/fastly/model/update_billing_address_request.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/update_billing_address_request_data.py` & `fastly-3.0.1/fastly/model/update_billing_address_request_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/user.py` & `fastly-3.0.1/fastly/model/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,18 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'login': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'limit_services': (bool,),  # noqa: E501
-            'locked': (bool,),  # noqa: E501
-            'require_new_password': (bool,),  # noqa: E501
+            'locked': (bool, none_type,),  # noqa: E501
+            'require_new_password': (bool, none_type,),  # noqa: E501
             'role': (RoleUser,),  # noqa: E501
-            'two_factor_auth_enabled': (bool,),  # noqa: E501
+            'two_factor_auth_enabled': (bool, none_type,),  # noqa: E501
             'two_factor_setup_required': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -152,18 +152,18 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             login (str): [optional]  # noqa: E501
             name (str): The real life name of the user.. [optional]  # noqa: E501
             limit_services (bool): Indicates that the user has limited access to the customer's services.. [optional]  # noqa: E501
-            locked (bool): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
-            require_new_password (bool): Indicates if a new password is required at next login.. [optional]  # noqa: E501
+            locked (bool, none_type): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
+            require_new_password (bool, none_type): Indicates if a new password is required at next login.. [optional]  # noqa: E501
             role (RoleUser): [optional]  # noqa: E501
-            two_factor_auth_enabled (bool): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
+            two_factor_auth_enabled (bool, none_type): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
             two_factor_setup_required (bool): Indicates if 2FA is required by the user's customer account.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -241,18 +241,18 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             login (str): [optional]  # noqa: E501
             name (str): The real life name of the user.. [optional]  # noqa: E501
             limit_services (bool): Indicates that the user has limited access to the customer's services.. [optional]  # noqa: E501
-            locked (bool): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
-            require_new_password (bool): Indicates if a new password is required at next login.. [optional]  # noqa: E501
+            locked (bool, none_type): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
+            require_new_password (bool, none_type): Indicates if a new password is required at next login.. [optional]  # noqa: E501
             role (RoleUser): [optional]  # noqa: E501
-            two_factor_auth_enabled (bool): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
+            two_factor_auth_enabled (bool, none_type): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
             two_factor_setup_required (bool): Indicates if 2FA is required by the user's customer account.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `fastly-3.0.0/fastly/model/user_response.py` & `fastly-3.0.1/fastly/model/schemas_user_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,24 +27,24 @@
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from fastly.model.role_user import RoleUser
+    from fastly.model.schemas_user_response_read_only import SchemasUserResponseReadOnly
     from fastly.model.timestamps import Timestamps
     from fastly.model.user import User
-    from fastly.model.user_response_all_of import UserResponseAllOf
     globals()['RoleUser'] = RoleUser
+    globals()['SchemasUserResponseReadOnly'] = SchemasUserResponseReadOnly
     globals()['Timestamps'] = Timestamps
     globals()['User'] = User
-    globals()['UserResponseAllOf'] = UserResponseAllOf
 
 
-class UserResponse(ModelComposed):
+class SchemasUserResponse(ModelComposed):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -90,18 +90,18 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'login': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'limit_services': (bool,),  # noqa: E501
-            'locked': (bool,),  # noqa: E501
-            'require_new_password': (bool,),  # noqa: E501
+            'locked': (bool, none_type,),  # noqa: E501
+            'require_new_password': (bool, none_type,),  # noqa: E501
             'role': (RoleUser,),  # noqa: E501
-            'two_factor_auth_enabled': (bool,),  # noqa: E501
+            'two_factor_auth_enabled': (bool, none_type,),  # noqa: E501
             'two_factor_setup_required': (bool,),  # noqa: E501
             'created_at': (datetime, none_type,),  # noqa: E501
             'deleted_at': (datetime, none_type,),  # noqa: E501
             'updated_at': (datetime, none_type,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'email_hash': (str,),  # noqa: E501
             'customer_id': (str,),  # noqa: E501
@@ -138,15 +138,15 @@
         'email_hash',  # noqa: E501
         'customer_id',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UserResponse - a model defined in OpenAPI
+        """SchemasUserResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -174,18 +174,18 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             login (str): [optional]  # noqa: E501
             name (str): The real life name of the user.. [optional]  # noqa: E501
             limit_services (bool): Indicates that the user has limited access to the customer's services.. [optional]  # noqa: E501
-            locked (bool): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
-            require_new_password (bool): Indicates if a new password is required at next login.. [optional]  # noqa: E501
+            locked (bool, none_type): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
+            require_new_password (bool, none_type): Indicates if a new password is required at next login.. [optional]  # noqa: E501
             role (RoleUser): [optional]  # noqa: E501
-            two_factor_auth_enabled (bool): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
+            two_factor_auth_enabled (bool, none_type): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
             two_factor_setup_required (bool): Indicates if 2FA is required by the user's customer account.. [optional]  # noqa: E501
             created_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             deleted_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             updated_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             email_hash (str): The alphanumeric string identifying a email login.. [optional]  # noqa: E501
             customer_id (str): [optional]  # noqa: E501
@@ -251,15 +251,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UserResponse - a model defined in OpenAPI
+        """SchemasUserResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -287,18 +287,18 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             login (str): [optional]  # noqa: E501
             name (str): The real life name of the user.. [optional]  # noqa: E501
             limit_services (bool): Indicates that the user has limited access to the customer's services.. [optional]  # noqa: E501
-            locked (bool): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
-            require_new_password (bool): Indicates if a new password is required at next login.. [optional]  # noqa: E501
+            locked (bool, none_type): Indicates whether the is account is locked for editing or not.. [optional]  # noqa: E501
+            require_new_password (bool, none_type): Indicates if a new password is required at next login.. [optional]  # noqa: E501
             role (RoleUser): [optional]  # noqa: E501
-            two_factor_auth_enabled (bool): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
+            two_factor_auth_enabled (bool, none_type): Indicates if 2FA is enabled on the user.. [optional]  # noqa: E501
             two_factor_setup_required (bool): Indicates if 2FA is required by the user's customer account.. [optional]  # noqa: E501
             created_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             deleted_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             updated_at (datetime, none_type): Date and time in ISO 8601 format.. [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
             email_hash (str): The alphanumeric string identifying a email login.. [optional]  # noqa: E501
             customer_id (str): [optional]  # noqa: E501
@@ -363,14 +363,14 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
+              SchemasUserResponseReadOnly,
               Timestamps,
               User,
-              UserResponseAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `fastly-3.0.0/fastly/model/user_response_all_of.py` & `fastly-3.0.1/fastly/model/user_response_read_only.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class UserResponseAllOf(ModelNormal):
+class UserResponseReadOnly(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -102,15 +102,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UserResponseAllOf - a model defined in OpenAPI
+        """UserResponseReadOnly - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -186,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UserResponseAllOf - a model defined in OpenAPI
+        """UserResponseReadOnly - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `fastly-3.0.0/fastly/model/validator_result.py` & `fastly-3.0.1/fastly/model/validator_result.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/validator_result_data.py` & `fastly-3.0.1/fastly/model/validator_result_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/validator_result_data_attributes.py` & `fastly-3.0.1/fastly/model/validator_result_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/validator_result_data_attributes_messages.py` & `fastly-3.0.1/fastly/model/validator_result_data_attributes_messages.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/values.py` & `fastly-3.0.1/fastly/model/values.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/vcl.py` & `fastly-3.0.1/fastly/model/vcl.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/vcl_diff.py` & `fastly-3.0.1/fastly/model/vcl_diff.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/vcl_response.py` & `fastly-3.0.1/fastly/model/vcl_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/vcl_syntax_highlighting_response.py` & `fastly-3.0.1/fastly/model/vcl_syntax_highlighting_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/version.py` & `fastly-3.0.1/fastly/model/version.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/version_create_response.py` & `fastly-3.0.1/fastly/model/version_create_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/version_detail.py` & `fastly-3.0.1/fastly/model/version_detail.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/version_detail_settings.py` & `fastly-3.0.1/fastly/model/version_detail_settings.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/version_response.py` & `fastly-3.0.1/fastly/model/version_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/version_response_all_of.py` & `fastly-3.0.1/fastly/model/waf_firewall_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.waf_firewall_version_data import WafFirewallVersionData
+    globals()['WafFirewallVersionData'] = WafFirewallVersionData
 
-class VersionResponseAllOf(ModelNormal):
+
+class WafFirewallVersion(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,51 +64,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'service_id': (str,),  # noqa: E501
+            'data': (WafFirewallVersionData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'service_id': 'service_id',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
-        'service_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """VersionResponseAllOf - a model defined in OpenAPI
+        """WafFirewallVersion - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -129,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            service_id (str): [optional]  # noqa: E501
+            data (WafFirewallVersionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """VersionResponseAllOf - a model defined in OpenAPI
+        """WafFirewallVersion - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -211,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            service_id (str): [optional]  # noqa: E501
+            data (WafFirewallVersionData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/waf_active_rule.py` & `fastly-3.0.1/fastly/model/waf_active_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rule_creation_response.py` & `fastly-3.0.1/fastly/model/waf_active_rule_creation_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rule_data.py` & `fastly-3.0.1/fastly/model/waf_active_rule_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rule_data_attributes.py` & `fastly-3.0.1/fastly/model/waf_active_rule_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rule_response.py` & `fastly-3.0.1/fastly/model/waf_active_rule_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rule_response_data.py` & `fastly-3.0.1/fastly/model/waf_active_rule_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rule_response_data_all_of.py` & `fastly-3.0.1/fastly/model/waf_active_rule_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rule_response_data_attributes.py` & `fastly-3.0.1/fastly/model/waf_active_rule_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rule_response_data_attributes_all_of.py` & `fastly-3.0.1/fastly/model/waf_active_rule_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rule_response_data_relationships.py` & `fastly-3.0.1/fastly/model/waf_active_rule_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rules_response.py` & `fastly-3.0.1/fastly/model/waf_active_rules_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_active_rules_response_all_of.py` & `fastly-3.0.1/fastly/model/waf_active_rules_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_exclusion.py` & `fastly-3.0.1/fastly/model/waf_firewall.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.waf_exclusion_data import WafExclusionData
-    globals()['WafExclusionData'] = WafExclusionData
+    from fastly.model.waf_firewall_data import WafFirewallData
+    globals()['WafFirewallData'] = WafFirewallData
 
 
-class WafExclusion(ModelNormal):
+class WafFirewall(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (WafExclusionData,),  # noqa: E501
+            'data': (WafFirewallData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -101,15 +101,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafExclusion - a model defined in OpenAPI
+        """WafFirewall - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafExclusionData): [optional]  # noqa: E501
+            data (WafFirewallData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafExclusion - a model defined in OpenAPI
+        """WafFirewall - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafExclusionData): [optional]  # noqa: E501
+            data (WafFirewallData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/waf_exclusion_data.py` & `fastly-3.0.1/fastly/model/waf_exclusion_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_exclusion_data_attributes.py` & `fastly-3.0.1/fastly/model/waf_exclusion_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_exclusion_response.py` & `fastly-3.0.1/fastly/model/waf_exclusion_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_exclusion_response_data.py` & `fastly-3.0.1/fastly/model/waf_exclusion_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_exclusion_response_data_all_of.py` & `fastly-3.0.1/fastly/model/waf_exclusion_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_exclusion_response_data_attributes.py` & `fastly-3.0.1/fastly/model/waf_exclusion_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_exclusion_response_data_attributes_all_of.py` & `fastly-3.0.1/fastly/model/waf_exclusion_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_exclusion_response_data_relationships.py` & `fastly-3.0.1/fastly/model/waf_exclusion_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_exclusions_response.py` & `fastly-3.0.1/fastly/model/waf_exclusions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_exclusions_response_all_of.py` & `fastly-3.0.1/fastly/model/waf_exclusions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall.py` & `fastly-3.0.1/fastly/model/waf_tag_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.waf_firewall_data import WafFirewallData
-    globals()['WafFirewallData'] = WafFirewallData
 
-
-class WafFirewall(ModelNormal):
+class WafTagAttributes(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -64,52 +60,51 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (WafFirewallData,),  # noqa: E501
+            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
+        'name',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewall - a model defined in OpenAPI
+        """WafTagAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +129,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafFirewallData): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +178,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewall - a model defined in OpenAPI
+        """WafTagAttributes - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +211,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafFirewallData): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_data.py` & `fastly-3.0.1/fastly/model/waf_firewall_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_data_attributes.py` & `fastly-3.0.1/fastly/model/waf_firewall_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_response.py` & `fastly-3.0.1/fastly/model/waf_firewall_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_response_data.py` & `fastly-3.0.1/fastly/model/waf_firewall_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_response_data_all_of.py` & `fastly-3.0.1/fastly/model/waf_firewall_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_response_data_attributes.py` & `fastly-3.0.1/fastly/model/waf_firewall_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_response_data_attributes_all_of.py` & `fastly-3.0.1/fastly/model/waf_firewall_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_version.py` & `fastly-3.0.1/fastly/model/waf_firewall_version_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.waf_firewall_version_data import WafFirewallVersionData
-    globals()['WafFirewallVersionData'] = WafFirewallVersionData
+    from fastly.model.type_waf_firewall_version import TypeWafFirewallVersion
+    from fastly.model.waf_firewall_version_data_attributes import WafFirewallVersionDataAttributes
+    globals()['TypeWafFirewallVersion'] = TypeWafFirewallVersion
+    globals()['WafFirewallVersionDataAttributes'] = WafFirewallVersionDataAttributes
 
 
-class WafFirewallVersion(ModelNormal):
+class WafFirewallVersionData(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -81,35 +83,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (WafFirewallVersionData,),  # noqa: E501
+            'type': (TypeWafFirewallVersion,),  # noqa: E501
+            'attributes': (WafFirewallVersionDataAttributes,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersion - a model defined in OpenAPI
+        """WafFirewallVersionData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafFirewallVersionData): [optional]  # noqa: E501
+            type (TypeWafFirewallVersion): [optional]  # noqa: E501
+            attributes (WafFirewallVersionDataAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersion - a model defined in OpenAPI
+        """WafFirewallVersionData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafFirewallVersionData): [optional]  # noqa: E501
+            type (TypeWafFirewallVersion): [optional]  # noqa: E501
+            attributes (WafFirewallVersionDataAttributes): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_version_data.py` & `fastly-3.0.1/fastly/model/waf_firewall_version_response_data_all_of.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.type_waf_firewall_version import TypeWafFirewallVersion
-    from fastly.model.waf_firewall_version_data_attributes import WafFirewallVersionDataAttributes
-    globals()['TypeWafFirewallVersion'] = TypeWafFirewallVersion
-    globals()['WafFirewallVersionDataAttributes'] = WafFirewallVersionDataAttributes
+    from fastly.model.relationships_for_waf_firewall_version import RelationshipsForWafFirewallVersion
+    from fastly.model.waf_firewall_version_response_data_attributes import WafFirewallVersionResponseDataAttributes
+    globals()['RelationshipsForWafFirewallVersion'] = RelationshipsForWafFirewallVersion
+    globals()['WafFirewallVersionResponseDataAttributes'] = WafFirewallVersionResponseDataAttributes
 
 
-class WafFirewallVersionData(ModelNormal):
+class WafFirewallVersionResponseDataAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,37 +83,40 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (TypeWafFirewallVersion,),  # noqa: E501
-            'attributes': (WafFirewallVersionDataAttributes,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'attributes': (WafFirewallVersionResponseDataAttributes,),  # noqa: E501
+            'relationships': (RelationshipsForWafFirewallVersion,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
+        'relationships': 'relationships',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersionData - a model defined in OpenAPI
+        """WafFirewallVersionResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafFirewallVersion): [optional]  # noqa: E501
-            attributes (WafFirewallVersionDataAttributes): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a Firewall version.. [optional]  # noqa: E501
+            attributes (WafFirewallVersionResponseDataAttributes): [optional]  # noqa: E501
+            relationships (RelationshipsForWafFirewallVersion): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersionData - a model defined in OpenAPI
+        """WafFirewallVersionResponseDataAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,16 +225,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (TypeWafFirewallVersion): [optional]  # noqa: E501
-            attributes (WafFirewallVersionDataAttributes): [optional]  # noqa: E501
+            id (str): Alphanumeric string identifying a Firewall version.. [optional]  # noqa: E501
+            attributes (WafFirewallVersionResponseDataAttributes): [optional]  # noqa: E501
+            relationships (RelationshipsForWafFirewallVersion): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_version_data_attributes.py` & `fastly-3.0.1/fastly/model/waf_firewall_version_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_version_response.py` & `fastly-3.0.1/fastly/model/waf_firewall_version_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_version_response_data.py` & `fastly-3.0.1/fastly/model/waf_firewall_version_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_version_response_data_all_of.py` & `fastly-3.0.1/fastly/model/waf_firewalls_response_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.relationships_for_waf_firewall_version import RelationshipsForWafFirewallVersion
-    from fastly.model.waf_firewall_version_response_data_attributes import WafFirewallVersionResponseDataAttributes
-    globals()['RelationshipsForWafFirewallVersion'] = RelationshipsForWafFirewallVersion
-    globals()['WafFirewallVersionResponseDataAttributes'] = WafFirewallVersionResponseDataAttributes
+    from fastly.model.included_with_waf_firewall import IncludedWithWafFirewall
+    from fastly.model.waf_firewall_response_data import WafFirewallResponseData
+    globals()['IncludedWithWafFirewall'] = IncludedWithWafFirewall
+    globals()['WafFirewallResponseData'] = WafFirewallResponseData
 
 
-class WafFirewallVersionResponseDataAllOf(ModelNormal):
+class WafFirewallsResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,40 +83,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'attributes': (WafFirewallVersionResponseDataAttributes,),  # noqa: E501
-            'relationships': (RelationshipsForWafFirewallVersion,),  # noqa: E501
+            'data': ([WafFirewallResponseData],),  # noqa: E501
+            'included': (IncludedWithWafFirewall,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
-        'relationships': 'relationships',  # noqa: E501
+        'data': 'data',  # noqa: E501
+        'included': 'included',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersionResponseDataAllOf - a model defined in OpenAPI
+        """WafFirewallsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,17 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Alphanumeric string identifying a Firewall version.. [optional]  # noqa: E501
-            attributes (WafFirewallVersionResponseDataAttributes): [optional]  # noqa: E501
-            relationships (RelationshipsForWafFirewallVersion): [optional]  # noqa: E501
+            data ([WafFirewallResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafFirewall): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewallVersionResponseDataAllOf - a model defined in OpenAPI
+        """WafFirewallsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,17 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Alphanumeric string identifying a Firewall version.. [optional]  # noqa: E501
-            attributes (WafFirewallVersionResponseDataAttributes): [optional]  # noqa: E501
-            relationships (RelationshipsForWafFirewallVersion): [optional]  # noqa: E501
+            data ([WafFirewallResponseData]): [optional]  # noqa: E501
+            included (IncludedWithWafFirewall): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_version_response_data_attributes.py` & `fastly-3.0.1/fastly/model/waf_firewall_version_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_version_response_data_attributes_all_of.py` & `fastly-3.0.1/fastly/model/waf_firewall_version_response_data_attributes_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_versions_response.py` & `fastly-3.0.1/fastly/model/waf_firewall_versions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewall_versions_response_all_of.py` & `fastly-3.0.1/fastly/model/waf_firewall_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewalls_response.py` & `fastly-3.0.1/fastly/model/waf_firewalls_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_firewalls_response_all_of.py` & `fastly-3.0.1/fastly/model/waf_rule_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.included_with_waf_firewall import IncludedWithWafFirewall
-    from fastly.model.waf_firewall_response_data import WafFirewallResponseData
-    globals()['IncludedWithWafFirewall'] = IncludedWithWafFirewall
-    globals()['WafFirewallResponseData'] = WafFirewallResponseData
+    from fastly.model.included_with_waf_rule import IncludedWithWafRule
+    from fastly.model.waf_rule_response_data import WafRuleResponseData
+    globals()['IncludedWithWafRule'] = IncludedWithWafRule
+    globals()['WafRuleResponseData'] = WafRuleResponseData
 
 
-class WafFirewallsResponseAllOf(ModelNormal):
+class WafRuleResponse(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,16 +83,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([WafFirewallResponseData],),  # noqa: E501
-            'included': (IncludedWithWafFirewall,),  # noqa: E501
+            'data': (WafRuleResponseData,),  # noqa: E501
+            'included': (IncludedWithWafRule,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafFirewallsResponseAllOf - a model defined in OpenAPI
+        """WafRuleResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafFirewallResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafFirewall): [optional]  # noqa: E501
+            data (WafRuleResponseData): [optional]  # noqa: E501
+            included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafFirewallsResponseAllOf - a model defined in OpenAPI
+        """WafRuleResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,16 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafFirewallResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafFirewall): [optional]  # noqa: E501
+            data (WafRuleResponseData): [optional]  # noqa: E501
+            included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/waf_rule.py` & `fastly-3.0.1/fastly/model/waf_rule.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_attributes.py` & `fastly-3.0.1/fastly/model/waf_rule_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_response.py` & `fastly-3.0.1/fastly/model/waf_rules_response_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def lazy_import():
     from fastly.model.included_with_waf_rule import IncludedWithWafRule
     from fastly.model.waf_rule_response_data import WafRuleResponseData
     globals()['IncludedWithWafRule'] = IncludedWithWafRule
     globals()['WafRuleResponseData'] = WafRuleResponseData
 
 
-class WafRuleResponse(ModelNormal):
+class WafRulesResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,15 +83,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (WafRuleResponseData,),  # noqa: E501
+            'data': ([WafRuleResponseData],),  # noqa: E501
             'included': (IncludedWithWafRule,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRuleResponse - a model defined in OpenAPI
+        """WafRulesResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,15 +138,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafRuleResponseData): [optional]  # noqa: E501
+            data ([WafRuleResponseData]): [optional]  # noqa: E501
             included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -188,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRuleResponse - a model defined in OpenAPI
+        """WafRulesResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,15 +221,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (WafRuleResponseData): [optional]  # noqa: E501
+            data ([WafRuleResponseData]): [optional]  # noqa: E501
             included (IncludedWithWafRule): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `fastly-3.0.0/fastly/model/waf_rule_response_data.py` & `fastly-3.0.1/fastly/model/waf_rule_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_response_data_all_of.py` & `fastly-3.0.1/fastly/model/waf_rule_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_revision.py` & `fastly-3.0.1/fastly/model/waf_rule_revision.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_revision_attributes.py` & `fastly-3.0.1/fastly/model/waf_rule_revision_attributes.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_revision_or_latest.py` & `fastly-3.0.1/fastly/model/waf_rule_revision_or_latest.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_revision_response.py` & `fastly-3.0.1/fastly/model/waf_rule_revision_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_revision_response_data.py` & `fastly-3.0.1/fastly/model/waf_rule_revision_response_data.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_revision_response_data_all_of.py` & `fastly-3.0.1/fastly/model/waf_rule_revision_response_data_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_revisions_response.py` & `fastly-3.0.1/fastly/model/waf_rule_revisions_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rule_revisions_response_all_of.py` & `fastly-3.0.1/fastly/model/waf_rule_revisions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rules_response.py` & `fastly-3.0.1/fastly/model/waf_rules_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_rules_response_all_of.py` & `fastly-3.0.1/fastly/model/waf_tags_response_all_of.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from fastly.model.included_with_waf_rule import IncludedWithWafRule
-    from fastly.model.waf_rule_response_data import WafRuleResponseData
-    globals()['IncludedWithWafRule'] = IncludedWithWafRule
-    globals()['WafRuleResponseData'] = WafRuleResponseData
+    from fastly.model.waf_rule import WafRule
+    from fastly.model.waf_tags_response_data_item import WafTagsResponseDataItem
+    globals()['WafRule'] = WafRule
+    globals()['WafTagsResponseDataItem'] = WafTagsResponseDataItem
 
 
-class WafRulesResponseAllOf(ModelNormal):
+class WafTagsResponseAllOf(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -83,16 +83,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([WafRuleResponseData],),  # noqa: E501
-            'included': (IncludedWithWafRule,),  # noqa: E501
+            'data': ([WafTagsResponseDataItem],),  # noqa: E501
+            'included': ([WafRule],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafRulesResponseAllOf - a model defined in OpenAPI
+        """WafTagsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafRuleResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafRule): [optional]  # noqa: E501
+            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
+            included ([WafRule]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafRulesResponseAllOf - a model defined in OpenAPI
+        """WafTagsResponseAllOf - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,16 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafRuleResponseData]): [optional]  # noqa: E501
-            included (IncludedWithWafRule): [optional]  # noqa: E501
+            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
+            included ([WafRule]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/waf_tag.py` & `fastly-3.0.1/fastly/model/waf_tag.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_tag_attributes.py` & `fastly-3.0.1/fastly/model/ws_message_format.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
 
-class WafTagAttributes(ModelNormal):
+class WsMessageFormat(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -75,36 +75,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str,),  # noqa: E501
+            'content': (str,),  # noqa: E501
+            'content_bin': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
+        'content': 'content',  # noqa: E501
+        'content_bin': 'content-bin',  # noqa: E501
     }
 
     read_only_vars = {
-        'name',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafTagAttributes - a model defined in OpenAPI
+        """WsMessageFormat - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -129,15 +130,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            content (str): The content of a WebSocket `TEXT` message.. [optional]  # noqa: E501
+            content_bin (str): The base64-encoded content of a WebSocket `BINARY` message.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,15 +180,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafTagAttributes - a model defined in OpenAPI
+        """WsMessageFormat - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -211,15 +213,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
+            content (str): The content of a WebSocket `TEXT` message.. [optional]  # noqa: E501
+            content_bin (str): The base64-encoded content of a WebSocket `BINARY` message.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/waf_tags_response.py` & `fastly-3.0.1/fastly/model/waf_tags_response.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/waf_tags_response_all_of.py` & `fastly-3.0.1/fastly/model/schemas_user_response_read_only.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,22 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from fastly.model.waf_rule import WafRule
-    from fastly.model.waf_tags_response_data_item import WafTagsResponseDataItem
-    globals()['WafRule'] = WafRule
-    globals()['WafTagsResponseDataItem'] = WafTagsResponseDataItem
 
-
-class WafTagsResponseAllOf(ModelNormal):
+class SchemasUserResponseReadOnly(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -66,54 +60,57 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': ([WafTagsResponseDataItem],),  # noqa: E501
-            'included': ([WafRule],),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'email_hash': (str,),  # noqa: E501
+            'customer_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
-        'included': 'included',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'email_hash': 'email_hash',  # noqa: E501
+        'customer_id': 'customer_id',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
+        'email_hash',  # noqa: E501
+        'customer_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WafTagsResponseAllOf - a model defined in OpenAPI
+        """SchemasUserResponseReadOnly - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
-            included ([WafRule]): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            email_hash (str): The alphanumeric string identifying a email login.. [optional]  # noqa: E501
+            customer_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WafTagsResponseAllOf - a model defined in OpenAPI
+        """SchemasUserResponseReadOnly - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,16 +219,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([WafTagsResponseDataItem]): [optional]  # noqa: E501
-            included ([WafRule]): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            email_hash (str): The alphanumeric string identifying a email login.. [optional]  # noqa: E501
+            customer_id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/model/waf_tags_response_data_item.py` & `fastly-3.0.1/fastly/model/waf_tags_response_data_item.py`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/fastly/model/ws_message_format.py` & `fastly-3.0.1/fastly/model/billing_estimate_lines.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from fastly.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from fastly.model.billing_estimate_lines_line_items import BillingEstimateLinesLineItems
+    globals()['BillingEstimateLinesLineItems'] = BillingEstimateLinesLineItems
 
-class WsMessageFormat(ModelNormal):
+
+class BillingEstimateLines(ModelNormal):
     """NOTE: This class is auto generated.
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -60,52 +64,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'content': (str,),  # noqa: E501
-            'content_bin': (str,),  # noqa: E501
+            'line_items': ([BillingEstimateLinesLineItems],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'content': 'content',  # noqa: E501
-        'content_bin': 'content-bin',  # noqa: E501
+        'line_items': 'line_items',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WsMessageFormat - a model defined in OpenAPI
+        """BillingEstimateLines - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,16 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            content (str): The content of a WebSocket `TEXT` message.. [optional]  # noqa: E501
-            content_bin (str): The base64-encoded content of a WebSocket `BINARY` message.. [optional]  # noqa: E501
+            line_items ([BillingEstimateLinesLineItems]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WsMessageFormat - a model defined in OpenAPI
+        """BillingEstimateLines - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,16 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            content (str): The content of a WebSocket `TEXT` message.. [optional]  # noqa: E501
-            content_bin (str): The base64-encoded content of a WebSocket `BINARY` message.. [optional]  # noqa: E501
+            line_items ([BillingEstimateLinesLineItems]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `fastly-3.0.0/fastly/models/__init__.py` & `fastly-3.0.1/fastly/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,22 +34,21 @@
 from fastly.model.billing_address_attributes import BillingAddressAttributes
 from fastly.model.billing_address_request import BillingAddressRequest
 from fastly.model.billing_address_request_data import BillingAddressRequestData
 from fastly.model.billing_address_response import BillingAddressResponse
 from fastly.model.billing_address_response_data import BillingAddressResponseData
 from fastly.model.billing_address_verification_error_response import BillingAddressVerificationErrorResponse
 from fastly.model.billing_address_verification_error_response_errors import BillingAddressVerificationErrorResponseErrors
+from fastly.model.billing_estimate_lines import BillingEstimateLines
+from fastly.model.billing_estimate_lines_line_items import BillingEstimateLinesLineItems
 from fastly.model.billing_estimate_response import BillingEstimateResponse
-from fastly.model.billing_estimate_response_all_of import BillingEstimateResponseAllOf
-from fastly.model.billing_estimate_response_all_of_line import BillingEstimateResponseAllOfLine
-from fastly.model.billing_estimate_response_all_of_lines import BillingEstimateResponseAllOfLines
 from fastly.model.billing_response import BillingResponse
-from fastly.model.billing_response_all_of import BillingResponseAllOf
+from fastly.model.billing_response_item_items_data import BillingResponseItemItemsData
 from fastly.model.billing_response_line_item import BillingResponseLineItem
-from fastly.model.billing_response_line_item_all_of import BillingResponseLineItemAllOf
+from fastly.model.billing_response_line_items import BillingResponseLineItems
 from fastly.model.billing_status import BillingStatus
 from fastly.model.billing_total import BillingTotal
 from fastly.model.billing_total_extras import BillingTotalExtras
 from fastly.model.bulk_update_acl_entries_request import BulkUpdateAclEntriesRequest
 from fastly.model.bulk_update_acl_entry import BulkUpdateAclEntry
 from fastly.model.bulk_update_acl_entry_all_of import BulkUpdateAclEntryAllOf
 from fastly.model.bulk_update_config_store_item import BulkUpdateConfigStoreItem
@@ -201,14 +200,16 @@
 from fastly.model.legacy_waf_firewall import LegacyWafFirewall
 from fastly.model.legacy_waf_owasp import LegacyWafOwasp
 from fastly.model.legacy_waf_rule import LegacyWafRule
 from fastly.model.legacy_waf_rule_status import LegacyWafRuleStatus
 from fastly.model.legacy_waf_ruleset import LegacyWafRuleset
 from fastly.model.legacy_waf_tag import LegacyWafTag
 from fastly.model.legacy_waf_update_status import LegacyWafUpdateStatus
+from fastly.model.line_item_data import LineItemData
+from fastly.model.line_item_data_read_only_invoice_id import LineItemDataReadOnlyInvoiceId
 from fastly.model.logging_address_and_port import LoggingAddressAndPort
 from fastly.model.logging_azureblob import LoggingAzureblob
 from fastly.model.logging_azureblob_all_of import LoggingAzureblobAllOf
 from fastly.model.logging_azureblob_response import LoggingAzureblobResponse
 from fastly.model.logging_bigquery import LoggingBigquery
 from fastly.model.logging_bigquery_all_of import LoggingBigqueryAllOf
 from fastly.model.logging_bigquery_response import LoggingBigqueryResponse
@@ -452,14 +453,15 @@
 from fastly.model.response_object import ResponseObject
 from fastly.model.response_object_response import ResponseObjectResponse
 from fastly.model.results import Results
 from fastly.model.role_user import RoleUser
 from fastly.model.schemas_contact_response import SchemasContactResponse
 from fastly.model.schemas_snippet_response import SchemasSnippetResponse
 from fastly.model.schemas_user_response import SchemasUserResponse
+from fastly.model.schemas_user_response_read_only import SchemasUserResponseReadOnly
 from fastly.model.schemas_vcl_response import SchemasVclResponse
 from fastly.model.schemas_version import SchemasVersion
 from fastly.model.schemas_version_response import SchemasVersionResponse
 from fastly.model.schemas_waf_firewall_version import SchemasWafFirewallVersion
 from fastly.model.schemas_waf_firewall_version_data import SchemasWafFirewallVersionData
 from fastly.model.secret import Secret
 from fastly.model.secret_response import SecretResponse
@@ -612,15 +614,15 @@
 from fastly.model.type_waf_rule import TypeWafRule
 from fastly.model.type_waf_rule_revision import TypeWafRuleRevision
 from fastly.model.type_waf_tag import TypeWafTag
 from fastly.model.update_billing_address_request import UpdateBillingAddressRequest
 from fastly.model.update_billing_address_request_data import UpdateBillingAddressRequestData
 from fastly.model.user import User
 from fastly.model.user_response import UserResponse
-from fastly.model.user_response_all_of import UserResponseAllOf
+from fastly.model.user_response_read_only import UserResponseReadOnly
 from fastly.model.validator_result import ValidatorResult
 from fastly.model.validator_result_data import ValidatorResultData
 from fastly.model.validator_result_data_attributes import ValidatorResultDataAttributes
 from fastly.model.validator_result_data_attributes_messages import ValidatorResultDataAttributesMessages
 from fastly.model.values import Values
 from fastly.model.vcl import Vcl
 from fastly.model.vcl_diff import VclDiff
```

### Comparing `fastly-3.0.0/.gitignore` & `fastly-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/LICENSE` & `fastly-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/README.md` & `fastly-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fastly-3.0.0/pyproject.toml` & `fastly-3.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastly"
-version = "3.0.0"
+version = "3.0.1"
 authors = [{ name = "Fastly", email = "oss@fastly.com" }]
 description = "A Python Fastly API client library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `fastly-3.0.0/PKG-INFO` & `fastly-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastly
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Python Fastly API client library
 Project-URL: Homepage, https://github.com/fastly/fastly-py
 Project-URL: Bug Tracker, https://github.com/fastly/fastly-py/issues
 Author-email: Fastly <oss@fastly.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

