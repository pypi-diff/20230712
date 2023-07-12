# Comparing `tmp/wire4-client-1.1.2.tar.gz` & `tmp/wire4-client-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wire4-client-1.1.2.tar", last modified: Fri Nov  5 19:49:49 2021, max compression
+gzip compressed data, was "wire4-client-1.1.3.tar", last modified: Tue Jul 11 23:16:56 2023, max compression
```

## Comparing `wire4-client-1.1.2.tar` & `wire4-client-1.1.3.tar`

### file list

```diff
@@ -1,252 +1,272 @@
-drwxr-xr-x   0 franciscoreyes   (501) staff       (20)        0 2021-11-05 19:49:49.000000 wire4-client-1.1.2/
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      275 2021-11-05 19:49:49.000000 wire4-client-1.1.2/PKG-INFO
-drwxr-xr-x   0 franciscoreyes   (501) staff       (20)        0 2021-11-05 19:49:48.000000 wire4-client-1.1.2/test/
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      793 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_contacto_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      782 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_billing.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      898 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_spid_classification_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      848 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_account_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      872 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_billing_transaction.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1127 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_transferencias_spid_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      782 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_deposit.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      774 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_compay.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      782 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_webhook.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      993 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_facturas_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      866 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_pre_enrollment_data.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      832 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_error_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1011 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_puntos_de_venta_co_di_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      824 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_urls_redirect.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      991 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_empresas_co_di_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      816 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_account_spid.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      898 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_pre_enrollment_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      988 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_beneficiaries_query_register_status.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      864 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_company_registered.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1023 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_depositantes_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      840 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_get_depositants.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      832 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_account_detail.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1014 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_web_hook_deposit_authorization_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      851 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_instituciones_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      898 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_token_required_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      824 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_webhooks_list.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      840 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_contact_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1004 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_deposit_authorization_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      930 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_spid_beneficiaries_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      940 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_payment_state_pending.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      806 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_operations.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      841 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_operaciones_co_di_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      840 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_service_banking.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      840 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_address_company.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      949 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_comprobante_electrnico_de_pago__cep_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1700 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_suscripciones_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      816 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_user_company.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      872 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_certificate_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      840 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_payment.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1061 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_webhooks_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      930 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_account_beneficiary.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     2057 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_transferencias_spei_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      898 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_request_changed.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)        0 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/__init__.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      858 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_pager_response_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      814 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_institution.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      906 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_contract_detail_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      924 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_codi_operation_response_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      866 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_sales_point_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      980 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_subscription_change_status_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      866 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_sales_point.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      880 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_subscription.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      978 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_authorized_beneficiaries_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      876 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_codi_code_request_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      866 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_payments_request_id.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      962 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_authorization_transaction_group.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      832 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_amount_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      880 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_depositants_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      962 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_deposits_authorization_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      902 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_codi_code_qr_response_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      880 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_transaction_outgoing.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1118 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_autorizacin_de_depsitos_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      872 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_institution.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      840 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_webhook_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      890 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_transaction_error_code.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      866 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_use_service_banking.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      808 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_sales_point.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      904 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_beneficiary_institution.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      848 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_authorized_users.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      966 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_payment_request_codi_response_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1092 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_peticiones_de_pago_por_co_di_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      774 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_person.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      808 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_cep.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      896 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_relationships_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      816 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_cep_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      806 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_depositant.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     2480 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_cuentas_de_beneficiarios_spei_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      914 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_spid_beneficiary_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      856 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_company_requested.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      840 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_account_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      898 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_pre_monex_authorization.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      848 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_webhook_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1161 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_cuentas_de_beneficiarios_spid_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      866 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_sales_point_respose.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      758 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_item.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      842 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_web_hook.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      782 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_saldo_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      782 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_balance.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      816 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_payment_codi.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      888 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_configurations_limits.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      782 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_payment.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      906 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_deposit_received.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      866 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_codi_action.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      856 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_institutions_list.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      898 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_user_authorized.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      882 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_balance_list_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      880 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_depositants_register.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      982 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_codi_operations_filters_request_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1006 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_web_hook_deposit_authorization_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      864 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_account_reassigned.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      782 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_account.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1445 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_contracts_details_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      898 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_detailed_error_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      946 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_message_configurations_limits.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      914 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_depositant_count_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      822 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_relationship.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      914 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_transaction_outgoing_spid.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      972 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_spid_classifications_response_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1030 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_lmites_de_montos_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      896 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_beneficiaries_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      972 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_update_configurations_request_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      954 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_transactions_outgoing_register.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      850 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_sales_point_found.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      858 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_cep_search_banxico.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      946 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_deposit_authorization_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      898 2021-11-05 19:06:32.000000 wire4-client-1.1.2/test/test_contract_detail_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    18478 2021-11-05 19:06:32.000000 wire4-client-1.1.2/README.md
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      844 2021-11-05 19:06:32.000000 wire4-client-1.1.2/setup.py
-drwxr-xr-x   0 franciscoreyes   (501) staff       (20)        0 2021-11-05 19:49:48.000000 wire4-client-1.1.2/wire4_client/
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     7819 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/configuration.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    13127 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/rest.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     8702 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/__init__.py
-drwxr-xr-x   0 franciscoreyes   (501) staff       (20)        0 2021-11-05 19:49:49.000000 wire4-client-1.1.2/wire4_client/models/
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5360 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/authorized_beneficiaries_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     9114 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/beneficiaries_query_register_status.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5829 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/certificate_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    18981 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/account_reassigned.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    15791 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/spid_beneficiary_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3535 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/spid_beneficiaries_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3285 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/balance_list_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     9815 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_web_hook.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4612 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/urls_redirect.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4403 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_request_changed.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5428 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/account_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3454 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/relationships_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4355 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/configurations_limits.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     7196 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/payment_codi.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4592 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_sales_point.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5190 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_account_beneficiary.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4899 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/person.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    12011 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/codi_code_qr_response_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     6270 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/sales_point_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3166 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/depositants_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4328 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/transaction_error_code.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     9496 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/billing.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    22095 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/deposit.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5222 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/webhook_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5387 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/institution.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     8611 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/codi_operation_response_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    10205 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/transaction_outgoing.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    11055 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/cep_search_banxico.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4201 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/relationship.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    23927 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_deposit_received.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5870 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/transactions_outgoing_register.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     7710 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/webhook.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5912 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/company_requested.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4181 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/token_required_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4936 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/pre_enrollment_data.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     9405 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/billing_transaction.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4231 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/pre_enrollment_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3144 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/depositant_count_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    13432 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/transaction_outgoing_spid.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     7485 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/authorized_users.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3379 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/institutions_list.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3462 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/beneficiaries_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     8190 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/amount_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3503 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/subscription_change_status_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     8936 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/codi_code_request_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     8942 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/sales_point_found.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     8321 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/web_hook_deposit_authorization_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     7195 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/__init__.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3577 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_configurations_limits.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    21822 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/cep_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3346 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/webhooks_list.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     6306 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/depositants_register.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     7876 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/webhook_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     6554 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/depositant.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4989 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/deposit_authorization_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4319 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/spid_classification_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     9989 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/user_company.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3913 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/contract_detail_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5645 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/contract_detail_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    10469 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/operations.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3456 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/get_depositants.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    24291 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_deposit_authorization_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3676 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/update_configurations_request_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    12375 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_codi_action.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4648 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/detailed_error_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3647 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/spid_classifications_response_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5822 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/sales_point_respose.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5249 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/compay.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     8646 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_user_authorized.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4521 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/authorization_transaction_group.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     7541 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/pager_response_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5297 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/deposits_authorization_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4608 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/use_service_banking.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    20296 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_payment.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    18562 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_payment_state_pending.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     6588 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/pre_monex_authorization.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5605 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_institution.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3735 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/error_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    17512 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/account_response.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     8170 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/payments_request_id.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     8089 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_subscription.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4604 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/sales_point.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    12851 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/payment_request_codi_response_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5314 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/balance.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     6971 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/contact_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     7406 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/account_detail.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    20802 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/message_cep.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4089 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/web_hook_deposit_authorization_request.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3236 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/beneficiary_institution.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    19175 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/payment.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     3720 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/service_banking.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    10433 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/address_company.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5026 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/item.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    14844 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/account.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     7515 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/company_registered.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    10511 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/codi_operations_filters_request_dto.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    15403 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/models/account_spid.py
-drwxr-xr-x   0 franciscoreyes   (501) staff       (20)        0 2021-11-05 19:49:48.000000 wire4-client-1.1.2/wire4_client/api/
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    20944 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/contracts_details_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5464 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/comprobante_electrnico_de_pago__cep_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    38177 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/transferencias_spei_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    10516 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/lmites_de_montos_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     1446 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/__init__.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    12628 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/transferencias_spid_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5470 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/saldo_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    11438 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/peticiones_de_pago_por_co_di_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     6098 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/operaciones_co_di_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    10909 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/puntos_de_venta_co_di_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     4731 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/instituciones_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    13697 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/webhooks_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    15013 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/cuentas_de_beneficiarios_spid_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     9720 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/facturas_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    50054 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/cuentas_de_beneficiarios_spei_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    26833 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/suscripciones_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    11387 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/autorizacin_de_depsitos_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     5274 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/contacto_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    15593 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/depositantes_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     9585 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api/empresas_co_di_api.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)    24696 2021-11-05 19:06:32.000000 wire4-client-1.1.2/wire4_client/api_client.py
--rw-r--r--   0 franciscoreyes   (501) staff       (20)       38 2021-11-05 19:49:49.000000 wire4-client-1.1.2/setup.cfg
-drwxr-xr-x   0 franciscoreyes   (501) staff       (20)        0 2021-11-05 19:49:48.000000 wire4-client-1.1.2/wire4_client.egg-info/
--rw-r--r--   0 franciscoreyes   (501) staff       (20)      275 2021-11-05 19:49:48.000000 wire4-client-1.1.2/wire4_client.egg-info/PKG-INFO
--rw-r--r--   0 franciscoreyes   (501) staff       (20)     9301 2021-11-05 19:49:48.000000 wire4-client-1.1.2/wire4_client.egg-info/SOURCES.txt
--rw-r--r--   0 franciscoreyes   (501) staff       (20)       48 2021-11-05 19:49:48.000000 wire4-client-1.1.2/wire4_client.egg-info/requires.txt
--rw-r--r--   0 franciscoreyes   (501) staff       (20)       18 2021-11-05 19:49:48.000000 wire4-client-1.1.2/wire4_client.egg-info/top_level.txt
--rw-r--r--   0 franciscoreyes   (501) staff       (20)        1 2021-11-05 19:49:48.000000 wire4-client-1.1.2/wire4_client.egg-info/dependency_links.txt
+drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-07-11 23:16:56.331578 wire4-client-1.1.3/
+-rw-r--r--   0 federico   (501) staff       (20)      190 2023-07-11 23:16:56.331120 wire4-client-1.1.3/PKG-INFO
+-rw-r--r--   0 federico   (501) staff       (20)    20565 2023-07-11 23:04:51.000000 wire4-client-1.1.3/README.md
+-rw-r--r--   0 federico   (501) staff       (20)       38 2023-07-11 23:16:56.331704 wire4-client-1.1.3/setup.cfg
+-rw-r--r--   0 federico   (501) staff       (20)      844 2023-07-11 23:05:34.000000 wire4-client-1.1.3/setup.py
+drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-07-11 23:16:56.229203 wire4-client-1.1.3/test/
+-rw-r--r--   0 federico   (501) staff       (20)       15 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/__init__.py
+-rw-r--r--   0 federico   (501) staff       (20)      795 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_account.py
+-rw-r--r--   0 federico   (501) staff       (20)      845 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_account_detail.py
+-rw-r--r--   0 federico   (501) staff       (20)      877 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_account_reassigned.py
+-rw-r--r--   0 federico   (501) staff       (20)      853 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_account_request.py
+-rw-r--r--   0 federico   (501) staff       (20)      861 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_account_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      829 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_account_spid.py
+-rw-r--r--   0 federico   (501) staff       (20)      853 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_address_company.py
+-rw-r--r--   0 federico   (501) staff       (20)      845 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_amount_request.py
+-rw-r--r--   0 federico   (501) staff       (20)      975 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_authorization_transaction_group.py
+-rw-r--r--   0 federico   (501) staff       (20)      991 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_authorized_beneficiaries_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      861 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_authorized_users.py
+-rw-r--r--   0 federico   (501) staff       (20)     1099 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_autorizacin_de_depsitos_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      795 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_balance.py
+-rw-r--r--   0 federico   (501) staff       (20)      895 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_balance_list_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     1001 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_beneficiaries_query_register_status.py
+-rw-r--r--   0 federico   (501) staff       (20)      909 2023-07-11 17:54:57.000000 wire4-client-1.1.3/test/test_beneficiaries_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      853 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_beneficiary_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)      917 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_beneficiary_institution.py
+-rw-r--r--   0 federico   (501) staff       (20)      795 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_billing.py
+-rw-r--r--   0 federico   (501) staff       (20)      885 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_billing_transaction.py
+-rw-r--r--   0 federico   (501) staff       (20)     1089 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_cargos_recurrentes_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      829 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_cep_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      871 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_cep_search_banxico.py
+-rw-r--r--   0 federico   (501) staff       (20)      885 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_certificate_request.py
+-rw-r--r--   0 federico   (501) staff       (20)      915 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_codi_code_qr_response_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)      889 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_codi_code_request_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)      937 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_codi_operation_response_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)      995 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_codi_operations_filters_request_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)      877 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_company_registered.py
+-rw-r--r--   0 federico   (501) staff       (20)      869 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_company_requested.py
+-rw-r--r--   0 federico   (501) staff       (20)      787 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_compay.py
+-rw-r--r--   0 federico   (501) staff       (20)      918 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_comprobante_electrnico_de_pago__cep_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      901 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_configurations_limits.py
+-rw-r--r--   0 federico   (501) staff       (20)      919 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_confirm_recurring_charge.py
+-rw-r--r--   0 federico   (501) staff       (20)      853 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_contact_request.py
+-rw-r--r--   0 federico   (501) staff       (20)      789 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_contacto_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      911 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_contract_detail_request.py
+-rw-r--r--   0 federico   (501) staff       (20)      919 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_contract_detail_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     1432 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_contracts_details_api.py
+-rw-r--r--   0 federico   (501) staff       (20)     2455 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_cuentas_de_beneficiarios_spei_api.py
+-rw-r--r--   0 federico   (501) staff       (20)     1136 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_cuentas_de_beneficiarios_spid_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      803 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_customer.py
+-rw-r--r--   0 federico   (501) staff       (20)      795 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_deposit.py
+-rw-r--r--   0 federico   (501) staff       (20)      959 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_deposit_authorization_request.py
+-rw-r--r--   0 federico   (501) staff       (20)      819 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_depositant.py
+-rw-r--r--   0 federico   (501) staff       (20)      927 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_depositant_count_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     1216 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_depositantes_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      893 2023-07-11 17:54:58.000000 wire4-client-1.1.3/test/test_depositants_register.py
+-rw-r--r--   0 federico   (501) staff       (20)      893 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_depositants_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      975 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_deposits_authorization_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      911 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_detailed_error_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      981 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_empresas_co_di_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      845 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_error_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      989 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_facturas_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      853 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_get_depositants.py
+-rw-r--r--   0 federico   (501) staff       (20)      842 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_instituciones_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      827 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_institution.py
+-rw-r--r--   0 federico   (501) staff       (20)      869 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_institutions_list.py
+-rw-r--r--   0 federico   (501) staff       (20)      771 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_item.py
+-rw-r--r--   0 federico   (501) staff       (20)     1018 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_lmites_de_montos_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      943 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_account_beneficiary.py
+-rw-r--r--   0 federico   (501) staff       (20)      821 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_cep.py
+-rw-r--r--   0 federico   (501) staff       (20)      879 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_codi_action.py
+-rw-r--r--   0 federico   (501) staff       (20)      959 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_configurations_limits.py
+-rw-r--r--   0 federico   (501) staff       (20)     1017 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_deposit_authorization_request.py
+-rw-r--r--   0 federico   (501) staff       (20)      919 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_deposit_received.py
+-rw-r--r--   0 federico   (501) staff       (20)      885 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_institution.py
+-rw-r--r--   0 federico   (501) staff       (20)      853 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_payment.py
+-rw-r--r--   0 federico   (501) staff       (20)      953 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_payment_state_pending.py
+-rw-r--r--   0 federico   (501) staff       (20)      911 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_request_changed.py
+-rw-r--r--   0 federico   (501) staff       (20)      879 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_sales_point.py
+-rw-r--r--   0 federico   (501) staff       (20)      893 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_subscription.py
+-rw-r--r--   0 federico   (501) staff       (20)      911 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_user_authorized.py
+-rw-r--r--   0 federico   (501) staff       (20)      855 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_message_web_hook.py
+-rw-r--r--   0 federico   (501) staff       (20)      828 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_operaciones_co_di_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      819 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_operations.py
+-rw-r--r--   0 federico   (501) staff       (20)      871 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_pager_response_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)      795 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_payment.py
+-rw-r--r--   0 federico   (501) staff       (20)      829 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_payment_codi.py
+-rw-r--r--   0 federico   (501) staff       (20)      979 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_payment_request_codi_response_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)      879 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_payments_request_id.py
+-rw-r--r--   0 federico   (501) staff       (20)      957 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_payments_spei_and_spid_order_id.py
+-rw-r--r--   0 federico   (501) staff       (20)      973 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_payments_spei_and_spid_request_id.py
+-rw-r--r--   0 federico   (501) staff       (20)      787 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_person.py
+-rw-r--r--   0 federico   (501) staff       (20)     1068 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_peticiones_de_pago_por_co_di_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      879 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_pre_enrollment_data.py
+-rw-r--r--   0 federico   (501) staff       (20)      911 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_pre_enrollment_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      911 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_pre_monex_authorization.py
+-rw-r--r--   0 federico   (501) staff       (20)      795 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_product.py
+-rw-r--r--   0 federico   (501) staff       (20)      994 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_puntos_de_venta_co_di_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      919 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_recurring_charge_request.py
+-rw-r--r--   0 federico   (501) staff       (20)      835 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_relationship.py
+-rw-r--r--   0 federico   (501) staff       (20)      909 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_relationships_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      781 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_saldo_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      821 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_sales_point.py
+-rw-r--r--   0 federico   (501) staff       (20)      863 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_sales_point_found.py
+-rw-r--r--   0 federico   (501) staff       (20)      879 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_sales_point_request.py
+-rw-r--r--   0 federico   (501) staff       (20)      879 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_sales_point_respose.py
+-rw-r--r--   0 federico   (501) staff       (20)      853 2023-07-11 17:54:59.000000 wire4-client-1.1.3/test/test_service_banking.py
+-rw-r--r--   0 federico   (501) staff       (20)      943 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_spid_beneficiaries_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      927 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_spid_beneficiary_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      911 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_spid_classification_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)      985 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_spid_classifications_response_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)      993 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_subscription_change_status_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     1691 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_suscripciones_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      911 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_token_required_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      903 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_transaction_error_code.py
+-rw-r--r--   0 federico   (501) staff       (20)      893 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_transaction_outgoing.py
+-rw-r--r--   0 federico   (501) staff       (20)      927 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_transaction_outgoing_spid.py
+-rw-r--r--   0 federico   (501) staff       (20)      895 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_transaction_spei_spid.py
+-rw-r--r--   0 federico   (501) staff       (20)      967 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_transactions_outgoing_register.py
+-rw-r--r--   0 federico   (501) staff       (20)      901 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_transactions_register.py
+-rw-r--r--   0 federico   (501) staff       (20)     2832 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_transferencias_spei_api.py
+-rw-r--r--   0 federico   (501) staff       (20)     1112 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_transferencias_spid_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      985 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_update_configurations_request_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)      837 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_urls_redirect.py
+-rw-r--r--   0 federico   (501) staff       (20)      879 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_use_service_banking.py
+-rw-r--r--   0 federico   (501) staff       (20)      829 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_user_company.py
+-rw-r--r--   0 federico   (501) staff       (20)     1019 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_web_hook_deposit_authorization_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     1027 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_web_hook_deposit_authorization_response.py
+-rw-r--r--   0 federico   (501) staff       (20)      795 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_webhook.py
+-rw-r--r--   0 federico   (501) staff       (20)      853 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_webhook_request.py
+-rw-r--r--   0 federico   (501) staff       (20)      861 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_webhook_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     1057 2023-07-11 17:55:01.000000 wire4-client-1.1.3/test/test_webhooks_api.py
+-rw-r--r--   0 federico   (501) staff       (20)      837 2023-07-11 17:55:00.000000 wire4-client-1.1.3/test/test_webhooks_list.py
+drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-07-11 23:16:56.232218 wire4-client-1.1.3/wire4_client/
+-rw-r--r--   0 federico   (501) staff       (20)     9431 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/__init__.py
+drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-07-11 23:16:56.248498 wire4-client-1.1.3/wire4_client/api/
+-rw-r--r--   0 federico   (501) staff       (20)     1519 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/__init__.py
+-rw-r--r--   0 federico   (501) staff       (20)    11387 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/api/autorizacin_de_depsitos_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    11260 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/api/cargos_recurrentes_api.py
+-rw-r--r--   0 federico   (501) staff       (20)     5464 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/api/comprobante_electrnico_de_pago__cep_api.py
+-rw-r--r--   0 federico   (501) staff       (20)     5274 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/api/contacto_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    20944 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/api/contracts_details_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    50476 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/api/cuentas_de_beneficiarios_spei_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    15435 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/api/cuentas_de_beneficiarios_spid_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    16074 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/api/depositantes_api.py
+-rw-r--r--   0 federico   (501) staff       (20)     9585 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/empresas_co_di_api.py
+-rw-r--r--   0 federico   (501) staff       (20)     9720 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/facturas_api.py
+-rw-r--r--   0 federico   (501) staff       (20)     4731 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/instituciones_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    10516 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/lmites_de_montos_api.py
+-rw-r--r--   0 federico   (501) staff       (20)     6098 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/operaciones_co_di_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    11438 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/peticiones_de_pago_por_co_di_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    10909 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/puntos_de_venta_co_di_api.py
+-rw-r--r--   0 federico   (501) staff       (20)     5470 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/saldo_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    26833 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/suscripciones_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    57734 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/transferencias_spei_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    12628 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/transferencias_spid_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    13697 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api/webhooks_api.py
+-rw-r--r--   0 federico   (501) staff       (20)    24991 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/api_client.py
+-rw-r--r--   0 federico   (501) staff       (20)     7939 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/configuration.py
+drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-07-11 23:16:56.330273 wire4-client-1.1.3/wire4_client/models/
+-rw-r--r--   0 federico   (501) staff       (20)     7851 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/models/__init__.py
+-rw-r--r--   0 federico   (501) staff       (20)    14680 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/account.py
+-rw-r--r--   0 federico   (501) staff       (20)     7323 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/account_detail.py
+-rw-r--r--   0 federico   (501) staff       (20)    18677 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/account_reassigned.py
+-rw-r--r--   0 federico   (501) staff       (20)     5360 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/account_request.py
+-rw-r--r--   0 federico   (501) staff       (20)    18557 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/account_response.py
+-rw-r--r--   0 federico   (501) staff       (20)    15304 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/account_spid.py
+-rw-r--r--   0 federico   (501) staff       (20)    10432 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/address_company.py
+-rw-r--r--   0 federico   (501) staff       (20)     8189 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/amount_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     4442 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/authorization_transaction_group.py
+-rw-r--r--   0 federico   (501) staff       (20)     5271 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/authorized_beneficiaries_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     7484 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/authorized_users.py
+-rw-r--r--   0 federico   (501) staff       (20)     5313 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/balance.py
+-rw-r--r--   0 federico   (501) staff       (20)     3217 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/balance_list_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     9029 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/beneficiaries_query_register_status.py
+-rw-r--r--   0 federico   (501) staff       (20)     3377 2023-07-11 17:54:57.000000 wire4-client-1.1.3/wire4_client/models/beneficiaries_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     4351 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/beneficiary_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)     3235 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/beneficiary_institution.py
+-rw-r--r--   0 federico   (501) staff       (20)     9405 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/billing.py
+-rw-r--r--   0 federico   (501) staff       (20)     9404 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/billing_transaction.py
+-rw-r--r--   0 federico   (501) staff       (20)    21821 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/cep_response.py
+-rw-r--r--   0 federico   (501) staff       (20)    11054 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/cep_search_banxico.py
+-rw-r--r--   0 federico   (501) staff       (20)     5826 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/certificate_request.py
+-rw-r--r--   0 federico   (501) staff       (20)    12914 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/codi_code_qr_response_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)    12233 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/codi_code_request_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)     8610 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/codi_operation_response_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)    10570 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/codi_operations_filters_request_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)     7514 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/company_registered.py
+-rw-r--r--   0 federico   (501) staff       (20)     5821 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/company_requested.py
+-rw-r--r--   0 federico   (501) staff       (20)     5248 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/compay.py
+-rw-r--r--   0 federico   (501) staff       (20)     4293 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/configurations_limits.py
+-rw-r--r--   0 federico   (501) staff       (20)     4076 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/confirm_recurring_charge.py
+-rw-r--r--   0 federico   (501) staff       (20)     6970 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/contact_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     5644 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/contract_detail_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     3756 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/contract_detail_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     3875 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/customer.py
+-rw-r--r--   0 federico   (501) staff       (20)    21930 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/deposit.py
+-rw-r--r--   0 federico   (501) staff       (20)     4863 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/deposit_authorization_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     6553 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/depositant.py
+-rw-r--r--   0 federico   (501) staff       (20)     3143 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/depositant_count_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     6305 2023-07-11 17:54:58.000000 wire4-client-1.1.3/wire4_client/models/depositants_register.py
+-rw-r--r--   0 federico   (501) staff       (20)     3165 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/depositants_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     5169 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/deposits_authorization_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     4552 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/detailed_error_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     3734 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/error_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     3382 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/get_depositants.py
+-rw-r--r--   0 federico   (501) staff       (20)     5386 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/institution.py
+-rw-r--r--   0 federico   (501) staff       (20)     3303 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/institutions_list.py
+-rw-r--r--   0 federico   (501) staff       (20)     5025 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/item.py
+-rw-r--r--   0 federico   (501) staff       (20)     5189 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_account_beneficiary.py
+-rw-r--r--   0 federico   (501) staff       (20)    20801 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_cep.py
+-rw-r--r--   0 federico   (501) staff       (20)    12374 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_codi_action.py
+-rw-r--r--   0 federico   (501) staff       (20)     3482 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_configurations_limits.py
+-rw-r--r--   0 federico   (501) staff       (20)    24200 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_deposit_authorization_request.py
+-rw-r--r--   0 federico   (501) staff       (20)    23762 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_deposit_received.py
+-rw-r--r--   0 federico   (501) staff       (20)     5604 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_institution.py
+-rw-r--r--   0 federico   (501) staff       (20)    20131 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_payment.py
+-rw-r--r--   0 federico   (501) staff       (20)    18471 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_payment_state_pending.py
+-rw-r--r--   0 federico   (501) staff       (20)     4402 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_request_changed.py
+-rw-r--r--   0 federico   (501) staff       (20)     4591 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_sales_point.py
+-rw-r--r--   0 federico   (501) staff       (20)     8088 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_subscription.py
+-rw-r--r--   0 federico   (501) staff       (20)     8645 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_user_authorized.py
+-rw-r--r--   0 federico   (501) staff       (20)     9814 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/message_web_hook.py
+-rw-r--r--   0 federico   (501) staff       (20)    10324 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/operations.py
+-rw-r--r--   0 federico   (501) staff       (20)     7467 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/pager_response_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)    19025 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/payment.py
+-rw-r--r--   0 federico   (501) staff       (20)     7255 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/payment_codi.py
+-rw-r--r--   0 federico   (501) staff       (20)    12746 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/payment_request_codi_response_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)     8102 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/payments_request_id.py
+-rw-r--r--   0 federico   (501) staff       (20)     4014 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/payments_spei_and_spid_order_id.py
+-rw-r--r--   0 federico   (501) staff       (20)     7079 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/payments_spei_and_spid_request_id.py
+-rw-r--r--   0 federico   (501) staff       (20)     4898 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/person.py
+-rw-r--r--   0 federico   (501) staff       (20)     4935 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/pre_enrollment_data.py
+-rw-r--r--   0 federico   (501) staff       (20)     4230 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/pre_enrollment_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     6587 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/pre_monex_authorization.py
+-rw-r--r--   0 federico   (501) staff       (20)     6418 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/product.py
+-rw-r--r--   0 federico   (501) staff       (20)     9288 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/recurring_charge_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     4200 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/relationship.py
+-rw-r--r--   0 federico   (501) staff       (20)     3376 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/relationships_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     4603 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/sales_point.py
+-rw-r--r--   0 federico   (501) staff       (20)     8941 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/sales_point_found.py
+-rw-r--r--   0 federico   (501) staff       (20)     6269 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/sales_point_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     5754 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/sales_point_respose.py
+-rw-r--r--   0 federico   (501) staff       (20)     3630 2023-07-11 17:54:59.000000 wire4-client-1.1.3/wire4_client/models/service_banking.py
+-rw-r--r--   0 federico   (501) staff       (20)     3433 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/spid_beneficiaries_response.py
+-rw-r--r--   0 federico   (501) staff       (20)    16673 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/spid_beneficiary_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     4318 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/spid_classification_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)     3549 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/spid_classifications_response_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)     3502 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/subscription_change_status_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     4180 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/token_required_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     4327 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/transaction_error_code.py
+-rw-r--r--   0 federico   (501) staff       (20)    10204 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/transaction_outgoing.py
+-rw-r--r--   0 federico   (501) staff       (20)    13431 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/transaction_outgoing_spid.py
+-rw-r--r--   0 federico   (501) staff       (20)    10444 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/transaction_spei_spid.py
+-rw-r--r--   0 federico   (501) staff       (20)     5777 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/transactions_outgoing_register.py
+-rw-r--r--   0 federico   (501) staff       (20)     6131 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/transactions_register.py
+-rw-r--r--   0 federico   (501) staff       (20)     3581 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/update_configurations_request_dto.py
+-rw-r--r--   0 federico   (501) staff       (20)     4611 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/urls_redirect.py
+-rw-r--r--   0 federico   (501) staff       (20)     4607 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/use_service_banking.py
+-rw-r--r--   0 federico   (501) staff       (20)     9988 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/user_company.py
+-rw-r--r--   0 federico   (501) staff       (20)     4088 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/web_hook_deposit_authorization_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     8320 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/web_hook_deposit_authorization_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     7709 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/webhook.py
+-rw-r--r--   0 federico   (501) staff       (20)     5221 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/webhook_request.py
+-rw-r--r--   0 federico   (501) staff       (20)     7875 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/webhook_response.py
+-rw-r--r--   0 federico   (501) staff       (20)     3261 2023-07-11 17:55:00.000000 wire4-client-1.1.3/wire4_client/models/webhooks_list.py
+-rw-r--r--   0 federico   (501) staff       (20)    12950 2023-07-11 17:55:01.000000 wire4-client-1.1.3/wire4_client/rest.py
+drwxr-xr-x   0 federico   (501) staff       (20)        0 2023-07-11 23:16:56.234475 wire4-client-1.1.3/wire4_client.egg-info/
+-rw-r--r--   0 federico   (501) staff       (20)      190 2023-07-11 23:16:56.000000 wire4-client-1.1.3/wire4_client.egg-info/PKG-INFO
+-rw-r--r--   0 federico   (501) staff       (20)    10090 2023-07-11 23:16:56.000000 wire4-client-1.1.3/wire4_client.egg-info/SOURCES.txt
+-rw-r--r--   0 federico   (501) staff       (20)        1 2023-07-11 23:16:56.000000 wire4-client-1.1.3/wire4_client.egg-info/dependency_links.txt
+-rw-r--r--   0 federico   (501) staff       (20)       48 2023-07-11 23:16:56.000000 wire4-client-1.1.3/wire4_client.egg-info/requires.txt
+-rw-r--r--   0 federico   (501) staff       (20)       18 2023-07-11 23:16:56.000000 wire4-client-1.1.3/wire4_client.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wire4-client-1.1.2/test/test_contacto_api.py` & `wire4-client-1.1.3/test/test_empresas_co_di_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,30 +11,37 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.contacto_api import ContactoApi  # noqa: E501
+from wire4_client.api.empresas_co_di_api import EmpresasCoDiApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestContactoApi(unittest.TestCase):
-    """ContactoApi unit test stubs"""
+class TestEmpresasCoDiApi(unittest.TestCase):
+    """EmpresasCoDiApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.contacto_api.ContactoApi()  # noqa: E501
+        self.api = EmpresasCoDiApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_send_contact_using_post(self):
-        """Test case for send_contact_using_post
+    def test_obtain_companies(self):
+        """Test case for obtain_companies
 
-        Solicitud de contacto  # noqa: E501
+        Consulta de empresas CODI®  # noqa: E501
+        """
+        pass
+
+    def test_register_company_using_post(self):
+        """Test case for register_company_using_post
+
+        Registro de empresas CODI®  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wire4-client-1.1.2/test/test_billing.py` & `wire4-client-1.1.3/test/test_item.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.billing import Billing  # noqa: E501
+from wire4_client.models.item import Item  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestBilling(unittest.TestCase):
-    """Billing unit test stubs"""
+class TestItem(unittest.TestCase):
+    """Item unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBilling(self):
-        """Test Billing"""
+    def testItem(self):
+        """Test Item"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.billing.Billing()  # noqa: E501
+        # model = wire4_client.models.item.Item()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_spid_classification_dto.py` & `wire4-client-1.1.3/test/test_spid_classification_dto.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.spid_classification_dto import SpidClassificationDTO  # noqa: E501
+from wire4_client.models.spid_classification_dto import SpidClassificationDTO  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestSpidClassificationDTO(unittest.TestCase):
     """SpidClassificationDTO unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_account_response.py` & `wire4-client-1.1.3/test/test_account_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.account_response import AccountResponse  # noqa: E501
