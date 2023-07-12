# Comparing `tmp/iparapheur-provisioning-1.7.0.tar.gz` & `tmp/iparapheur-provisioning-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-provisioning-1.7.0.tar", last modified: Thu Jun 22 14:40:21 2023, max compression
+gzip compressed data, was "iparapheur-provisioning-1.7.1.tar", last modified: Wed Jul 12 16:47:15 2023, max compression
```

## Comparing `iparapheur-provisioning-1.7.0.tar` & `iparapheur-provisioning-1.7.1.tar`

### file list

```diff
@@ -1,264 +1,314 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.087868 iparapheur-provisioning-1.7.0/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-22 14:40:21.087868 iparapheur-provisioning-1.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18391 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.047867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/
--rw-r--r--   0 root         (0) root         (0)      907 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58620 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.051867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5602 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.051867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      250 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
--rw-r--r--   0 root         (0) root         (0)      315 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.055867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      512 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_all_users_api.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_tenant_api.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)    15677 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.059867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-06-22 14:38:57.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    24041 2023-06-22 14:38:59.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/desk_dto.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-22 14:39:00.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-06-22 14:39:00.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)     4891 2023-06-22 14:39:00.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     2680 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3284 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     7908 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     9141 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/sort_object.py
--rw-r--r--   0 root         (0) root         (0)    28616 2023-06-22 14:39:04.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     9365 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/type_representation.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-06-22 14:39:06.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    29666 2023-06-22 14:39:06.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_dto.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.059867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/models/
--rw-r--r--   0 root         (0) root         (0)     3743 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.059867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/
--rw-r--r--   0 root         (0) root         (0)     1942 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.059867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13629 2023-06-22 14:39:14.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11083 2023-06-22 14:39:14.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11332 2023-06-22 14:39:14.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15808 2023-06-22 14:39:14.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15034 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
--rw-r--r--   0 root         (0) root         (0)    16302 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-06-22 14:39:10.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11677 2023-06-22 14:39:10.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16545 2023-06-22 14:39:10.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15486 2023-06-22 14:39:12.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
--rw-r--r--   0 root         (0) root         (0)    16907 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11413 2023-06-22 14:39:12.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-06-22 14:39:12.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16979 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.063867 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14728 2023-06-22 14:39:19.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
--rw-r--r--   0 root         (0) root         (0)    15777 2023-06-22 14:39:18.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-06-22 14:39:18.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-06-22 14:39:19.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15521 2023-06-22 14:39:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)      449 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15050 2023-06-22 14:39:19.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)      471 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11672 2023-06-22 14:39:18.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11934 2023-06-22 14:39:18.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16645 2023-06-22 14:39:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15944 2023-06-22 14:39:16.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
--rw-r--r--   0 root         (0) root         (0)    15781 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-06-22 14:39:16.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11580 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16046 2023-06-22 14:39:16.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.067868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-06-22 14:39:08.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.071868 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11207 2023-06-22 14:39:08.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11978 2023-06-22 14:39:08.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15946 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/rest.py
--rw-r--r--   0 root         (0) root         (0)    97752 2023-06-22 14:39:22.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.051867 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-22 14:40:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15193 2023-06-22 14:40:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:40:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-22 14:40:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-22 14:40:20.000000 iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-22 14:40:21.087868 iparapheur-provisioning-1.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.043867 iparapheur-provisioning-1.7.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.075868 iparapheur-provisioning-1.7.0/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-22 14:38:57.000000 iparapheur-provisioning-1.7.0/test/test_models/test_delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-22 14:38:59.000000 iparapheur-provisioning-1.7.0/test/test_models/test_desk_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-22 14:39:00.000000 iparapheur-provisioning-1.7.0/test/test_models/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-22 14:39:00.000000 iparapheur-provisioning-1.7.0/test/test_models/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-06-22 14:39:01.000000 iparapheur-provisioning-1.7.0/test/test_models/test_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/test/test_models/test_metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/test/test_models/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/test/test_models/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/test/test_models/test_page_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-22 14:39:02.000000 iparapheur-provisioning-1.7.0/test/test_models/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-06-22 14:39:03.000000 iparapheur-provisioning-1.7.0/test/test_models/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-22 14:39:04.000000 iparapheur-provisioning-1.7.0/test/test_models/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-22 14:39:04.000000 iparapheur-provisioning-1.7.0/test/test_models/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-22 14:39:05.000000 iparapheur-provisioning-1.7.0/test/test_models/test_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-22 14:39:06.000000 iparapheur-provisioning-1.7.0/test/test_models/test_typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-22 14:39:06.000000 iparapheur-provisioning-1.7.0/test/test_models/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/test/test_models/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/test/test_models/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/test/test_models/test_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-22 14:39:07.000000 iparapheur-provisioning-1.7.0/test/test_models/test_workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.075868 iparapheur-provisioning-1.7.0/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-22 14:39:15.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-06-22 14:39:11.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-06-22 14:39:13.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.079868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-06-22 14:39:21.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-06-22 14:39:17.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.083868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:40:21.087868 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-22 14:39:09.000000 iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20775 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.009614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58620 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.009614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.013614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      261 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+-rw-r--r--   0 root         (0) root         (0)      315 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
+-rw-r--r--   0 root         (0) root         (0)      338 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      210 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.013614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      622 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_all_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_tenant_api.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py
+-rw-r--r--   0 root         (0) root         (0)    15677 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-07-12 16:45:38.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    24041 2023-07-12 16:45:40.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-07-12 16:45:41.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     7908 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9141 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9205 2023-07-12 16:45:45.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-07-12 16:45:45.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-07-12 16:45:45.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-07-12 16:45:46.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-07-12 16:45:46.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9232 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     6982 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/seal_certificate_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4500 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)    29448 2023-07-12 16:45:49.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     9365 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-07-12 16:45:52.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-12 16:45:53.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-07-12 16:45:53.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     4499 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/models/
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13070 2023-07-12 16:46:08.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2023-07-12 16:46:08.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11332 2023-07-12 16:46:08.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15034 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
+-rw-r--r--   0 root         (0) root         (0)    16302 2023-07-12 16:45:58.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-07-12 16:45:58.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2023-07-12 16:45:59.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16545 2023-07-12 16:45:59.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15486 2023-07-12 16:46:02.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
+-rw-r--r--   0 root         (0) root         (0)    16907 2023-07-12 16:46:01.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11413 2023-07-12 16:46:01.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-07-12 16:46:02.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16979 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14894 2023-07-12 16:46:05.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py
+-rw-r--r--   0 root         (0) root         (0)    19934 2023-07-12 16:46:04.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12091 2023-07-12 16:46:04.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    12371 2023-07-12 16:46:05.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    20252 2023-07-12 16:46:06.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14728 2023-07-12 16:46:15.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15777 2023-07-12 16:46:12.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-07-12 16:46:13.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-07-12 16:46:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15050 2023-07-12 16:46:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-07-12 16:46:12.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-07-12 16:46:13.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11934 2023-07-12 16:46:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16645 2023-07-12 16:46:15.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15944 2023-07-12 16:46:10.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    15781 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2023-07-12 16:46:10.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16046 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
+-rw-r--r--   0 root         (0) root         (0)      429 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15256 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
+-rw-r--r--   0 root         (0) root         (0)      477 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11623 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-07-12 16:45:56.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11207 2023-07-12 16:45:55.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11978 2023-07-12 16:45:56.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/rest.py
+-rw-r--r--   0 root         (0) root         (0)    97752 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.009614 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-12 16:47:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19038 2023-07-12 16:47:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 16:47:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-12 16:47:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 16:47:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.005614 iparapheur-provisioning-1.7.1/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.037614 iparapheur-provisioning-1.7.1/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-07-12 16:45:39.000000 iparapheur-provisioning-1.7.1/test/test_models/test_delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-07-12 16:45:41.000000 iparapheur-provisioning-1.7.1/test/test_models/test_desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-12 16:45:41.000000 iparapheur-provisioning-1.7.1/test/test_models/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/test/test_models/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/test/test_models/test_layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/test/test_models/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/test/test_models/test_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/test/test_models/test_metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/test/test_models/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-07-12 16:45:45.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-07-12 16:45:45.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-07-12 16:45:46.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-12 16:45:46.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-12 16:45:46.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      763 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/test/test_models/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/test/test_models/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_seal_certificate_dto.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/test/test_models/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/test/test_models/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/test/test_models/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/test/test_models/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/test/test_models/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-07-12 16:45:53.000000 iparapheur-provisioning-1.7.1/test/test_models/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-12 16:45:53.000000 iparapheur-provisioning-1.7.1/test/test_models/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/test/test_models/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/test/test_models/test_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/test/test_models/test_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/test/test_models/test_workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.037614 iparapheur-provisioning-1.7.1/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.037614 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.7.0/LICENSE.md` & `iparapheur-provisioning-1.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/README.md` & `iparapheur-provisioning-1.7.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.7.0
+- Package version: 1.7.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
 