+from wire4_client.models.account_response import AccountResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestAccountResponse(unittest.TestCase):
     """AccountResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_billing_transaction.py` & `wire4-client-1.1.3/test/test_billing_transaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.billing_transaction import BillingTransaction  # noqa: E501
+from wire4_client.models.billing_transaction import BillingTransaction  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestBillingTransaction(unittest.TestCase):
     """BillingTransaction unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_transferencias_spid_api.py` & `wire4-client-1.1.3/test/test_transferencias_spid_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.transferencias_spid_api import TransferenciasSPIDApi  # noqa: E501
+from wire4_client.api.transferencias_spid_api import TransferenciasSPIDApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestTransferenciasSPIDApi(unittest.TestCase):
     """TransferenciasSPIDApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.transferencias_spid_api.TransferenciasSPIDApi()  # noqa: E501
+        self.api = TransferenciasSPIDApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_spid_classifications_using_get(self):
         """Test case for get_spid_classifications_using_get
```

### Comparing `wire4-client-1.1.2/test/test_deposit.py` & `wire4-client-1.1.3/test/test_deposit.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.deposit import Deposit  # noqa: E501
+from wire4_client.models.deposit import Deposit  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestDeposit(unittest.TestCase):
     """Deposit unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_compay.py` & `wire4-client-1.1.3/test/test_compay.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.compay import Compay  # noqa: E501
+from wire4_client.models.compay import Compay  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestCompay(unittest.TestCase):
     """Compay unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_webhook.py` & `wire4-client-1.1.3/test/test_webhooks_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.webhook import Webhook  # noqa: E501
+from wire4_client.models.webhooks_list import WebhooksList  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestWebhook(unittest.TestCase):
-    """Webhook unit test stubs"""
+class TestWebhooksList(unittest.TestCase):
+    """WebhooksList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWebhook(self):
-        """Test Webhook"""
+    def testWebhooksList(self):
+        """Test WebhooksList"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.webhook.Webhook()  # noqa: E501
+        # model = wire4_client.models.webhooks_list.WebhooksList()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_facturas_api.py` & `wire4-client-1.1.3/test/test_facturas_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.facturas_api import FacturasApi  # noqa: E501
+from wire4_client.api.facturas_api import FacturasApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestFacturasApi(unittest.TestCase):
     """FacturasApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.facturas_api.FacturasApi()  # noqa: E501
+        self.api = FacturasApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_billings_report_by_id_using_get(self):
         """Test case for billings_report_by_id_using_get
```

### Comparing `wire4-client-1.1.2/test/test_pre_enrollment_data.py` & `wire4-client-1.1.3/test/test_pre_enrollment_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.pre_enrollment_data import PreEnrollmentData  # noqa: E501
+from wire4_client.models.pre_enrollment_data import PreEnrollmentData  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestPreEnrollmentData(unittest.TestCase):
     """PreEnrollmentData unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_error_response.py` & `wire4-client-1.1.3/test/test_cep_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.error_response import ErrorResponse  # noqa: E501
+from wire4_client.models.cep_response import CepResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestErrorResponse(unittest.TestCase):
-    """ErrorResponse unit test stubs"""
+class TestCepResponse(unittest.TestCase):
+    """CepResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testErrorResponse(self):
-        """Test ErrorResponse"""
+    def testCepResponse(self):
+        """Test CepResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.error_response.ErrorResponse()  # noqa: E501
+        # model = wire4_client.models.cep_response.CepResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_puntos_de_venta_co_di_api.py` & `wire4-client-1.1.3/test/test_puntos_de_venta_co_di_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.puntos_de_venta_co_di_api import PuntosDeVentaCoDiApi  # noqa: E501
+from wire4_client.api.puntos_de_venta_co_di_api import PuntosDeVentaCoDiApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestPuntosDeVentaCoDiApi(unittest.TestCase):
     """PuntosDeVentaCoDiApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.puntos_de_venta_co_di_api.PuntosDeVentaCoDiApi()  # noqa: E501
+        self.api = PuntosDeVentaCoDiApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_create_sales_point(self):
         """Test case for create_sales_point
```

### Comparing `wire4-client-1.1.2/test/test_urls_redirect.py` & `wire4-client-1.1.3/test/test_urls_redirect.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.urls_redirect import UrlsRedirect  # noqa: E501
+from wire4_client.models.urls_redirect import UrlsRedirect  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestUrlsRedirect(unittest.TestCase):
     """UrlsRedirect unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_empresas_co_di_api.py` & `wire4-client-1.1.3/test/test_saldo_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,37 +11,30 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.empresas_co_di_api import EmpresasCoDiApi  # noqa: E501
+from wire4_client.api.saldo_api import SaldoApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestEmpresasCoDiApi(unittest.TestCase):
-    """EmpresasCoDiApi unit test stubs"""
+class TestSaldoApi(unittest.TestCase):
+    """SaldoApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.empresas_co_di_api.EmpresasCoDiApi()  # noqa: E501
+        self.api = SaldoApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_obtain_companies(self):
-        """Test case for obtain_companies
+    def test_get_balance_using_get(self):
+        """Test case for get_balance_using_get
 
-        Consulta de empresas CODI®  # noqa: E501
-        """
-        pass
-
-    def test_register_company_using_post(self):
-        """Test case for register_company_using_post
-
-        Registro de empresas CODI®  # noqa: E501
+        Consulta los saldo de una cuenta  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `wire4-client-1.1.2/test/test_account_spid.py` & `wire4-client-1.1.3/test/test_account_spid.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.account_spid import AccountSpid  # noqa: E501
+from wire4_client.models.account_spid import AccountSpid  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestAccountSpid(unittest.TestCase):
     """AccountSpid unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_pre_enrollment_response.py` & `wire4-client-1.1.3/test/test_pre_enrollment_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.pre_enrollment_response import PreEnrollmentResponse  # noqa: E501
+from wire4_client.models.pre_enrollment_response import PreEnrollmentResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestPreEnrollmentResponse(unittest.TestCase):
     """PreEnrollmentResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_beneficiaries_query_register_status.py` & `wire4-client-1.1.3/test/test_beneficiaries_query_register_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.beneficiaries_query_register_status import BeneficiariesQueryRegisterStatus  # noqa: E501
+from wire4_client.models.beneficiaries_query_register_status import BeneficiariesQueryRegisterStatus  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestBeneficiariesQueryRegisterStatus(unittest.TestCase):
     """BeneficiariesQueryRegisterStatus unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_company_registered.py` & `wire4-client-1.1.3/test/test_company_registered.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.company_registered import CompanyRegistered  # noqa: E501
+from wire4_client.models.company_registered import CompanyRegistered  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestCompanyRegistered(unittest.TestCase):
     """CompanyRegistered unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_depositantes_api.py` & `wire4-client-1.1.3/test/test_depositantes_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,27 +11,34 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.depositantes_api import DepositantesApi  # noqa: E501
+from wire4_client.api.depositantes_api import DepositantesApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestDepositantesApi(unittest.TestCase):
     """DepositantesApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.depositantes_api.DepositantesApi()  # noqa: E501
+        self.api = DepositantesApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
+    def test_get_depositants_totals_using_get(self):
+        """Test case for get_depositants_totals_using_get
+
+        Número de depositantes por suscripción  # noqa: E501
+        """
+        pass
+
     def test_get_depositants_using_get(self):
         """Test case for get_depositants_using_get
 
         Consulta de cuentas de depositantes  # noqa: E501
         """
         pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wire4-client-1.1.2/test/test_get_depositants.py` & `wire4-client-1.1.3/test/test_customer.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.get_depositants import GetDepositants  # noqa: E501
+from wire4_client.models.customer import Customer  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestGetDepositants(unittest.TestCase):
-    """GetDepositants unit test stubs"""
+class TestCustomer(unittest.TestCase):
+    """Customer unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGetDepositants(self):
-        """Test GetDepositants"""
+    def testCustomer(self):
+        """Test Customer"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.get_depositants.GetDepositants()  # noqa: E501
+        # model = wire4_client.models.customer.Customer()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_account_detail.py` & `wire4-client-1.1.3/test/test_account_detail.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.account_detail import AccountDetail  # noqa: E501
+from wire4_client.models.account_detail import AccountDetail  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestAccountDetail(unittest.TestCase):
     """AccountDetail unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_web_hook_deposit_authorization_response.py` & `wire4-client-1.1.3/test/test_web_hook_deposit_authorization_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.web_hook_deposit_authorization_response import WebHookDepositAuthorizationResponse  # noqa: E501
+from wire4_client.models.web_hook_deposit_authorization_response import WebHookDepositAuthorizationResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestWebHookDepositAuthorizationResponse(unittest.TestCase):
     """WebHookDepositAuthorizationResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_instituciones_api.py` & `wire4-client-1.1.3/test/test_instituciones_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.instituciones_api import InstitucionesApi  # noqa: E501
+from wire4_client.api.instituciones_api import InstitucionesApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestInstitucionesApi(unittest.TestCase):
     """InstitucionesApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.instituciones_api.InstitucionesApi()  # noqa: E501
+        self.api = InstitucionesApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_all_institutions_using_get(self):
         """Test case for get_all_institutions_using_get
```

### Comparing `wire4-client-1.1.2/test/test_token_required_response.py` & `wire4-client-1.1.3/test/test_token_required_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.token_required_response import TokenRequiredResponse  # noqa: E501
+from wire4_client.models.token_required_response import TokenRequiredResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestTokenRequiredResponse(unittest.TestCase):
     """TokenRequiredResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_webhooks_list.py` & `wire4-client-1.1.3/test/test_webhook_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.webhooks_list import WebhooksList  # noqa: E501
+from wire4_client.models.webhook_request import WebhookRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestWebhooksList(unittest.TestCase):
-    """WebhooksList unit test stubs"""
+class TestWebhookRequest(unittest.TestCase):
+    """WebhookRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWebhooksList(self):
-        """Test WebhooksList"""
+    def testWebhookRequest(self):
+        """Test WebhookRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.webhooks_list.WebhooksList()  # noqa: E501
+        # model = wire4_client.models.webhook_request.WebhookRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_contact_request.py` & `wire4-client-1.1.3/test/test_contact_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.contact_request import ContactRequest  # noqa: E501
+from wire4_client.models.contact_request import ContactRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestContactRequest(unittest.TestCase):
     """ContactRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_message_deposit_authorization_request.py` & `wire4-client-1.1.3/test/test_message_deposit_authorization_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_deposit_authorization_request import MessageDepositAuthorizationRequest  # noqa: E501
+from wire4_client.models.message_deposit_authorization_request import MessageDepositAuthorizationRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestMessageDepositAuthorizationRequest(unittest.TestCase):
     """MessageDepositAuthorizationRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_spid_beneficiaries_response.py` & `wire4-client-1.1.3/test/test_spid_beneficiaries_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.spid_beneficiaries_response import SpidBeneficiariesResponse  # noqa: E501
+from wire4_client.models.spid_beneficiaries_response import SpidBeneficiariesResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestSpidBeneficiariesResponse(unittest.TestCase):
     """SpidBeneficiariesResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_message_payment_state_pending.py` & `wire4-client-1.1.3/test/test_account.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_payment_state_pending import MessagePaymentStatePending  # noqa: E501
+from wire4_client.models.account import Account  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestMessagePaymentStatePending(unittest.TestCase):
-    """MessagePaymentStatePending unit test stubs"""
+class TestAccount(unittest.TestCase):
+    """Account unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMessagePaymentStatePending(self):
-        """Test MessagePaymentStatePending"""
+    def testAccount(self):
+        """Test Account"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.message_payment_state_pending.MessagePaymentStatePending()  # noqa: E501
+        # model = wire4_client.models.account.Account()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_operations.py` & `wire4-client-1.1.3/test/test_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.operations import Operations  # noqa: E501
+from wire4_client.models.operations import Operations  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestOperations(unittest.TestCase):
     """Operations unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_operaciones_co_di_api.py` & `wire4-client-1.1.3/test/test_operaciones_co_di_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.operaciones_co_di_api import OperacionesCoDiApi  # noqa: E501
+from wire4_client.api.operaciones_co_di_api import OperacionesCoDiApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestOperacionesCoDiApi(unittest.TestCase):
     """OperacionesCoDiApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.operaciones_co_di_api.OperacionesCoDiApi()  # noqa: E501
+        self.api = OperacionesCoDiApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_consult_codi_operations(self):
         """Test case for consult_codi_operations
```

### Comparing `wire4-client-1.1.2/test/test_service_banking.py` & `wire4-client-1.1.3/test/test_service_banking.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.service_banking import ServiceBanking  # noqa: E501
+from wire4_client.models.service_banking import ServiceBanking  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestServiceBanking(unittest.TestCase):
     """ServiceBanking unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_address_company.py` & `wire4-client-1.1.3/test/test_user_company.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.address_company import AddressCompany  # noqa: E501
+from wire4_client.models.user_company import UserCompany  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestAddressCompany(unittest.TestCase):
-    """AddressCompany unit test stubs"""
+class TestUserCompany(unittest.TestCase):
+    """UserCompany unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAddressCompany(self):
-        """Test AddressCompany"""
+    def testUserCompany(self):
+        """Test UserCompany"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.address_company.AddressCompany()  # noqa: E501
+        # model = wire4_client.models.user_company.UserCompany()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_comprobante_electrnico_de_pago__cep_api.py` & `wire4-client-1.1.3/test/test_comprobante_electrnico_de_pago__cep_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.comprobante_electrnico_de_pago__cep_api import ComprobanteElectrnicoDePagoCEPApi  # noqa: E501
+from wire4_client.api.comprobante_electrnico_de_pago__cep_api import ComprobanteElectrnicoDePagoCEPApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestComprobanteElectrnicoDePagoCEPApi(unittest.TestCase):
     """ComprobanteElectrnicoDePagoCEPApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.comprobante_electrnico_de_pago__cep_api.ComprobanteElectrnicoDePagoCEPApi()  # noqa: E501
+        self.api = ComprobanteElectrnicoDePagoCEPApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_obtain_transaction_cep_using_post(self):
         """Test case for obtain_transaction_cep_using_post
```

### Comparing `wire4-client-1.1.2/test/test_suscripciones_api.py` & `wire4-client-1.1.3/test/test_suscripciones_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.suscripciones_api import SuscripcionesApi  # noqa: E501
+from wire4_client.api.suscripciones_api import SuscripcionesApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestSuscripcionesApi(unittest.TestCase):
     """SuscripcionesApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.suscripciones_api.SuscripcionesApi()  # noqa: E501
+        self.api = SuscripcionesApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_change_subscription_status_using_put(self):
         """Test case for change_subscription_status_using_put
```

### Comparing `wire4-client-1.1.2/test/test_user_company.py` & `wire4-client-1.1.3/test/test_person.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.user_company import UserCompany  # noqa: E501
+from wire4_client.models.person import Person  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestUserCompany(unittest.TestCase):
-    """UserCompany unit test stubs"""
+class TestPerson(unittest.TestCase):
+    """Person unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserCompany(self):
-        """Test UserCompany"""
+    def testPerson(self):
+        """Test Person"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.user_company.UserCompany()  # noqa: E501
+        # model = wire4_client.models.person.Person()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_certificate_request.py` & `wire4-client-1.1.3/test/test_certificate_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.certificate_request import CertificateRequest  # noqa: E501
+from wire4_client.models.certificate_request import CertificateRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestCertificateRequest(unittest.TestCase):
     """CertificateRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_message_payment.py` & `wire4-client-1.1.3/test/test_message_payment.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_payment import MessagePayment  # noqa: E501
+from wire4_client.models.message_payment import MessagePayment  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestMessagePayment(unittest.TestCase):
     """MessagePayment unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_webhooks_api.py` & `wire4-client-1.1.3/test/test_webhooks_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.webhooks_api import WebhooksApi  # noqa: E501
+from wire4_client.api.webhooks_api import WebhooksApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestWebhooksApi(unittest.TestCase):
     """WebhooksApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.webhooks_api.WebhooksApi()  # noqa: E501
+        self.api = WebhooksApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_webhook(self):
         """Test case for get_webhook
```

### Comparing `wire4-client-1.1.2/test/test_message_account_beneficiary.py` & `wire4-client-1.1.3/test/test_message_account_beneficiary.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_account_beneficiary import MessageAccountBeneficiary  # noqa: E501
+from wire4_client.models.message_account_beneficiary import MessageAccountBeneficiary  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestMessageAccountBeneficiary(unittest.TestCase):
     """MessageAccountBeneficiary unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_transferencias_spei_api.py` & `wire4-client-1.1.3/test/test_transferencias_spei_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.transferencias_spei_api import TransferenciasSPEIApi  # noqa: E501
+from wire4_client.api.transferencias_spei_api import TransferenciasSPEIApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestTransferenciasSPEIApi(unittest.TestCase):
     """TransferenciasSPEIApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.transferencias_spei_api.TransferenciasSPEIApi()  # noqa: E501
+        self.api = TransferenciasSPEIApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_create_authorization_transactions_group(self):
         """Test case for create_authorization_transactions_group
 
@@ -52,24 +52,45 @@
     def test_out_comming_spei_request_id_transactions_report_using_get(self):
         """Test case for out_comming_spei_request_id_transactions_report_using_get
 
         Consulta de transferencias de salida por identificador de petición  # noqa: E501
         """
         pass
 
+    def test_out_comming_spei_spid_order_id_transaction_report_using_get(self):
+        """Test case for out_comming_spei_spid_order_id_transaction_report_using_get
+
+        Consulta de transferencias realizadas por order_id  # noqa: E501
+        """
+        pass
+
+    def test_out_comming_spei_spid_request_id_transactions_report_using_get(self):
+        """Test case for out_comming_spei_spid_request_id_transactions_report_using_get
+
+        Consulta de transferencias de salida por identificador de petición  # noqa: E501
+        """
+        pass
+
     def test_outgoing_spei_transactions_report_using_get(self):
         """Test case for outgoing_spei_transactions_report_using_get
 
         Consulta de transferencias realizadas  # noqa: E501
         """
         pass
 
     def test_register_outgoing_spei_transaction_using_post(self):
         """Test case for register_outgoing_spei_transaction_using_post
 
         Registro de transferencias  # noqa: E501
         """
         pass
 
+    def test_register_spei_spid_outgoing_transactions_using_post(self):
+        """Test case for register_spei_spid_outgoing_transactions_using_post
+
+        Registro de transferencias SPEI y SPID  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_message_request_changed.py` & `wire4-client-1.1.3/test/test_message_request_changed.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_request_changed import MessageRequestChanged  # noqa: E501
+from wire4_client.models.message_request_changed import MessageRequestChanged  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestMessageRequestChanged(unittest.TestCase):
     """MessageRequestChanged unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_pager_response_dto.py` & `wire4-client-1.1.3/test/test_pager_response_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.pager_response_dto import PagerResponseDto  # noqa: E501
+from wire4_client.models.pager_response_dto import PagerResponseDto  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestPagerResponseDto(unittest.TestCase):
     """PagerResponseDto unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_institution.py` & `wire4-client-1.1.3/test/test_institution.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.institution import Institution  # noqa: E501
+from wire4_client.models.institution import Institution  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestInstitution(unittest.TestCase):
     """Institution unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_contract_detail_response.py` & `wire4-client-1.1.3/test/test_contract_detail_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.contract_detail_response import ContractDetailResponse  # noqa: E501
+from wire4_client.models.contract_detail_response import ContractDetailResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestContractDetailResponse(unittest.TestCase):
     """ContractDetailResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_codi_operation_response_dto.py` & `wire4-client-1.1.3/test/test_codi_operation_response_dto.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.codi_operation_response_dto import CodiOperationResponseDTO  # noqa: E501
+from wire4_client.models.codi_operation_response_dto import CodiOperationResponseDTO  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestCodiOperationResponseDTO(unittest.TestCase):
     """CodiOperationResponseDTO unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_sales_point_request.py` & `wire4-client-1.1.3/test/test_sales_point_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.sales_point_request import SalesPointRequest  # noqa: E501
+from wire4_client.models.sales_point_request import SalesPointRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestSalesPointRequest(unittest.TestCase):
     """SalesPointRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_subscription_change_status_request.py` & `wire4-client-1.1.3/test/test_subscription_change_status_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.subscription_change_status_request import SubscriptionChangeStatusRequest  # noqa: E501
+from wire4_client.models.subscription_change_status_request import SubscriptionChangeStatusRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestSubscriptionChangeStatusRequest(unittest.TestCase):
     """SubscriptionChangeStatusRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_message_sales_point.py` & `wire4-client-1.1.3/test/test_message_sales_point.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_sales_point import MessageSalesPoint  # noqa: E501
+from wire4_client.models.message_sales_point import MessageSalesPoint  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestMessageSalesPoint(unittest.TestCase):
     """MessageSalesPoint unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_message_subscription.py` & `wire4-client-1.1.3/test/test_message_subscription.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_subscription import MessageSubscription  # noqa: E501
+from wire4_client.models.message_subscription import MessageSubscription  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestMessageSubscription(unittest.TestCase):
     """MessageSubscription unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_authorized_beneficiaries_response.py` & `wire4-client-1.1.3/test/test_authorized_beneficiaries_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.authorized_beneficiaries_response import AuthorizedBeneficiariesResponse  # noqa: E501
+from wire4_client.models.authorized_beneficiaries_response import AuthorizedBeneficiariesResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestAuthorizedBeneficiariesResponse(unittest.TestCase):
     """AuthorizedBeneficiariesResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_codi_code_request_dto.py` & `wire4-client-1.1.3/test/test_codi_code_request_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.codi_code_request_dto import CodiCodeRequestDTO  # noqa: E501
+from wire4_client.models.codi_code_request_dto import CodiCodeRequestDTO  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestCodiCodeRequestDTO(unittest.TestCase):
     """CodiCodeRequestDTO unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_payments_request_id.py` & `wire4-client-1.1.3/test/test_payments_request_id.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.payments_request_id import PaymentsRequestId  # noqa: E501
+from wire4_client.models.payments_request_id import PaymentsRequestId  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestPaymentsRequestId(unittest.TestCase):
     """PaymentsRequestId unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_authorization_transaction_group.py` & `wire4-client-1.1.3/test/test_authorization_transaction_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.authorization_transaction_group import AuthorizationTransactionGroup  # noqa: E501
+from wire4_client.models.authorization_transaction_group import AuthorizationTransactionGroup  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestAuthorizationTransactionGroup(unittest.TestCase):
     """AuthorizationTransactionGroup unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_amount_request.py` & `wire4-client-1.1.3/test/test_amount_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.amount_request import AmountRequest  # noqa: E501
+from wire4_client.models.amount_request import AmountRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestAmountRequest(unittest.TestCase):
     """AmountRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_depositants_response.py` & `wire4-client-1.1.3/test/test_depositants_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.depositants_response import DepositantsResponse  # noqa: E501
+from wire4_client.models.depositants_response import DepositantsResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestDepositantsResponse(unittest.TestCase):
     """DepositantsResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_deposits_authorization_response.py` & `wire4-client-1.1.3/test/test_deposits_authorization_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.deposits_authorization_response import DepositsAuthorizationResponse  # noqa: E501
+from wire4_client.models.deposits_authorization_response import DepositsAuthorizationResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestDepositsAuthorizationResponse(unittest.TestCase):
     """DepositsAuthorizationResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_codi_code_qr_response_dto.py` & `wire4-client-1.1.3/test/test_codi_code_qr_response_dto.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.codi_code_qr_response_dto import CodiCodeQrResponseDTO  # noqa: E501
+from wire4_client.models.codi_code_qr_response_dto import CodiCodeQrResponseDTO  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestCodiCodeQrResponseDTO(unittest.TestCase):
     """CodiCodeQrResponseDTO unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_transaction_outgoing.py` & `wire4-client-1.1.3/test/test_transaction_outgoing.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.transaction_outgoing import TransactionOutgoing  # noqa: E501
+from wire4_client.models.transaction_outgoing import TransactionOutgoing  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestTransactionOutgoing(unittest.TestCase):
     """TransactionOutgoing unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_autorizacin_de_depsitos_api.py` & `wire4-client-1.1.3/test/test_autorizacin_de_depsitos_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.autorizacin_de_depsitos_api import AutorizacinDeDepsitosApi  # noqa: E501
+from wire4_client.api.autorizacin_de_depsitos_api import AutorizacinDeDepsitosApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestAutorizacinDeDepsitosApi(unittest.TestCase):
     """AutorizacinDeDepsitosApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.autorizacin_de_depsitos_api.AutorizacinDeDepsitosApi()  # noqa: E501
+        self.api = AutorizacinDeDepsitosApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_deposit_auth_configurations(self):
         """Test case for get_deposit_auth_configurations
```

### Comparing `wire4-client-1.1.2/test/test_message_institution.py` & `wire4-client-1.1.3/test/test_message_institution.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_institution import MessageInstitution  # noqa: E501
+from wire4_client.models.message_institution import MessageInstitution  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestMessageInstitution(unittest.TestCase):
     """MessageInstitution unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_webhook_request.py` & `wire4-client-1.1.3/test/test_webhook.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.webhook_request import WebhookRequest  # noqa: E501
+from wire4_client.models.webhook import Webhook  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestWebhookRequest(unittest.TestCase):
-    """WebhookRequest unit test stubs"""
+class TestWebhook(unittest.TestCase):
+    """Webhook unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWebhookRequest(self):
-        """Test WebhookRequest"""
+    def testWebhook(self):
+        """Test Webhook"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.webhook_request.WebhookRequest()  # noqa: E501
+        # model = wire4_client.models.webhook.Webhook()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_transaction_error_code.py` & `wire4-client-1.1.3/test/test_transaction_error_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.transaction_error_code import TransactionErrorCode  # noqa: E501
+from wire4_client.models.transaction_error_code import TransactionErrorCode  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestTransactionErrorCode(unittest.TestCase):
     """TransactionErrorCode unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_use_service_banking.py` & `wire4-client-1.1.3/test/test_use_service_banking.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.use_service_banking import UseServiceBanking  # noqa: E501
+from wire4_client.models.use_service_banking import UseServiceBanking  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestUseServiceBanking(unittest.TestCase):
     """UseServiceBanking unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_sales_point.py` & `wire4-client-1.1.3/test/test_sales_point_found.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.sales_point import SalesPoint  # noqa: E501
+from wire4_client.models.sales_point_found import SalesPointFound  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestSalesPoint(unittest.TestCase):
-    """SalesPoint unit test stubs"""
+class TestSalesPointFound(unittest.TestCase):
+    """SalesPointFound unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSalesPoint(self):
-        """Test SalesPoint"""
+    def testSalesPointFound(self):
+        """Test SalesPointFound"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.sales_point.SalesPoint()  # noqa: E501
+        # model = wire4_client.models.sales_point_found.SalesPointFound()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_beneficiary_institution.py` & `wire4-client-1.1.3/test/test_beneficiary_institution.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.beneficiary_institution import BeneficiaryInstitution  # noqa: E501
+from wire4_client.models.beneficiary_institution import BeneficiaryInstitution  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestBeneficiaryInstitution(unittest.TestCase):
     """BeneficiaryInstitution unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_authorized_users.py` & `wire4-client-1.1.3/test/test_authorized_users.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.authorized_users import AuthorizedUsers  # noqa: E501
+from wire4_client.models.authorized_users import AuthorizedUsers  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestAuthorizedUsers(unittest.TestCase):
     """AuthorizedUsers unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_payment_request_codi_response_dto.py` & `wire4-client-1.1.3/test/test_payment_request_codi_response_dto.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.payment_request_codi_response_dto import PaymentRequestCodiResponseDTO  # noqa: E501
+from wire4_client.models.payment_request_codi_response_dto import PaymentRequestCodiResponseDTO  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestPaymentRequestCodiResponseDTO(unittest.TestCase):
     """PaymentRequestCodiResponseDTO unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_peticiones_de_pago_por_co_di_api.py` & `wire4-client-1.1.3/test/test_peticiones_de_pago_por_co_di_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.peticiones_de_pago_por_co_di_api import PeticionesDePagoPorCoDiApi  # noqa: E501
+from wire4_client.api.peticiones_de_pago_por_co_di_api import PeticionesDePagoPorCoDiApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestPeticionesDePagoPorCoDiApi(unittest.TestCase):
     """PeticionesDePagoPorCoDiApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.peticiones_de_pago_por_co_di_api.PeticionesDePagoPorCoDiApi()  # noqa: E501
+        self.api = PeticionesDePagoPorCoDiApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_consult_codi_request_by_order_id(self):
         """Test case for consult_codi_request_by_order_id
```

### Comparing `wire4-client-1.1.2/test/test_person.py` & `wire4-client-1.1.3/test/test_payment.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.person import Person  # noqa: E501
+from wire4_client.models.payment import Payment  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestPerson(unittest.TestCase):
-    """Person unit test stubs"""
+class TestPayment(unittest.TestCase):
+    """Payment unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPerson(self):
-        """Test Person"""
+    def testPayment(self):
+        """Test Payment"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.person.Person()  # noqa: E501
+        # model = wire4_client.models.payment.Payment()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_message_cep.py` & `wire4-client-1.1.3/test/test_message_cep.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_cep import MessageCEP  # noqa: E501
+from wire4_client.models.message_cep import MessageCEP  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestMessageCEP(unittest.TestCase):
     """MessageCEP unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_relationships_response.py` & `wire4-client-1.1.3/test/test_relationships_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.relationships_response import RelationshipsResponse  # noqa: E501
+from wire4_client.models.relationships_response import RelationshipsResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestRelationshipsResponse(unittest.TestCase):
     """RelationshipsResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_cep_response.py` & `wire4-client-1.1.3/test/test_webhook_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.cep_response import CepResponse  # noqa: E501
+from wire4_client.models.webhook_response import WebhookResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestCepResponse(unittest.TestCase):
-    """CepResponse unit test stubs"""
+class TestWebhookResponse(unittest.TestCase):
+    """WebhookResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCepResponse(self):
-        """Test CepResponse"""
+    def testWebhookResponse(self):
+        """Test WebhookResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.cep_response.CepResponse()  # noqa: E501
+        # model = wire4_client.models.webhook_response.WebhookResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_depositant.py` & `wire4-client-1.1.3/test/test_depositant.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.depositant import Depositant  # noqa: E501
+from wire4_client.models.depositant import Depositant  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestDepositant(unittest.TestCase):
     """Depositant unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_cuentas_de_beneficiarios_spei_api.py` & `wire4-client-1.1.3/test/test_cuentas_de_beneficiarios_spei_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.cuentas_de_beneficiarios_spei_api import CuentasDeBeneficiariosSPEIApi  # noqa: E501
+from wire4_client.api.cuentas_de_beneficiarios_spei_api import CuentasDeBeneficiariosSPEIApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestCuentasDeBeneficiariosSPEIApi(unittest.TestCase):
     """CuentasDeBeneficiariosSPEIApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.cuentas_de_beneficiarios_spei_api.CuentasDeBeneficiariosSPEIApi()  # noqa: E501
+        self.api = CuentasDeBeneficiariosSPEIApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_authorize_accounts_pending_put(self):
         """Test case for authorize_accounts_pending_put
```

### Comparing `wire4-client-1.1.2/test/test_spid_beneficiary_response.py` & `wire4-client-1.1.3/test/test_spid_beneficiary_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.spid_beneficiary_response import SpidBeneficiaryResponse  # noqa: E501
+from wire4_client.models.spid_beneficiary_response import SpidBeneficiaryResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestSpidBeneficiaryResponse(unittest.TestCase):
     """SpidBeneficiaryResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_company_requested.py` & `wire4-client-1.1.3/test/test_company_requested.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.company_requested import CompanyRequested  # noqa: E501
+from wire4_client.models.company_requested import CompanyRequested  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestCompanyRequested(unittest.TestCase):
     """CompanyRequested unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_account_request.py` & `wire4-client-1.1.3/test/test_account_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.account_request import AccountRequest  # noqa: E501
+from wire4_client.models.account_request import AccountRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestAccountRequest(unittest.TestCase):
     """AccountRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_pre_monex_authorization.py` & `wire4-client-1.1.3/test/test_pre_monex_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.pre_monex_authorization import PreMonexAuthorization  # noqa: E501
+from wire4_client.models.pre_monex_authorization import PreMonexAuthorization  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestPreMonexAuthorization(unittest.TestCase):
     """PreMonexAuthorization unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_webhook_response.py` & `wire4-client-1.1.3/test/test_balance.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.webhook_response import WebhookResponse  # noqa: E501
+from wire4_client.models.balance import Balance  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestWebhookResponse(unittest.TestCase):
-    """WebhookResponse unit test stubs"""
+class TestBalance(unittest.TestCase):
+    """Balance unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWebhookResponse(self):
-        """Test WebhookResponse"""
+    def testBalance(self):
+        """Test Balance"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.webhook_response.WebhookResponse()  # noqa: E501
+        # model = wire4_client.models.balance.Balance()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_cuentas_de_beneficiarios_spid_api.py` & `wire4-client-1.1.3/test/test_cuentas_de_beneficiarios_spid_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.cuentas_de_beneficiarios_spid_api import CuentasDeBeneficiariosSPIDApi  # noqa: E501
+from wire4_client.api.cuentas_de_beneficiarios_spid_api import CuentasDeBeneficiariosSPIDApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestCuentasDeBeneficiariosSPIDApi(unittest.TestCase):
     """CuentasDeBeneficiariosSPIDApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.cuentas_de_beneficiarios_spid_api.CuentasDeBeneficiariosSPIDApi()  # noqa: E501
+        self.api = CuentasDeBeneficiariosSPIDApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_spid_beneficiaries_for_account(self):
         """Test case for get_spid_beneficiaries_for_account
```

### Comparing `wire4-client-1.1.2/test/test_sales_point_respose.py` & `wire4-client-1.1.3/test/test_payment_codi.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.sales_point_respose import SalesPointRespose  # noqa: E501
+from wire4_client.models.payment_codi import PaymentCODI  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestSalesPointRespose(unittest.TestCase):
-    """SalesPointRespose unit test stubs"""
+class TestPaymentCODI(unittest.TestCase):
+    """PaymentCODI unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSalesPointRespose(self):
-        """Test SalesPointRespose"""
+    def testPaymentCODI(self):
+        """Test PaymentCODI"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.sales_point_respose.SalesPointRespose()  # noqa: E501
+        # model = wire4_client.models.payment_codi.PaymentCODI()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_item.py` & `wire4-client-1.1.3/test/test_account_reassigned.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.item import Item  # noqa: E501
+from wire4_client.models.account_reassigned import AccountReassigned  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestItem(unittest.TestCase):
-    """Item unit test stubs"""
+class TestAccountReassigned(unittest.TestCase):
+    """AccountReassigned unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testItem(self):
-        """Test Item"""
+    def testAccountReassigned(self):
+        """Test AccountReassigned"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.item.Item()  # noqa: E501
+        # model = wire4_client.models.account_reassigned.AccountReassigned()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_message_web_hook.py` & `wire4-client-1.1.3/test/test_message_web_hook.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_web_hook import MessageWebHook  # noqa: E501
+from wire4_client.models.message_web_hook import MessageWebHook  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestMessageWebHook(unittest.TestCase):
     """MessageWebHook unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_saldo_api.py` & `wire4-client-1.1.3/test/test_product.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,30 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.saldo_api import SaldoApi  # noqa: E501
+from wire4_client.models.product import Product  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestSaldoApi(unittest.TestCase):
-    """SaldoApi unit test stubs"""
+class TestProduct(unittest.TestCase):
+    """Product unit test stubs"""
 
     def setUp(self):
-        self.api = api.saldo_api.SaldoApi()  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    def test_get_balance_using_get(self):
-        """Test case for get_balance_using_get
-
-        Consulta los saldo de una cuenta  # noqa: E501
-        """
+    def testProduct(self):
+        """Test Product"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = wire4_client.models.product.Product()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_balance.py` & `wire4-client-1.1.3/test/test_cep_search_banxico.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.balance import Balance  # noqa: E501
+from wire4_client.models.cep_search_banxico import CepSearchBanxico  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestBalance(unittest.TestCase):
-    """Balance unit test stubs"""
+class TestCepSearchBanxico(unittest.TestCase):
+    """CepSearchBanxico unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBalance(self):
-        """Test Balance"""
+    def testCepSearchBanxico(self):
+        """Test CepSearchBanxico"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.balance.Balance()  # noqa: E501
+        # model = wire4_client.models.cep_search_banxico.CepSearchBanxico()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_payment_codi.py` & `wire4-client-1.1.3/test/test_recurring_charge_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.payment_codi import PaymentCODI  # noqa: E501
+from wire4_client.models.recurring_charge_request import RecurringChargeRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestPaymentCODI(unittest.TestCase):
-    """PaymentCODI unit test stubs"""
+class TestRecurringChargeRequest(unittest.TestCase):
+    """RecurringChargeRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaymentCODI(self):
-        """Test PaymentCODI"""
+    def testRecurringChargeRequest(self):
+        """Test RecurringChargeRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.payment_codi.PaymentCODI()  # noqa: E501
+        # model = wire4_client.models.recurring_charge_request.RecurringChargeRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_configurations_limits.py` & `wire4-client-1.1.3/test/test_configurations_limits.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.configurations_limits import ConfigurationsLimits  # noqa: E501
+from wire4_client.models.configurations_limits import ConfigurationsLimits  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestConfigurationsLimits(unittest.TestCase):
     """ConfigurationsLimits unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_payment.py` & `wire4-client-1.1.3/test/test_institutions_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.payment import Payment  # noqa: E501
+from wire4_client.models.institutions_list import InstitutionsList  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestPayment(unittest.TestCase):
-    """Payment unit test stubs"""
+class TestInstitutionsList(unittest.TestCase):
+    """InstitutionsList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPayment(self):
-        """Test Payment"""
+    def testInstitutionsList(self):
+        """Test InstitutionsList"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.payment.Payment()  # noqa: E501
+        # model = wire4_client.models.institutions_list.InstitutionsList()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_message_deposit_received.py` & `wire4-client-1.1.3/test/test_message_codi_action.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_deposit_received import MessageDepositReceived  # noqa: E501
+from wire4_client.models.message_codi_action import MessageCodiAction  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestMessageDepositReceived(unittest.TestCase):
-    """MessageDepositReceived unit test stubs"""
+class TestMessageCodiAction(unittest.TestCase):
+    """MessageCodiAction unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMessageDepositReceived(self):
-        """Test MessageDepositReceived"""
+    def testMessageCodiAction(self):
+        """Test MessageCodiAction"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.message_deposit_received.MessageDepositReceived()  # noqa: E501
+        # model = wire4_client.models.message_codi_action.MessageCodiAction()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_message_codi_action.py` & `wire4-client-1.1.3/test/test_message_configurations_limits.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_codi_action import MessageCodiAction  # noqa: E501
+from wire4_client.models.message_configurations_limits import MessageConfigurationsLimits  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestMessageCodiAction(unittest.TestCase):
-    """MessageCodiAction unit test stubs"""
+class TestMessageConfigurationsLimits(unittest.TestCase):
+    """MessageConfigurationsLimits unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMessageCodiAction(self):
-        """Test MessageCodiAction"""
+    def testMessageConfigurationsLimits(self):
+        """Test MessageConfigurationsLimits"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.message_codi_action.MessageCodiAction()  # noqa: E501
+        # model = wire4_client.models.message_configurations_limits.MessageConfigurationsLimits()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_institutions_list.py` & `wire4-client-1.1.3/test/test_beneficiaries_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.institutions_list import InstitutionsList  # noqa: E501
+from wire4_client.models.beneficiaries_response import BeneficiariesResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestInstitutionsList(unittest.TestCase):
-    """InstitutionsList unit test stubs"""
+class TestBeneficiariesResponse(unittest.TestCase):
+    """BeneficiariesResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testInstitutionsList(self):
-        """Test InstitutionsList"""
+    def testBeneficiariesResponse(self):
+        """Test BeneficiariesResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.institutions_list.InstitutionsList()  # noqa: E501
+        # model = wire4_client.models.beneficiaries_response.BeneficiariesResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_message_user_authorized.py` & `wire4-client-1.1.3/test/test_message_user_authorized.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_user_authorized import MessageUserAuthorized  # noqa: E501
+from wire4_client.models.message_user_authorized import MessageUserAuthorized  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestMessageUserAuthorized(unittest.TestCase):
     """MessageUserAuthorized unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_balance_list_response.py` & `wire4-client-1.1.3/test/test_balance_list_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.balance_list_response import BalanceListResponse  # noqa: E501
+from wire4_client.models.balance_list_response import BalanceListResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestBalanceListResponse(unittest.TestCase):
     """BalanceListResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_depositants_register.py` & `wire4-client-1.1.3/test/test_transactions_outgoing_register.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.depositants_register import DepositantsRegister  # noqa: E501
+from wire4_client.models.transactions_outgoing_register import TransactionsOutgoingRegister  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestDepositantsRegister(unittest.TestCase):
-    """DepositantsRegister unit test stubs"""
+class TestTransactionsOutgoingRegister(unittest.TestCase):
+    """TransactionsOutgoingRegister unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDepositantsRegister(self):
-        """Test DepositantsRegister"""
+    def testTransactionsOutgoingRegister(self):
+        """Test TransactionsOutgoingRegister"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.depositants_register.DepositantsRegister()  # noqa: E501
+        # model = wire4_client.models.transactions_outgoing_register.TransactionsOutgoingRegister()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_codi_operations_filters_request_dto.py` & `wire4-client-1.1.3/test/test_codi_operations_filters_request_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.codi_operations_filters_request_dto import CodiOperationsFiltersRequestDTO  # noqa: E501
+from wire4_client.models.codi_operations_filters_request_dto import CodiOperationsFiltersRequestDTO  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestCodiOperationsFiltersRequestDTO(unittest.TestCase):
     """CodiOperationsFiltersRequestDTO unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_web_hook_deposit_authorization_request.py` & `wire4-client-1.1.3/test/test_web_hook_deposit_authorization_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.web_hook_deposit_authorization_request import WebHookDepositAuthorizationRequest  # noqa: E501
+from wire4_client.models.web_hook_deposit_authorization_request import WebHookDepositAuthorizationRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestWebHookDepositAuthorizationRequest(unittest.TestCase):
     """WebHookDepositAuthorizationRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_account_reassigned.py` & `wire4-client-1.1.3/test/test_message_deposit_received.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.account_reassigned import AccountReassigned  # noqa: E501
+from wire4_client.models.message_deposit_received import MessageDepositReceived  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestAccountReassigned(unittest.TestCase):
-    """AccountReassigned unit test stubs"""
+class TestMessageDepositReceived(unittest.TestCase):
+    """MessageDepositReceived unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAccountReassigned(self):
-        """Test AccountReassigned"""
+    def testMessageDepositReceived(self):
+        """Test MessageDepositReceived"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.account_reassigned.AccountReassigned()  # noqa: E501
+        # model = wire4_client.models.message_deposit_received.MessageDepositReceived()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_account.py` & `wire4-client-1.1.3/test/test_message_payment_state_pending.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.account import Account  # noqa: E501
+from wire4_client.models.message_payment_state_pending import MessagePaymentStatePending  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestAccount(unittest.TestCase):
-    """Account unit test stubs"""
+class TestMessagePaymentStatePending(unittest.TestCase):
+    """MessagePaymentStatePending unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAccount(self):
-        """Test Account"""
+    def testMessagePaymentStatePending(self):
+        """Test MessagePaymentStatePending"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.account.Account()  # noqa: E501
+        # model = wire4_client.models.message_payment_state_pending.MessagePaymentStatePending()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_contracts_details_api.py` & `wire4-client-1.1.3/test/test_contracts_details_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.contracts_details_api import ContractsDetailsApi  # noqa: E501
+from wire4_client.api.contracts_details_api import ContractsDetailsApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestContractsDetailsApi(unittest.TestCase):
     """ContractsDetailsApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.contracts_details_api.ContractsDetailsApi()  # noqa: E501
+        self.api = ContractsDetailsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_create_authorization(self):
         """Test case for create_authorization
```

### Comparing `wire4-client-1.1.2/test/test_detailed_error_response.py` & `wire4-client-1.1.3/test/test_detailed_error_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.detailed_error_response import DetailedErrorResponse  # noqa: E501
+from wire4_client.models.detailed_error_response import DetailedErrorResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestDetailedErrorResponse(unittest.TestCase):
     """DetailedErrorResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_message_configurations_limits.py` & `wire4-client-1.1.3/test/test_update_configurations_request_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.message_configurations_limits import MessageConfigurationsLimits  # noqa: E501
+from wire4_client.models.update_configurations_request_dto import UpdateConfigurationsRequestDTO  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestMessageConfigurationsLimits(unittest.TestCase):
-    """MessageConfigurationsLimits unit test stubs"""
+class TestUpdateConfigurationsRequestDTO(unittest.TestCase):
+    """UpdateConfigurationsRequestDTO unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMessageConfigurationsLimits(self):
-        """Test MessageConfigurationsLimits"""
+    def testUpdateConfigurationsRequestDTO(self):
+        """Test UpdateConfigurationsRequestDTO"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.message_configurations_limits.MessageConfigurationsLimits()  # noqa: E501
+        # model = wire4_client.models.update_configurations_request_dto.UpdateConfigurationsRequestDTO()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_depositant_count_response.py` & `wire4-client-1.1.3/test/test_depositant_count_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.depositant_count_response import DepositantCountResponse  # noqa: E501
+from wire4_client.models.depositant_count_response import DepositantCountResponse  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestDepositantCountResponse(unittest.TestCase):
     """DepositantCountResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_relationship.py` & `wire4-client-1.1.3/test/test_relationship.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.relationship import Relationship  # noqa: E501
+from wire4_client.models.relationship import Relationship  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestRelationship(unittest.TestCase):
     """Relationship unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_transaction_outgoing_spid.py` & `wire4-client-1.1.3/test/test_transaction_outgoing_spid.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.transaction_outgoing_spid import TransactionOutgoingSpid  # noqa: E501
+from wire4_client.models.transaction_outgoing_spid import TransactionOutgoingSpid  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestTransactionOutgoingSpid(unittest.TestCase):
     """TransactionOutgoingSpid unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_spid_classifications_response_dto.py` & `wire4-client-1.1.3/test/test_spid_classifications_response_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.spid_classifications_response_dto import SpidClassificationsResponseDTO  # noqa: E501
+from wire4_client.models.spid_classifications_response_dto import SpidClassificationsResponseDTO  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestSpidClassificationsResponseDTO(unittest.TestCase):
     """SpidClassificationsResponseDTO unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_lmites_de_montos_api.py` & `wire4-client-1.1.3/test/test_lmites_de_montos_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from api.lmites_de_montos_api import LmitesDeMontosApi  # noqa: E501
+from wire4_client.api.lmites_de_montos_api import LmitesDeMontosApi  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestLmitesDeMontosApi(unittest.TestCase):
     """LmitesDeMontosApi unit test stubs"""
 
     def setUp(self):
-        self.api = api.lmites_de_montos_api.LmitesDeMontosApi()  # noqa: E501
+        self.api = LmitesDeMontosApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_obtain_configurations_limits(self):
         """Test case for obtain_configurations_limits