@@ -194,17 +194,23 @@
 *AdminDeskApi* | [**get_desk_as_admin**](docs/apis/tags/AdminDeskApi.md#get_desk_as_admin) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/desk/{deskId} | Get a full desk description
 *AdminDeskApi* | [**list_desks**](docs/apis/tags/AdminDeskApi.md#list_desks) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/desk | List desks
 *AdminMetadataApi* | [**create_metadata**](docs/apis/tags/AdminMetadataApi.md#create_metadata) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/metadata | Create a metadata
 *AdminMetadataApi* | [**delete_metadata**](docs/apis/tags/AdminMetadataApi.md#delete_metadata) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/metadata/{metadataId} | Delete a metadata
 *AdminMetadataApi* | [**get_metadata**](docs/apis/tags/AdminMetadataApi.md#get_metadata) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/metadata/{metadataId} | Get a full metadata description
 *AdminMetadataApi* | [**list_metadata**](docs/apis/tags/AdminMetadataApi.md#list_metadata) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/metadata | List all metadata associated with the tenant
 *AdminMetadataApi* | [**update_metadata**](docs/apis/tags/AdminMetadataApi.md#update_metadata) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/metadata/{metadataId} | Edit a metadata
+*AdminSealCertificateApi* | [**create_seal_certificate**](docs/apis/tags/AdminSealCertificateApi.md#create_seal_certificate) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/sealCertificate | Create a seal certificate
+*AdminSealCertificateApi* | [**delete_seal_certificate**](docs/apis/tags/AdminSealCertificateApi.md#delete_seal_certificate) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/sealCertificate/{sealCertificateId} | Delete a stored seal certificate
+*AdminSealCertificateApi* | [**get_seal_certificate**](docs/apis/tags/AdminSealCertificateApi.md#get_seal_certificate) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/sealCertificate/{sealCertificateId} | Get a seal certificate with every information set
+*AdminSealCertificateApi* | [**list_seal_certificate**](docs/apis/tags/AdminSealCertificateApi.md#list_seal_certificate) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/sealCertificate | List seal certificates
+*AdminSealCertificateApi* | [**update_seal_certificate**](docs/apis/tags/AdminSealCertificateApi.md#update_seal_certificate) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/sealCertificate/{sealCertificateId} | Edit a seal certificate
 *AdminTenantApi* | [**create_tenant**](docs/apis/tags/AdminTenantApi.md#create_tenant) | **post** /api/provisioning/v1/admin/tenant | Create a new tenant
 *AdminTenantApi* | [**delete_tenant**](docs/apis/tags/AdminTenantApi.md#delete_tenant) | **delete** /api/provisioning/v1/admin/tenant/{tenantId} | Delete a tenant
 *AdminTenantApi* | [**get_tenant**](docs/apis/tags/AdminTenantApi.md#get_tenant) | **get** /api/provisioning/v1/admin/tenant/{tenantId} | Get a full tenant description
+*AdminTenantApi* | [**list_tenants**](docs/apis/tags/AdminTenantApi.md#list_tenants) | **get** /api/provisioning/v1/admin/tenant | List tenants
 *AdminTenantApi* | [**update_tenant**](docs/apis/tags/AdminTenantApi.md#update_tenant) | **put** /api/provisioning/v1/admin/tenant/{tenantId} | Edit a tenant
 *AdminTenantUserApi* | [**create_user**](docs/apis/tags/AdminTenantUserApi.md#create_user) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/user | Create a new user
 *AdminTenantUserApi* | [**get_user**](docs/apis/tags/AdminTenantUserApi.md#get_user) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/user/{userId} | Get a full user description
 *AdminTenantUserApi* | [**list_tenant_users**](docs/apis/tags/AdminTenantUserApi.md#list_tenant_users) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/user | List all users associated with the tenant
 *AdminTenantUserApi* | [**remove_user**](docs/apis/tags/AdminTenantUserApi.md#remove_user) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/user/{userId} | Remove the given user from the tenant, deleting it if it was the last tenant linked
 *AdminTenantUserApi* | [**update_user**](docs/apis/tags/AdminTenantUserApi.md#update_user) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/user/{userId} | Edit a user
 *AdminTypologyApi* | [**create_subtype**](docs/apis/tags/AdminTypologyApi.md#create_subtype) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype | Create a subtype
@@ -213,14 +219,16 @@
 *AdminTypologyApi* | [**delete_type**](docs/apis/tags/AdminTypologyApi.md#delete_type) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId} | Delete a type
 *AdminTypologyApi* | [**get_subtype**](docs/apis/tags/AdminTypologyApi.md#get_subtype) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId} | Get a subtype with every information set
 *AdminTypologyApi* | [**get_type**](docs/apis/tags/AdminTypologyApi.md#get_type) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId} | Get a type with every information set
 *AdminTypologyApi* | [**list_subtypes**](docs/apis/tags/AdminTypologyApi.md#list_subtypes) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype | Get subtypes
 *AdminTypologyApi* | [**list_types**](docs/apis/tags/AdminTypologyApi.md#list_types) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type | List types
 *AdminTypologyApi* | [**update_subtype**](docs/apis/tags/AdminTypologyApi.md#update_subtype) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId} | Edit a subtype
 *AdminTypologyApi* | [**update_type**](docs/apis/tags/AdminTypologyApi.md#update_type) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId} | Edit a type
+*AdminWorkflowDefinitionApi* | [**delete_workflow_definition**](docs/apis/tags/AdminWorkflowDefinitionApi.md#delete_workflow_definition) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/workflowDefinition/{workflowDefinitionKey} | Delete a workflow definition
+*AdminWorkflowDefinitionApi* | [**list_workflow_definitions**](docs/apis/tags/AdminWorkflowDefinitionApi.md#list_workflow_definitions) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/workflowDefinition | List workflow definitions
 
 ## Documentation For Models
 
  - [DelegationSortBy](docs/models/DelegationSortBy.md)
  - [DeskDto](docs/models/DeskDto.md)
  - [DeskRepresentation](docs/models/DeskRepresentation.md)
  - [ErrorResponse](docs/models/ErrorResponse.md)
@@ -233,19 +241,24 @@
  - [LayerSortBy](docs/models/LayerSortBy.md)
  - [MetadataDto](docs/models/MetadataDto.md)
  - [MetadataRepresentation](docs/models/MetadataRepresentation.md)
  - [MetadataSortBy](docs/models/MetadataSortBy.md)
  - [MetadataType](docs/models/MetadataType.md)
  - [PageDeskRepresentation](docs/models/PageDeskRepresentation.md)
  - [PageMetadataRepresentation](docs/models/PageMetadataRepresentation.md)
+ - [PageSealCertificateRepresentation](docs/models/PageSealCertificateRepresentation.md)
  - [PageSubtypeRepresentation](docs/models/PageSubtypeRepresentation.md)
+ - [PageTenantRepresentation](docs/models/PageTenantRepresentation.md)
  - [PageTypeRepresentation](docs/models/PageTypeRepresentation.md)
  - [PageUserRepresentation](docs/models/PageUserRepresentation.md)
+ - [PageWorkflowDefinitionRepresentation](docs/models/PageWorkflowDefinitionRepresentation.md)
  - [PageableObject](docs/models/PageableObject.md)
  - [PdfSignaturePosition](docs/models/PdfSignaturePosition.md)
+ - [SealCertificateDto](docs/models/SealCertificateDto.md)
+ - [SealCertificateRepresentation](docs/models/SealCertificateRepresentation.md)
  - [SealCertificateSortBy](docs/models/SealCertificateSortBy.md)
  - [SignatureFormat](docs/models/SignatureFormat.md)
  - [SignatureProtocol](docs/models/SignatureProtocol.md)
  - [SortObject](docs/models/SortObject.md)
  - [SubtypeDto](docs/models/SubtypeDto.md)
  - [SubtypeLayerAssociation](docs/models/SubtypeLayerAssociation.md)
  - [SubtypeLayerDto](docs/models/SubtypeLayerDto.md)
@@ -257,14 +270,15 @@
  - [TypeDto](docs/models/TypeDto.md)
  - [TypeRepresentation](docs/models/TypeRepresentation.md)
  - [TypologySortBy](docs/models/TypologySortBy.md)
  - [UserDto](docs/models/UserDto.md)
  - [UserPrivilege](docs/models/UserPrivilege.md)
  - [UserRepresentation](docs/models/UserRepresentation.md)
  - [UserSortBy](docs/models/UserSortBy.md)
+ - [WorkflowDefinitionRepresentation](docs/models/WorkflowDefinitionRepresentation.md)
  - [WorkflowDefinitionSortBy](docs/models/WorkflowDefinitionSortBy.md)
 
 ## Documentation For Authorization
 
  Authentication schemes defined for the API:
 ## spring_oauth
 
@@ -278,14 +292,16 @@
 
 iparapheur@libriciel.coop
 iparapheur@libriciel.coop
 iparapheur@libriciel.coop
 iparapheur@libriciel.coop
 iparapheur@libriciel.coop
 iparapheur@libriciel.coop
+iparapheur@libriciel.coop
+iparapheur@libriciel.coop
 
 ## Notes for Large OpenAPI documents
 If the OpenAPI document is large, imports in iparapheur_provisioning.apis and iparapheur_provisioning.models may fail with a
 RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
 
 Solution 1:
 Use specific imports for apis and models like:
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/__init__.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.7.0"
+__version__ = "1.7.1"
 
 # import ApiClient
 from iparapheur_provisioning.api_client import ApiClient
 
 # import Configuration
 from iparapheur_provisioning.configuration import Configuration
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/api_client.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.7.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.7.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/path_to_api.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/path_to_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,55 +2,67 @@
 
 from iparapheur_provisioning.paths import PathValues
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_user_user_id import ApiProvisioningV1AdminUserUserId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id import ApiProvisioningV1AdminTenantTenantId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import ApiProvisioningV1AdminTenantTenantIdUserUserId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId
+from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id import ApiProvisioningV1AdminTenantTenantIdSealCertificateSealCertificateId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import ApiProvisioningV1AdminTenantTenantIdDeskDeskId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant import ApiProvisioningV1AdminTenant
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_user import ApiProvisioningV1AdminTenantTenantIdUser
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import ApiProvisioningV1AdminTenantTenantIdTypologyType
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype
+from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_seal_certificate import ApiProvisioningV1AdminTenantTenantIdSealCertificate
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata import ApiProvisioningV1AdminTenantTenantIdMetadata
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_desk import ApiProvisioningV1AdminTenantTenantIdDesk
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_user import ApiProvisioningV1AdminUser
+from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_workflow_definition import ApiProvisioningV1AdminTenantTenantIdWorkflowDefinition
+from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key import ApiProvisioningV1AdminTenantTenantIdWorkflowDefinitionWorkflowDefinitionKey
 
 PathToApi = typing_extensions.TypedDict(
     'PathToApi',
     {
         PathValues.API_PROVISIONING_V1_ADMIN_USER_USER_ID: ApiProvisioningV1AdminUserUserId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID: ApiProvisioningV1AdminTenantTenantId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER_USER_ID: ApiProvisioningV1AdminTenantTenantIdUserUserId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_SEAL_CERTIFICATE_SEAL_CERTIFICATE_ID: ApiProvisioningV1AdminTenantTenantIdSealCertificateSealCertificateId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA_METADATA_ID: ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK_DESK_ID: ApiProvisioningV1AdminTenantTenantIdDeskDeskId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT: ApiProvisioningV1AdminTenant,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER: ApiProvisioningV1AdminTenantTenantIdUser,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE: ApiProvisioningV1AdminTenantTenantIdTypologyType,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_SEAL_CERTIFICATE: ApiProvisioningV1AdminTenantTenantIdSealCertificate,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA: ApiProvisioningV1AdminTenantTenantIdMetadata,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK: ApiProvisioningV1AdminTenantTenantIdDesk,
         PathValues.API_PROVISIONING_V1_ADMIN_USER: ApiProvisioningV1AdminUser,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_WORKFLOW_DEFINITION: ApiProvisioningV1AdminTenantTenantIdWorkflowDefinition,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_WORKFLOW_DEFINITION_WORKFLOW_DEFINITION_KEY: ApiProvisioningV1AdminTenantTenantIdWorkflowDefinitionWorkflowDefinitionKey,
     }
 )
 
 path_to_api = PathToApi(
     {
         PathValues.API_PROVISIONING_V1_ADMIN_USER_USER_ID: ApiProvisioningV1AdminUserUserId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID: ApiProvisioningV1AdminTenantTenantId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER_USER_ID: ApiProvisioningV1AdminTenantTenantIdUserUserId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_SEAL_CERTIFICATE_SEAL_CERTIFICATE_ID: ApiProvisioningV1AdminTenantTenantIdSealCertificateSealCertificateId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA_METADATA_ID: ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK_DESK_ID: ApiProvisioningV1AdminTenantTenantIdDeskDeskId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT: ApiProvisioningV1AdminTenant,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER: ApiProvisioningV1AdminTenantTenantIdUser,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE: ApiProvisioningV1AdminTenantTenantIdTypologyType,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_SEAL_CERTIFICATE: ApiProvisioningV1AdminTenantTenantIdSealCertificate,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA: ApiProvisioningV1AdminTenantTenantIdMetadata,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK: ApiProvisioningV1AdminTenantTenantIdDesk,
         PathValues.API_PROVISIONING_V1_ADMIN_USER: ApiProvisioningV1AdminUser,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_WORKFLOW_DEFINITION: ApiProvisioningV1AdminTenantTenantIdWorkflowDefinition,
+        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_WORKFLOW_DEFINITION_WORKFLOW_DEFINITION_KEY: ApiProvisioningV1AdminTenantTenantIdWorkflowDefinitionWorkflowDefinitionKey,
     }
 )
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/__init__.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,9 +6,11 @@
 
 
 class TagValues(str, enum.Enum):
     ADMINTENANTUSER = "admin-tenant-user"
     ADMINDESK = "admin-desk"
     ADMINMETADATA = "admin-metadata"
     ADMINTYPOLOGY = "admin-typology"
+    ADMINWORKFLOWDEFINITION = "admin-workflow-definition"
     ADMINTENANT = "admin-tenant"
     ADMINALLUSERS = "admin-all-users"
+    ADMINSEALCERTIFICATE = "admin-seal-certificate"
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_all_users_api.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_all_users_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_desk_api.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_metadata_api.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_metadata_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_tenant_api.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,25 +6,27 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant.post import CreateTenant
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id.delete import DeleteTenant
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id.get import GetTenant
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id.put import UpdateTenant
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user.post import CreateUser
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id.get import GetUser
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user.get import ListTenantUsers
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id.delete import RemoveUser
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id.put import UpdateUser
 
 
-class AdminTenantApi(
-    CreateTenant,
-    DeleteTenant,
-    GetTenant,
-    UpdateTenant,
+class AdminTenantUserApi(
+    CreateUser,
+    GetUser,
+    ListTenantUsers,
+    RemoveUser,
+    UpdateUser,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     pass
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,27 +6,21 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user.post import CreateUser
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id.get import GetUser
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user.get import ListTenantUsers
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id.delete import RemoveUser
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id.put import UpdateUser
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key.delete import DeleteWorkflowDefinition
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_workflow_definition.get import ListWorkflowDefinitions
 
 
-class AdminTenantUserApi(
-    CreateUser,
-    GetUser,
-    ListTenantUsers,
-    RemoveUser,
-    UpdateUser,
+class AdminWorkflowDefinitionApi(
+    DeleteWorkflowDefinition,
+    ListWorkflowDefinitions,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     pass
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/apis/tags/admin_typology_api.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/configuration.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.7.0".\
+               "SDK Package Version: 1.7.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/exceptions.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/delegation_sort_by.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/desk_dto.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/desk_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             
             
             class shortName(
                 schemas.StrSchema
             ):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/desk_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/desk_representation.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             tenantId = schemas.StrSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
                 "tenantId": tenantId,
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/error_response.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_config_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_config_representation.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,18 @@
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
 class ExternalSignatureConfigRepresentation(
-    schemas.DictSchema
+    schemas.DictBase,
+    schemas.NoneBase,
+    schemas.Schema,
+    schemas.NoneFrozenDictMixin
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -57,14 +60,15 @@
             __annotations__ = {
                 "id": id,
                 "name": name,
                 "serviceName": serviceName,
                 "url": url,
                 "login": login,
             }
+
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
@@ -105,15 +109,15 @@
     
     def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "name", "serviceName", "url", "login", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
+        *_args: typing.Union[dict, frozendict.frozendict, None, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
         name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
         serviceName: typing.Union['ExternalSignatureProvider', schemas.Unset] = schemas.unset,
         url: typing.Union[MetaOapg.properties.url, str, schemas.Unset] = schemas.unset,
         login: typing.Union[MetaOapg.properties.login, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_config_sort_by.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/external_signature_provider.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/folder_sort_by.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/internal_metadata.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/layer_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/layer_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
             }
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/layer_sort_by.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_dto.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             
             
             class key(
                 schemas.StrSchema
             ):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_representation.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             
             
             class key(
                 schemas.StrSchema
             ):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_sort_by.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/metadata_type.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_desk_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_metadata_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_subtype_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_type_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/page_user_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/pageable_object.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/pdf_signature_position.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/seal_certificate_sort_by.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/signature_format.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/signature_protocol.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/sort_object.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_dto.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             
             
             class description(
                 schemas.StrSchema
             ):
@@ -153,14 +153,18 @@
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'sealCertificateId':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
+        
+            @staticmethod
+            def sealCertificate() -> typing.Type['SealCertificateRepresentation']:
+                return SealCertificateRepresentation
             
             
             class subtypeMetadataList(
                 schemas.ListSchema
             ):
             
             
@@ -386,14 +390,15 @@
                 "creationWorkflowId": creationWorkflowId,
                 "validationWorkflowId": validationWorkflowId,
                 "workflowSelectionScript": workflowSelectionScript,
                 "annotationsAllowed": annotationsAllowed,
                 "externalSignatureAutomatic": externalSignatureAutomatic,
                 "secureMailServerId": secureMailServerId,
                 "sealCertificateId": sealCertificateId,
+                "sealCertificate": sealCertificate,
                 "subtypeMetadataList": subtypeMetadataList,
                 "subtypeLayers": subtypeLayers,
                 "externalSignatureConfigId": externalSignatureConfigId,
                 "externalSignatureConfig": externalSignatureConfig,
                 "creationPermittedDeskIds": creationPermittedDeskIds,
                 "creationPermittedDesks": creationPermittedDesks,
                 "filterableByDeskIds": filterableByDeskIds,
@@ -435,14 +440,17 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["secureMailServerId"]) -> MetaOapg.properties.secureMailServerId: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sealCertificateId"]) -> MetaOapg.properties.sealCertificateId: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["sealCertificate"]) -> 'SealCertificateRepresentation': ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["subtypeMetadataList"]) -> MetaOapg.properties.subtypeMetadataList: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["subtypeLayers"]) -> MetaOapg.properties.subtypeLayers: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["externalSignatureConfigId"]) -> MetaOapg.properties.externalSignatureConfigId: ...
@@ -479,15 +487,15 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sealAutomatic"]) -> MetaOapg.properties.sealAutomatic: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "sealCertificate", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
@@ -515,14 +523,17 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["secureMailServerId"]) -> typing.Union[MetaOapg.properties.secureMailServerId, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sealCertificateId"]) -> typing.Union[MetaOapg.properties.sealCertificateId, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["sealCertificate"]) -> typing.Union['SealCertificateRepresentation', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["subtypeMetadataList"]) -> typing.Union[MetaOapg.properties.subtypeMetadataList, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["subtypeLayers"]) -> typing.Union[MetaOapg.properties.subtypeLayers, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["externalSignatureConfigId"]) -> typing.Union[MetaOapg.properties.externalSignatureConfigId, schemas.Unset]: ...
@@ -559,15 +570,15 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sealAutomatic"]) -> typing.Union[MetaOapg.properties.sealAutomatic, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "sealCertificate", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
@@ -576,14 +587,15 @@
         creationWorkflowId: typing.Union[MetaOapg.properties.creationWorkflowId, None, str, schemas.Unset] = schemas.unset,
         validationWorkflowId: typing.Union[MetaOapg.properties.validationWorkflowId, str, schemas.Unset] = schemas.unset,
         workflowSelectionScript: typing.Union[MetaOapg.properties.workflowSelectionScript, None, str, schemas.Unset] = schemas.unset,
         annotationsAllowed: typing.Union[MetaOapg.properties.annotationsAllowed, bool, schemas.Unset] = schemas.unset,
         externalSignatureAutomatic: typing.Union[MetaOapg.properties.externalSignatureAutomatic, bool, schemas.Unset] = schemas.unset,
         secureMailServerId: typing.Union[MetaOapg.properties.secureMailServerId, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sealCertificateId: typing.Union[MetaOapg.properties.sealCertificateId, None, str, schemas.Unset] = schemas.unset,
+        sealCertificate: typing.Union['SealCertificateRepresentation', schemas.Unset] = schemas.unset,
         subtypeMetadataList: typing.Union[MetaOapg.properties.subtypeMetadataList, list, tuple, schemas.Unset] = schemas.unset,
         subtypeLayers: typing.Union[MetaOapg.properties.subtypeLayers, list, tuple, schemas.Unset] = schemas.unset,
         externalSignatureConfigId: typing.Union[MetaOapg.properties.externalSignatureConfigId, None, str, schemas.Unset] = schemas.unset,
         externalSignatureConfig: typing.Union['ExternalSignatureConfigRepresentation', schemas.Unset] = schemas.unset,
         creationPermittedDeskIds: typing.Union[MetaOapg.properties.creationPermittedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
         creationPermittedDesks: typing.Union[MetaOapg.properties.creationPermittedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
         filterableByDeskIds: typing.Union[MetaOapg.properties.filterableByDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
@@ -606,14 +618,15 @@
             creationWorkflowId=creationWorkflowId,
             validationWorkflowId=validationWorkflowId,
             workflowSelectionScript=workflowSelectionScript,
             annotationsAllowed=annotationsAllowed,
             externalSignatureAutomatic=externalSignatureAutomatic,
             secureMailServerId=secureMailServerId,
             sealCertificateId=sealCertificateId,
+            sealCertificate=sealCertificate,
             subtypeMetadataList=subtypeMetadataList,
             subtypeLayers=subtypeLayers,
             externalSignatureConfigId=externalSignatureConfigId,
             externalSignatureConfig=externalSignatureConfig,
             creationPermittedDeskIds=creationPermittedDeskIds,
             creationPermittedDesks=creationPermittedDesks,
             filterableByDeskIds=filterableByDeskIds,
@@ -626,9 +639,10 @@
             sealAutomatic=sealAutomatic,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.desk_representation import DeskRepresentation
 from iparapheur_provisioning.model.external_signature_config_representation import ExternalSignatureConfigRepresentation
+from iparapheur_provisioning.model.seal_certificate_representation import SealCertificateRepresentation
 from iparapheur_provisioning.model.subtype_layer_dto import SubtypeLayerDto
 from iparapheur_provisioning.model.subtype_metadata_dto import SubtypeMetadataDto
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_layer_association.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_layer_dto.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_metadata_dto.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/subtype_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
             }
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_dto.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
             }
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
             }
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/tenant_sort_by.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/type_dto.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/type_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             
             
             class description(
                 schemas.StrSchema
             ):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/type_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/type_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]*$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             
             
             class description(
                 schemas.StrSchema
             ):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/typology_sort_by.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_dto.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_privilege.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_representation.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/user_sort_by.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/model/workflow_definition_sort_by.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/__init__.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 
 class PathValues(str, enum.Enum):
     API_PROVISIONING_V1_ADMIN_USER_USER_ID = "/api/provisioning/v1/admin/user/{userId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID = "/api/provisioning/v1/admin/tenant/{tenantId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER_USER_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/user/{userId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId}"
+    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_SEAL_CERTIFICATE_SEAL_CERTIFICATE_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/sealCertificate/{sealCertificateId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA_METADATA_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/metadata/{metadataId}"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK_DESK_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/desk/{deskId}"
     API_PROVISIONING_V1_ADMIN_TENANT = "/api/provisioning/v1/admin/tenant"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER = "/api/provisioning/v1/admin/tenant/{tenantId}/user"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype"
+    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_SEAL_CERTIFICATE = "/api/provisioning/v1/admin/tenant/{tenantId}/sealCertificate"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_METADATA = "/api/provisioning/v1/admin/tenant/{tenantId}/metadata"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK = "/api/provisioning/v1/admin/tenant/{tenantId}/desk"
     API_PROVISIONING_V1_ADMIN_USER = "/api/provisioning/v1/admin/user"
+    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_WORKFLOW_DEFINITION = "/api/provisioning/v1/admin/tenant/{tenantId}/workflowDefinition"
+    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_WORKFLOW_DEFINITION_WORKFLOW_DEFINITION_KEY = "/api/provisioning/v1/admin/tenant/{tenantId}/workflowDefinition/{workflowDefinitionKey}"
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,115 +40,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = TenantDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
-    '400': _response_for_400,
+    '507': _response_for_507,
     '201': _response_for_201,
     '403': _response_for_403,
-    '507': _response_for_507,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -66,31 +66,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -104,38 +104,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '401': _response_for_401,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,50 +55,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -112,38 +112,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '400': _response_for_400,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,50 +143,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -200,38 +200,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '400': _response_for_400,
     '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,135 +66,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = DeskDto
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
+    '507': _response_for_507,
+    '409': _response_for_409,
+    '404': _response_for_404,
     '201': _response_for_201,
     '403': _response_for_403,
-    '404': _response_for_404,
-    '409': _response_for_409,
-    '507': _response_for_507,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -112,38 +112,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '401': _response_for_401,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,50 +63,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -120,38 +120,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,69 +74,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -150,59 +150,59 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
+    '507': _response_for_507,
+    '409': _response_for_409,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
-    '409': _response_for_409,
-    '507': _response_for_507,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -151,50 +151,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageMetadataRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageMetadataRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -208,38 +208,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,155 +66,155 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = MetadataDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = MetadataDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
-    '400': _response_for_400,
+    '507': _response_for_507,
+    '409': _response_for_409,
+    '404': _response_for_404,
     '201': _response_for_201,
     '403': _response_for_403,
-    '404': _response_for_404,
-    '409': _response_for_409,
-    '507': _response_for_507,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -112,38 +112,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '401': _response_for_401,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,50 +63,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=MetadataIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = MetadataDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = MetadataDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -120,38 +120,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,81 +74,81 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -162,60 +162,60 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '507': _response_for_507,
     '406': _response_for_406,
-    '401': _response_for_401,
     '200': _response_for_200,
-    '400': _response_for_400,
-    '403': _response_for_403,
     '404': _response_for_404,
-    '507': _response_for_507,
+    '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -135,50 +135,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -192,38 +192,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = TypeDto
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
+    '507': _response_for_507,
+    '409': _response_for_409,
     '201': _response_for_201,
     '403': _response_for_403,
-    '409': _response_for_409,
-    '507': _response_for_507,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -112,38 +112,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '401': _response_for_401,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,50 +63,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -120,38 +120,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,50 +74,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -131,38 +131,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,50 +143,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -200,38 +200,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,135 +74,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = SubtypeDto
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
+    '507': _response_for_507,
+    '409': _response_for_409,
+    '404': _response_for_404,
     '201': _response_for_201,
     '403': _response_for_403,
-    '404': _response_for_404,
-    '409': _response_for_409,
-    '507': _response_for_507,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,31 +82,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -120,38 +120,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '401': _response_for_401,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,50 +71,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = SubtypeDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -128,38 +128,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,31 +101,31 @@
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor204ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -139,31 +139,31 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -179,17 +179,17 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '401': _response_for_401,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -151,115 +151,115 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '400': _response_for_400,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = UserDto
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
+    '507': _response_for_507,
+    '409': _response_for_409,
     '201': _response_for_201,
     '403': _response_for_403,
-    '409': _response_for_409,
-    '507': _response_for_507,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,57 +93,57 @@
 _response_for_406 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
     '406': _response_for_406,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,50 +63,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -120,38 +120,38 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,50 +93,50 @@
 _response_for_406 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -150,39 +150,39 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '406': _response_for_406,
-    '401': _response_for_401,
     '200': _response_for_200,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -117,50 +117,50 @@
     style=api_client.ParameterStyle.FORM,
     schema=SearchTermSchema,
     explode=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -174,38 +174,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '400': _response_for_400,
     '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,31 +66,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -104,38 +104,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '401': _response_for_401,
-    '400': _response_for_400,
     '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,115 +55,115 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '400': _response_for_400,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '200': _response_for_200,
-    '400': _response_for_400,
-    '403': _response_for_403,
     '404': _response_for_404,
+    '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/rest.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning/schemas.py` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning/schemas.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/iparapheur_provisioning.egg-info/SOURCES.txt` & `iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -19,29 +19,35 @@
 iparapheur_provisioning/apis/paths/__init__.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
+iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate.py
+iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition.py
+iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
 iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
 iparapheur_provisioning/apis/tags/__init__.py
 iparapheur_provisioning/apis/tags/admin_all_users_api.py
 iparapheur_provisioning/apis/tags/admin_desk_api.py
 iparapheur_provisioning/apis/tags/admin_metadata_api.py
+iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py
 iparapheur_provisioning/apis/tags/admin_tenant_api.py
 iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
 iparapheur_provisioning/apis/tags/admin_typology_api.py
+iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py
 iparapheur_provisioning/model/__init__.py
 iparapheur_provisioning/model/delegation_sort_by.py
 iparapheur_provisioning/model/desk_dto.py
 iparapheur_provisioning/model/desk_representation.py
 iparapheur_provisioning/model/error_response.py
 iparapheur_provisioning/model/external_signature_config_representation.py
 iparapheur_provisioning/model/external_signature_config_sort_by.py
@@ -52,19 +58,24 @@
 iparapheur_provisioning/model/layer_sort_by.py
 iparapheur_provisioning/model/metadata_dto.py
 iparapheur_provisioning/model/metadata_representation.py
 iparapheur_provisioning/model/metadata_sort_by.py
 iparapheur_provisioning/model/metadata_type.py
 iparapheur_provisioning/model/page_desk_representation.py
 iparapheur_provisioning/model/page_metadata_representation.py
+iparapheur_provisioning/model/page_seal_certificate_representation.py
 iparapheur_provisioning/model/page_subtype_representation.py
+iparapheur_provisioning/model/page_tenant_representation.py
 iparapheur_provisioning/model/page_type_representation.py
 iparapheur_provisioning/model/page_user_representation.py
+iparapheur_provisioning/model/page_workflow_definition_representation.py
 iparapheur_provisioning/model/pageable_object.py
 iparapheur_provisioning/model/pdf_signature_position.py
+iparapheur_provisioning/model/seal_certificate_dto.py
+iparapheur_provisioning/model/seal_certificate_representation.py
 iparapheur_provisioning/model/seal_certificate_sort_by.py
 iparapheur_provisioning/model/signature_format.py
 iparapheur_provisioning/model/signature_protocol.py
 iparapheur_provisioning/model/sort_object.py
 iparapheur_provisioning/model/subtype_dto.py
 iparapheur_provisioning/model/subtype_layer_association.py
 iparapheur_provisioning/model/subtype_layer_dto.py
@@ -76,18 +87,20 @@
 iparapheur_provisioning/model/type_dto.py
 iparapheur_provisioning/model/type_representation.py
 iparapheur_provisioning/model/typology_sort_by.py
 iparapheur_provisioning/model/user_dto.py
 iparapheur_provisioning/model/user_privilege.py
 iparapheur_provisioning/model/user_representation.py
 iparapheur_provisioning/model/user_sort_by.py
+iparapheur_provisioning/model/workflow_definition_representation.py
 iparapheur_provisioning/model/workflow_definition_sort_by.py
 iparapheur_provisioning/models/__init__.py
 iparapheur_provisioning/paths/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
@@ -99,14 +112,21 @@
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
@@ -120,14 +140,18 @@
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
+iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
 test/test_models/__init__.py
@@ -144,19 +168,24 @@
 test/test_models/test_layer_sort_by.py
 test/test_models/test_metadata_dto.py
 test/test_models/test_metadata_representation.py
 test/test_models/test_metadata_sort_by.py
 test/test_models/test_metadata_type.py
 test/test_models/test_page_desk_representation.py
 test/test_models/test_page_metadata_representation.py
+test/test_models/test_page_seal_certificate_representation.py
 test/test_models/test_page_subtype_representation.py
+test/test_models/test_page_tenant_representation.py
 test/test_models/test_page_type_representation.py
 test/test_models/test_page_user_representation.py
+test/test_models/test_page_workflow_definition_representation.py
 test/test_models/test_pageable_object.py
 test/test_models/test_pdf_signature_position.py
+test/test_models/test_seal_certificate_dto.py
+test/test_models/test_seal_certificate_representation.py
 test/test_models/test_seal_certificate_sort_by.py
 test/test_models/test_signature_format.py
 test/test_models/test_signature_protocol.py
 test/test_models/test_sort_object.py
 test/test_models/test_subtype_dto.py
 test/test_models/test_subtype_layer_association.py
 test/test_models/test_subtype_layer_dto.py
@@ -168,17 +197,19 @@
 test/test_models/test_type_dto.py
 test/test_models/test_type_representation.py
 test/test_models/test_typology_sort_by.py
 test/test_models/test_user_dto.py
 test/test_models/test_user_privilege.py
 test/test_models/test_user_representation.py
 test/test_models/test_user_sort_by.py
+test/test_models/test_workflow_definition_representation.py
 test/test_models/test_workflow_definition_sort_by.py
 test/test_paths/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
@@ -190,14 +221,21 @@
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
@@ -211,13 +249,17 @@
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
+test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py
 test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
 test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
 test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
 test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.7.0/setup.py` & `iparapheur-provisioning-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "iparapheur-provisioning"
-VERSION = "1.7.0"
+VERSION = "1.7.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_delegation_sort_by.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_desk_dto.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_desk_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_error_response.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_config_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_config_sort_by.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_external_signature_provider.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_folder_sort_by.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_internal_metadata.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_layer_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_layer_sort_by.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_metadata_dto.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_metadata_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_metadata_sort_by.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_metadata_type.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_page_desk_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_page_metadata_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_page_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_page_subtype_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_page_type_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_page_user_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_pageable_object.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_pdf_signature_position.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_seal_certificate_sort_by.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_signature_format.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_signature_protocol.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_sort_object.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_subtype_dto.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_subtype_layer_association.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_subtype_layer_dto.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_subtype_metadata_dto.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_subtype_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_tenant_dto.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_tenant_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_tenant_sort_by.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_type_dto.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_type_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_typology_sort_by.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_user_dto.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_user_privilege.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_user_representation.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_user_sort_by.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_models/test_workflow_definition_sort_by.py` & `iparapheur-provisioning-1.7.1/test/test_models/test_workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/__init__.py` & `iparapheur-provisioning-1.7.1/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenant unit test stubs
-        Create a new tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantId unit test stubs
+        Edit a tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDesk(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Edit a tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDesk unit test stubs
+        List desks  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
-
-
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDesk(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDesk unit test stubs
-        List desks  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
+        Get a full desk description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 507
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Get a full desk description  # noqa: E501
+        Edit a desk  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 507
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Edit a desk  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 406
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdMetadata(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdMetadata unit test stubs
-        Create a metadata  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
+        Create a type  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 507
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 406
+    response_status = 507
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
-        Create a type  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        List all users associated with the tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
-
-
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 507
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        List all users associated with the tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Remove the given user from the tenant, deleting it if it was the last tenant linked  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
-
-
+    response_status = 204
+    response_body = ''
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_seal_certificate import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdSealCertificate(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        Create a new user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdSealCertificate unit test stubs
+        Create a seal certificate  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
-
-
+    response_status = 507
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Remove the given user from the tenant, deleting it if it was the last tenant linked  # noqa: E501
+        Get a full user description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 200
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Get a full user description  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Get a full user representation  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Edit a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        Create a new user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 406
+    response_status = 507
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdMetadata(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Get a full user representation  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdMetadata unit test stubs
+        Create a metadata  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 507
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.0/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py` & `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 200
 
 
 
 
 
 
 if __name__ == '__main__':
```