```

### Comparing `wire4-client-1.1.2/test/test_beneficiaries_response.py` & `wire4-client-1.1.3/test/test_sales_point_respose.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.beneficiaries_response import BeneficiariesResponse  # noqa: E501
+from wire4_client.models.sales_point_respose import SalesPointRespose  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestBeneficiariesResponse(unittest.TestCase):
-    """BeneficiariesResponse unit test stubs"""
+class TestSalesPointRespose(unittest.TestCase):
+    """SalesPointRespose unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBeneficiariesResponse(self):
-        """Test BeneficiariesResponse"""
+    def testSalesPointRespose(self):
+        """Test SalesPointRespose"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.beneficiaries_response.BeneficiariesResponse()  # noqa: E501
+        # model = wire4_client.models.sales_point_respose.SalesPointRespose()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_update_configurations_request_dto.py` & `wire4-client-1.1.3/test/test_beneficiary_dto.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.update_configurations_request_dto import UpdateConfigurationsRequestDTO  # noqa: E501
+from wire4_client.models.beneficiary_dto import BeneficiaryDTO  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestUpdateConfigurationsRequestDTO(unittest.TestCase):
-    """UpdateConfigurationsRequestDTO unit test stubs"""
+class TestBeneficiaryDTO(unittest.TestCase):
+    """BeneficiaryDTO unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUpdateConfigurationsRequestDTO(self):
-        """Test UpdateConfigurationsRequestDTO"""
+    def testBeneficiaryDTO(self):
+        """Test BeneficiaryDTO"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.update_configurations_request_dto.UpdateConfigurationsRequestDTO()  # noqa: E501
+        # model = wire4_client.models.beneficiary_dto.BeneficiaryDTO()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_transactions_outgoing_register.py` & `wire4-client-1.1.3/test/test_payments_spei_and_spid_order_id.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.transactions_outgoing_register import TransactionsOutgoingRegister  # noqa: E501
+from wire4_client.models.payments_spei_and_spid_order_id import PaymentsSpeiAndSpidOrderId  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestTransactionsOutgoingRegister(unittest.TestCase):
-    """TransactionsOutgoingRegister unit test stubs"""
+class TestPaymentsSpeiAndSpidOrderId(unittest.TestCase):
+    """PaymentsSpeiAndSpidOrderId unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTransactionsOutgoingRegister(self):
-        """Test TransactionsOutgoingRegister"""
+    def testPaymentsSpeiAndSpidOrderId(self):
+        """Test PaymentsSpeiAndSpidOrderId"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.transactions_outgoing_register.TransactionsOutgoingRegister()  # noqa: E501
+        # model = wire4_client.models.payments_spei_and_spid_order_id.PaymentsSpeiAndSpidOrderId()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_sales_point_found.py` & `wire4-client-1.1.3/test/test_sales_point.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.sales_point_found import SalesPointFound  # noqa: E501
+from wire4_client.models.sales_point import SalesPoint  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestSalesPointFound(unittest.TestCase):
-    """SalesPointFound unit test stubs"""
+class TestSalesPoint(unittest.TestCase):
+    """SalesPoint unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSalesPointFound(self):
-        """Test SalesPointFound"""
+    def testSalesPoint(self):
+        """Test SalesPoint"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.sales_point_found.SalesPointFound()  # noqa: E501
+        # model = wire4_client.models.sales_point.SalesPoint()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_cep_search_banxico.py` & `wire4-client-1.1.3/test/test_payments_spei_and_spid_request_id.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.cep_search_banxico import CepSearchBanxico  # noqa: E501
+from wire4_client.models.payments_spei_and_spid_request_id import PaymentsSpeiAndSpidRequestId  # noqa: E501
 from wire4_client.rest import ApiException
 
 
-class TestCepSearchBanxico(unittest.TestCase):
-    """CepSearchBanxico unit test stubs"""
+class TestPaymentsSpeiAndSpidRequestId(unittest.TestCase):
+    """PaymentsSpeiAndSpidRequestId unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCepSearchBanxico(self):
-        """Test CepSearchBanxico"""
+    def testPaymentsSpeiAndSpidRequestId(self):
+        """Test PaymentsSpeiAndSpidRequestId"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = wire4_client.models.cep_search_banxico.CepSearchBanxico()  # noqa: E501
+        # model = wire4_client.models.payments_spei_and_spid_request_id.PaymentsSpeiAndSpidRequestId()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `wire4-client-1.1.2/test/test_deposit_authorization_request.py` & `wire4-client-1.1.3/test/test_deposit_authorization_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.deposit_authorization_request import DepositAuthorizationRequest  # noqa: E501
+from wire4_client.models.deposit_authorization_request import DepositAuthorizationRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestDepositAuthorizationRequest(unittest.TestCase):
     """DepositAuthorizationRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/test/test_contract_detail_request.py` & `wire4-client-1.1.3/test/test_contract_detail_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import wire4_client
-from models.contract_detail_request import ContractDetailRequest  # noqa: E501
+from wire4_client.models.contract_detail_request import ContractDetailRequest  # noqa: E501
 from wire4_client.rest import ApiException
 
 
 class TestContractDetailRequest(unittest.TestCase):
     """ContractDetailRequest unit test stubs"""
 
     def setUp(self):
```

### Comparing `wire4-client-1.1.2/README.md` & `wire4-client-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # wire4-client
 Referencia de la API de Wire4
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1.0.0
-- Package version: 1.1.2
+- Package version: 1.1.3
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -81,14 +81,16 @@
 
 All URIs are relative to *https://sandbox-api.wire4.mx/wire4/1.0.0*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AutorizacinDeDepsitosApi* | [**get_deposit_auth_configurations**](docs/AutorizacinDeDepsitosApi.md#get_deposit_auth_configurations) | **GET** /subscriptions/{subscription}/configurations/deposit-authorization | Consulta autorización de depósitos
 *AutorizacinDeDepsitosApi* | [**put_deposit_auth_configurations**](docs/AutorizacinDeDepsitosApi.md#put_deposit_auth_configurations) | **PUT** /subscriptions/{subscription}/configurations/deposit-authorization | Habilita / Deshabilita la autorización de depósitos
+*CargosRecurrentesApi* | [**delete_recurring_charge_using_delete**](docs/CargosRecurrentesApi.md#delete_recurring_charge_using_delete) | **DELETE** /recurring-charge/{orderId} | Cancelación/desubscripción de cargos recurrentes
+*CargosRecurrentesApi* | [**register_recurring_charge_using_post**](docs/CargosRecurrentesApi.md#register_recurring_charge_using_post) | **POST** /recurring-charge | Registro de cargos recurrentes
 *ComprobanteElectrnicoDePagoCEPApi* | [**obtain_transaction_cep_using_post**](docs/ComprobanteElectrnicoDePagoCEPApi.md#obtain_transaction_cep_using_post) | **POST** /ceps | Consulta de CEP
 *ContactoApi* | [**send_contact_using_post**](docs/ContactoApi.md#send_contact_using_post) | **POST** /contact | Solicitud de contacto
 *ContractsDetailsApi* | [**create_authorization**](docs/ContractsDetailsApi.md#create_authorization) | **POST** /onboarding/accounts/authorize | Devuelve la URL para autorización del usuario Monex
 *ContractsDetailsApi* | [**obtain_authorized_users**](docs/ContractsDetailsApi.md#obtain_authorized_users) | **GET** /onboarding/accounts/{requestId}/authorized-users | Obtiene los usuarios autorizados
 *ContractsDetailsApi* | [**obtain_authorized_users_by_contract**](docs/ContractsDetailsApi.md#obtain_authorized_users_by_contract) | **GET** /onboarding/accounts/authorized-users | Obtiene los usuarios autorizados por contrato
 *ContractsDetailsApi* | [**obtain_contract_details**](docs/ContractsDetailsApi.md#obtain_contract_details) | **POST** /onboarding/accounts/details | Obtiene los detalles de la empresa del contrato
 *CuentasDeBeneficiariosSPEIApi* | [**authorize_accounts_pending_put**](docs/CuentasDeBeneficiariosSPEIApi.md#authorize_accounts_pending_put) | **PUT** /subscriptions/{subscription}/beneficiaries/pending | Solicitud para agrupar cuentas de beneficiarios SPEI/SPID en estado pendiente.
@@ -97,14 +99,15 @@
 *CuentasDeBeneficiariosSPEIApi* | [**get_beneficiaries_by_request_id**](docs/CuentasDeBeneficiariosSPEIApi.md#get_beneficiaries_by_request_id) | **GET** /subscriptions/{subscription}/beneficiaries/spei/{requestId} | Consulta los beneficiarios por el identificador de la petición de registro
 *CuentasDeBeneficiariosSPEIApi* | [**get_beneficiaries_for_account_using_get**](docs/CuentasDeBeneficiariosSPEIApi.md#get_beneficiaries_for_account_using_get) | **GET** /subscriptions/{subscription}/beneficiaries/spei | Consulta los beneficiarios registrados
 *CuentasDeBeneficiariosSPEIApi* | [**pre_register_accounts_using_post**](docs/CuentasDeBeneficiariosSPEIApi.md#pre_register_accounts_using_post) | **POST** /subscriptions/{subscription}/beneficiaries/spei | Pre-registro de cuentas de beneficiarios SPEI®.
 *CuentasDeBeneficiariosSPEIApi* | [**remove_beneficiaries_pending_using_delete**](docs/CuentasDeBeneficiariosSPEIApi.md#remove_beneficiaries_pending_using_delete) | **DELETE** /subscriptions/{subscription}/beneficiaries/spei/request/{requestId} | Eliminación de beneficiarios SPEI® sin confirmar
 *CuentasDeBeneficiariosSPEIApi* | [**update_amount_limit_account_using_put**](docs/CuentasDeBeneficiariosSPEIApi.md#update_amount_limit_account_using_put) | **PUT** /subscriptions/{subscription}/beneficiaries/spei/{account} | Solicitud para actualizar el monto límite de una cuenta
 *CuentasDeBeneficiariosSPIDApi* | [**get_spid_beneficiaries_for_account**](docs/CuentasDeBeneficiariosSPIDApi.md#get_spid_beneficiaries_for_account) | **GET** /subscriptions/{subscription}/beneficiaries/spid | Consulta los beneficiarios SPID registrados
 *CuentasDeBeneficiariosSPIDApi* | [**pre_register_accounts_using_post1**](docs/CuentasDeBeneficiariosSPIDApi.md#pre_register_accounts_using_post1) | **POST** /subscriptions/{subscription}/beneficiaries/spid | Pre-registro de cuentas de beneficiarios SPID®
+*DepositantesApi* | [**get_depositants_totals_using_get**](docs/DepositantesApi.md#get_depositants_totals_using_get) | **GET** /subscriptions/{subscription}/depositants/count | Número de depositantes por suscripción
 *DepositantesApi* | [**get_depositants_using_get**](docs/DepositantesApi.md#get_depositants_using_get) | **GET** /subscriptions/{subscription}/depositants | Consulta de cuentas de depositantes
 *DepositantesApi* | [**register_depositants_using_post**](docs/DepositantesApi.md#register_depositants_using_post) | **POST** /subscriptions/{subscription}/depositants | Registra un nuevo depositante
 *EmpresasCoDiApi* | [**obtain_companies**](docs/EmpresasCoDiApi.md#obtain_companies) | **GET** /codi/companies | Consulta de empresas CODI®
 *EmpresasCoDiApi* | [**register_company_using_post**](docs/EmpresasCoDiApi.md#register_company_using_post) | **POST** /codi/companies | Registro de empresas CODI®
 *FacturasApi* | [**billings_report_by_id_using_get**](docs/FacturasApi.md#billings_report_by_id_using_get) | **GET** /billings/{id} | Consulta de facturas por identificador
 *FacturasApi* | [**billings_report_using_get**](docs/FacturasApi.md#billings_report_using_get) | **GET** /billings | Consulta de facturas
 *InstitucionesApi* | [**get_all_institutions_using_get**](docs/InstitucionesApi.md#get_all_institutions_using_get) | **GET** /institutions | Consulta de instituciones bancarias
@@ -121,16 +124,19 @@
 *SuscripcionesApi* | [**pre_enrollment_monex_user_using_post**](docs/SuscripcionesApi.md#pre_enrollment_monex_user_using_post) | **POST** /subscriptions/pre-subscription | Pre-registro de una suscripción
 *SuscripcionesApi* | [**remove_enrollment_user_using_delete**](docs/SuscripcionesApi.md#remove_enrollment_user_using_delete) | **DELETE** /subscriptions/{subscription} | Elimina suscripción por su identificador.
 *SuscripcionesApi* | [**remove_subscription_pending_status_using_delete**](docs/SuscripcionesApi.md#remove_subscription_pending_status_using_delete) | **DELETE** /subscriptions/pre-subscription/{subscription} | Elimina pre-registro de suscripción
 *TransferenciasSPEIApi* | [**create_authorization_transactions_group**](docs/TransferenciasSPEIApi.md#create_authorization_transactions_group) | **POST** /subscriptions/{subscription}/transactions/group | Agrupa transacciones bajo un request_id 
 *TransferenciasSPEIApi* | [**drop_transactions_pending_using_delete**](docs/TransferenciasSPEIApi.md#drop_transactions_pending_using_delete) | **DELETE** /subscriptions/{subscription}/transactions/outcoming/spei/request/{requestId} | Eliminación de transferencias SPEI® pendientes
 *TransferenciasSPEIApi* | [**incoming_spei_transactions_report_using_get**](docs/TransferenciasSPEIApi.md#incoming_spei_transactions_report_using_get) | **GET** /subscriptions/{subscription}/transactions/incoming/spei | Consulta de transferencias recibidas
 *TransferenciasSPEIApi* | [**out_comming_spei_request_id_transactions_report_using_get**](docs/TransferenciasSPEIApi.md#out_comming_spei_request_id_transactions_report_using_get) | **GET** /subscriptions/{subscription}/transactions/outcoming/spei/{requestId} | Consulta de transferencias de salida por identificador de petición
+*TransferenciasSPEIApi* | [**out_comming_spei_spid_order_id_transaction_report_using_get**](docs/TransferenciasSPEIApi.md#out_comming_spei_spid_order_id_transaction_report_using_get) | **GET** /subscriptions/{subscription}/transactions/outcoming | Consulta de transferencias realizadas por order_id
+*TransferenciasSPEIApi* | [**out_comming_spei_spid_request_id_transactions_report_using_get**](docs/TransferenciasSPEIApi.md#out_comming_spei_spid_request_id_transactions_report_using_get) | **GET** /subscriptions/{subscription}/transactions/outcoming/{requestId} | Consulta de transferencias de salida por identificador de petición
 *TransferenciasSPEIApi* | [**outgoing_spei_transactions_report_using_get**](docs/TransferenciasSPEIApi.md#outgoing_spei_transactions_report_using_get) | **GET** /subscriptions/{subscription}/transactions/outcoming/spei | Consulta de transferencias realizadas
 *TransferenciasSPEIApi* | [**register_outgoing_spei_transaction_using_post**](docs/TransferenciasSPEIApi.md#register_outgoing_spei_transaction_using_post) | **POST** /subscriptions/{subscription}/transactions/outcoming/spei | Registro de transferencias
+*TransferenciasSPEIApi* | [**register_spei_spid_outgoing_transactions_using_post**](docs/TransferenciasSPEIApi.md#register_spei_spid_outgoing_transactions_using_post) | **POST** /subscriptions/{subscription}/transactions/outcoming | Registro de transferencias SPEI y SPID
 *TransferenciasSPIDApi* | [**get_spid_classifications_using_get**](docs/TransferenciasSPIDApi.md#get_spid_classifications_using_get) | **GET** /subscriptions/{subscription}/beneficiaries/spid/classifications | Consulta de clasificaciones para operaciones SPID®
 *TransferenciasSPIDApi* | [**register_outgoing_spid_transaction_using_post**](docs/TransferenciasSPIDApi.md#register_outgoing_spid_transaction_using_post) | **POST** /subscriptions/{subscription}/transactions/outcoming/spid | Registro de transferencias SPID®
 *WebhooksApi* | [**get_webhook**](docs/WebhooksApi.md#get_webhook) | **GET** /webhooks/{webhook_id} | Consulta de Webhook
 *WebhooksApi* | [**get_webhooks**](docs/WebhooksApi.md#get_webhooks) | **GET** /webhooks | Consulta la lista de Webhooks
 *WebhooksApi* | [**register_webhook**](docs/WebhooksApi.md#register_webhook) | **POST** /webhooks | Alta de Webhook
 
 ## Documentation For Models
@@ -146,34 +152,38 @@
  - [AuthorizationTransactionGroup](docs/AuthorizationTransactionGroup.md)
  - [AuthorizedBeneficiariesResponse](docs/AuthorizedBeneficiariesResponse.md)
  - [AuthorizedUsers](docs/AuthorizedUsers.md)
  - [Balance](docs/Balance.md)
  - [BalanceListResponse](docs/BalanceListResponse.md)
  - [BeneficiariesQueryRegisterStatus](docs/BeneficiariesQueryRegisterStatus.md)
  - [BeneficiariesResponse](docs/BeneficiariesResponse.md)
+ - [BeneficiaryDTO](docs/BeneficiaryDTO.md)
  - [BeneficiaryInstitution](docs/BeneficiaryInstitution.md)
  - [Billing](docs/Billing.md)
  - [BillingTransaction](docs/BillingTransaction.md)
  - [CepResponse](docs/CepResponse.md)
  - [CepSearchBanxico](docs/CepSearchBanxico.md)
  - [CertificateRequest](docs/CertificateRequest.md)
  - [CodiCodeQrResponseDTO](docs/CodiCodeQrResponseDTO.md)
  - [CodiCodeRequestDTO](docs/CodiCodeRequestDTO.md)
  - [CodiOperationResponseDTO](docs/CodiOperationResponseDTO.md)
  - [CodiOperationsFiltersRequestDTO](docs/CodiOperationsFiltersRequestDTO.md)
  - [CompanyRegistered](docs/CompanyRegistered.md)
  - [CompanyRequested](docs/CompanyRequested.md)
  - [Compay](docs/Compay.md)
  - [ConfigurationsLimits](docs/ConfigurationsLimits.md)
+ - [ConfirmRecurringCharge](docs/ConfirmRecurringCharge.md)
  - [ContactRequest](docs/ContactRequest.md)
  - [ContractDetailRequest](docs/ContractDetailRequest.md)
  - [ContractDetailResponse](docs/ContractDetailResponse.md)
+ - [Customer](docs/Customer.md)
  - [Deposit](docs/Deposit.md)
  - [DepositAuthorizationRequest](docs/DepositAuthorizationRequest.md)
  - [Depositant](docs/Depositant.md)
+ - [DepositantCountResponse](docs/DepositantCountResponse.md)
  - [DepositantsRegister](docs/DepositantsRegister.md)
  - [DepositantsResponse](docs/DepositantsResponse.md)
  - [DepositsAuthorizationResponse](docs/DepositsAuthorizationResponse.md)
  - [DetailedErrorResponse](docs/DetailedErrorResponse.md)
  - [ErrorResponse](docs/ErrorResponse.md)
  - [GetDepositants](docs/GetDepositants.md)
  - [Institution](docs/Institution.md)
@@ -195,18 +205,22 @@
  - [MessageWebHook](docs/MessageWebHook.md)
  - [Operations](docs/Operations.md)
  - [PagerResponseDto](docs/PagerResponseDto.md)
  - [Payment](docs/Payment.md)
  - [PaymentCODI](docs/PaymentCODI.md)
  - [PaymentRequestCodiResponseDTO](docs/PaymentRequestCodiResponseDTO.md)
  - [PaymentsRequestId](docs/PaymentsRequestId.md)
+ - [PaymentsSpeiAndSpidOrderId](docs/PaymentsSpeiAndSpidOrderId.md)
+ - [PaymentsSpeiAndSpidRequestId](docs/PaymentsSpeiAndSpidRequestId.md)
  - [Person](docs/Person.md)
  - [PreEnrollmentData](docs/PreEnrollmentData.md)
  - [PreEnrollmentResponse](docs/PreEnrollmentResponse.md)
  - [PreMonexAuthorization](docs/PreMonexAuthorization.md)
+ - [Product](docs/Product.md)
+ - [RecurringChargeRequest](docs/RecurringChargeRequest.md)
  - [Relationship](docs/Relationship.md)
  - [RelationshipsResponse](docs/RelationshipsResponse.md)
  - [SalesPoint](docs/SalesPoint.md)
  - [SalesPointFound](docs/SalesPointFound.md)
  - [SalesPointRequest](docs/SalesPointRequest.md)
  - [SalesPointRespose](docs/SalesPointRespose.md)
  - [ServiceBanking](docs/ServiceBanking.md)
@@ -215,15 +229,17 @@
  - [SpidClassificationDTO](docs/SpidClassificationDTO.md)
  - [SpidClassificationsResponseDTO](docs/SpidClassificationsResponseDTO.md)
  - [SubscriptionChangeStatusRequest](docs/SubscriptionChangeStatusRequest.md)
  - [TokenRequiredResponse](docs/TokenRequiredResponse.md)
  - [TransactionErrorCode](docs/TransactionErrorCode.md)
  - [TransactionOutgoing](docs/TransactionOutgoing.md)
  - [TransactionOutgoingSpid](docs/TransactionOutgoingSpid.md)
+ - [TransactionSpeiSpid](docs/TransactionSpeiSpid.md)
  - [TransactionsOutgoingRegister](docs/TransactionsOutgoingRegister.md)
+ - [TransactionsRegister](docs/TransactionsRegister.md)
  - [UpdateConfigurationsRequestDTO](docs/UpdateConfigurationsRequestDTO.md)
  - [UrlsRedirect](docs/UrlsRedirect.md)
  - [UseServiceBanking](docs/UseServiceBanking.md)
  - [UserCompany](docs/UserCompany.md)
  - [WebHookDepositAuthorizationRequest](docs/WebHookDepositAuthorizationRequest.md)
  - [WebHookDepositAuthorizationResponse](docs/WebHookDepositAuthorizationResponse.md)
  - [Webhook](docs/Webhook.md)
```

### Comparing `wire4-client-1.1.2/setup.py` & `wire4-client-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wire4-client"
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `wire4-client-1.1.2/wire4_client/configuration.py` & `wire4-client-1.1.3/wire4_client/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
         self.api_key_prefix = {}
+        # function to refresh API key if expired
+        self.refresh_api_key_hook = None
         # Username for HTTP basic authentication
         self.username = ""
         # Password for HTTP basic authentication
         self.password = ""
         # Logging Settings
         self.logger = {}
         self.logger["package_logger"] = logging.getLogger("wire4_client")
@@ -197,19 +199,24 @@
 
     def get_api_key_with_prefix(self, identifier):
         """Gets API key (with prefix if set).
 
         :param identifier: The identifier of apiKey.
         :return: The token for api key authentication.
         """
-        if (self.api_key.get(identifier) and
-                self.api_key_prefix.get(identifier)):
-            return self.api_key_prefix[identifier] + ' ' + self.api_key[identifier]  # noqa: E501
-        elif self.api_key.get(identifier):
-            return self.api_key[identifier]
+        if self.refresh_api_key_hook:
+            self.refresh_api_key_hook(self)
+
+        key = self.api_key.get(identifier)
+        if key:
+            prefix = self.api_key_prefix.get(identifier)
+            if prefix:
+                return "%s %s" % (prefix, key)
+            else:
+                return key
 
     def get_basic_auth_token(self):
         """Gets HTTP basic authentication header (string).
 
         :return: The token for basic HTTP authentication.
         """
         return urllib3.util.make_headers(
```

### Comparing `wire4-client-1.1.2/wire4_client/rest.py` & `wire4-client-1.1.3/wire4_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
                 if query_params:
                     url += '?' + urlencode(query_params)
                 if re.search('json', headers['Content-Type'], re.IGNORECASE):
-                    request_body = None
+                    request_body = '{}'
                     if body is not None:
                         request_body = json.dumps(body)
                     r = self.pool_manager.request(
                         method, url,
                         body=request_body,
                         preload_content=_preload_content,
                         timeout=timeout,
@@ -211,19 +211,14 @@
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
         if _preload_content:
             r = RESTResponse(r)
 
-            # In the python 3, the response.data is bytes.
-            # we need to decode it to string.
-            if six.PY3:
-                r.data = r.data.decode('utf8')
-
             # log response body
             logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
             raise ApiException(http_resp=r)
 
         return r
```

### Comparing `wire4-client-1.1.2/wire4_client/__init__.py` & `wire4-client-1.1.3/wire4_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
 from wire4_client.api.autorizacin_de_depsitos_api import AutorizacinDeDepsitosApi
+from wire4_client.api.cargos_recurrentes_api import CargosRecurrentesApi
 from wire4_client.api.comprobante_electrnico_de_pago__cep_api import ComprobanteElectrnicoDePagoCEPApi
 from wire4_client.api.contacto_api import ContactoApi
 from wire4_client.api.contracts_details_api import ContractsDetailsApi
 from wire4_client.api.cuentas_de_beneficiarios_spei_api import CuentasDeBeneficiariosSPEIApi
 from wire4_client.api.cuentas_de_beneficiarios_spid_api import CuentasDeBeneficiariosSPIDApi
 from wire4_client.api.depositantes_api import DepositantesApi
 from wire4_client.api.empresas_co_di_api import EmpresasCoDiApi
@@ -49,36 +50,39 @@
 from wire4_client.models.authorization_transaction_group import AuthorizationTransactionGroup
 from wire4_client.models.authorized_beneficiaries_response import AuthorizedBeneficiariesResponse
 from wire4_client.models.authorized_users import AuthorizedUsers
 from wire4_client.models.balance import Balance
 from wire4_client.models.balance_list_response import BalanceListResponse
 from wire4_client.models.beneficiaries_query_register_status import BeneficiariesQueryRegisterStatus
 from wire4_client.models.beneficiaries_response import BeneficiariesResponse
+from wire4_client.models.beneficiary_dto import BeneficiaryDTO
 from wire4_client.models.beneficiary_institution import BeneficiaryInstitution
 from wire4_client.models.billing import Billing
 from wire4_client.models.billing_transaction import BillingTransaction
 from wire4_client.models.cep_response import CepResponse
 from wire4_client.models.cep_search_banxico import CepSearchBanxico
 from wire4_client.models.certificate_request import CertificateRequest
 from wire4_client.models.codi_code_qr_response_dto import CodiCodeQrResponseDTO
 from wire4_client.models.codi_code_request_dto import CodiCodeRequestDTO
 from wire4_client.models.codi_operation_response_dto import CodiOperationResponseDTO
 from wire4_client.models.codi_operations_filters_request_dto import CodiOperationsFiltersRequestDTO
 from wire4_client.models.company_registered import CompanyRegistered
 from wire4_client.models.company_requested import CompanyRequested
 from wire4_client.models.compay import Compay
 from wire4_client.models.configurations_limits import ConfigurationsLimits
+from wire4_client.models.confirm_recurring_charge import ConfirmRecurringCharge
 from wire4_client.models.contact_request import ContactRequest
 from wire4_client.models.contract_detail_request import ContractDetailRequest
 from wire4_client.models.contract_detail_response import ContractDetailResponse
+from wire4_client.models.customer import Customer
 from wire4_client.models.deposit import Deposit
 from wire4_client.models.deposit_authorization_request import DepositAuthorizationRequest
 from wire4_client.models.depositant import Depositant
-from wire4_client.models.depositants_register import DepositantsRegister
 from wire4_client.models.depositant_count_response import DepositantCountResponse
+from wire4_client.models.depositants_register import DepositantsRegister
 from wire4_client.models.depositants_response import DepositantsResponse
 from wire4_client.models.deposits_authorization_response import DepositsAuthorizationResponse
 from wire4_client.models.detailed_error_response import DetailedErrorResponse
 from wire4_client.models.error_response import ErrorResponse
 from wire4_client.models.get_depositants import GetDepositants
 from wire4_client.models.institution import Institution
 from wire4_client.models.institutions_list import InstitutionsList
@@ -99,18 +103,22 @@
 from wire4_client.models.message_web_hook import MessageWebHook
 from wire4_client.models.operations import Operations
 from wire4_client.models.pager_response_dto import PagerResponseDto
 from wire4_client.models.payment import Payment
 from wire4_client.models.payment_codi import PaymentCODI
 from wire4_client.models.payment_request_codi_response_dto import PaymentRequestCodiResponseDTO
 from wire4_client.models.payments_request_id import PaymentsRequestId
+from wire4_client.models.payments_spei_and_spid_order_id import PaymentsSpeiAndSpidOrderId
+from wire4_client.models.payments_spei_and_spid_request_id import PaymentsSpeiAndSpidRequestId
 from wire4_client.models.person import Person
 from wire4_client.models.pre_enrollment_data import PreEnrollmentData
 from wire4_client.models.pre_enrollment_response import PreEnrollmentResponse
 from wire4_client.models.pre_monex_authorization import PreMonexAuthorization
+from wire4_client.models.product import Product
+from wire4_client.models.recurring_charge_request import RecurringChargeRequest
 from wire4_client.models.relationship import Relationship
 from wire4_client.models.relationships_response import RelationshipsResponse
 from wire4_client.models.sales_point import SalesPoint
 from wire4_client.models.sales_point_found import SalesPointFound
 from wire4_client.models.sales_point_request import SalesPointRequest
 from wire4_client.models.sales_point_respose import SalesPointRespose
 from wire4_client.models.service_banking import ServiceBanking
@@ -119,15 +127,17 @@
 from wire4_client.models.spid_classification_dto import SpidClassificationDTO
 from wire4_client.models.spid_classifications_response_dto import SpidClassificationsResponseDTO
 from wire4_client.models.subscription_change_status_request import SubscriptionChangeStatusRequest
 from wire4_client.models.token_required_response import TokenRequiredResponse
 from wire4_client.models.transaction_error_code import TransactionErrorCode
 from wire4_client.models.transaction_outgoing import TransactionOutgoing
 from wire4_client.models.transaction_outgoing_spid import TransactionOutgoingSpid
+from wire4_client.models.transaction_spei_spid import TransactionSpeiSpid
 from wire4_client.models.transactions_outgoing_register import TransactionsOutgoingRegister
+from wire4_client.models.transactions_register import TransactionsRegister
 from wire4_client.models.update_configurations_request_dto import UpdateConfigurationsRequestDTO
 from wire4_client.models.urls_redirect import UrlsRedirect
 from wire4_client.models.use_service_banking import UseServiceBanking
 from wire4_client.models.user_company import UserCompany
 from wire4_client.models.web_hook_deposit_authorization_request import WebHookDepositAuthorizationRequest
 from wire4_client.models.web_hook_deposit_authorization_response import WebHookDepositAuthorizationResponse
 from wire4_client.models.webhook import Webhook
```

### Comparing `wire4-client-1.1.2/wire4_client/models/authorized_beneficiaries_response.py` & `wire4-client-1.1.3/wire4_client/models/authorized_beneficiaries_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.account_reassigned import AccountReassigned  # noqa: F401,E501
-
 
 class AuthorizedBeneficiariesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/beneficiaries_query_register_status.py` & `wire4-client-1.1.3/wire4_client/models/beneficiaries_query_register_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.account_response import AccountResponse  # noqa: F401,E501
-
 
 class BeneficiariesQueryRegisterStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/certificate_request.py` & `wire4-client-1.1.3/wire4_client/models/certificate_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class CertificateRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
@@ -104,26 +103,26 @@
 
         self._certificate_number = certificate_number
 
     @property
     def check_digit(self):
         """Gets the check_digit of this CertificateRequest.  # noqa: E501
 
-        Es el dígito verificador. Es un sólo dígito.  # noqa: E501
+        Es el dígito verificador. Máximo 3 dígitos.  # noqa: E501
 
         :return: The check_digit of this CertificateRequest.  # noqa: E501
         :rtype: str
         """
         return self._check_digit
 
     @check_digit.setter
     def check_digit(self, check_digit):
         """Sets the check_digit of this CertificateRequest.
 
-        Es el dígito verificador. Es un sólo dígito.  # noqa: E501
+        Es el dígito verificador. Máximo 3 dígitos.  # noqa: E501
 
         :param check_digit: The check_digit of this CertificateRequest.  # noqa: E501
         :type: str
         """
 
         self._check_digit = check_digit
```

### Comparing `wire4-client-1.1.2/wire4_client/models/account_reassigned.py` & `wire4-client-1.1.3/wire4_client/models/account_reassigned.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.beneficiary_institution import BeneficiaryInstitution  # noqa: F401,E501
-from wire4_client.models.institution import Institution  # noqa: F401,E501
-from wire4_client.models.person import Person  # noqa: F401,E501
-
 
 class AccountReassigned(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
@@ -29,69 +25,69 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'amount_limit': 'float',
+        'authorization_date': 'datetime',
         'bank': 'Institution',
         'beneficiary_account': 'str',
-        'currency_code': 'str',
         'email': 'list[str]',
         'institution': 'BeneficiaryInstitution',
         'kind_of_relationship': 'str',
         'numeric_reference_spei': 'str',
         'payment_concept_spei': 'str',
         'person': 'Person',
         'register_date': 'datetime',
         'relationship': 'str',
         'rfc': 'str',
         'status': 'str'
     }
 
     attribute_map = {
         'amount_limit': 'amount_limit',
+        'authorization_date': 'authorization_date',
         'bank': 'bank',
         'beneficiary_account': 'beneficiary_account',
-        'currency_code': 'currency_code',
         'email': 'email',
         'institution': 'institution',
         'kind_of_relationship': 'kind_of_relationship',
         'numeric_reference_spei': 'numeric_reference_spei',
         'payment_concept_spei': 'payment_concept_spei',
         'person': 'person',
         'register_date': 'register_date',
         'relationship': 'relationship',
         'rfc': 'rfc',
         'status': 'status'
     }
 
-    def __init__(self, amount_limit=None, bank=None, beneficiary_account=None, currency_code=None, email=None, institution=None, kind_of_relationship=None, numeric_reference_spei=None, payment_concept_spei=None, person=None, register_date=None, relationship=None, rfc=None, status=None):  # noqa: E501
+    def __init__(self, amount_limit=None, authorization_date=None, bank=None, beneficiary_account=None, email=None, institution=None, kind_of_relationship=None, numeric_reference_spei=None, payment_concept_spei=None, person=None, register_date=None, relationship=None, rfc=None, status=None):  # noqa: E501
         """AccountReassigned - a model defined in Swagger"""  # noqa: E501
         self._amount_limit = None
+        self._authorization_date = None
         self._bank = None
         self._beneficiary_account = None
-        self._currency_code = None
         self._email = None
         self._institution = None
         self._kind_of_relationship = None
         self._numeric_reference_spei = None
         self._payment_concept_spei = None
         self._person = None
         self._register_date = None
         self._relationship = None
         self._rfc = None
         self._status = None
         self.discriminator = None
         self.amount_limit = amount_limit
+        if authorization_date is not None:
+            self.authorization_date = authorization_date
         if bank is not None:
             self.bank = bank
         self.beneficiary_account = beneficiary_account
-        if currency_code is not None:
-            self.currency_code = currency_code
         if email is not None:
             self.email = email
         if institution is not None:
             self.institution = institution
         self.kind_of_relationship = kind_of_relationship
         if numeric_reference_spei is not None:
             self.numeric_reference_spei = numeric_reference_spei
@@ -128,14 +124,37 @@
         """
         if amount_limit is None:
             raise ValueError("Invalid value for `amount_limit`, must not be `None`")  # noqa: E501
 
         self._amount_limit = amount_limit
 
     @property
+    def authorization_date(self):
+        """Gets the authorization_date of this AccountReassigned.  # noqa: E501
+
+        Es la fecha en la que se autorizó el registro del beneficiario. Ésta fecha viene en formato ISO 8601 con zona horaria, ejemplo: <strong>2020-10-27T11:03:15.000-06:00</strong>.  # noqa: E501
+
+        :return: The authorization_date of this AccountReassigned.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._authorization_date
+
+    @authorization_date.setter
+    def authorization_date(self, authorization_date):
+        """Sets the authorization_date of this AccountReassigned.
+
+        Es la fecha en la que se autorizó el registro del beneficiario. Ésta fecha viene en formato ISO 8601 con zona horaria, ejemplo: <strong>2020-10-27T11:03:15.000-06:00</strong>.  # noqa: E501
+
+        :param authorization_date: The authorization_date of this AccountReassigned.  # noqa: E501
+        :type: datetime
+        """
+
+        self._authorization_date = authorization_date
+
+    @property
     def bank(self):
         """Gets the bank of this AccountReassigned.  # noqa: E501
 
 
         :return: The bank of this AccountReassigned.  # noqa: E501
         :rtype: Institution
         """
@@ -174,37 +193,14 @@
         """
         if beneficiary_account is None:
             raise ValueError("Invalid value for `beneficiary_account`, must not be `None`")  # noqa: E501
 
         self._beneficiary_account = beneficiary_account
 
     @property
-    def currency_code(self):
-        """Gets the currency_code of this AccountReassigned.  # noqa: E501
-
-        Es el código de divisa. Es en el formato estándar de 3 dígitos, por ejemplo para el peso mexicano: <b>MXP</b>, para el dólar estadounidense: <b>USD</b>.<br/><br/>Este dato es opcional, al registrar una cuenta si no se cuenta con este valor se asignará <b>MXP</b>  # noqa: E501
-
-        :return: The currency_code of this AccountReassigned.  # noqa: E501
-        :rtype: str
-        """
-        return self._currency_code
-
-    @currency_code.setter
-    def currency_code(self, currency_code):
-        """Sets the currency_code of this AccountReassigned.
-
-        Es el código de divisa. Es en el formato estándar de 3 dígitos, por ejemplo para el peso mexicano: <b>MXP</b>, para el dólar estadounidense: <b>USD</b>.<br/><br/>Este dato es opcional, al registrar una cuenta si no se cuenta con este valor se asignará <b>MXP</b>  # noqa: E501
-
-        :param currency_code: The currency_code of this AccountReassigned.  # noqa: E501
-        :type: str
-        """
-
-        self._currency_code = currency_code
-
-    @property
     def email(self):
         """Gets the email of this AccountReassigned.  # noqa: E501
 
         Es una lista de correos electrónicos (emails). Se valida el formato de email. Este campo es opcional.  # noqa: E501
 
         :return: The email of this AccountReassigned.  # noqa: E501
         :rtype: list[str]
```

### Comparing `wire4-client-1.1.2/wire4_client/models/spid_beneficiary_response.py` & `wire4-client-1.1.3/wire4_client/models/spid_beneficiary_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.beneficiary_institution import BeneficiaryInstitution  # noqa: F401,E501
-from wire4_client.models.institution import Institution  # noqa: F401,E501
-
 
 class SpidBeneficiaryResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
@@ -28,14 +25,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'amount_limit': 'float',
+        'authorization_date': 'datetime',
         'bank': 'Institution',
         'beneficiary_account': 'str',
         'email': 'list[str]',
         'institution': 'BeneficiaryInstitution',
         'kind_of_relationship': 'str',
         'numeric_reference_spid': 'str',
         'payment_concept_spid': 'str',
@@ -43,43 +41,47 @@
         'relationship': 'str',
         'rfc': 'str',
         'status': 'str'
     }
 
     attribute_map = {
         'amount_limit': 'amount_limit',
+        'authorization_date': 'authorization_date',
         'bank': 'bank',
         'beneficiary_account': 'beneficiary_account',
         'email': 'email',
         'institution': 'institution',
         'kind_of_relationship': 'kind_of_relationship',
         'numeric_reference_spid': 'numeric_reference_spid',
         'payment_concept_spid': 'payment_concept_spid',
         'register_date': 'register_date',
         'relationship': 'relationship',
         'rfc': 'rfc',
         'status': 'status'
     }
 
-    def __init__(self, amount_limit=None, bank=None, beneficiary_account=None, email=None, institution=None, kind_of_relationship=None, numeric_reference_spid=None, payment_concept_spid=None, register_date=None, relationship=None, rfc=None, status=None):  # noqa: E501
+    def __init__(self, amount_limit=None, authorization_date=None, bank=None, beneficiary_account=None, email=None, institution=None, kind_of_relationship=None, numeric_reference_spid=None, payment_concept_spid=None, register_date=None, relationship=None, rfc=None, status=None):  # noqa: E501
         """SpidBeneficiaryResponse - a model defined in Swagger"""  # noqa: E501
         self._amount_limit = None
+        self._authorization_date = None
         self._bank = None
         self._beneficiary_account = None
         self._email = None
         self._institution = None
         self._kind_of_relationship = None
         self._numeric_reference_spid = None
         self._payment_concept_spid = None
         self._register_date = None
         self._relationship = None
         self._rfc = None
         self._status = None
         self.discriminator = None
         self.amount_limit = amount_limit
+        if authorization_date is not None:
+            self.authorization_date = authorization_date
         if bank is not None:
             self.bank = bank
         self.beneficiary_account = beneficiary_account
         if email is not None:
             self.email = email
         self.institution = institution
         self.kind_of_relationship = kind_of_relationship
@@ -117,14 +119,37 @@
         """
         if amount_limit is None:
             raise ValueError("Invalid value for `amount_limit`, must not be `None`")  # noqa: E501
 
         self._amount_limit = amount_limit
 
     @property
+    def authorization_date(self):
+        """Gets the authorization_date of this SpidBeneficiaryResponse.  # noqa: E501
+
+        La fecha en la que se registro el beneficiario.  # noqa: E501
+
+        :return: The authorization_date of this SpidBeneficiaryResponse.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._authorization_date
+
+    @authorization_date.setter
+    def authorization_date(self, authorization_date):
+        """Sets the authorization_date of this SpidBeneficiaryResponse.
+
+        La fecha en la que se registro el beneficiario.  # noqa: E501
+
+        :param authorization_date: The authorization_date of this SpidBeneficiaryResponse.  # noqa: E501
+        :type: datetime
+        """
+
+        self._authorization_date = authorization_date
+
+    @property
     def bank(self):
         """Gets the bank of this SpidBeneficiaryResponse.  # noqa: E501
 
 
         :return: The bank of this SpidBeneficiaryResponse.  # noqa: E501
         :rtype: Institution
         """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/spid_beneficiaries_response.py` & `wire4-client-1.1.3/wire4_client/models/spid_beneficiaries_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.spid_beneficiary_response import SpidBeneficiaryResponse  # noqa: F401,E501
-
 
 class SpidBeneficiariesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/balance_list_response.py` & `wire4-client-1.1.3/wire4_client/models/balance_list_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.balance import Balance  # noqa: F401,E501
-
 
 class BalanceListResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_web_hook.py` & `wire4-client-1.1.3/wire4_client/models/message_web_hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class MessageWebHook(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/urls_redirect.py` & `wire4-client-1.1.3/wire4_client/models/urls_redirect.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class UrlsRedirect(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_request_changed.py` & `wire4-client-1.1.3/wire4_client/models/message_request_changed.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class MessageRequestChanged(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/account_request.py` & `wire4-client-1.1.3/wire4_client/models/account_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.account import Account  # noqa: F401,E501
-
 
 class AccountRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/relationships_response.py` & `wire4-client-1.1.3/wire4_client/models/relationships_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.relationship import Relationship  # noqa: F401,E501
-
 
 class RelationshipsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/configurations_limits.py` & `wire4-client-1.1.3/wire4_client/models/configurations_limits.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.item import Item  # noqa: F401,E501
-
 
 class ConfigurationsLimits(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/payment_codi.py` & `wire4-client-1.1.3/wire4_client/models/payment_codi.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class PaymentCODI(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
@@ -199,15 +198,15 @@
         """Sets the status of this PaymentCODI.
 
         Estatus del pago  # noqa: E501
 
         :param status: The status of this PaymentCODI.  # noqa: E501
         :type: str
         """
-        allowed_values = ["RECEIVED", "COMPLETED", "CANCELLED"]  # noqa: E501
+        allowed_values = ["ACCEPTED", "RECEIVED", "COMPLETED", "CANCELLED", "POSTPONED", "REJECTED", "REVERSED", "PENDING"]  # noqa: E501
         if status not in allowed_values:
             raise ValueError(
                 "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
                 .format(status, allowed_values)
             )
 
         self._status = status
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_sales_point.py` & `wire4-client-1.1.3/wire4_client/models/message_sales_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class MessageSalesPoint(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_account_beneficiary.py` & `wire4-client-1.1.3/wire4_client/models/message_account_beneficiary.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class MessageAccountBeneficiary(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/person.py` & `wire4-client-1.1.3/wire4_client/models/person.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class Person(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/codi_code_qr_response_dto.py` & `wire4-client-1.1.3/wire4_client/models/codi_code_qr_response_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class CodiCodeQrResponseDTO(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
@@ -33,41 +32,44 @@
         'barcode_base64': 'str',
         'barcode_url': 'str',
         'concept': 'str',
         'creation_date': 'datetime',
         'due_date': 'datetime',
         'order_id': 'str',
         'phone_number': 'str',
+        'reference': 'int',
         'status': 'str',
         'type': 'str'
     }
 
     attribute_map = {
         'amount': 'amount',
         'barcode_base64': 'barcode_base64',
         'barcode_url': 'barcode_url',
         'concept': 'concept',
         'creation_date': 'creation_date',
         'due_date': 'due_date',
         'order_id': 'order_id',
         'phone_number': 'phone_number',
+        'reference': 'reference',
         'status': 'status',
         'type': 'type'
     }
 
-    def __init__(self, amount=None, barcode_base64=None, barcode_url=None, concept=None, creation_date=None, due_date=None, order_id=None, phone_number=None, status=None, type=None):  # noqa: E501
+    def __init__(self, amount=None, barcode_base64=None, barcode_url=None, concept=None, creation_date=None, due_date=None, order_id=None, phone_number=None, reference=None, status=None, type=None):  # noqa: E501
         """CodiCodeQrResponseDTO - a model defined in Swagger"""  # noqa: E501
         self._amount = None
         self._barcode_base64 = None
         self._barcode_url = None
         self._concept = None
         self._creation_date = None
         self._due_date = None
         self._order_id = None
         self._phone_number = None
+        self._reference = None
         self._status = None
         self._type = None
         self.discriminator = None
         if amount is not None:
             self.amount = amount
         if barcode_base64 is not None:
             self.barcode_base64 = barcode_base64
@@ -79,14 +81,16 @@
             self.creation_date = creation_date
         if due_date is not None:
             self.due_date = due_date
         if order_id is not None:
             self.order_id = order_id
         if phone_number is not None:
             self.phone_number = phone_number
+        if reference is not None:
+            self.reference = reference
         if status is not None:
             self.status = status
         if type is not None:
             self.type = type
 
     @property
     def amount(self):
@@ -269,14 +273,37 @@
         :param phone_number: The phone_number of this CodiCodeQrResponseDTO.  # noqa: E501
         :type: str
         """
 
         self._phone_number = phone_number
 
     @property
+    def reference(self):
+        """Gets the reference of this CodiCodeQrResponseDTO.  # noqa: E501
+
+        Referencia numérica del pago CODI®.  # noqa: E501
+
+        :return: The reference of this CodiCodeQrResponseDTO.  # noqa: E501
+        :rtype: int
+        """
+        return self._reference
+
+    @reference.setter
+    def reference(self, reference):
+        """Sets the reference of this CodiCodeQrResponseDTO.
+
+        Referencia numérica del pago CODI®.  # noqa: E501
+
+        :param reference: The reference of this CodiCodeQrResponseDTO.  # noqa: E501
+        :type: int
+        """
+
+        self._reference = reference
+
+    @property
     def status(self):
         """Gets the status of this CodiCodeQrResponseDTO.  # noqa: E501
 
         El estado del código QR para pago CODI®.  # noqa: E501
 
         :return: The status of this CodiCodeQrResponseDTO.  # noqa: E501
         :rtype: str
@@ -288,15 +315,15 @@
         """Sets the status of this CodiCodeQrResponseDTO.
 
         El estado del código QR para pago CODI®.  # noqa: E501
 
         :param status: The status of this CodiCodeQrResponseDTO.  # noqa: E501
         :type: str
         """
-        allowed_values = ["RECEIVED", "COMPLETED", "CANCELLED"]  # noqa: E501
+        allowed_values = ["ACCEPTED", "RECEIVED", "COMPLETED", "CANCELLED", "POSTPONED", "REJECTED", "REVERSED", "PENDING"]  # noqa: E501
         if status not in allowed_values:
             raise ValueError(
                 "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
                 .format(status, allowed_values)
             )
 
         self._status = status
@@ -317,15 +344,15 @@
         """Sets the type of this CodiCodeQrResponseDTO.
 
         Es el tipo de código QR para pago con CODI®.  # noqa: E501
 
         :param type: The type of this CodiCodeQrResponseDTO.  # noqa: E501
         :type: str
         """
-        allowed_values = ["PUSH_NOTIFICATION", "QR_CODE"]  # noqa: E501
+        allowed_values = ["PUSH_NOTIFICATION", "QR_CODE", "UNKNOWN"]  # noqa: E501
         if type not in allowed_values:
             raise ValueError(
                 "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
                 .format(type, allowed_values)
             )
 
         self._type = type
```

### Comparing `wire4-client-1.1.2/wire4_client/models/sales_point_request.py` & `wire4-client-1.1.3/wire4_client/models/sales_point_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class SalesPointRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/depositants_response.py` & `wire4-client-1.1.3/wire4_client/models/depositants_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class DepositantsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/transaction_error_code.py` & `wire4-client-1.1.3/wire4_client/models/transaction_error_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class TransactionErrorCode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/billing.py` & `wire4-client-1.1.3/wire4_client/models/billing.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.billing_transaction import BillingTransaction  # noqa: F401,E501
-
 
 class Billing(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/deposit.py` & `wire4-client-1.1.3/wire4_client/models/deposit.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.message_cep import MessageCEP  # noqa: F401,E501
-from wire4_client.models.message_institution import MessageInstitution  # noqa: F401,E501
-
 
 class Deposit(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/webhook_request.py` & `wire4-client-1.1.3/wire4_client/models/webhook_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class WebhookRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/institution.py` & `wire4-client-1.1.3/wire4_client/models/institution.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class Institution(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/codi_operation_response_dto.py` & `wire4-client-1.1.3/wire4_client/models/codi_operation_response_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class CodiOperationResponseDTO(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/transaction_outgoing.py` & `wire4-client-1.1.3/wire4_client/models/transaction_outgoing.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class TransactionOutgoing(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/cep_search_banxico.py` & `wire4-client-1.1.3/wire4_client/models/cep_search_banxico.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class CepSearchBanxico(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/relationship.py` & `wire4-client-1.1.3/wire4_client/models/relationship.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class Relationship(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_deposit_received.py` & `wire4-client-1.1.3/wire4_client/models/message_deposit_received.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.message_cep import MessageCEP  # noqa: F401,E501
-from wire4_client.models.message_institution import MessageInstitution  # noqa: F401,E501
-
 
 class MessageDepositReceived(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/transactions_outgoing_register.py` & `wire4-client-1.1.3/wire4_client/models/transactions_outgoing_register.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.transaction_outgoing import TransactionOutgoing  # noqa: F401,E501
-
 
 class TransactionsOutgoingRegister(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/webhook.py` & `wire4-client-1.1.3/wire4_client/models/webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class Webhook(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/company_requested.py` & `wire4-client-1.1.3/wire4_client/models/company_requested.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.certificate_request import CertificateRequest  # noqa: F401,E501
-
 
 class CompanyRequested(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/token_required_response.py` & `wire4-client-1.1.3/wire4_client/models/token_required_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class TokenRequiredResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/pre_enrollment_data.py` & `wire4-client-1.1.3/wire4_client/models/pre_enrollment_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class PreEnrollmentData(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/billing_transaction.py` & `wire4-client-1.1.3/wire4_client/models/billing_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class BillingTransaction(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/pre_enrollment_response.py` & `wire4-client-1.1.3/wire4_client/models/pre_enrollment_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class PreEnrollmentResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/depositant_count_response.py` & `wire4-client-1.1.3/wire4_client/models/depositant_count_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class DepositantCountResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/transaction_outgoing_spid.py` & `wire4-client-1.1.3/wire4_client/models/transaction_outgoing_spid.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class TransactionOutgoingSpid(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/authorized_users.py` & `wire4-client-1.1.3/wire4_client/models/authorized_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class AuthorizedUsers(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/institutions_list.py` & `wire4-client-1.1.3/wire4_client/models/institutions_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.institution import Institution  # noqa: F401,E501
-
 
 class InstitutionsList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/beneficiaries_response.py` & `wire4-client-1.1.3/wire4_client/models/beneficiaries_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.account_response import AccountResponse  # noqa: F401,E501
-
 
 class BeneficiariesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/amount_request.py` & `wire4-client-1.1.3/wire4_client/models/amount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class AmountRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/subscription_change_status_request.py` & `wire4-client-1.1.3/wire4_client/models/subscription_change_status_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class SubscriptionChangeStatusRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/codi_code_request_dto.py` & `wire4-client-1.1.3/wire4_client/models/web_hook_deposit_authorization_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,242 +11,203 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
-class CodiCodeRequestDTO(object):
+class WebHookDepositAuthorizationResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'amount': 'float',
-        'concept': 'str',
-        'due_date': 'datetime',
-        'metadata': 'str',
-        'order_id': 'str',
-        'phone_number': 'str',
-        'type': 'str'
+        'events': 'list[str]',
+        'name': 'str',
+        'secret': 'str',
+        'status': 'str',
+        'url': 'str',
+        'wh_uuid': 'str'
     }
 
     attribute_map = {
-        'amount': 'amount',
-        'concept': 'concept',
-        'due_date': 'due_date',
-        'metadata': 'metadata',
-        'order_id': 'order_id',
-        'phone_number': 'phone_number',
-        'type': 'type'
+        'events': 'events',
+        'name': 'name',
+        'secret': 'secret',
+        'status': 'status',
+        'url': 'url',
+        'wh_uuid': 'wh_uuid'
     }
 
-    def __init__(self, amount=None, concept=None, due_date=None, metadata=None, order_id=None, phone_number=None, type=None):  # noqa: E501
-        """CodiCodeRequestDTO - a model defined in Swagger"""  # noqa: E501
-        self._amount = None
-        self._concept = None
-        self._due_date = None
-        self._metadata = None
-        self._order_id = None
-        self._phone_number = None
-        self._type = None
+    def __init__(self, events=None, name=None, secret=None, status=None, url=None, wh_uuid=None):  # noqa: E501
+        """WebHookDepositAuthorizationResponse - a model defined in Swagger"""  # noqa: E501
+        self._events = None
+        self._name = None
+        self._secret = None
+        self._status = None
+        self._url = None
+        self._wh_uuid = None
         self.discriminator = None
-        if amount is not None:
-            self.amount = amount
-        self.concept = concept
-        self.due_date = due_date
-        if metadata is not None:
-            self.metadata = metadata
-        self.order_id = order_id
-        if phone_number is not None:
-            self.phone_number = phone_number
-        self.type = type
+        if events is not None:
+            self.events = events
+        if name is not None:
+            self.name = name
+        if secret is not None:
+            self.secret = secret
+        if status is not None:
+            self.status = status
+        if url is not None:
+            self.url = url
+        if wh_uuid is not None:
+            self.wh_uuid = wh_uuid
 
     @property
-    def amount(self):
-        """Gets the amount of this CodiCodeRequestDTO.  # noqa: E501
+    def events(self):
+        """Gets the events of this WebHookDepositAuthorizationResponse.  # noqa: E501
 
-        Monto del pago CODI®  # noqa: E501
+        Tipo de evento manejado por el webhook, para mas referencia sobre los tipos de eventos soportados, revise la siguiente liga: <a href=\"https://developers.wire4.mx/#section/Eventos\">https://developers.wire4.mx/#section/Eventos.</a>  # noqa: E501
 
-        :return: The amount of this CodiCodeRequestDTO.  # noqa: E501
-        :rtype: float
+        :return: The events of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._amount
+        return self._events
 
-    @amount.setter
-    def amount(self, amount):
-        """Sets the amount of this CodiCodeRequestDTO.
+    @events.setter
+    def events(self, events):
+        """Sets the events of this WebHookDepositAuthorizationResponse.
 
-        Monto del pago CODI®  # noqa: E501
+        Tipo de evento manejado por el webhook, para mas referencia sobre los tipos de eventos soportados, revise la siguiente liga: <a href=\"https://developers.wire4.mx/#section/Eventos\">https://developers.wire4.mx/#section/Eventos.</a>  # noqa: E501
 
-        :param amount: The amount of this CodiCodeRequestDTO.  # noqa: E501
-        :type: float
+        :param events: The events of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :type: list[str]
         """
 
-        self._amount = amount
+        self._events = events
 
     @property
-    def concept(self):
-        """Gets the concept of this CodiCodeRequestDTO.  # noqa: E501
+    def name(self):
+        """Gets the name of this WebHookDepositAuthorizationResponse.  # noqa: E501
 
-        Descripción del pago CODI®  # noqa: E501
+        Es el nombre del webhook.  # noqa: E501
 
-        :return: The concept of this CodiCodeRequestDTO.  # noqa: E501
+        :return: The name of this WebHookDepositAuthorizationResponse.  # noqa: E501
         :rtype: str
         """
-        return self._concept
+        return self._name
 
-    @concept.setter
-    def concept(self, concept):
-        """Sets the concept of this CodiCodeRequestDTO.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this WebHookDepositAuthorizationResponse.
 
-        Descripción del pago CODI®  # noqa: E501
+        Es el nombre del webhook.  # noqa: E501
 
-        :param concept: The concept of this CodiCodeRequestDTO.  # noqa: E501
+        :param name: The name of this WebHookDepositAuthorizationResponse.  # noqa: E501
         :type: str
         """
-        if concept is None:
-            raise ValueError("Invalid value for `concept`, must not be `None`")  # noqa: E501
-
-        self._concept = concept
-
-    @property
-    def due_date(self):
-        """Gets the due_date of this CodiCodeRequestDTO.  # noqa: E501
-
-        Fecha de operación pago CODI®, formato: yyyy-MM-dd'T'HH:mm:ss  # noqa: E501
-
-        :return: The due_date of this CodiCodeRequestDTO.  # noqa: E501
-        :rtype: datetime
-        """
-        return self._due_date
-
-    @due_date.setter
-    def due_date(self, due_date):
-        """Sets the due_date of this CodiCodeRequestDTO.
-
-        Fecha de operación pago CODI®, formato: yyyy-MM-dd'T'HH:mm:ss  # noqa: E501
-
-        :param due_date: The due_date of this CodiCodeRequestDTO.  # noqa: E501
-        :type: datetime
-        """
-        if due_date is None:
-            raise ValueError("Invalid value for `due_date`, must not be `None`")  # noqa: E501
 
-        self._due_date = due_date
+        self._name = name
 
     @property
-    def metadata(self):
-        """Gets the metadata of this CodiCodeRequestDTO.  # noqa: E501
+    def secret(self):
+        """Gets the secret of this WebHookDepositAuthorizationResponse.  # noqa: E501
 
-        Campo de metada CODI®, longitud máxima determinada por configuracion de la empresa, por defecto 100 caracteres  # noqa: E501
+        Es la llave con la cuál se debe de identificar que el webhook fue enviado por Wire4. Para mayor información revisar la guía de notificaciones en la sección de  <a href=\"https://wire4.mx/#/guides/notificaciones\">\"Comprobación de firmas de Webhook\".</a>  # noqa: E501
 
-        :return: The metadata of this CodiCodeRequestDTO.  # noqa: E501
+        :return: The secret of this WebHookDepositAuthorizationResponse.  # noqa: E501
         :rtype: str
         """
-        return self._metadata
+        return self._secret
 
-    @metadata.setter
-    def metadata(self, metadata):
-        """Sets the metadata of this CodiCodeRequestDTO.
+    @secret.setter
+    def secret(self, secret):
+        """Sets the secret of this WebHookDepositAuthorizationResponse.
 
-        Campo de metada CODI®, longitud máxima determinada por configuracion de la empresa, por defecto 100 caracteres  # noqa: E501
+        Es la llave con la cuál se debe de identificar que el webhook fue enviado por Wire4. Para mayor información revisar la guía de notificaciones en la sección de  <a href=\"https://wire4.mx/#/guides/notificaciones\">\"Comprobación de firmas de Webhook\".</a>  # noqa: E501
 
-        :param metadata: The metadata of this CodiCodeRequestDTO.  # noqa: E501
+        :param secret: The secret of this WebHookDepositAuthorizationResponse.  # noqa: E501
         :type: str
         """
 
-        self._metadata = metadata
+        self._secret = secret
 
     @property
-    def order_id(self):
-        """Gets the order_id of this CodiCodeRequestDTO.  # noqa: E501
+    def status(self):
+        """Gets the status of this WebHookDepositAuthorizationResponse.  # noqa: E501
 
-        Referencia de la transferencia asignada por el cliente  # noqa: E501
+        Es el estado (estatus) en el que se encuentra el webhook.  # noqa: E501
 
-        :return: The order_id of this CodiCodeRequestDTO.  # noqa: E501
+        :return: The status of this WebHookDepositAuthorizationResponse.  # noqa: E501
         :rtype: str
         """
-        return self._order_id
+        return self._status
 
-    @order_id.setter
-    def order_id(self, order_id):
-        """Sets the order_id of this CodiCodeRequestDTO.
+    @status.setter
+    def status(self, status):
+        """Sets the status of this WebHookDepositAuthorizationResponse.
 
-        Referencia de la transferencia asignada por el cliente  # noqa: E501
+        Es el estado (estatus) en el que se encuentra el webhook.  # noqa: E501
 
-        :param order_id: The order_id of this CodiCodeRequestDTO.  # noqa: E501
+        :param status: The status of this WebHookDepositAuthorizationResponse.  # noqa: E501
         :type: str
         """
-        if order_id is None:
-            raise ValueError("Invalid value for `order_id`, must not be `None`")  # noqa: E501
 
-        self._order_id = order_id
+        self._status = status
 
     @property
-    def phone_number(self):
-        """Gets the phone_number of this CodiCodeRequestDTO.  # noqa: E501
+    def url(self):
+        """Gets the url of this WebHookDepositAuthorizationResponse.  # noqa: E501
 
-        Número de teléfono móvil en caso de ser un pago CODI® usando 'PUSH_NOTIFICATION' estecampo sería obligatorio  # noqa: E501
+        Es la dirección URL a la cuál Wire4 enviará las notificaciones cuando un evento ocurra.  # noqa: E501
 
-        :return: The phone_number of this CodiCodeRequestDTO.  # noqa: E501
+        :return: The url of this WebHookDepositAuthorizationResponse.  # noqa: E501
         :rtype: str
         """
-        return self._phone_number
+        return self._url
 
-    @phone_number.setter
-    def phone_number(self, phone_number):
-        """Sets the phone_number of this CodiCodeRequestDTO.
+    @url.setter
+    def url(self, url):
+        """Sets the url of this WebHookDepositAuthorizationResponse.
 
-        Número de teléfono móvil en caso de ser un pago CODI® usando 'PUSH_NOTIFICATION' estecampo sería obligatorio  # noqa: E501
+        Es la dirección URL a la cuál Wire4 enviará las notificaciones cuando un evento ocurra.  # noqa: E501
 
-        :param phone_number: The phone_number of this CodiCodeRequestDTO.  # noqa: E501
+        :param url: The url of this WebHookDepositAuthorizationResponse.  # noqa: E501
         :type: str
         """
 
-        self._phone_number = phone_number
+        self._url = url
 
     @property
-    def type(self):
-        """Gets the type of this CodiCodeRequestDTO.  # noqa: E501
+    def wh_uuid(self):
+        """Gets the wh_uuid of this WebHookDepositAuthorizationResponse.  # noqa: E501
 
-        El tipo de código QR para pago con CODI®  # noqa: E501
+         Es el identificador del webhook.  # noqa: E501
 
-        :return: The type of this CodiCodeRequestDTO.  # noqa: E501
+        :return: The wh_uuid of this WebHookDepositAuthorizationResponse.  # noqa: E501
         :rtype: str
         """
-        return self._type
+        return self._wh_uuid
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this CodiCodeRequestDTO.
+    @wh_uuid.setter
+    def wh_uuid(self, wh_uuid):
+        """Sets the wh_uuid of this WebHookDepositAuthorizationResponse.
 
-        El tipo de código QR para pago con CODI®  # noqa: E501
+         Es el identificador del webhook.  # noqa: E501
 
-        :param type: The type of this CodiCodeRequestDTO.  # noqa: E501
+        :param wh_uuid: The wh_uuid of this WebHookDepositAuthorizationResponse.  # noqa: E501
         :type: str
         """
-        if type is None:
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        allowed_values = ["PUSH_NOTIFICATION", "QR_CODE"]  # noqa: E501
-        if type not in allowed_values:
-            raise ValueError(
-                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
-                .format(type, allowed_values)
-            )
 
-        self._type = type
+        self._wh_uuid = wh_uuid
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -261,15 +222,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(CodiCodeRequestDTO, dict):
+        if issubclass(WebHookDepositAuthorizationResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -277,15 +238,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CodiCodeRequestDTO):
+        if not isinstance(other, WebHookDepositAuthorizationResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `wire4-client-1.1.2/wire4_client/models/sales_point_found.py` & `wire4-client-1.1.3/wire4_client/models/sales_point_found.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class SalesPointFound(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/web_hook_deposit_authorization_response.py` & `wire4-client-1.1.3/wire4_client/models/webhook_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
-class WebHookDepositAuthorizationResponse(object):
+class WebhookResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -43,15 +42,15 @@
         'secret': 'secret',
         'status': 'status',
         'url': 'url',
         'wh_uuid': 'wh_uuid'
     }
 
     def __init__(self, events=None, name=None, secret=None, status=None, url=None, wh_uuid=None):  # noqa: E501
-        """WebHookDepositAuthorizationResponse - a model defined in Swagger"""  # noqa: E501
+        """WebhookResponse - a model defined in Swagger"""  # noqa: E501
         self._events = None
         self._name = None
         self._secret = None
         self._status = None
         self._url = None
         self._wh_uuid = None
         self.discriminator = None
@@ -66,145 +65,151 @@
         if url is not None:
             self.url = url
         if wh_uuid is not None:
             self.wh_uuid = wh_uuid
 
     @property
     def events(self):
-        """Gets the events of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        """Gets the events of this WebhookResponse.  # noqa: E501
 
-        Tipo de evento manejado por el webhook, para mas referencia sobre los tipos de eventos soportados, revise la siguiente liga: <a href=\"https://developers.wire4.mx/#section/Eventos\">https://developers.wire4.mx/#section/Eventos.</a>  # noqa: E501
+        Tipos de eventos de los cuales Wire4 te enviará información.  # noqa: E501
 
-        :return: The events of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :return: The events of this WebhookResponse.  # noqa: E501
         :rtype: list[str]
         """
         return self._events
 
     @events.setter
     def events(self, events):
-        """Sets the events of this WebHookDepositAuthorizationResponse.
+        """Sets the events of this WebhookResponse.
 
-        Tipo de evento manejado por el webhook, para mas referencia sobre los tipos de eventos soportados, revise la siguiente liga: <a href=\"https://developers.wire4.mx/#section/Eventos\">https://developers.wire4.mx/#section/Eventos.</a>  # noqa: E501
+        Tipos de eventos de los cuales Wire4 te enviará información.  # noqa: E501
 
-        :param events: The events of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :param events: The events of this WebhookResponse.  # noqa: E501
         :type: list[str]
         """
 
         self._events = events
 
     @property
     def name(self):
-        """Gets the name of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        """Gets the name of this WebhookResponse.  # noqa: E501
 
         Es el nombre del webhook.  # noqa: E501
 
-        :return: The name of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :return: The name of this WebhookResponse.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this WebHookDepositAuthorizationResponse.
+        """Sets the name of this WebhookResponse.
 
         Es el nombre del webhook.  # noqa: E501
 
-        :param name: The name of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :param name: The name of this WebhookResponse.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
     def secret(self):
-        """Gets the secret of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        """Gets the secret of this WebhookResponse.  # noqa: E501
 
-        Es la llave con la cuál se debe de identificar que el webhook fue enviado por Wire4. Para mayor información revisar la guía de notificaciones en la sección de  <a href=\"https://wire4.mx/#/guides/notificaciones\">\"Comprobación de firmas de Webhook\".</a>  # noqa: E501
+        Llave con la cual se debe de identificar que el webhook fue enviado por Wire4, para mayor información revisar la guía de notificaciones (https://wire4.mx/#/guides/notificaciones),  en la sección de  <a href=\"https://wire4.mx/#/guides/notificaciones\">\"Comprobación de firmas de Webhook\".</a>  # noqa: E501
 
-        :return: The secret of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :return: The secret of this WebhookResponse.  # noqa: E501
         :rtype: str
         """
         return self._secret
 
     @secret.setter
     def secret(self, secret):
-        """Sets the secret of this WebHookDepositAuthorizationResponse.
+        """Sets the secret of this WebhookResponse.
 
-        Es la llave con la cuál se debe de identificar que el webhook fue enviado por Wire4. Para mayor información revisar la guía de notificaciones en la sección de  <a href=\"https://wire4.mx/#/guides/notificaciones\">\"Comprobación de firmas de Webhook\".</a>  # noqa: E501
+        Llave con la cual se debe de identificar que el webhook fue enviado por Wire4, para mayor información revisar la guía de notificaciones (https://wire4.mx/#/guides/notificaciones),  en la sección de  <a href=\"https://wire4.mx/#/guides/notificaciones\">\"Comprobación de firmas de Webhook\".</a>  # noqa: E501
 
-        :param secret: The secret of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :param secret: The secret of this WebhookResponse.  # noqa: E501
         :type: str
         """
 
         self._secret = secret
 
     @property
     def status(self):
-        """Gets the status of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        """Gets the status of this WebhookResponse.  # noqa: E501
 
         Es el estado (estatus) en el que se encuentra el webhook.  # noqa: E501
 
-        :return: The status of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :return: The status of this WebhookResponse.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this WebHookDepositAuthorizationResponse.
+        """Sets the status of this WebhookResponse.
 
         Es el estado (estatus) en el que se encuentra el webhook.  # noqa: E501
 
-        :param status: The status of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :param status: The status of this WebhookResponse.  # noqa: E501
         :type: str
         """
+        allowed_values = ["ACTIVE", "INACTIVE", "DELETED"]  # noqa: E501
+        if status not in allowed_values:
+            raise ValueError(
+                "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
+                .format(status, allowed_values)
+            )
 
         self._status = status
 
     @property
     def url(self):
-        """Gets the url of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        """Gets the url of this WebhookResponse.  # noqa: E501
 
-        Es la dirección URL a la cuál Wire4 enviará las notificaciones cuando un evento ocurra.  # noqa: E501
+        Es la dirección URL a la que Wire4 enviará las notificaciones cuando un evento ocurra.  # noqa: E501
 
-        :return: The url of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :return: The url of this WebhookResponse.  # noqa: E501
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
-        """Sets the url of this WebHookDepositAuthorizationResponse.
+        """Sets the url of this WebhookResponse.
 
-        Es la dirección URL a la cuál Wire4 enviará las notificaciones cuando un evento ocurra.  # noqa: E501
+        Es la dirección URL a la que Wire4 enviará las notificaciones cuando un evento ocurra.  # noqa: E501
 
-        :param url: The url of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :param url: The url of this WebhookResponse.  # noqa: E501
         :type: str
         """
 
         self._url = url
 
     @property
     def wh_uuid(self):
-        """Gets the wh_uuid of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        """Gets the wh_uuid of this WebhookResponse.  # noqa: E501
 
-         Es el identificador del webhook.  # noqa: E501
+        Es el identificador del webhook. Ejemplo: wh_54a832866f784b439bc625c0f4e04e12.  # noqa: E501
 
-        :return: The wh_uuid of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :return: The wh_uuid of this WebhookResponse.  # noqa: E501
         :rtype: str
         """
         return self._wh_uuid
 
     @wh_uuid.setter
     def wh_uuid(self, wh_uuid):
-        """Sets the wh_uuid of this WebHookDepositAuthorizationResponse.
+        """Sets the wh_uuid of this WebhookResponse.
 
-         Es el identificador del webhook.  # noqa: E501
+        Es el identificador del webhook. Ejemplo: wh_54a832866f784b439bc625c0f4e04e12.  # noqa: E501
 
-        :param wh_uuid: The wh_uuid of this WebHookDepositAuthorizationResponse.  # noqa: E501
+        :param wh_uuid: The wh_uuid of this WebhookResponse.  # noqa: E501
         :type: str
         """
 
         self._wh_uuid = wh_uuid
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -223,15 +228,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WebHookDepositAuthorizationResponse, dict):
+        if issubclass(WebhookResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -239,15 +244,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WebHookDepositAuthorizationResponse):
+        if not isinstance(other, WebhookResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `wire4-client-1.1.2/wire4_client/models/__init__.py` & `wire4-client-1.1.3/wire4_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,36 +25,39 @@
 from wire4_client.models.authorization_transaction_group import AuthorizationTransactionGroup
 from wire4_client.models.authorized_beneficiaries_response import AuthorizedBeneficiariesResponse
 from wire4_client.models.authorized_users import AuthorizedUsers
 from wire4_client.models.balance import Balance
 from wire4_client.models.balance_list_response import BalanceListResponse
 from wire4_client.models.beneficiaries_query_register_status import BeneficiariesQueryRegisterStatus
 from wire4_client.models.beneficiaries_response import BeneficiariesResponse
+from wire4_client.models.beneficiary_dto import BeneficiaryDTO
 from wire4_client.models.beneficiary_institution import BeneficiaryInstitution
 from wire4_client.models.billing import Billing
 from wire4_client.models.billing_transaction import BillingTransaction
 from wire4_client.models.cep_response import CepResponse
 from wire4_client.models.cep_search_banxico import CepSearchBanxico
 from wire4_client.models.certificate_request import CertificateRequest
 from wire4_client.models.codi_code_qr_response_dto import CodiCodeQrResponseDTO
 from wire4_client.models.codi_code_request_dto import CodiCodeRequestDTO
 from wire4_client.models.codi_operation_response_dto import CodiOperationResponseDTO
 from wire4_client.models.codi_operations_filters_request_dto import CodiOperationsFiltersRequestDTO
 from wire4_client.models.company_registered import CompanyRegistered
 from wire4_client.models.company_requested import CompanyRequested
 from wire4_client.models.compay import Compay
 from wire4_client.models.configurations_limits import ConfigurationsLimits
+from wire4_client.models.confirm_recurring_charge import ConfirmRecurringCharge
 from wire4_client.models.contact_request import ContactRequest
 from wire4_client.models.contract_detail_request import ContractDetailRequest
 from wire4_client.models.contract_detail_response import ContractDetailResponse
+from wire4_client.models.customer import Customer
 from wire4_client.models.deposit import Deposit
 from wire4_client.models.deposit_authorization_request import DepositAuthorizationRequest
 from wire4_client.models.depositant import Depositant
-from wire4_client.models.depositants_register import DepositantsRegister
 from wire4_client.models.depositant_count_response import DepositantCountResponse
+from wire4_client.models.depositants_register import DepositantsRegister
 from wire4_client.models.depositants_response import DepositantsResponse
 from wire4_client.models.deposits_authorization_response import DepositsAuthorizationResponse
 from wire4_client.models.detailed_error_response import DetailedErrorResponse
 from wire4_client.models.error_response import ErrorResponse
 from wire4_client.models.get_depositants import GetDepositants
 from wire4_client.models.institution import Institution
 from wire4_client.models.institutions_list import InstitutionsList
@@ -75,18 +78,22 @@
 from wire4_client.models.message_web_hook import MessageWebHook
 from wire4_client.models.operations import Operations
 from wire4_client.models.pager_response_dto import PagerResponseDto
 from wire4_client.models.payment import Payment
 from wire4_client.models.payment_codi import PaymentCODI
 from wire4_client.models.payment_request_codi_response_dto import PaymentRequestCodiResponseDTO
 from wire4_client.models.payments_request_id import PaymentsRequestId
+from wire4_client.models.payments_spei_and_spid_order_id import PaymentsSpeiAndSpidOrderId
+from wire4_client.models.payments_spei_and_spid_request_id import PaymentsSpeiAndSpidRequestId
 from wire4_client.models.person import Person
 from wire4_client.models.pre_enrollment_data import PreEnrollmentData
 from wire4_client.models.pre_enrollment_response import PreEnrollmentResponse
 from wire4_client.models.pre_monex_authorization import PreMonexAuthorization
+from wire4_client.models.product import Product
+from wire4_client.models.recurring_charge_request import RecurringChargeRequest
 from wire4_client.models.relationship import Relationship
 from wire4_client.models.relationships_response import RelationshipsResponse
 from wire4_client.models.sales_point import SalesPoint
 from wire4_client.models.sales_point_found import SalesPointFound
 from wire4_client.models.sales_point_request import SalesPointRequest
 from wire4_client.models.sales_point_respose import SalesPointRespose
 from wire4_client.models.service_banking import ServiceBanking
@@ -95,15 +102,17 @@
 from wire4_client.models.spid_classification_dto import SpidClassificationDTO
 from wire4_client.models.spid_classifications_response_dto import SpidClassificationsResponseDTO
 from wire4_client.models.subscription_change_status_request import SubscriptionChangeStatusRequest
 from wire4_client.models.token_required_response import TokenRequiredResponse
 from wire4_client.models.transaction_error_code import TransactionErrorCode
 from wire4_client.models.transaction_outgoing import TransactionOutgoing
 from wire4_client.models.transaction_outgoing_spid import TransactionOutgoingSpid
+from wire4_client.models.transaction_spei_spid import TransactionSpeiSpid
 from wire4_client.models.transactions_outgoing_register import TransactionsOutgoingRegister
+from wire4_client.models.transactions_register import TransactionsRegister
 from wire4_client.models.update_configurations_request_dto import UpdateConfigurationsRequestDTO
 from wire4_client.models.urls_redirect import UrlsRedirect
 from wire4_client.models.use_service_banking import UseServiceBanking
 from wire4_client.models.user_company import UserCompany
 from wire4_client.models.web_hook_deposit_authorization_request import WebHookDepositAuthorizationRequest
 from wire4_client.models.web_hook_deposit_authorization_response import WebHookDepositAuthorizationResponse
 from wire4_client.models.webhook import Webhook
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_configurations_limits.py` & `wire4-client-1.1.3/wire4_client/models/message_configurations_limits.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.configurations_limits import ConfigurationsLimits  # noqa: F401,E501
-
 
 class MessageConfigurationsLimits(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/cep_response.py` & `wire4-client-1.1.3/wire4_client/models/cep_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class CepResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/webhooks_list.py` & `wire4-client-1.1.3/wire4_client/models/webhooks_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.webhook_response import WebhookResponse  # noqa: F401,E501
-
 
 class WebhooksList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/depositants_register.py` & `wire4-client-1.1.3/wire4_client/models/depositants_register.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class DepositantsRegister(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/webhook_response.py` & `wire4-client-1.1.3/wire4_client/models/pager_response_dto.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,210 +11,203 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
-class WebhookResponse(object):
+class PagerResponseDto(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'events': 'list[str]',
-        'name': 'str',
-        'secret': 'str',
-        'status': 'str',
-        'url': 'str',
-        'wh_uuid': 'str'
+        'content': 'list[Operations]',
+        'number_of_elements': 'int',
+        'page': 'int',
+        'size': 'int',
+        'total_items': 'int',
+        'total_pages': 'int'
     }
 
     attribute_map = {
-        'events': 'events',
-        'name': 'name',
-        'secret': 'secret',
-        'status': 'status',
-        'url': 'url',
-        'wh_uuid': 'wh_uuid'
+        'content': 'content',
+        'number_of_elements': 'number_of_elements',
+        'page': 'page',
+        'size': 'size',
+        'total_items': 'total_items',
+        'total_pages': 'total_pages'
     }
 
-    def __init__(self, events=None, name=None, secret=None, status=None, url=None, wh_uuid=None):  # noqa: E501
-        """WebhookResponse - a model defined in Swagger"""  # noqa: E501
-        self._events = None
-        self._name = None
-        self._secret = None
-        self._status = None
-        self._url = None
-        self._wh_uuid = None
+    def __init__(self, content=None, number_of_elements=None, page=None, size=None, total_items=None, total_pages=None):  # noqa: E501
+        """PagerResponseDto - a model defined in Swagger"""  # noqa: E501
+        self._content = None
+        self._number_of_elements = None
+        self._page = None
+        self._size = None
+        self._total_items = None
+        self._total_pages = None
         self.discriminator = None
-        if events is not None:
-            self.events = events
-        if name is not None:
-            self.name = name
-        if secret is not None:
-            self.secret = secret
-        if status is not None:
-            self.status = status
-        if url is not None:
-            self.url = url
-        if wh_uuid is not None:
-            self.wh_uuid = wh_uuid
+        if content is not None:
+            self.content = content
+        if number_of_elements is not None:
+            self.number_of_elements = number_of_elements
+        if page is not None:
+            self.page = page
+        if size is not None:
+            self.size = size
+        if total_items is not None:
+            self.total_items = total_items
+        if total_pages is not None:
+            self.total_pages = total_pages
 
     @property
-    def events(self):
-        """Gets the events of this WebhookResponse.  # noqa: E501
+    def content(self):
+        """Gets the content of this PagerResponseDto.  # noqa: E501
 
-        Tipos de eventos de los cuales Wire4 te enviará información.  # noqa: E501
+        Es el contenido de la respuesta paginada.  # noqa: E501
 
-        :return: The events of this WebhookResponse.  # noqa: E501
-        :rtype: list[str]
+        :return: The content of this PagerResponseDto.  # noqa: E501
+        :rtype: list[Operations]
         """
-        return self._events
+        return self._content
 
-    @events.setter
-    def events(self, events):
-        """Sets the events of this WebhookResponse.
+    @content.setter
+    def content(self, content):
+        """Sets the content of this PagerResponseDto.
 
-        Tipos de eventos de los cuales Wire4 te enviará información.  # noqa: E501
+        Es el contenido de la respuesta paginada.  # noqa: E501
 
-        :param events: The events of this WebhookResponse.  # noqa: E501
-        :type: list[str]
+        :param content: The content of this PagerResponseDto.  # noqa: E501
+        :type: list[Operations]
         """
 
-        self._events = events
+        self._content = content
 
     @property
-    def name(self):
-        """Gets the name of this WebhookResponse.  # noqa: E501
+    def number_of_elements(self):
+        """Gets the number_of_elements of this PagerResponseDto.  # noqa: E501
 
-        Es el nombre del webhook.  # noqa: E501
+        Es el número de elementos en la página actual.  # noqa: E501
 
-        :return: The name of this WebhookResponse.  # noqa: E501
-        :rtype: str
+        :return: The number_of_elements of this PagerResponseDto.  # noqa: E501
+        :rtype: int
         """
-        return self._name
+        return self._number_of_elements
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this WebhookResponse.
+    @number_of_elements.setter
+    def number_of_elements(self, number_of_elements):
+        """Sets the number_of_elements of this PagerResponseDto.
 
-        Es el nombre del webhook.  # noqa: E501
+        Es el número de elementos en la página actual.  # noqa: E501
 
-        :param name: The name of this WebhookResponse.  # noqa: E501
-        :type: str
+        :param number_of_elements: The number_of_elements of this PagerResponseDto.  # noqa: E501
+        :type: int
         """
 
-        self._name = name
+        self._number_of_elements = number_of_elements
 
     @property
-    def secret(self):
-        """Gets the secret of this WebhookResponse.  # noqa: E501
+    def page(self):
+        """Gets the page of this PagerResponseDto.  # noqa: E501
 
-        Llave con la cual se debe de identificar que el webhook fue enviado por Wire4, para mayor información revisar la guía de notificaciones (https://wire4.mx/#/guides/notificaciones),  en la sección de  <a href=\"https://wire4.mx/#/guides/notificaciones\">\"Comprobación de firmas de Webhook\".</a>  # noqa: E501
+        Es el número de página.  # noqa: E501
 
-        :return: The secret of this WebhookResponse.  # noqa: E501
-        :rtype: str
+        :return: The page of this PagerResponseDto.  # noqa: E501
+        :rtype: int
         """
-        return self._secret
+        return self._page
 
-    @secret.setter
-    def secret(self, secret):
-        """Sets the secret of this WebhookResponse.
+    @page.setter
+    def page(self, page):
+        """Sets the page of this PagerResponseDto.
 
-        Llave con la cual se debe de identificar que el webhook fue enviado por Wire4, para mayor información revisar la guía de notificaciones (https://wire4.mx/#/guides/notificaciones),  en la sección de  <a href=\"https://wire4.mx/#/guides/notificaciones\">\"Comprobación de firmas de Webhook\".</a>  # noqa: E501
+        Es el número de página.  # noqa: E501
 
-        :param secret: The secret of this WebhookResponse.  # noqa: E501
-        :type: str
+        :param page: The page of this PagerResponseDto.  # noqa: E501
+        :type: int
         """
 
-        self._secret = secret
+        self._page = page
 
     @property
-    def status(self):
-        """Gets the status of this WebhookResponse.  # noqa: E501
+    def size(self):
+        """Gets the size of this PagerResponseDto.  # noqa: E501
 
-        Es el estado (estatus) en el que se encuentra el webhook.  # noqa: E501
+        Es el tamaño de la página, por ejemplo puede ser 20, que significa que son 20 registros por página.  # noqa: E501
 
-        :return: The status of this WebhookResponse.  # noqa: E501
-        :rtype: str
+        :return: The size of this PagerResponseDto.  # noqa: E501
+        :rtype: int
         """
-        return self._status
+        return self._size
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this WebhookResponse.
+    @size.setter
+    def size(self, size):
+        """Sets the size of this PagerResponseDto.
 
-        Es el estado (estatus) en el que se encuentra el webhook.  # noqa: E501
+        Es el tamaño de la página, por ejemplo puede ser 20, que significa que son 20 registros por página.  # noqa: E501
 
-        :param status: The status of this WebhookResponse.  # noqa: E501
-        :type: str
+        :param size: The size of this PagerResponseDto.  # noqa: E501
+        :type: int
         """
-        allowed_values = ["ACTIVE", "INACTIVE", "DELETED"]  # noqa: E501
-        if status not in allowed_values:
-            raise ValueError(
-                "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
-                .format(status, allowed_values)
-            )
 
-        self._status = status
+        self._size = size
 
     @property
-    def url(self):
-        """Gets the url of this WebhookResponse.  # noqa: E501
+    def total_items(self):
+        """Gets the total_items of this PagerResponseDto.  # noqa: E501
 
-        Es la dirección URL a la que Wire4 enviará las notificaciones cuando un evento ocurra.  # noqa: E501
+        Es el número total de elementos de la consulta.  # noqa: E501
 
-        :return: The url of this WebhookResponse.  # noqa: E501
-        :rtype: str
+        :return: The total_items of this PagerResponseDto.  # noqa: E501
+        :rtype: int
         """
-        return self._url
+        return self._total_items
 
-    @url.setter
-    def url(self, url):
-        """Sets the url of this WebhookResponse.
+    @total_items.setter
+    def total_items(self, total_items):
+        """Sets the total_items of this PagerResponseDto.
 
-        Es la dirección URL a la que Wire4 enviará las notificaciones cuando un evento ocurra.  # noqa: E501
+        Es el número total de elementos de la consulta.  # noqa: E501
 
-        :param url: The url of this WebhookResponse.  # noqa: E501
-        :type: str
+        :param total_items: The total_items of this PagerResponseDto.  # noqa: E501
+        :type: int
         """
 
-        self._url = url
+        self._total_items = total_items
 
     @property
-    def wh_uuid(self):
-        """Gets the wh_uuid of this WebhookResponse.  # noqa: E501
+    def total_pages(self):
+        """Gets the total_pages of this PagerResponseDto.  # noqa: E501
 
-        Es el identificador del webhook. Ejemplo: wh_54a832866f784b439bc625c0f4e04e12.  # noqa: E501
+        Es el número total de paginas.  # noqa: E501
 
-        :return: The wh_uuid of this WebhookResponse.  # noqa: E501
-        :rtype: str
+        :return: The total_pages of this PagerResponseDto.  # noqa: E501
+        :rtype: int
         """
-        return self._wh_uuid
+        return self._total_pages
 
-    @wh_uuid.setter
-    def wh_uuid(self, wh_uuid):
-        """Sets the wh_uuid of this WebhookResponse.
+    @total_pages.setter
+    def total_pages(self, total_pages):
+        """Sets the total_pages of this PagerResponseDto.
 
-        Es el identificador del webhook. Ejemplo: wh_54a832866f784b439bc625c0f4e04e12.  # noqa: E501
+        Es el número total de paginas.  # noqa: E501
 
-        :param wh_uuid: The wh_uuid of this WebhookResponse.  # noqa: E501
-        :type: str
+        :param total_pages: The total_pages of this PagerResponseDto.  # noqa: E501
+        :type: int
         """
 
-        self._wh_uuid = wh_uuid
+        self._total_pages = total_pages
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -229,15 +222,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WebhookResponse, dict):
+        if issubclass(PagerResponseDto, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -245,15 +238,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WebhookResponse):
+        if not isinstance(other, PagerResponseDto):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `wire4-client-1.1.2/wire4_client/models/depositant.py` & `wire4-client-1.1.3/wire4_client/models/depositant.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class Depositant(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/deposit_authorization_request.py` & `wire4-client-1.1.3/wire4_client/models/deposit_authorization_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.web_hook_deposit_authorization_request import WebHookDepositAuthorizationRequest  # noqa: F401,E501
-
 
 class DepositAuthorizationRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/spid_classification_dto.py` & `wire4-client-1.1.3/wire4_client/models/spid_classification_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class SpidClassificationDTO(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/user_company.py` & `wire4-client-1.1.3/wire4_client/models/user_company.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class UserCompany(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/contract_detail_response.py` & `wire4-client-1.1.3/wire4_client/models/contract_detail_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.account_detail import AccountDetail  # noqa: F401,E501
-from wire4_client.models.user_company import UserCompany  # noqa: F401,E501
-
 
 class ContractDetailResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/contract_detail_request.py` & `wire4-client-1.1.3/wire4_client/models/contract_detail_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class ContractDetailRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/operations.py` & `wire4-client-1.1.3/wire4_client/models/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.compay import Compay  # noqa: F401,E501
-from wire4_client.models.payment_codi import PaymentCODI  # noqa: F401,E501
-from wire4_client.models.sales_point import SalesPoint  # noqa: F401,E501
-
 
 class Operations(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
@@ -285,15 +281,15 @@
         """Sets the status of this Operations.
 
         Estatus de la petición  # noqa: E501
 
         :param status: The status of this Operations.  # noqa: E501
         :type: str
         """
-        allowed_values = ["RECEIVED", "COMPLETED", "CANCELLED"]  # noqa: E501
+        allowed_values = ["ACCEPTED", "RECEIVED", "COMPLETED", "CANCELLED", "POSTPONED", "REJECTED", "REVERSED", "PENDING"]  # noqa: E501
         if status not in allowed_values:
             raise ValueError(
                 "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
                 .format(status, allowed_values)
             )
 
         self._status = status
@@ -314,15 +310,15 @@
         """Sets the type of this Operations.
 
         Es el tipo de petición de cobro.  # noqa: E501
 
         :param type: The type of this Operations.  # noqa: E501
         :type: str
         """
-        allowed_values = ["PUSH_NOTIFICATION", "QR_CODE"]  # noqa: E501
+        allowed_values = ["PUSH_NOTIFICATION", "QR_CODE", "UNKNOWN"]  # noqa: E501
         if type not in allowed_values:
             raise ValueError(
                 "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
                 .format(type, allowed_values)
             )
 
         self._type = type
```

### Comparing `wire4-client-1.1.2/wire4_client/models/get_depositants.py` & `wire4-client-1.1.3/wire4_client/models/get_depositants.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.depositant import Depositant  # noqa: F401,E501
-
 
 class GetDepositants(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_deposit_authorization_request.py` & `wire4-client-1.1.3/wire4_client/models/message_deposit_authorization_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.message_institution import MessageInstitution  # noqa: F401,E501
-
 
 class MessageDepositAuthorizationRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/update_configurations_request_dto.py` & `wire4-client-1.1.3/wire4_client/models/update_configurations_request_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.configurations_limits import ConfigurationsLimits  # noqa: F401,E501
-
 
 class UpdateConfigurationsRequestDTO(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_codi_action.py` & `wire4-client-1.1.3/wire4_client/models/message_codi_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class MessageCodiAction(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/detailed_error_response.py` & `wire4-client-1.1.3/wire4_client/models/detailed_error_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.transaction_error_code import TransactionErrorCode  # noqa: F401,E501
-
 
 class DetailedErrorResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/spid_classifications_response_dto.py` & `wire4-client-1.1.3/wire4_client/models/spid_classifications_response_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.spid_classification_dto import SpidClassificationDTO  # noqa: F401,E501
-
 
 class SpidClassificationsResponseDTO(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/sales_point_respose.py` & `wire4-client-1.1.3/wire4_client/models/sales_point_respose.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.webhook import Webhook  # noqa: F401,E501
-
 
 class SalesPointRespose(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/compay.py` & `wire4-client-1.1.3/wire4_client/models/compay.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class Compay(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_user_authorized.py` & `wire4-client-1.1.3/wire4_client/models/message_user_authorized.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class MessageUserAuthorized(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/authorization_transaction_group.py` & `wire4-client-1.1.3/wire4_client/models/authorization_transaction_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.urls_redirect import UrlsRedirect  # noqa: F401,E501
-
 
 class AuthorizationTransactionGroup(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/deposits_authorization_response.py` & `wire4-client-1.1.3/wire4_client/models/deposits_authorization_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.web_hook_deposit_authorization_response import WebHookDepositAuthorizationResponse  # noqa: F401,E501
-
 
 class DepositsAuthorizationResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/use_service_banking.py` & `wire4-client-1.1.3/wire4_client/models/use_service_banking.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class UseServiceBanking(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_payment.py` & `wire4-client-1.1.3/wire4_client/models/message_payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.message_cep import MessageCEP  # noqa: F401,E501
-from wire4_client.models.message_institution import MessageInstitution  # noqa: F401,E501
-
 
 class MessagePayment(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_payment_state_pending.py` & `wire4-client-1.1.3/wire4_client/models/message_payment_state_pending.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.message_institution import MessageInstitution  # noqa: F401,E501
-
 
 class MessagePaymentStatePending(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/pre_monex_authorization.py` & `wire4-client-1.1.3/wire4_client/models/pre_monex_authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class PreMonexAuthorization(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_institution.py` & `wire4-client-1.1.3/wire4_client/models/message_institution.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class MessageInstitution(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/error_response.py` & `wire4-client-1.1.3/wire4_client/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class ErrorResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/account_response.py` & `wire4-client-1.1.3/wire4_client/models/account_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.beneficiary_institution import BeneficiaryInstitution  # noqa: F401,E501
-from wire4_client.models.institution import Institution  # noqa: F401,E501
-from wire4_client.models.person import Person  # noqa: F401,E501
-
 
 class AccountResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
@@ -29,14 +25,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'amount_limit': 'float',
+        'authorization_date': 'datetime',
         'bank': 'Institution',
         'beneficiary_account': 'str',
         'email': 'list[str]',
         'institution': 'BeneficiaryInstitution',
         'kind_of_relationship': 'str',
         'numeric_reference_spei': 'str',
         'payment_concept_spei': 'str',
@@ -45,45 +42,49 @@
         'relationship': 'str',
         'rfc': 'str',
         'status': 'str'
     }
 
     attribute_map = {
         'amount_limit': 'amount_limit',
+        'authorization_date': 'authorization_date',
         'bank': 'bank',
         'beneficiary_account': 'beneficiary_account',
         'email': 'email',
         'institution': 'institution',
         'kind_of_relationship': 'kind_of_relationship',
         'numeric_reference_spei': 'numeric_reference_spei',
         'payment_concept_spei': 'payment_concept_spei',
         'person': 'person',
         'register_date': 'register_date',
         'relationship': 'relationship',
         'rfc': 'rfc',
         'status': 'status'
     }
 
-    def __init__(self, amount_limit=None, bank=None, beneficiary_account=None, email=None, institution=None, kind_of_relationship=None, numeric_reference_spei=None, payment_concept_spei=None, person=None, register_date=None, relationship=None, rfc=None, status=None):  # noqa: E501
+    def __init__(self, amount_limit=None, authorization_date=None, bank=None, beneficiary_account=None, email=None, institution=None, kind_of_relationship=None, numeric_reference_spei=None, payment_concept_spei=None, person=None, register_date=None, relationship=None, rfc=None, status=None):  # noqa: E501
         """AccountResponse - a model defined in Swagger"""  # noqa: E501
         self._amount_limit = None
+        self._authorization_date = None
         self._bank = None
         self._beneficiary_account = None
         self._email = None
         self._institution = None
         self._kind_of_relationship = None
         self._numeric_reference_spei = None
         self._payment_concept_spei = None
         self._person = None
         self._register_date = None
         self._relationship = None
         self._rfc = None
         self._status = None
         self.discriminator = None
         self.amount_limit = amount_limit
+        if authorization_date is not None:
+            self.authorization_date = authorization_date
         if bank is not None:
             self.bank = bank
         self.beneficiary_account = beneficiary_account
         if email is not None:
             self.email = email
         if institution is not None:
             self.institution = institution
@@ -123,14 +124,37 @@
         """
         if amount_limit is None:
             raise ValueError("Invalid value for `amount_limit`, must not be `None`")  # noqa: E501
 
         self._amount_limit = amount_limit
 
     @property
+    def authorization_date(self):
+        """Gets the authorization_date of this AccountResponse.  # noqa: E501
+
+        Es la fecha en la que se autorizó el registro del beneficiario. Ésta fecha viene en formato ISO 8601 con zona horaria, ejemplo: <strong>2020-10-27T11:03:15.000-06:00</strong>.  # noqa: E501
+
+        :return: The authorization_date of this AccountResponse.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._authorization_date
+
+    @authorization_date.setter
+    def authorization_date(self, authorization_date):
+        """Sets the authorization_date of this AccountResponse.
+
+        Es la fecha en la que se autorizó el registro del beneficiario. Ésta fecha viene en formato ISO 8601 con zona horaria, ejemplo: <strong>2020-10-27T11:03:15.000-06:00</strong>.  # noqa: E501
+
+        :param authorization_date: The authorization_date of this AccountResponse.  # noqa: E501
+        :type: datetime
+        """
+
+        self._authorization_date = authorization_date
+
+    @property
     def bank(self):
         """Gets the bank of this AccountResponse.  # noqa: E501
 
 
         :return: The bank of this AccountResponse.  # noqa: E501
         :rtype: Institution
         """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/payments_request_id.py` & `wire4-client-1.1.3/wire4_client/models/payments_request_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.payment import Payment  # noqa: F401,E501
-
 
 class PaymentsRequestId(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_subscription.py` & `wire4-client-1.1.3/wire4_client/models/message_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class MessageSubscription(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/sales_point.py` & `wire4-client-1.1.3/wire4_client/models/sales_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class SalesPoint(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/payment_request_codi_response_dto.py` & `wire4-client-1.1.3/wire4_client/models/payment_request_codi_response_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.codi_operation_response_dto import CodiOperationResponseDTO  # noqa: F401,E501
-
 
 class PaymentRequestCodiResponseDTO(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/balance.py` & `wire4-client-1.1.3/wire4_client/models/balance.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class Balance(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/contact_request.py` & `wire4-client-1.1.3/wire4_client/models/contact_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class ContactRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/account_detail.py` & `wire4-client-1.1.3/wire4_client/models/account_detail.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.address_company import AddressCompany  # noqa: F401,E501
-
 
 class AccountDetail(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/message_cep.py` & `wire4-client-1.1.3/wire4_client/models/message_cep.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class MessageCEP(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/web_hook_deposit_authorization_request.py` & `wire4-client-1.1.3/wire4_client/models/web_hook_deposit_authorization_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class WebHookDepositAuthorizationRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/beneficiary_institution.py` & `wire4-client-1.1.3/wire4_client/models/beneficiary_institution.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class BeneficiaryInstitution(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/payment.py` & `wire4-client-1.1.3/wire4_client/models/payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.institution import Institution  # noqa: F401,E501
-from wire4_client.models.message_cep import MessageCEP  # noqa: F401,E501
-
 
 class Payment(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/service_banking.py` & `wire4-client-1.1.3/wire4_client/models/service_banking.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.use_service_banking import UseServiceBanking  # noqa: F401,E501
-
 
 class ServiceBanking(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/address_company.py` & `wire4-client-1.1.3/wire4_client/models/address_company.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class AddressCompany(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/item.py` & `wire4-client-1.1.3/wire4_client/models/item.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class Item(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/account.py` & `wire4-client-1.1.3/wire4_client/models/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.beneficiary_institution import BeneficiaryInstitution  # noqa: F401,E501
-from wire4_client.models.person import Person  # noqa: F401,E501
-
 
 class Account(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/models/company_registered.py` & `wire4-client-1.1.3/wire4_client/models/company_registered.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class CompanyRegistered(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
```

### Comparing `wire4-client-1.1.2/wire4_client/models/codi_operations_filters_request_dto.py` & `wire4-client-1.1.3/wire4_client/models/codi_operations_filters_request_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-
 class CodiOperationsFiltersRequestDTO(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
@@ -255,15 +254,15 @@
         """Sets the status of this CodiOperationsFiltersRequestDTO.
 
         Es el estado (estatus) de la petición.  # noqa: E501
 
         :param status: The status of this CodiOperationsFiltersRequestDTO.  # noqa: E501
         :type: str
         """
-        allowed_values = ["RECEIVED", "COMPLETED", "CANCELLED"]  # noqa: E501
+        allowed_values = ["ACCEPTED", "RECEIVED", "COMPLETED", "CANCELLED", "POSTPONED", "REJECTED", "REVERSED", "PENDING"]  # noqa: E501
         if status not in allowed_values:
             raise ValueError(
                 "Invalid value for `status` ({0}), must be one of {1}"  # noqa: E501
                 .format(status, allowed_values)
             )
 
         self._status = status
```

### Comparing `wire4-client-1.1.2/wire4_client/models/account_spid.py` & `wire4-client-1.1.3/wire4_client/models/account_spid.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from wire4_client.models.beneficiary_institution import BeneficiaryInstitution  # noqa: F401,E501
-
 
 class AccountSpid(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `wire4-client-1.1.2/wire4_client/api/contracts_details_api.py` & `wire4-client-1.1.3/wire4_client/api/contracts_details_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/comprobante_electrnico_de_pago__cep_api.py` & `wire4-client-1.1.3/wire4_client/api/comprobante_electrnico_de_pago__cep_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/transferencias_spei_api.py` & `wire4-client-1.1.3/wire4_client/api/transferencias_spei_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -476,14 +476,232 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def out_comming_spei_spid_order_id_transaction_report_using_get(self, authorization, subscription, **kwargs):  # noqa: E501
+        """Consulta de transferencias realizadas por order_id  # noqa: E501
+
+        Consulta las transferencias que regresa este recuso son únicamente las transferencias recibidas en el día en el que se realiza la consulta o las transferencias identificadas con el <strong>order_id</strong> proporcionado, para este tipo de consultas no importa el día en el que se realizó la transferencia. <br> Es importante que conozca que la respuesta puede dar como resultado un objeto con una lista spei o una lista spid con el/los elementos ya que un identificador order_id solo puede pertenecer a una transacción sea spei o spid.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.out_comming_spei_spid_order_id_transaction_report_using_get(authorization, subscription, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str authorization: Header para token (required)
+        :param str subscription: Es el identificador de la suscripción a esta API. (required)
+        :param str order_id: Es el identificador de la orden a buscar.
+        :return: PaymentsSpeiAndSpidOrderId
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.out_comming_spei_spid_order_id_transaction_report_using_get_with_http_info(authorization, subscription, **kwargs)  # noqa: E501
+        else:
+            (data) = self.out_comming_spei_spid_order_id_transaction_report_using_get_with_http_info(authorization, subscription, **kwargs)  # noqa: E501
+            return data
+
+    def out_comming_spei_spid_order_id_transaction_report_using_get_with_http_info(self, authorization, subscription, **kwargs):  # noqa: E501
+        """Consulta de transferencias realizadas por order_id  # noqa: E501
+
+        Consulta las transferencias que regresa este recuso son únicamente las transferencias recibidas en el día en el que se realiza la consulta o las transferencias identificadas con el <strong>order_id</strong> proporcionado, para este tipo de consultas no importa el día en el que se realizó la transferencia. <br> Es importante que conozca que la respuesta puede dar como resultado un objeto con una lista spei o una lista spid con el/los elementos ya que un identificador order_id solo puede pertenecer a una transacción sea spei o spid.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.out_comming_spei_spid_order_id_transaction_report_using_get_with_http_info(authorization, subscription, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str authorization: Header para token (required)
+        :param str subscription: Es el identificador de la suscripción a esta API. (required)
+        :param str order_id: Es el identificador de la orden a buscar.
+        :return: PaymentsSpeiAndSpidOrderId
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['authorization', 'subscription', 'order_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method out_comming_spei_spid_order_id_transaction_report_using_get" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'authorization' is set
+        if ('authorization' not in params or
+                params['authorization'] is None):
+            raise ValueError("Missing the required parameter `authorization` when calling `out_comming_spei_spid_order_id_transaction_report_using_get`")  # noqa: E501
+        # verify the required parameter 'subscription' is set
+        if ('subscription' not in params or
+                params['subscription'] is None):
+            raise ValueError("Missing the required parameter `subscription` when calling `out_comming_spei_spid_order_id_transaction_report_using_get`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'subscription' in params:
+            path_params['subscription'] = params['subscription']  # noqa: E501
+
+        query_params = []
+        if 'order_id' in params:
+            query_params.append(('order_id', params['order_id']))  # noqa: E501
+
+        header_params = {}
+        if 'authorization' in params:
+            header_params['Authorization'] = params['authorization']  # noqa: E501
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
+        auth_settings = []  # noqa: E501
+
+        return self.api_client.call_api(
+            '/subscriptions/{subscription}/transactions/outcoming', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PaymentsSpeiAndSpidOrderId',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def out_comming_spei_spid_request_id_transactions_report_using_get(self, authorization, request_id, subscription, **kwargs):  # noqa: E501
+        """Consulta de transferencias de salida por identificador de petición  # noqa: E501
+
+        Consulta las transferencias de salida registradas en una petición, las transferencias que regresa este recuso son únicamente las transferencias de salida agrupadas al identificador de la petición que se generó al hacer el registro de las transacciones el cuál se debe especificar como parte del path de este endpoint.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.out_comming_spei_spid_request_id_transactions_report_using_get(authorization, request_id, subscription, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str authorization: Header para token (required)
+        :param str request_id: Identificador de la petición a buscar. (required)
+        :param str subscription: Es el identificador de la suscripción a esta API. (required)
+        :return: PaymentsSpeiAndSpidRequestId
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.out_comming_spei_spid_request_id_transactions_report_using_get_with_http_info(authorization, request_id, subscription, **kwargs)  # noqa: E501
+        else:
+            (data) = self.out_comming_spei_spid_request_id_transactions_report_using_get_with_http_info(authorization, request_id, subscription, **kwargs)  # noqa: E501
+            return data
+
+    def out_comming_spei_spid_request_id_transactions_report_using_get_with_http_info(self, authorization, request_id, subscription, **kwargs):  # noqa: E501
+        """Consulta de transferencias de salida por identificador de petición  # noqa: E501
+
+        Consulta las transferencias de salida registradas en una petición, las transferencias que regresa este recuso son únicamente las transferencias de salida agrupadas al identificador de la petición que se generó al hacer el registro de las transacciones el cuál se debe especificar como parte del path de este endpoint.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.out_comming_spei_spid_request_id_transactions_report_using_get_with_http_info(authorization, request_id, subscription, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str authorization: Header para token (required)
+        :param str request_id: Identificador de la petición a buscar. (required)
+        :param str subscription: Es el identificador de la suscripción a esta API. (required)
+        :return: PaymentsSpeiAndSpidRequestId
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['authorization', 'request_id', 'subscription']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method out_comming_spei_spid_request_id_transactions_report_using_get" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'authorization' is set
+        if ('authorization' not in params or
+                params['authorization'] is None):
+            raise ValueError("Missing the required parameter `authorization` when calling `out_comming_spei_spid_request_id_transactions_report_using_get`")  # noqa: E501
+        # verify the required parameter 'request_id' is set
+        if ('request_id' not in params or
+                params['request_id'] is None):
+            raise ValueError("Missing the required parameter `request_id` when calling `out_comming_spei_spid_request_id_transactions_report_using_get`")  # noqa: E501
+        # verify the required parameter 'subscription' is set
+        if ('subscription' not in params or
+                params['subscription'] is None):
+            raise ValueError("Missing the required parameter `subscription` when calling `out_comming_spei_spid_request_id_transactions_report_using_get`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'request_id' in params:
+            path_params['requestId'] = params['request_id']  # noqa: E501
+        if 'subscription' in params:
+            path_params['subscription'] = params['subscription']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+        if 'authorization' in params:
+            header_params['Authorization'] = params['authorization']  # noqa: E501
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
+        auth_settings = []  # noqa: E501
+
+        return self.api_client.call_api(
+            '/subscriptions/{subscription}/transactions/outcoming/{requestId}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PaymentsSpeiAndSpidRequestId',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def outgoing_spei_transactions_report_using_get(self, authorization, subscription, **kwargs):  # noqa: E501
         """Consulta de transferencias realizadas  # noqa: E501
 
         Consulta las transferencias realizadas en la cuenta del cliente Monex relacionada a la suscripción, las transferencias que regresa este recuso son únicamente las transferencias recibidas en el día en el que se realiza la consulta.<br>Se pueden realizar consultas por <strong>order_id</strong> al realizar este tipo de consultas no importa el día en el que se realizó la transferencia  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.outgoing_spei_transactions_report_using_get(authorization, subscription, async_req=True)
@@ -691,13 +909,128 @@
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='TokenRequiredResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def register_spei_spid_outgoing_transactions_using_post(self, body, authorization, subscription, **kwargs):  # noqa: E501
+        """Registro de transferencias SPEI y SPID  # noqa: E501
+
+        Se registra un conjunto de transferencias (una o más) tanto SPEI como SPID en una sola petición en la cuenta del cliente Monex relacionada a la suscripción. En la respuesta se proporcionará una dirección URL que lo llevará al centro de autorización para que las transferencias sean confirmadas (autorizadas) por el cliente para que se efectúen, para ello debe ingresar la llave electrónica (Token).<br>  Nota: Debe considerar que el concepto de cada una de las transacciones solo debe contener caracteres alfanuméricos por lo que en caso de que se reciban caracteres como ñ o acentos serán sustituidos por n o en su caso por la letra sin acento. Los caracteres no alfanuméricos como pueden ser caracteres especiales serán eliminados.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.register_spei_spid_outgoing_transactions_using_post(body, authorization, subscription, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param TransactionsRegister body: Información de las transferencias SPEI y SPID de salida (required)
+        :param str authorization: Header para token (required)
+        :param str subscription: Es el identificador de la suscripción a esta API. (required)
+        :return: TokenRequiredResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.register_spei_spid_outgoing_transactions_using_post_with_http_info(body, authorization, subscription, **kwargs)  # noqa: E501
+        else:
+            (data) = self.register_spei_spid_outgoing_transactions_using_post_with_http_info(body, authorization, subscription, **kwargs)  # noqa: E501
+            return data
+
+    def register_spei_spid_outgoing_transactions_using_post_with_http_info(self, body, authorization, subscription, **kwargs):  # noqa: E501
+        """Registro de transferencias SPEI y SPID  # noqa: E501
+
+        Se registra un conjunto de transferencias (una o más) tanto SPEI como SPID en una sola petición en la cuenta del cliente Monex relacionada a la suscripción. En la respuesta se proporcionará una dirección URL que lo llevará al centro de autorización para que las transferencias sean confirmadas (autorizadas) por el cliente para que se efectúen, para ello debe ingresar la llave electrónica (Token).<br>  Nota: Debe considerar que el concepto de cada una de las transacciones solo debe contener caracteres alfanuméricos por lo que en caso de que se reciban caracteres como ñ o acentos serán sustituidos por n o en su caso por la letra sin acento. Los caracteres no alfanuméricos como pueden ser caracteres especiales serán eliminados.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.register_spei_spid_outgoing_transactions_using_post_with_http_info(body, authorization, subscription, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param TransactionsRegister body: Información de las transferencias SPEI y SPID de salida (required)
+        :param str authorization: Header para token (required)
+        :param str subscription: Es el identificador de la suscripción a esta API. (required)
+        :return: TokenRequiredResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body', 'authorization', 'subscription']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method register_spei_spid_outgoing_transactions_using_post" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `register_spei_spid_outgoing_transactions_using_post`")  # noqa: E501
+        # verify the required parameter 'authorization' is set
+        if ('authorization' not in params or
+                params['authorization'] is None):
+            raise ValueError("Missing the required parameter `authorization` when calling `register_spei_spid_outgoing_transactions_using_post`")  # noqa: E501
+        # verify the required parameter 'subscription' is set
+        if ('subscription' not in params or
+                params['subscription'] is None):
+            raise ValueError("Missing the required parameter `subscription` when calling `register_spei_spid_outgoing_transactions_using_post`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'subscription' in params:
+            path_params['subscription'] = params['subscription']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+        if 'authorization' in params:
+            header_params['Authorization'] = params['authorization']  # noqa: E501
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = []  # noqa: E501
+
+        return self.api_client.call_api(
+            '/subscriptions/{subscription}/transactions/outcoming', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='TokenRequiredResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `wire4-client-1.1.2/wire4_client/api/lmites_de_montos_api.py` & `wire4-client-1.1.3/wire4_client/api/lmites_de_montos_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/__init__.py` & `wire4-client-1.1.3/wire4_client/api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import absolute_import
 
 # flake8: noqa
 
 # import apis into api package
 from wire4_client.api.autorizacin_de_depsitos_api import AutorizacinDeDepsitosApi
+from wire4_client.api.cargos_recurrentes_api import CargosRecurrentesApi
 from wire4_client.api.comprobante_electrnico_de_pago__cep_api import ComprobanteElectrnicoDePagoCEPApi
 from wire4_client.api.contacto_api import ContactoApi
 from wire4_client.api.contracts_details_api import ContractsDetailsApi
 from wire4_client.api.cuentas_de_beneficiarios_spei_api import CuentasDeBeneficiariosSPEIApi
 from wire4_client.api.cuentas_de_beneficiarios_spid_api import CuentasDeBeneficiariosSPIDApi
 from wire4_client.api.depositantes_api import DepositantesApi
 from wire4_client.api.empresas_co_di_api import EmpresasCoDiApi
```

### Comparing `wire4-client-1.1.2/wire4_client/api/transferencias_spid_api.py` & `wire4-client-1.1.3/wire4_client/api/transferencias_spid_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/saldo_api.py` & `wire4-client-1.1.3/wire4_client/api/saldo_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/peticiones_de_pago_por_co_di_api.py` & `wire4-client-1.1.3/wire4_client/api/peticiones_de_pago_por_co_di_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/operaciones_co_di_api.py` & `wire4-client-1.1.3/wire4_client/api/operaciones_co_di_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/puntos_de_venta_co_di_api.py` & `wire4-client-1.1.3/wire4_client/api/puntos_de_venta_co_di_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/instituciones_api.py` & `wire4-client-1.1.3/wire4_client/api/instituciones_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/webhooks_api.py` & `wire4-client-1.1.3/wire4_client/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/cuentas_de_beneficiarios_spid_api.py` & `wire4-client-1.1.3/wire4_client/api/cuentas_de_beneficiarios_spid_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         :param str authorization: Header para token (required)
         :param str subscription: Es el identificador de la suscripción a esta API. (required)
         :param str account: Cuenta del beneficiario, puede ser CLABE (18 dígitos), Tarjeta de débito  (TDD, 16 dígitos) o número de celular (10 dígitos).
         :param str beneficiary_bank: Es la clave del banco beneficiario. Se puede obtener del catalogo de <a href=\"#operation/getAllInstitutionsUsingGET\">instituciones.</a>
         :param str beneficiary_name: Es el nombre del beneficiario.
         :param str end_date: Es la fecha de inicio del periodo a filtrar en formato dd-mm-yyyy.
         :param str init_date: Es la fecha de inicio del periodo a filtrar en formato dd-mm-yyyy.
+        :param str page: Es el número de página.
         :param str rfc: Es el Registro Federal de Contribuyentes (RFC) del beneficiario.
+        :param str size: Es el tamaño de página.
         :param str status: Es el estado (estatus) de la cuenta, Los valores pueden ser <b>PENDING</b> y <b>REGISTERED</b>.
         :return: SpidBeneficiariesResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -75,22 +77,24 @@
         :param str authorization: Header para token (required)
         :param str subscription: Es el identificador de la suscripción a esta API. (required)
         :param str account: Cuenta del beneficiario, puede ser CLABE (18 dígitos), Tarjeta de débito  (TDD, 16 dígitos) o número de celular (10 dígitos).
         :param str beneficiary_bank: Es la clave del banco beneficiario. Se puede obtener del catalogo de <a href=\"#operation/getAllInstitutionsUsingGET\">instituciones.</a>
         :param str beneficiary_name: Es el nombre del beneficiario.
         :param str end_date: Es la fecha de inicio del periodo a filtrar en formato dd-mm-yyyy.
         :param str init_date: Es la fecha de inicio del periodo a filtrar en formato dd-mm-yyyy.
+        :param str page: Es el número de página.
         :param str rfc: Es el Registro Federal de Contribuyentes (RFC) del beneficiario.
+        :param str size: Es el tamaño de página.
         :param str status: Es el estado (estatus) de la cuenta, Los valores pueden ser <b>PENDING</b> y <b>REGISTERED</b>.
         :return: SpidBeneficiariesResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['authorization', 'subscription', 'account', 'beneficiary_bank', 'beneficiary_name', 'end_date', 'init_date', 'rfc', 'status']  # noqa: E501
+        all_params = ['authorization', 'subscription', 'account', 'beneficiary_bank', 'beneficiary_name', 'end_date', 'init_date', 'page', 'rfc', 'size', 'status']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -123,16 +127,20 @@
             query_params.append(('beneficiary_bank', params['beneficiary_bank']))  # noqa: E501
         if 'beneficiary_name' in params:
             query_params.append(('beneficiary_name', params['beneficiary_name']))  # noqa: E501
         if 'end_date' in params:
             query_params.append(('end_date', params['end_date']))  # noqa: E501
         if 'init_date' in params:
             query_params.append(('init_date', params['init_date']))  # noqa: E501
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
         if 'rfc' in params:
             query_params.append(('rfc', params['rfc']))  # noqa: E501
+        if 'size' in params:
+            query_params.append(('size', params['size']))  # noqa: E501
         if 'status' in params:
             query_params.append(('status', params['status']))  # noqa: E501
 
         header_params = {}
         if 'authorization' in params:
             header_params['Authorization'] = params['authorization']  # noqa: E501
```

### Comparing `wire4-client-1.1.2/wire4_client/api/facturas_api.py` & `wire4-client-1.1.3/wire4_client/api/facturas_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/cuentas_de_beneficiarios_spei_api.py` & `wire4-client-1.1.3/wire4_client/api/cuentas_de_beneficiarios_spei_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -481,15 +481,17 @@
         :param str authorization: Header para token (required)
         :param str subscription: Es el identificador de la suscripción a esta API. (required)
         :param str account: Es la cuenta del beneficiario, podría ser teléfono celular (es de 10 dígitos), Tarjeta de débito (TDD, es de 16 dígitos) o cuenta CLABE (es de 18 dígitos). <br/><br/>Por ejemplo Teléfono celular: 5525072600, TDD: 4323 1234 5678 9123, CLABE: 032180000118359719.
         :param str beneficiary_bank: Es la clave del banco beneficiario. Se puede obtener del recurso de las <a href=\"#operation/getAllInstitutionsUsingGET\">instituciones.</a>
         :param str beneficiary_name: Es el nombre del beneficiario.
         :param str end_date: Es la fecha de inicio del perido a filtrar en formato dd-mm-yyyy.
         :param str init_date: Es la fºecha de inicio del perido a filtrar en formato dd-mm-yyyy.
+        :param str page: Es el número de página.
         :param str rfc: Es el Registro Federal de Controbuyentes (RFC) del beneficiario.
+        :param str size: Es el tamaño de página.
         :param str status: Es el estado (estatus) de la cuenta. Los valores pueden ser <b>PENDING</b> y <b>REGISTERED</b>.
         :return: BeneficiariesResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -511,22 +513,24 @@
         :param str authorization: Header para token (required)
         :param str subscription: Es el identificador de la suscripción a esta API. (required)
         :param str account: Es la cuenta del beneficiario, podría ser teléfono celular (es de 10 dígitos), Tarjeta de débito (TDD, es de 16 dígitos) o cuenta CLABE (es de 18 dígitos). <br/><br/>Por ejemplo Teléfono celular: 5525072600, TDD: 4323 1234 5678 9123, CLABE: 032180000118359719.
         :param str beneficiary_bank: Es la clave del banco beneficiario. Se puede obtener del recurso de las <a href=\"#operation/getAllInstitutionsUsingGET\">instituciones.</a>
         :param str beneficiary_name: Es el nombre del beneficiario.
         :param str end_date: Es la fecha de inicio del perido a filtrar en formato dd-mm-yyyy.
         :param str init_date: Es la fºecha de inicio del perido a filtrar en formato dd-mm-yyyy.
+        :param str page: Es el número de página.
         :param str rfc: Es el Registro Federal de Controbuyentes (RFC) del beneficiario.
+        :param str size: Es el tamaño de página.
         :param str status: Es el estado (estatus) de la cuenta. Los valores pueden ser <b>PENDING</b> y <b>REGISTERED</b>.
         :return: BeneficiariesResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['authorization', 'subscription', 'account', 'beneficiary_bank', 'beneficiary_name', 'end_date', 'init_date', 'rfc', 'status']  # noqa: E501
+        all_params = ['authorization', 'subscription', 'account', 'beneficiary_bank', 'beneficiary_name', 'end_date', 'init_date', 'page', 'rfc', 'size', 'status']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -559,16 +563,20 @@
             query_params.append(('beneficiary_bank', params['beneficiary_bank']))  # noqa: E501
         if 'beneficiary_name' in params:
             query_params.append(('beneficiary_name', params['beneficiary_name']))  # noqa: E501
         if 'end_date' in params:
             query_params.append(('end_date', params['end_date']))  # noqa: E501
         if 'init_date' in params:
             query_params.append(('init_date', params['init_date']))  # noqa: E501
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
         if 'rfc' in params:
             query_params.append(('rfc', params['rfc']))  # noqa: E501
+        if 'size' in params:
+            query_params.append(('size', params['size']))  # noqa: E501
         if 'status' in params:
             query_params.append(('status', params['status']))  # noqa: E501
 
         header_params = {}
         if 'authorization' in params:
             header_params['Authorization'] = params['authorization']  # noqa: E501
```

### Comparing `wire4-client-1.1.2/wire4_client/api/suscripciones_api.py` & `wire4-client-1.1.3/wire4_client/api/suscripciones_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/autorizacin_de_depsitos_api.py` & `wire4-client-1.1.3/wire4_client/api/autorizacin_de_depsitos_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/contacto_api.py` & `wire4-client-1.1.3/wire4_client/api/contacto_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api/depositantes_api.py` & `wire4-client-1.1.3/wire4_client/api/depositantes_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def get_depositants_totals_using_get(self, authorization, subscription, **kwargs):  # noqa: E501
-        """Consulta cuantas cuentas de depositantes existen  # noqa: E501
+        """Número de depositantes por suscripción  # noqa: E501
 
         Obtiene la cantidad el total de depositantes asociados al contrato relacionado a la suscripción.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_depositants_totals_using_get(authorization, subscription, async_req=True)
         >>> result = thread.get()
 
@@ -52,15 +52,15 @@
         if kwargs.get('async_req'):
             return self.get_depositants_totals_using_get_with_http_info(authorization, subscription, **kwargs)  # noqa: E501
         else:
             (data) = self.get_depositants_totals_using_get_with_http_info(authorization, subscription, **kwargs)  # noqa: E501
             return data
 
     def get_depositants_totals_using_get_with_http_info(self, authorization, subscription, **kwargs):  # noqa: E501
-        """Consulta cuantas cuentas de depositantes existen  # noqa: E501
+        """Número de depositantes por suscripción  # noqa: E501
 
         Obtiene la cantidad el total de depositantes asociados al contrato relacionado a la suscripción.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_depositants_totals_using_get_with_http_info(authorization, subscription, async_req=True)
         >>> result = thread.get()
 
@@ -131,15 +131,14 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-
     def get_depositants_using_get(self, authorization, subscription, **kwargs):  # noqa: E501
         """Consulta de cuentas de depositantes  # noqa: E501
 
         Obtiene una lista de depositantes asociados al contrato relacionado a la suscripción.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_depositants_using_get(authorization, subscription, async_req=True)
@@ -238,15 +237,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def register_depositants_using_post(self, body, authorization, subscription, **kwargs):  # noqa: E501
         """Registra un nuevo depositante  # noqa: E501
 
-        Registra un nuevo depositante en el contrato asociado a la suscripción.  # noqa: E501
+        Registra un nuevo depositante en el contrato asociado a la suscripción. Si intenta registrar un depositante que previamente se había registrado, se devolverá la cuenta clabe asociada al Álias que está intentando registrar. Queda bajo responsabilidad del cliente verificar que los álias sean únicos en sus sistemas.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.register_depositants_using_post(body, authorization, subscription, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param DepositantsRegister body: Depositant info (required)
@@ -262,15 +261,15 @@
         else:
             (data) = self.register_depositants_using_post_with_http_info(body, authorization, subscription, **kwargs)  # noqa: E501
             return data
 
     def register_depositants_using_post_with_http_info(self, body, authorization, subscription, **kwargs):  # noqa: E501
         """Registra un nuevo depositante  # noqa: E501
 
-        Registra un nuevo depositante en el contrato asociado a la suscripción.  # noqa: E501
+        Registra un nuevo depositante en el contrato asociado a la suscripción. Si intenta registrar un depositante que previamente se había registrado, se devolverá la cuenta clabe asociada al Álias que está intentando registrar. Queda bajo responsabilidad del cliente verificar que los álias sean únicos en sus sistemas.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.register_depositants_using_post_with_http_info(body, authorization, subscription, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param DepositantsRegister body: Depositant info (required)
```

### Comparing `wire4-client-1.1.2/wire4_client/api/empresas_co_di_api.py` & `wire4-client-1.1.3/wire4_client/api/empresas_co_di_api.py`

 * *Files identical despite different names*

### Comparing `wire4-client-1.1.2/wire4_client/api_client.py` & `wire4-client-1.1.3/wire4_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,18 +519,22 @@
         os.remove(path)
 
         content_disposition = response.getheader("Content-Disposition")
         if content_disposition:
             filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
                                  content_disposition).group(1)
             path = os.path.join(os.path.dirname(path), filename)
-
-        with open(path, "wb") as f:
-            f.write(response.data)
-
+            response_data = response.data
+            with open(path, "wb") as f:
+                if isinstance(response_data, str):
+                    # change str to bytes so we can write it
+                    response_data = response_data.encode('utf-8')
+                    f.write(response_data)
+                else:
+                    f.write(response_data)
         return path
 
     def __deserialize_primitive(self, data, klass):
         """Deserializes string to primitive type.
 
         :param data: str.
         :param klass: class literal.
```

### Comparing `wire4-client-1.1.2/wire4_client.egg-info/SOURCES.txt` & `wire4-client-1.1.3/wire4_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,36 +13,40 @@
 test/test_authorized_beneficiaries_response.py
 test/test_authorized_users.py
 test/test_autorizacin_de_depsitos_api.py
 test/test_balance.py
 test/test_balance_list_response.py
 test/test_beneficiaries_query_register_status.py
 test/test_beneficiaries_response.py
+test/test_beneficiary_dto.py
 test/test_beneficiary_institution.py
 test/test_billing.py
 test/test_billing_transaction.py
+test/test_cargos_recurrentes_api.py
 test/test_cep_response.py
 test/test_cep_search_banxico.py
 test/test_certificate_request.py
 test/test_codi_code_qr_response_dto.py
 test/test_codi_code_request_dto.py
 test/test_codi_operation_response_dto.py
 test/test_codi_operations_filters_request_dto.py
 test/test_company_registered.py
 test/test_company_requested.py
 test/test_compay.py
 test/test_comprobante_electrnico_de_pago__cep_api.py
 test/test_configurations_limits.py
+test/test_confirm_recurring_charge.py
 test/test_contact_request.py
 test/test_contacto_api.py
 test/test_contract_detail_request.py
 test/test_contract_detail_response.py
 test/test_contracts_details_api.py
 test/test_cuentas_de_beneficiarios_spei_api.py
 test/test_cuentas_de_beneficiarios_spid_api.py
+test/test_customer.py
 test/test_deposit.py
 test/test_deposit_authorization_request.py
 test/test_depositant.py
 test/test_depositant_count_response.py
 test/test_depositantes_api.py
 test/test_depositants_register.py
 test/test_depositants_response.py
@@ -74,20 +78,24 @@
 test/test_operaciones_co_di_api.py
 test/test_operations.py
 test/test_pager_response_dto.py
 test/test_payment.py
 test/test_payment_codi.py
 test/test_payment_request_codi_response_dto.py
 test/test_payments_request_id.py
+test/test_payments_spei_and_spid_order_id.py
+test/test_payments_spei_and_spid_request_id.py
 test/test_person.py
 test/test_peticiones_de_pago_por_co_di_api.py
 test/test_pre_enrollment_data.py
 test/test_pre_enrollment_response.py
 test/test_pre_monex_authorization.py
+test/test_product.py
 test/test_puntos_de_venta_co_di_api.py
+test/test_recurring_charge_request.py
 test/test_relationship.py
 test/test_relationships_response.py
 test/test_saldo_api.py
 test/test_sales_point.py
 test/test_sales_point_found.py
 test/test_sales_point_request.py
 test/test_sales_point_respose.py
@@ -98,15 +106,17 @@
 test/test_spid_classifications_response_dto.py
 test/test_subscription_change_status_request.py
 test/test_suscripciones_api.py
 test/test_token_required_response.py
 test/test_transaction_error_code.py
 test/test_transaction_outgoing.py
 test/test_transaction_outgoing_spid.py
+test/test_transaction_spei_spid.py
 test/test_transactions_outgoing_register.py
+test/test_transactions_register.py
 test/test_transferencias_spei_api.py
 test/test_transferencias_spid_api.py
 test/test_update_configurations_request_dto.py
 test/test_urls_redirect.py
 test/test_use_service_banking.py
 test/test_user_company.py
 test/test_web_hook_deposit_authorization_request.py
@@ -123,14 +133,15 @@
 wire4_client.egg-info/PKG-INFO
 wire4_client.egg-info/SOURCES.txt
 wire4_client.egg-info/dependency_links.txt
 wire4_client.egg-info/requires.txt
 wire4_client.egg-info/top_level.txt
 wire4_client/api/__init__.py
 wire4_client/api/autorizacin_de_depsitos_api.py
+wire4_client/api/cargos_recurrentes_api.py
 wire4_client/api/comprobante_electrnico_de_pago__cep_api.py
 wire4_client/api/contacto_api.py
 wire4_client/api/contracts_details_api.py
 wire4_client/api/cuentas_de_beneficiarios_spei_api.py
 wire4_client/api/cuentas_de_beneficiarios_spid_api.py
 wire4_client/api/depositantes_api.py
 wire4_client/api/empresas_co_di_api.py
@@ -157,31 +168,34 @@
 wire4_client/models/authorization_transaction_group.py
 wire4_client/models/authorized_beneficiaries_response.py
 wire4_client/models/authorized_users.py
 wire4_client/models/balance.py
 wire4_client/models/balance_list_response.py
 wire4_client/models/beneficiaries_query_register_status.py
 wire4_client/models/beneficiaries_response.py
+wire4_client/models/beneficiary_dto.py
 wire4_client/models/beneficiary_institution.py
 wire4_client/models/billing.py
 wire4_client/models/billing_transaction.py
 wire4_client/models/cep_response.py
 wire4_client/models/cep_search_banxico.py
 wire4_client/models/certificate_request.py
 wire4_client/models/codi_code_qr_response_dto.py
 wire4_client/models/codi_code_request_dto.py
 wire4_client/models/codi_operation_response_dto.py
 wire4_client/models/codi_operations_filters_request_dto.py
 wire4_client/models/company_registered.py
 wire4_client/models/company_requested.py
 wire4_client/models/compay.py
 wire4_client/models/configurations_limits.py
+wire4_client/models/confirm_recurring_charge.py
 wire4_client/models/contact_request.py
 wire4_client/models/contract_detail_request.py
 wire4_client/models/contract_detail_response.py
+wire4_client/models/customer.py
 wire4_client/models/deposit.py
 wire4_client/models/deposit_authorization_request.py
 wire4_client/models/depositant.py
 wire4_client/models/depositant_count_response.py
 wire4_client/models/depositants_register.py
 wire4_client/models/depositants_response.py
 wire4_client/models/deposits_authorization_response.py
@@ -207,18 +221,22 @@
 wire4_client/models/message_web_hook.py
 wire4_client/models/operations.py
 wire4_client/models/pager_response_dto.py
 wire4_client/models/payment.py
 wire4_client/models/payment_codi.py
 wire4_client/models/payment_request_codi_response_dto.py
 wire4_client/models/payments_request_id.py
+wire4_client/models/payments_spei_and_spid_order_id.py
+wire4_client/models/payments_spei_and_spid_request_id.py
 wire4_client/models/person.py
 wire4_client/models/pre_enrollment_data.py
 wire4_client/models/pre_enrollment_response.py
 wire4_client/models/pre_monex_authorization.py
+wire4_client/models/product.py
+wire4_client/models/recurring_charge_request.py
 wire4_client/models/relationship.py
 wire4_client/models/relationships_response.py
 wire4_client/models/sales_point.py
 wire4_client/models/sales_point_found.py
 wire4_client/models/sales_point_request.py
 wire4_client/models/sales_point_respose.py
 wire4_client/models/service_banking.py
@@ -227,15 +245,17 @@
 wire4_client/models/spid_classification_dto.py
 wire4_client/models/spid_classifications_response_dto.py
 wire4_client/models/subscription_change_status_request.py
 wire4_client/models/token_required_response.py
 wire4_client/models/transaction_error_code.py
 wire4_client/models/transaction_outgoing.py
 wire4_client/models/transaction_outgoing_spid.py
+wire4_client/models/transaction_spei_spid.py
 wire4_client/models/transactions_outgoing_register.py
+wire4_client/models/transactions_register.py
 wire4_client/models/update_configurations_request_dto.py
 wire4_client/models/urls_redirect.py
 wire4_client/models/use_service_banking.py
 wire4_client/models/user_company.py
 wire4_client/models/web_hook_deposit_authorization_request.py
 wire4_client/models/web_hook_deposit_authorization_response.py
 wire4_client/models/webhook.py
```

