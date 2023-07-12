# Comparing `tmp/semantha_sdk-5.5.0.tar.gz` & `tmp/semantha_sdk-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-5.5.0.tar", max compression
+gzip compressed data, was "semantha_sdk-5.6.0.tar", max compression
```

## Comparing `semantha_sdk-5.5.0.tar` & `semantha_sdk-5.6.0.tar`

### file list

```diff
@@ -1,152 +1,199 @@
--rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.5.0/LICENSE
--rw-r--r--   0        0        0     1618 2023-06-30 08:53:09.443616 semantha_sdk-5.5.0/pyproject.toml
--rw-r--r--   0        0        0    14524 2023-06-30 08:52:57.695383 semantha_sdk-5.5.0/README.md
--rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.5.0/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 06:39:31.917641 semantha_sdk-5.5.0/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0     1681 2023-06-30 06:26:01.750523 semantha_sdk-5.5.0/semantha_sdk/api/answers.py
--rw-r--r--   0        0        0     1004 2023-06-30 06:26:01.700367 semantha_sdk-5.5.0/semantha_sdk/api/bulk.py
--rw-r--r--   0        0        0      839 2023-06-30 06:26:01.701367 semantha_sdk-5.5.0/semantha_sdk/api/bulk_domains.py
--rw-r--r--   0        0        0      817 2023-06-30 06:26:01.724526 semantha_sdk-5.5.0/semantha_sdk/api/bulk_model.py
--rw-r--r--   0        0        0     1792 2023-06-30 06:26:01.717524 semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_documentclasses.py
--rw-r--r--   0        0        0     1576 2023-06-30 06:26:01.706366 semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_domain.py
--rw-r--r--   0        0        0     3758 2023-06-30 06:26:01.721524 semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_referencedocuments.py
--rw-r--r--   0        0        0     3406 2023-06-30 06:26:01.723526 semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_references.py
--rw-r--r--   0        0        0     1346 2023-06-30 06:26:01.728526 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_boostwords.py
--rw-r--r--   0        0        0      923 2023-06-30 06:26:01.732523 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_class.py
--rw-r--r--   0        0        0     1913 2023-06-30 06:26:01.730523 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_classes.py
--rw-r--r--   0        0        0     1735 2023-06-30 06:26:01.734526 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_dataproperties.py
--rw-r--r--   0        0        0     2785 2023-06-30 06:26:01.727526 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_domain.py
--rw-r--r--   0        0        0      836 2023-06-30 06:26:01.725524 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_domains.py
--rw-r--r--   0        0        0     1662 2023-06-30 06:26:01.736524 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_instances.py
--rw-r--r--   0        0        0     1661 2023-06-30 06:26:01.739524 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_metadata.py
--rw-r--r--   0        0        0     1373 2023-06-30 06:26:01.741524 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_namedentities.py
--rw-r--r--   0        0        0     1261 2023-06-30 06:26:01.742523 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_stopwords.py
--rw-r--r--   0        0        0     1322 2023-06-30 06:26:01.743524 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_synonyms.py
--rw-r--r--   0        0        0     1098 2023-06-30 06:26:01.733523 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodelclass_instances.py
--rw-r--r--   0        0        0     5664 2023-06-30 06:26:01.762533 semantha_sdk-5.5.0/semantha_sdk/api/clusters.py
--rw-r--r--   0        0        0     1168 2023-06-30 06:26:01.744523 semantha_sdk-5.5.0/semantha_sdk/api/currentuser.py
--rw-r--r--   0        0        0     1425 2023-06-30 06:26:01.746524 semantha_sdk-5.5.0/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     2385 2023-06-30 06:26:01.751524 semantha_sdk-5.5.0/semantha_sdk/api/documentannotations.py
--rw-r--r--   0        0        0     1565 2023-06-30 06:26:01.753524 semantha_sdk-5.5.0/semantha_sdk/api/documentclass.py
--rw-r--r--   0        0        0     1997 2023-06-30 06:26:01.752523 semantha_sdk-5.5.0/semantha_sdk/api/documentclasses.py
--rw-r--r--   0        0        0     3592 2023-06-30 06:26:01.754524 semantha_sdk-5.5.0/semantha_sdk/api/documentcomparisons.py
--rw-r--r--   0        0        0     3521 2023-06-30 06:26:01.755523 semantha_sdk-5.5.0/semantha_sdk/api/documents.py
--rw-r--r--   0        0        0     4497 2023-06-30 06:26:01.748524 semantha_sdk-5.5.0/semantha_sdk/api/domain.py
--rw-r--r--   0        0        0     1157 2023-06-30 06:26:01.747523 semantha_sdk-5.5.0/semantha_sdk/api/domains.py
--rw-r--r--   0        0        0      905 2023-06-30 06:26:01.781038 semantha_sdk-5.5.0/semantha_sdk/api/info.py
--rw-r--r--   0        0        0     1757 2023-06-30 06:26:01.782036 semantha_sdk-5.5.0/semantha_sdk/api/languages.py
--rw-r--r--   0        0        0     1595 2023-06-30 06:26:01.783035 semantha_sdk-5.5.0/semantha_sdk/api/model.py
--rw-r--r--   0        0        0     1460 2023-06-30 06:26:01.787039 semantha_sdk-5.5.0/semantha_sdk/api/model_boostword.py
--rw-r--r--   0        0        0     1924 2023-06-30 06:26:01.786035 semantha_sdk-5.5.0/semantha_sdk/api/model_boostwords.py
--rw-r--r--   0        0        0      840 2023-06-30 06:26:01.783035 semantha_sdk-5.5.0/semantha_sdk/api/model_datatypes.py
--rw-r--r--   0        0        0     2186 2023-06-30 06:26:01.785036 semantha_sdk-5.5.0/semantha_sdk/api/model_domain.py
--rw-r--r--   0        0        0      816 2023-06-30 06:26:01.784036 semantha_sdk-5.5.0/semantha_sdk/api/model_domains.py
--rw-r--r--   0        0        0      855 2023-06-30 06:26:01.793038 semantha_sdk-5.5.0/semantha_sdk/api/model_extractortypes.py
--rw-r--r--   0        0        0      852 2023-06-30 06:26:01.793038 semantha_sdk-5.5.0/semantha_sdk/api/model_metadatatypes.py
--rw-r--r--   0        0        0     1970 2023-06-30 06:26:01.788036 semantha_sdk-5.5.0/semantha_sdk/api/model_namedentities.py
--rw-r--r--   0        0        0     1494 2023-06-30 06:26:01.789036 semantha_sdk-5.5.0/semantha_sdk/api/model_namedentity.py
--rw-r--r--   0        0        0     1449 2023-06-30 06:26:01.790038 semantha_sdk-5.5.0/semantha_sdk/api/model_stopword.py
--rw-r--r--   0        0        0     1907 2023-06-30 06:26:01.790038 semantha_sdk-5.5.0/semantha_sdk/api/model_stopwords.py
--rw-r--r--   0        0        0     1430 2023-06-30 06:26:01.792039 semantha_sdk-5.5.0/semantha_sdk/api/model_synonym.py
--rw-r--r--   0        0        0     1882 2023-06-30 06:26:01.791038 semantha_sdk-5.5.0/semantha_sdk/api/model_synonyms.py
--rw-r--r--   0        0        0     1217 2023-06-30 06:26:01.756523 semantha_sdk-5.5.0/semantha_sdk/api/modelclasses.py
--rw-r--r--   0        0        0     2361 2023-06-30 06:26:01.757528 semantha_sdk-5.5.0/semantha_sdk/api/modelinstances.py
--rw-r--r--   0        0        0     1663 2023-06-30 06:26:01.763535 semantha_sdk-5.5.0/semantha_sdk/api/namedentities.py
--rw-r--r--   0        0        0     1711 2023-06-30 06:26:01.770527 semantha_sdk-5.5.0/semantha_sdk/api/paragraph.py
--rw-r--r--   0        0        0      792 2023-06-30 06:26:01.768528 semantha_sdk-5.5.0/semantha_sdk/api/paragraphs.py
--rw-r--r--   0        0        0     2267 2023-06-30 06:26:01.767527 semantha_sdk-5.5.0/semantha_sdk/api/referencedocument.py
--rw-r--r--   0        0        0     8885 2023-06-30 06:26:01.759528 semantha_sdk-5.5.0/semantha_sdk/api/referencedocuments.py
--rw-r--r--   0        0        0     6394 2023-06-30 06:26:01.774030 semantha_sdk-5.5.0/semantha_sdk/api/references.py
--rw-r--r--   0        0        0      867 2023-06-30 06:26:01.745528 semantha_sdk-5.5.0/semantha_sdk/api/roles.py
--rw-r--r--   0        0        0     2113 2023-06-29 06:39:31.918640 semantha_sdk-5.5.0/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0      413 2023-06-29 06:39:31.920640 semantha_sdk-5.5.0/semantha_sdk/api/semantha_endpoint.py
--rw-r--r--   0        0        0      967 2023-06-30 06:26:01.772524 semantha_sdk-5.5.0/semantha_sdk/api/sentence.py
--rw-r--r--   0        0        0      786 2023-06-30 06:26:01.771524 semantha_sdk-5.5.0/semantha_sdk/api/sentences.py
--rw-r--r--   0        0        0     1497 2023-06-30 06:26:01.775039 semantha_sdk-5.5.0/semantha_sdk/api/settings.py
--rw-r--r--   0        0        0     5217 2023-06-30 06:26:01.776039 semantha_sdk-5.5.0/semantha_sdk/api/similaritymatrix.py
--rw-r--r--   0        0        0     4070 2023-06-30 06:26:01.777036 semantha_sdk-5.5.0/semantha_sdk/api/similaritymatrix_cluster.py
--rw-r--r--   0        0        0      963 2023-06-30 06:26:01.764535 semantha_sdk-5.5.0/semantha_sdk/api/statistic.py
--rw-r--r--   0        0        0     1207 2023-06-30 06:26:01.778036 semantha_sdk-5.5.0/semantha_sdk/api/summarizations.py
--rw-r--r--   0        0        0      931 2023-06-30 06:26:01.779036 semantha_sdk-5.5.0/semantha_sdk/api/tag.py
--rw-r--r--   0        0        0     1285 2023-06-30 06:26:01.779036 semantha_sdk-5.5.0/semantha_sdk/api/tag_referencedocuments.py
--rw-r--r--   0        0        0     1018 2023-06-30 06:26:01.778036 semantha_sdk-5.5.0/semantha_sdk/api/tags.py
--rw-r--r--   0        0        0     1383 2023-06-30 06:26:01.780037 semantha_sdk-5.5.0/semantha_sdk/api/validation.py
--rw-r--r--   0        0        0     4351 2023-06-30 06:26:01.959034 semantha_sdk-5.5.0/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      619 2023-06-30 06:26:01.932037 semantha_sdk-5.5.0/semantha_sdk/model/annotation_cell.py
--rw-r--r--   0        0        0      689 2023-06-30 06:26:01.928039 semantha_sdk-5.5.0/semantha_sdk/model/annotation_page.py
--rw-r--r--   0        0        0      582 2023-06-30 06:26:01.923037 semantha_sdk-5.5.0/semantha_sdk/model/answer.py
--rw-r--r--   0        0        0      546 2023-06-30 06:26:01.926041 semantha_sdk-5.5.0/semantha_sdk/model/answer_reference.py
--rw-r--r--   0        0        0      579 2023-06-30 06:26:01.912036 semantha_sdk-5.5.0/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      991 2023-06-30 06:26:01.893036 semantha_sdk-5.5.0/semantha_sdk/model/class_bulk.py
--rw-r--r--   0        0        0      513 2023-06-30 06:26:01.892037 semantha_sdk-5.5.0/semantha_sdk/model/clustered_document.py
--rw-r--r--   0        0        0      719 2023-06-30 06:26:01.890038 semantha_sdk-5.5.0/semantha_sdk/model/clustering_response.py
--rw-r--r--   0        0        0     1209 2023-06-30 06:26:01.905040 semantha_sdk-5.5.0/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      543 2023-06-30 06:26:01.940037 semantha_sdk-5.5.0/semantha_sdk/model/current_user.py
--rw-r--r--   0        0        0      639 2023-06-30 06:26:01.895035 semantha_sdk-5.5.0/semantha_sdk/model/data_property.py
--rw-r--r--   0        0        0      481 2023-06-30 06:26:01.918040 semantha_sdk-5.5.0/semantha_sdk/model/difference.py
--rw-r--r--   0        0        0      530 2023-06-30 06:26:01.885036 semantha_sdk-5.5.0/semantha_sdk/model/distance.py
--rw-r--r--   0        0        0     1306 2023-06-30 06:26:01.904036 semantha_sdk-5.5.0/semantha_sdk/model/document.py
--rw-r--r--   0        0        0     1004 2023-06-30 06:26:01.936036 semantha_sdk-5.5.0/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0      771 2023-06-30 06:26:01.940037 semantha_sdk-5.5.0/semantha_sdk/model/document_class_bulk.py
--rw-r--r--   0        0        0      580 2023-06-30 06:26:01.941037 semantha_sdk-5.5.0/semantha_sdk/model/document_class_node.py
--rw-r--r--   0        0        0      660 2023-06-30 06:26:01.939037 semantha_sdk-5.5.0/semantha_sdk/model/document_cluster.py
--rw-r--r--   0        0        0     1078 2023-06-30 06:26:01.910038 semantha_sdk-5.5.0/semantha_sdk/model/document_information.py
--rw-r--r--   0        0        0      508 2023-06-30 06:26:01.922037 semantha_sdk-5.5.0/semantha_sdk/model/document_meta_data.py
--rw-r--r--   0        0        0      503 2023-06-30 06:26:01.945037 semantha_sdk-5.5.0/semantha_sdk/model/document_named_entity.py
--rw-r--r--   0        0        0      533 2023-06-30 06:26:01.942037 semantha_sdk-5.5.0/semantha_sdk/model/document_table.py
--rw-r--r--   0        0        0      577 2023-06-30 06:26:01.911036 semantha_sdk-5.5.0/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      452 2023-06-30 06:26:01.937036 semantha_sdk-5.5.0/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      606 2023-06-30 06:26:01.906036 semantha_sdk-5.5.0/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      757 2023-06-30 06:26:01.930035 semantha_sdk-5.5.0/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      544 2023-06-30 06:26:01.920037 semantha_sdk-5.5.0/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      882 2023-06-30 06:26:01.938036 semantha_sdk-5.5.0/semantha_sdk/model/features.py
--rw-r--r--   0        0        0      520 2023-06-30 06:26:01.889038 semantha_sdk-5.5.0/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      506 2023-06-30 06:26:01.933037 semantha_sdk-5.5.0/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      538 2023-06-30 06:26:01.917037 semantha_sdk-5.5.0/semantha_sdk/model/info.py
--rw-r--r--   0        0        0      891 2023-06-30 06:26:01.900035 semantha_sdk-5.5.0/semantha_sdk/model/instance.py
--rw-r--r--   0        0        0      545 2023-06-30 06:26:01.895035 semantha_sdk-5.5.0/semantha_sdk/model/instance_child.py
--rw-r--r--   0        0        0      413 2023-06-30 06:26:01.944037 semantha_sdk-5.5.0/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      476 2023-06-30 06:26:01.882036 semantha_sdk-5.5.0/semantha_sdk/model/language_detection.py
--rw-r--r--   0        0        0      602 2023-06-30 06:26:01.908037 semantha_sdk-5.5.0/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      488 2023-06-30 06:26:01.898038 semantha_sdk-5.5.0/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      611 2023-06-30 06:26:01.883037 semantha_sdk-5.5.0/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      507 2023-06-30 06:26:01.909037 semantha_sdk-5.5.0/semantha_sdk/model/meta_info_page.py
--rw-r--r--   0        0        0      504 2023-06-30 06:26:01.929036 semantha_sdk-5.5.0/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      435 2023-06-30 06:26:01.919036 semantha_sdk-5.5.0/semantha_sdk/model/metadata_value.py
--rw-r--r--   0        0        0      555 2023-06-30 06:26:01.891036 semantha_sdk-5.5.0/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1577 2023-06-30 07:31:02.968921 semantha_sdk-5.5.0/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      493 2023-06-30 06:26:01.923037 semantha_sdk-5.5.0/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      850 2023-06-30 06:26:01.930035 semantha_sdk-5.5.0/semantha_sdk/model/page.py
--rw-r--r--   0        0        0      551 2023-06-30 06:26:01.886036 semantha_sdk-5.5.0/semantha_sdk/model/page_content.py
--rw-r--r--   0        0        0     1027 2023-06-30 06:26:01.931037 semantha_sdk-5.5.0/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      491 2023-06-30 06:26:01.925036 semantha_sdk-5.5.0/semantha_sdk/model/paragraph_update.py
--rw-r--r--   0        0        0      536 2023-06-30 06:26:01.942037 semantha_sdk-5.5.0/semantha_sdk/model/plotly_chart.py
--rw-r--r--   0        0        0      587 2023-06-30 06:26:01.926041 semantha_sdk-5.5.0/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      459 2023-06-30 06:26:01.943035 semantha_sdk-5.5.0/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      829 2023-06-30 06:26:01.907036 semantha_sdk-5.5.0/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0      756 2023-06-30 06:26:01.901036 semantha_sdk-5.5.0/semantha_sdk/model/reference_documents_response_container.py
--rw-r--r--   0        0        0      716 2023-06-30 06:26:01.934036 semantha_sdk-5.5.0/semantha_sdk/model/response_meta_info.py
--rw-r--r--   0        0        0      523 2023-06-30 06:26:01.902036 semantha_sdk-5.5.0/semantha_sdk/model/row.py
--rw-r--r--   0        0        0      650 2023-06-29 06:39:31.921661 semantha_sdk-5.5.0/semantha_sdk/model/semantha_entity.py
--rw-r--r--   0        0        0      911 2023-06-30 06:26:01.921036 semantha_sdk-5.5.0/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      523 2023-06-30 06:26:01.881034 semantha_sdk-5.5.0/semantha_sdk/model/semi_super_vised_document.py
--rw-r--r--   0        0        0      834 2023-06-30 06:26:01.888035 semantha_sdk-5.5.0/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0     1755 2023-06-30 06:26:01.894036 semantha_sdk-5.5.0/semantha_sdk/model/settings.py
--rw-r--r--   0        0        0      462 2023-06-30 06:26:01.907036 semantha_sdk-5.5.0/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      704 2023-06-30 06:26:01.935037 semantha_sdk-5.5.0/semantha_sdk/model/smart_cluster_response_container.py
--rw-r--r--   0        0        0      892 2023-06-30 06:26:01.914037 semantha_sdk-5.5.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
--rw-r--r--   0        0        0      640 2023-06-30 06:26:01.913036 semantha_sdk-5.5.0/semantha_sdk/model/statistic.py
--rw-r--r--   0        0        0      488 2023-06-30 06:26:01.903038 semantha_sdk-5.5.0/semantha_sdk/model/stop_word.py
--rw-r--r--   0        0        0      575 2023-06-30 06:26:01.915037 semantha_sdk-5.5.0/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      448 2023-06-30 06:26:01.937036 semantha_sdk-5.5.0/semantha_sdk/model/table_cell.py
--rw-r--r--   0        0        0      572 2023-06-30 06:26:01.888035 semantha_sdk-5.5.0/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      467 2023-06-30 06:26:01.916036 semantha_sdk-5.5.0/semantha_sdk/model/tag_docs.py
--rw-r--r--   0        0        0      469 2023-06-30 06:26:01.914037 semantha_sdk-5.5.0/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.5.0/semantha_sdk/request/__init__.py
--rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.5.0/semantha_sdk/request/semantha_request.py
--rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.5.0/semantha_sdk/response/__init__.py
--rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.5.0/semantha_sdk/response/semantha_error.py
--rw-r--r--   0        0        0     3712 2023-06-20 12:43:00.735650 semantha_sdk-5.5.0/semantha_sdk/response/semantha_response.py
--rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.5.0/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.5.0/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0    15077 1970-01-01 00:00:00.000000 semantha_sdk-5.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.6.0/LICENSE
+-rw-r--r--   0        0        0     1618 2023-07-12 16:11:36.552533 semantha_sdk-5.6.0/pyproject.toml
+-rw-r--r--   0        0        0    17578 2023-07-12 16:09:09.354313 semantha_sdk-5.6.0/README.md
+-rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.6.0/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 06:39:31.917641 semantha_sdk-5.6.0/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0     1681 2023-07-12 16:01:12.009737 semantha_sdk-5.6.0/semantha_sdk/api/answers.py
+-rw-r--r--   0        0        0     1004 2023-07-12 16:01:11.925323 semantha_sdk-5.6.0/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      839 2023-07-12 16:01:11.928367 semantha_sdk-5.6.0/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      817 2023-07-12 16:01:11.961988 semantha_sdk-5.6.0/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1792 2023-07-12 16:01:11.949923 semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1576 2023-07-12 16:01:11.932882 semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     3766 2023-07-12 16:01:11.955987 semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3283 2023-07-12 16:01:11.959984 semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1346 2023-07-12 16:01:11.970505 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      923 2023-07-12 16:01:11.974018 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1913 2023-07-12 16:01:11.972507 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1735 2023-07-12 16:01:11.979031 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     3018 2023-07-12 16:01:11.967502 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      836 2023-07-12 16:01:11.964493 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1662 2023-07-12 16:01:11.982028 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1661 2023-07-12 16:01:11.987149 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1373 2023-07-12 16:01:11.991675 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1603 2023-07-12 16:01:11.994297 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_rules.py
+-rw-r--r--   0        0        0     1261 2023-07-12 16:01:11.996205 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1322 2023-07-12 16:01:11.997201 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0     1098 2023-07-12 16:01:11.977031 semantha_sdk-5.6.0/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0     1262 2023-07-12 16:01:12.089837 semantha_sdk-5.6.0/semantha_sdk/api/child_extractorclasses.py
+-rw-r--r--   0        0        0     5664 2023-07-12 16:01:12.036865 semantha_sdk-5.6.0/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1168 2023-07-12 16:01:11.999201 semantha_sdk-5.6.0/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1425 2023-07-12 16:01:12.004205 semantha_sdk-5.6.0/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     4012 2023-07-12 16:01:12.012736 semantha_sdk-5.6.0/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     1565 2023-07-12 16:01:12.017262 semantha_sdk-5.6.0/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1997 2023-07-12 16:01:12.015263 semantha_sdk-5.6.0/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     3464 2023-07-12 16:01:12.019266 semantha_sdk-5.6.0/semantha_sdk/api/documentcomparisons.py
+-rw-r--r--   0        0        0     8589 2023-07-12 16:01:12.021795 semantha_sdk-5.6.0/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     4497 2023-07-12 16:01:12.007737 semantha_sdk-5.6.0/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1157 2023-07-12 16:01:12.005736 semantha_sdk-5.6.0/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      905 2023-07-12 16:01:12.067244 semantha_sdk-5.6.0/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1757 2023-07-12 16:01:12.068246 semantha_sdk-5.6.0/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1595 2023-07-12 16:01:12.070245 semantha_sdk-5.6.0/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1019 2023-07-12 16:01:12.075763 semantha_sdk-5.6.0/semantha_sdk/api/model_attributes.py
+-rw-r--r--   0        0        0     1460 2023-07-12 16:01:12.079763 semantha_sdk-5.6.0/semantha_sdk/api/model_boostword.py
+-rw-r--r--   0        0        0     1924 2023-07-12 16:01:12.077767 semantha_sdk-5.6.0/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0     2088 2023-07-12 16:01:12.081765 semantha_sdk-5.6.0/semantha_sdk/api/model_dataproperties.py
+-rw-r--r--   0        0        0     1505 2023-07-12 16:01:12.084812 semantha_sdk-5.6.0/semantha_sdk/api/model_dataproperty.py
+-rw-r--r--   0        0        0      840 2023-07-12 16:01:12.071249 semantha_sdk-5.6.0/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     5566 2023-07-12 16:01:12.074753 semantha_sdk-5.6.0/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      816 2023-07-12 16:01:12.072249 semantha_sdk-5.6.0/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0     1830 2023-07-12 16:01:12.088836 semantha_sdk-5.6.0/semantha_sdk/api/model_extractorclass.py
+-rw-r--r--   0        0        0     2487 2023-07-12 16:01:12.086823 semantha_sdk-5.6.0/semantha_sdk/api/model_extractorclasses.py
+-rw-r--r--   0        0        0      951 2023-07-12 16:01:12.090831 semantha_sdk-5.6.0/semantha_sdk/api/model_extractors.py
+-rw-r--r--   0        0        0     1536 2023-07-12 16:01:12.094343 semantha_sdk-5.6.0/semantha_sdk/api/model_extractortable.py
+-rw-r--r--   0        0        0     2103 2023-07-12 16:01:12.092835 semantha_sdk-5.6.0/semantha_sdk/api/model_extractortables.py
+-rw-r--r--   0        0        0      855 2023-07-12 16:01:12.128055 semantha_sdk-5.6.0/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0      969 2023-07-12 16:01:12.095353 semantha_sdk-5.6.0/semantha_sdk/api/model_formatters.py
+-rw-r--r--   0        0        0     1904 2023-07-12 16:01:12.101358 semantha_sdk-5.6.0/semantha_sdk/api/model_metadata.py
+-rw-r--r--   0        0        0      852 2023-07-12 16:01:12.129053 semantha_sdk-5.6.0/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1970 2023-07-12 16:01:12.104354 semantha_sdk-5.6.0/semantha_sdk/api/model_namedentities.py
+-rw-r--r--   0        0        0     1494 2023-07-12 16:01:12.105482 semantha_sdk-5.6.0/semantha_sdk/api/model_namedentity.py
+-rw-r--r--   0        0        0      982 2023-07-12 16:01:12.106482 semantha_sdk-5.6.0/semantha_sdk/api/model_objectproperties.py
+-rw-r--r--   0        0        0     1441 2023-07-12 16:01:12.102358 semantha_sdk-5.6.0/semantha_sdk/api/model_onemetadata.py
+-rw-r--r--   0        0        0     1401 2023-07-12 16:01:12.111486 semantha_sdk-5.6.0/semantha_sdk/api/model_regex.py
+-rw-r--r--   0        0        0     1850 2023-07-12 16:01:12.108485 semantha_sdk-5.6.0/semantha_sdk/api/model_regexes.py
+-rw-r--r--   0        0        0     1444 2023-07-12 16:01:12.116004 semantha_sdk-5.6.0/semantha_sdk/api/model_relation.py
+-rw-r--r--   0        0        0     1902 2023-07-12 16:01:12.113482 semantha_sdk-5.6.0/semantha_sdk/api/model_relations.py
+-rw-r--r--   0        0        0     1388 2023-07-12 16:01:12.121535 semantha_sdk-5.6.0/semantha_sdk/api/model_rule.py
+-rw-r--r--   0        0        0      999 2023-07-12 16:01:12.118013 semantha_sdk-5.6.0/semantha_sdk/api/model_rulefunctions.py
+-rw-r--r--   0        0        0     1962 2023-07-12 16:01:12.119536 semantha_sdk-5.6.0/semantha_sdk/api/model_rules.py
+-rw-r--r--   0        0        0     1449 2023-07-12 16:01:12.124045 semantha_sdk-5.6.0/semantha_sdk/api/model_stopword.py
+-rw-r--r--   0        0        0     1907 2023-07-12 16:01:12.122533 semantha_sdk-5.6.0/semantha_sdk/api/model_stopwords.py
+-rw-r--r--   0        0        0     1430 2023-07-12 16:01:12.127054 semantha_sdk-5.6.0/semantha_sdk/api/model_synonym.py
+-rw-r--r--   0        0        0     1882 2023-07-12 16:01:12.126054 semantha_sdk-5.6.0/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1217 2023-07-12 16:01:12.022796 semantha_sdk-5.6.0/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     3928 2023-07-12 16:01:12.025320 semantha_sdk-5.6.0/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1450 2023-07-12 16:01:12.099352 semantha_sdk-5.6.0/semantha_sdk/api/modelont_instance.py
+-rw-r--r--   0        0        0     2592 2023-07-12 16:01:12.098353 semantha_sdk-5.6.0/semantha_sdk/api/modelont_instances.py
+-rw-r--r--   0        0        0     1663 2023-07-12 16:01:12.038854 semantha_sdk-5.6.0/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1711 2023-07-12 16:01:12.046376 semantha_sdk-5.6.0/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      792 2023-07-12 16:01:12.044363 semantha_sdk-5.6.0/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0     2267 2023-07-12 16:01:12.042852 semantha_sdk-5.6.0/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0    13183 2023-07-12 16:01:12.031320 semantha_sdk-5.6.0/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0    22267 2023-07-12 16:01:12.052898 semantha_sdk-5.6.0/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      867 2023-07-12 16:01:12.001202 semantha_sdk-5.6.0/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2113 2023-06-29 06:39:31.918640 semantha_sdk-5.6.0/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0      413 2023-06-29 06:39:31.920640 semantha_sdk-5.6.0/semantha_sdk/api/semantha_endpoint.py
+-rw-r--r--   0        0        0      967 2023-07-12 16:01:12.050218 semantha_sdk-5.6.0/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      786 2023-07-12 16:01:12.047385 semantha_sdk-5.6.0/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1497 2023-07-12 16:01:12.054983 semantha_sdk-5.6.0/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     5081 2023-07-12 16:01:12.057028 semantha_sdk-5.6.0/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     3934 2023-07-12 16:01:12.058000 semantha_sdk-5.6.0/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0      963 2023-07-12 16:01:12.040852 semantha_sdk-5.6.0/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0     1207 2023-07-12 16:01:12.060028 semantha_sdk-5.6.0/semantha_sdk/api/summarizations.py
+-rw-r--r--   0        0        0      931 2023-07-12 16:01:12.061997 semantha_sdk-5.6.0/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1285 2023-07-12 16:01:12.063995 semantha_sdk-5.6.0/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0     1018 2023-07-12 16:01:12.061028 semantha_sdk-5.6.0/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1383 2023-07-12 16:01:12.065238 semantha_sdk-5.6.0/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     5700 2023-07-12 16:01:12.372308 semantha_sdk-5.6.0/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      617 2023-07-12 16:01:12.305463 semantha_sdk-5.6.0/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      689 2023-07-12 16:01:12.245293 semantha_sdk-5.6.0/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      582 2023-07-12 16:01:12.332539 semantha_sdk-5.6.0/semantha_sdk/model/answer.py
+-rw-r--r--   0        0        0      548 2023-07-12 16:01:12.282596 semantha_sdk-5.6.0/semantha_sdk/model/answer_reference.py
+-rw-r--r--   0        0        0      658 2023-07-12 16:01:12.352331 semantha_sdk-5.6.0/semantha_sdk/model/argument.py
+-rw-r--r--   0        0        0      547 2023-07-12 16:01:12.339095 semantha_sdk-5.6.0/semantha_sdk/model/attribute_overview.py
+-rw-r--r--   0        0        0      581 2023-07-12 16:01:12.230242 semantha_sdk-5.6.0/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      989 2023-07-12 16:01:12.264429 semantha_sdk-5.6.0/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      515 2023-07-12 16:01:12.253293 semantha_sdk-5.6.0/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      717 2023-07-12 16:01:12.319004 semantha_sdk-5.6.0/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0      519 2023-07-12 16:01:12.233237 semantha_sdk-5.6.0/semantha_sdk/model/column.py
+-rw-r--r--   0        0        0     1201 2023-07-12 16:01:12.302276 semantha_sdk-5.6.0/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      627 2023-07-12 16:01:12.320004 semantha_sdk-5.6.0/semantha_sdk/model/condition.py
+-rw-r--r--   0        0        0      587 2023-07-12 16:01:12.303277 semantha_sdk-5.6.0/semantha_sdk/model/condition_value.py
+-rw-r--r--   0        0        0      545 2023-07-12 16:01:12.270379 semantha_sdk-5.6.0/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      639 2023-07-12 16:01:12.346320 semantha_sdk-5.6.0/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      483 2023-07-12 16:01:12.320998 semantha_sdk-5.6.0/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      532 2023-07-12 16:01:12.304280 semantha_sdk-5.6.0/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1302 2023-07-12 16:01:12.298274 semantha_sdk-5.6.0/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0     1004 2023-07-12 16:01:12.341091 semantha_sdk-5.6.0/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0      773 2023-07-12 16:01:12.309466 semantha_sdk-5.6.0/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      582 2023-07-12 16:01:12.306464 semantha_sdk-5.6.0/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      660 2023-07-12 16:01:12.272382 semantha_sdk-5.6.0/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1078 2023-07-12 16:01:12.268382 semantha_sdk-5.6.0/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      510 2023-07-12 16:01:12.329536 semantha_sdk-5.6.0/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      505 2023-07-12 16:01:12.236760 semantha_sdk-5.6.0/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      533 2023-07-12 16:01:12.226714 semantha_sdk-5.6.0/semantha_sdk/model/document_table.py
+-rw-r--r--   0        0        0      577 2023-07-12 16:01:12.292129 semantha_sdk-5.6.0/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      454 2023-07-12 16:01:12.314988 semantha_sdk-5.6.0/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      705 2023-07-12 16:01:12.307459 semantha_sdk-5.6.0/semantha_sdk/model/expression.py
+-rw-r--r--   0        0        0      604 2023-07-12 16:01:12.279596 semantha_sdk-5.6.0/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      757 2023-07-12 16:01:12.317005 semantha_sdk-5.6.0/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      546 2023-07-12 16:01:12.350333 semantha_sdk-5.6.0/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      671 2023-07-12 16:01:12.311460 semantha_sdk-5.6.0/semantha_sdk/model/extractor.py
+-rw-r--r--   0        0        0      762 2023-07-12 16:01:12.242775 semantha_sdk-5.6.0/semantha_sdk/model/extractor_attribute.py
+-rw-r--r--   0        0        0      924 2023-07-12 16:01:12.343095 semantha_sdk-5.6.0/semantha_sdk/model/extractor_class.py
+-rw-r--r--   0        0        0      704 2023-07-12 16:01:12.337097 semantha_sdk-5.6.0/semantha_sdk/model/extractor_class_overview.py
+-rw-r--r--   0        0        0      908 2023-07-12 16:01:12.323002 semantha_sdk-5.6.0/semantha_sdk/model/extractor_table.py
+-rw-r--r--   0        0        0      882 2023-07-12 16:01:12.349335 semantha_sdk-5.6.0/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      412 2023-07-12 16:01:12.278594 semantha_sdk-5.6.0/semantha_sdk/model/field.py
+-rw-r--r--   0        0        0      522 2023-07-12 16:01:12.251300 semantha_sdk-5.6.0/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      508 2023-07-12 16:01:12.284111 semantha_sdk-5.6.0/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      495 2023-07-12 16:01:12.287129 semantha_sdk-5.6.0/semantha_sdk/model/formatter.py
+-rw-r--r--   0        0        0      540 2023-07-12 16:01:12.312461 semantha_sdk-5.6.0/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0      889 2023-07-12 16:01:12.249294 semantha_sdk-5.6.0/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      547 2023-07-12 16:01:12.330531 semantha_sdk-5.6.0/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      575 2023-07-12 16:01:12.254818 semantha_sdk-5.6.0/semantha_sdk/model/instance_overview.py
+-rw-r--r--   0        0        0      415 2023-07-12 16:01:12.260316 semantha_sdk-5.6.0/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      478 2023-07-12 16:01:12.238770 semantha_sdk-5.6.0/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      602 2023-07-12 16:01:12.269377 semantha_sdk-5.6.0/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      490 2023-07-12 16:01:12.255334 semantha_sdk-5.6.0/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      421 2023-07-12 16:01:12.237770 semantha_sdk-5.6.0/semantha_sdk/model/matcher.py
+-rw-r--r--   0        0        0      611 2023-07-12 16:01:12.328537 semantha_sdk-5.6.0/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      509 2023-07-12 16:01:12.273382 semantha_sdk-5.6.0/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      506 2023-07-12 16:01:12.299276 semantha_sdk-5.6.0/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      437 2023-07-12 16:01:12.307459 semantha_sdk-5.6.0/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      557 2023-07-12 16:01:12.286131 semantha_sdk-5.6.0/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1553 2023-07-12 16:01:12.289699 semantha_sdk-5.6.0/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      495 2023-07-12 16:01:12.296275 semantha_sdk-5.6.0/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      491 2023-07-12 16:01:12.336080 semantha_sdk-5.6.0/semantha_sdk/model/overview.py
+-rw-r--r--   0        0        0      844 2023-07-12 16:01:12.301275 semantha_sdk-5.6.0/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      551 2023-07-12 16:01:12.354334 semantha_sdk-5.6.0/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0     1023 2023-07-12 16:01:12.316004 semantha_sdk-5.6.0/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      493 2023-07-12 16:01:12.277595 semantha_sdk-5.6.0/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      538 2023-07-12 16:01:12.327531 semantha_sdk-5.6.0/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      587 2023-07-12 16:01:12.276592 semantha_sdk-5.6.0/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      506 2023-07-12 16:01:12.344098 semantha_sdk-5.6.0/semantha_sdk/model/range.py
+-rw-r--r--   0        0        0      461 2023-07-12 16:01:12.347335 semantha_sdk-5.6.0/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      831 2023-07-12 16:01:12.266388 semantha_sdk-5.6.0/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      754 2023-07-12 16:01:12.355437 semantha_sdk-5.6.0/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      467 2023-07-12 16:01:12.357259 semantha_sdk-5.6.0/semantha_sdk/model/regex.py
+-rw-r--r--   0        0        0      705 2023-07-12 16:01:12.282596 semantha_sdk-5.6.0/semantha_sdk/model/relation.py
+-rw-r--r--   0        0        0      514 2023-07-12 16:01:12.348332 semantha_sdk-5.6.0/semantha_sdk/model/relation_condition.py
+-rw-r--r--   0        0        0      716 2023-07-12 16:01:12.275591 semantha_sdk-5.6.0/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      523 2023-07-12 16:01:12.262853 semantha_sdk-5.6.0/semantha_sdk/model/row.py
+-rw-r--r--   0        0        0      670 2023-07-12 16:01:12.246293 semantha_sdk-5.6.0/semantha_sdk/model/rule.py
+-rw-r--r--   0        0        0      554 2023-07-12 16:01:12.335070 semantha_sdk-5.6.0/semantha_sdk/model/rule_function.py
+-rw-r--r--   0        0        0      591 2023-07-12 16:01:12.313464 semantha_sdk-5.6.0/semantha_sdk/model/rule_overview.py
+-rw-r--r--   0        0        0      650 2023-06-29 06:39:31.921661 semantha_sdk-5.6.0/semantha_sdk/model/semantha_entity.py
+-rw-r--r--   0        0        0      905 2023-07-12 16:01:12.271384 semantha_sdk-5.6.0/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      525 2023-07-12 16:01:12.280596 semantha_sdk-5.6.0/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      830 2023-07-12 16:01:12.331537 semantha_sdk-5.6.0/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1757 2023-07-12 16:01:12.325531 semantha_sdk-5.6.0/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      464 2023-07-12 16:01:12.247297 semantha_sdk-5.6.0/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      702 2023-07-12 16:01:12.293197 semantha_sdk-5.6.0/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      892 2023-07-12 16:01:12.353333 semantha_sdk-5.6.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      640 2023-07-12 16:01:12.291128 semantha_sdk-5.6.0/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      490 2023-07-12 16:01:12.318007 semantha_sdk-5.6.0/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      577 2023-07-12 16:01:12.310463 semantha_sdk-5.6.0/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      476 2023-07-12 16:01:12.334057 semantha_sdk-5.6.0/semantha_sdk/model/table.py
+-rw-r--r--   0        0        0      450 2023-07-12 16:01:12.345320 semantha_sdk-5.6.0/semantha_sdk/model/table_cell.py
+-rw-r--r--   0        0        0      572 2023-07-12 16:01:12.338094 semantha_sdk-5.6.0/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      469 2023-07-12 16:01:12.294207 semantha_sdk-5.6.0/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      471 2023-07-12 16:01:12.351331 semantha_sdk-5.6.0/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.6.0/semantha_sdk/request/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.6.0/semantha_sdk/request/semantha_request.py
+-rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.6.0/semantha_sdk/response/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.6.0/semantha_sdk/response/semantha_error.py
+-rw-r--r--   0        0        0     3712 2023-06-20 12:43:00.735650 semantha_sdk-5.6.0/semantha_sdk/response/semantha_response.py
+-rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.6.0/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.6.0/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0    18061 1970-01-01 00:00:00.000000 semantha_sdk-5.6.0/PKG-INFO
```

### Comparing `semantha_sdk-5.5.0/LICENSE` & `semantha_sdk-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/pyproject.toml` & `semantha_sdk-5.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "5.5.0"
+version = "5.6.0"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
```

### Comparing `semantha_sdk-5.5.0/README.md` & `semantha_sdk-5.6.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 ### Disclaimer
 
 **IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
 Use with caution and on own risk.
 
 ## Update Notes
 
+### Version 5.6.0
+Adde most endpoints in **/api/models/* **
+
 ### Version 5.5.0
 Removed language parameter on **/api/domains/{domainname}/references**
 Fixed bug on serialization of **/api/domains/{domainname}/modelinstances** response.
 Fixed return of binary responses of bulk services.
 
 ### Version 5.4.0
 Added **new** service: 
@@ -127,15 +130,15 @@
 - [x] **/bulk/domains/{domainname}** -> BulkdomainsDomainEndpoint
 - [x] **/bulk/domains/{domainname}/documentclasses** -> BulkdomainsDocumentclassesEndpoint
     - [x] **GET** -> List[DocumentClassBulk]
     - [x] **POST** -> None
 - [x] **/bulk/domains/{domainname}/referencedocuments** -> BulkdomainsReferencedocumentsEndpoint
     - [x] **GET** -> List[Document]
     - [x] **POST** -> None
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/bulk/domains/{domainname}/references** -> BulkdomainsReferencesEndpoint
     - [x] **POST** -> List[Document]
 - [x] **/bulk/model** -> BulkModelEndpoint
 - [x] **/bulk/model/domains** -> BulkmodelDomainsEndpoint
 - [x] **/bulk/model/domains/{domainname}** -> BulkmodelDomainEndpoint
 - [x] **/bulk/model/domains/{domainname}/boostwords** -> BulkmodelBoostwordsEndpoint
     - [x] **POST** -> None
@@ -152,15 +155,17 @@
     - [x] **GET** -> List[Instance]
     - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/metadata** -> BulkmodelMetadataEndpoint
     - [x] **GET** -> List[Metadata]
     - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/namedentities** -> BulkmodelNamedentitiesEndpoint
     - [x] **POST** -> None
-- [ ] **/bulk/model/domains/{domainname}/rules** 
+- [x] **/bulk/model/domains/{domainname}/rules** -> BulkmodelRulesEndpoint
+    - [x] **GET** -> List[Rule]
+    - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/stopwords** -> BulkmodelStopwordsEndpoint
     - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/synonyms** -> BulkmodelSynonymsEndpoint
     - [x] **POST** -> None
 - [x] **/currentuser** -> CurrentuserEndpoint
     - [x] **GET** -> CurrentUser
 - [x] **/currentuser/roles** -> RolesEndpoint
@@ -170,143 +175,208 @@
 - [x] **/domains** -> DomainsEndpoint
     - [x] **GET** -> List[Domain]
 - [x] **/domains/{domainname}** -> DomainEndpoint
     - [x] **GET** -> Domain
 - [x] **/domains/{domainname}/answers** -> AnswersEndpoint
     - [x] **POST** -> Answer
 - [x] **/domains/{domainname}/documentannotations** -> DocumentannotationsEndpoint
-    - [x] **POST** -> IOBase
+    - [x] **POST** (Accept: docx) -> IOBase
+    - [x] **POST** (Accept: pdf) -> IOBase
 - [x] **/domains/{domainname}/documentclasses** -> DocumentclassesEndpoint
     - [x] **GET** -> List[DocumentClass]
     - [x] **POST** -> DocumentClass
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/domains/{domainname}/documentclasses/{id}** -> DocumentclassEndpoint
     - [x] **GET** -> DocumentClass
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PUT** -> DocumentClass
 - [ ] **/domains/{domainname}/documentclasses/{id}/documentclasses** 
 - [ ] **/domains/{domainname}/documentclasses/{id}/referencedocuments** 
 - [x] **/domains/{domainname}/documentcomparisons** -> DocumentcomparisonsEndpoint
-    - [x] **POST** -> IOBase
+    - [x] **POST** (Accept: xlsx) -> IOBase
 - [x] **/domains/{domainname}/documents** -> DocumentsEndpoint
     - [x] **POST** -> List[Document]
+    - [x] **POST** (Accept: xlsx) -> IOBase
+    - [x] **POST** (Accept: docx) -> IOBase
 - [x] **/domains/{domainname}/modelclasses** -> ModelclassesEndpoint
     - [x] **GET** -> List[ModelClass]
 - [x] **/domains/{domainname}/modelinstances** -> ModelinstancesEndpoint
     - [x] **POST** -> SemanticModel
+    - [x] **POST** (Accept: xlsx) -> IOBase
 - [x] **/domains/{domainname}/referencedocuments** -> ReferencedocumentsEndpoint
     - [x] **GET** -> ReferenceDocumentsResponseContainer
+    - [x] **GET** (Accept: xlsx) -> IOBase
     - [x] **POST** -> List[DocumentInformation]
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/domains/{domainname}/referencedocuments/clusters** -> ClustersEndpoint
     - [x] **GET** -> SmartClusterResponseContainer
     - [x] **PUT** -> SmartClusterResponseContainer
 - [x] **/domains/{domainname}/referencedocuments/namedentities** -> NamedentitiesEndpoint
     - [x] **GET** -> List[DocumentNamedEntity]
 - [x] **/domains/{domainname}/referencedocuments/statistic** -> StatisticEndpoint
     - [x] **GET** -> Statistic
 - [x] **/domains/{domainname}/referencedocuments/{documentid}** -> ReferencedocumentEndpoint
     - [x] **GET** -> Document
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PATCH** -> DocumentInformation
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs** -> ParagraphsEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs/{id}** -> ParagraphEndpoint
     - [x] **GET** -> Paragraph
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PATCH** -> Paragraph
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences** -> SentencesEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences/{id}** -> SentenceEndpoint
     - [x] **GET** -> Sentence
 - [x] **/domains/{domainname}/references** -> ReferencesEndpoint
     - [x] **POST** -> Document
+    - [x] **POST** (Accept: xlsx) -> IOBase
+    - [x] **POST** (Accept: docx) -> IOBase
+    - [x] **POST** (Accept: pdf) -> IOBase
 - [x] **/domains/{domainname}/settings** -> SettingsEndpoint
     - [x] **GET** -> Settings
     - [x] **PATCH** -> Settings
 - [x] **/domains/{domainname}/similaritymatrix** -> SimilaritymatrixEndpoint
     - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/similaritymatrix/cluster** -> SimilaritymatrixClusterEndpoint
     - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/summarizations** -> SummarizationsEndpoint
     - [x] **POST** -> str
 - [x] **/domains/{domainname}/tags** -> TagsEndpoint
     - [x] **GET** -> List[str]
 - [x] **/domains/{domainname}/tags/{tagname}** -> TagEndpoint
 - [x] **/domains/{domainname}/tags/{tagname}/referencedocuments** -> TagReferencedocumentsEndpoint
     - [x] **GET** -> List[DocumentInformation]
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/domains/{domainname}/validation** -> ValidationEndpoint
     - [x] **POST** -> SemanticModel
 - [x] **/info** -> InfoEndpoint
     - [x] **GET** -> Info
 - [x] **/languages** -> LanguagesEndpoint
     - [x] **POST** -> LanguageDetection
 - [x] **/model** -> ModelEndpoint
 - [x] **/model/datatypes** -> ModelDatatypesEndpoint
     - [x] **GET** -> List[str]
 - [x] **/model/domains** -> ModelDomainsEndpoint
 - [x] **/model/domains/{domainname}** -> ModelDomainEndpoint
-    - [x] **GET** -> IOBase
+    - [x] **GET** (Accept: xlsx) -> IOBase
     - [x] **PATCH** -> IOBase
-- [ ] **/model/domains/{domainname}/attributes** 
+- [x] **/model/domains/{domainname}/attributes** -> ModelAttributesEndpoint
+    - [x] **GET** -> List[AttributeOverview]
 - [ ] **/model/domains/{domainname}/backups** 
 - [x] **/model/domains/{domainname}/boostwords** -> ModelBoostwordsEndpoint
     - [x] **GET** -> List[BoostWord]
     - [x] **POST** -> BoostWord
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/boostwords/{id}** -> ModelBoostwordEndpoint
     - [x] **GET** -> BoostWord
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PUT** -> BoostWord
 - [ ] **/model/domains/{domainname}/classes** 
 - [ ] **/model/domains/{domainname}/classes/{classid}** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/attributes** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/attributes/{id}** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/instances** 
-- [ ] **/model/domains/{domainname}/dataproperties** 
-- [ ] **/model/domains/{domainname}/dataproperties/{id}** 
-- [ ] **/model/domains/{domainname}/extractorclasses** 
-- [ ] **/model/domains/{domainname}/extractorclasses/{id}** 
-- [ ] **/model/domains/{domainname}/extractorclasses/{id}/extractorclasses** 
-- [ ] **/model/domains/{domainname}/extractors** 
-- [ ] **/model/domains/{domainname}/extractortables** 
-- [ ] **/model/domains/{domainname}/extractortables/{id}** 
-- [ ] **/model/domains/{domainname}/formatters** 
-- [ ] **/model/domains/{domainname}/instances** 
-- [ ] **/model/domains/{domainname}/instances/{id}** 
-- [ ] **/model/domains/{domainname}/metadata** 
-- [ ] **/model/domains/{domainname}/metadata/{id}** 
+- [x] **/model/domains/{domainname}/dataproperties** -> ModelDatapropertiesEndpoint
+    - [x] **GET** -> List[Overview]
+    - [x] **POST** -> DataProperty
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/dataproperties/{id}** -> ModelDatapropertyEndpoint
+    - [x] **GET** -> DataProperty
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> DataProperty
+- [x] **/model/domains/{domainname}/extractorclasses** -> ModelExtractorclassesEndpoint
+    - [x] **GET** -> List[ExtractorClassOverview]
+    - [x] **POST** -> ExtractorClass
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> None
+- [x] **/model/domains/{domainname}/extractorclasses/{id}** -> ModelExtractorclassEndpoint
+    - [x] **GET** -> ExtractorClass
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> ExtractorClass
+- [x] **/model/domains/{domainname}/extractorclasses/{id}/extractorclasses** -> ChildExtractorclassesEndpoint
+    - [x] **POST** -> ExtractorClass
+- [x] **/model/domains/{domainname}/extractors** -> ModelExtractorsEndpoint
+    - [x] **GET** -> List[Entity]
+- [x] **/model/domains/{domainname}/extractortables** -> ModelExtractortablesEndpoint
+    - [x] **GET** -> List[Table]
+    - [x] **POST** -> ExtractorTable
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/extractortables/{id}** -> ModelExtractortableEndpoint
+    - [x] **GET** -> ExtractorTable
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> ExtractorTable
+- [x] **/model/domains/{domainname}/formatters** -> ModelFormattersEndpoint
+    - [x] **GET** -> List[Formatter]
+- [x] **/model/domains/{domainname}/instances** -> ModelontInstancesEndpoint
+    - [x] **GET** -> List[InstanceOverview]
+    - [x] **GET** (Accept: xlsx) -> IOBase
+    - [x] **POST** -> Instance
+    - [x] **DELETE** -> None
+    - [x] **PATCH** -> None
+- [x] **/model/domains/{domainname}/instances/{id}** -> ModelontInstanceEndpoint
+    - [x] **GET** -> Instance
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Instance
+- [x] **/model/domains/{domainname}/metadata** -> ModelMetadataEndpoint
+    - [x] **GET** -> List[Metadata]
+    - [x] **POST** -> Metadata
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/metadata/{id}** -> ModelOnemetadataEndpoint
+    - [x] **GET** -> Metadata
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Metadata
 - [x] **/model/domains/{domainname}/namedentities** -> ModelNamedentitiesEndpoint
     - [x] **GET** -> List[NamedEntity]
     - [x] **POST** -> NamedEntity
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/namedentities/{id}** -> ModelNamedentityEndpoint
     - [x] **GET** -> NamedEntity
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PUT** -> NamedEntity
-- [ ] **/model/domains/{domainname}/objectproperties** 
-- [ ] **/model/domains/{domainname}/regexes** 
-- [ ] **/model/domains/{domainname}/regexes/{id}** 
-- [ ] **/model/domains/{domainname}/relations** 
-- [ ] **/model/domains/{domainname}/relations/{id}** 
-- [ ] **/model/domains/{domainname}/rulefunctions** 
-- [ ] **/model/domains/{domainname}/rules** 
-- [ ] **/model/domains/{domainname}/rules/{id}** 
+- [x] **/model/domains/{domainname}/objectproperties** -> ModelObjectpropertiesEndpoint
+    - [x] **GET** -> List[Overview]
+- [x] **/model/domains/{domainname}/regexes** -> ModelRegexesEndpoint
+    - [x] **GET** -> List[Regex]
+    - [x] **POST** -> Regex
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/regexes/{id}** -> ModelRegexEndpoint
+    - [x] **GET** -> Regex
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Regex
+- [x] **/model/domains/{domainname}/relations** -> ModelRelationsEndpoint
+    - [x] **GET** -> List[Relation]
+    - [x] **POST** -> Relation
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/relations/{id}** -> ModelRelationEndpoint
+    - [x] **GET** -> Relation
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Relation
+- [x] **/model/domains/{domainname}/rulefunctions** -> ModelRulefunctionsEndpoint
+    - [x] **GET** -> List[RuleFunction]
+- [x] **/model/domains/{domainname}/rules** -> ModelRulesEndpoint
+    - [x] **GET** -> List[RuleOverview]
+    - [x] **POST** -> Rule
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/rules/{id}** -> ModelRuleEndpoint
+    - [x] **GET** -> Rule
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Rule
 - [x] **/model/domains/{domainname}/stopwords** -> ModelStopwordsEndpoint
     - [x] **GET** -> List[StopWord]
     - [x] **POST** -> StopWord
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/stopwords/{id}** -> ModelStopwordEndpoint
     - [x] **GET** -> StopWord
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PUT** -> StopWord
 - [x] **/model/domains/{domainname}/synonyms** -> ModelSynonymsEndpoint
     - [x] **GET** -> List[Synonym]
     - [x] **POST** -> Synonym
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/synonyms/{id}** -> ModelSynonymEndpoint
     - [x] **GET** -> Synonym
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PUT** -> Synonym
 - [x] **/model/extractortypes** -> ModelExtractortypesEndpoint
     - [x] **GET** -> List[str]
 - [x] **/model/metadatatypes** -> ModelMetadatatypesEndpoint
     - [x] **GET** -> List[str]
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/__init__.py` & `semantha_sdk-5.6.0/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/answers.py` & `semantha_sdk-5.6.0/semantha_sdk/api/answers.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulk.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulk_domains.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulk_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulk_model.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulk_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_documentclasses.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_domain.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_referencedocuments.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_referencedocuments.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         tags: str = None,
         metadata: str = None,
         file: IOBase = None,
         text: str = None,
         documenttype: str = None,
         color: str = None,
         comment: str = None,
-        documentclass: str = None,
+        documentclassid: str = None,
         addparagraphsasdocuments: bool = None,
         detectlanguage: bool = None,
     ) -> None:
         """
         Upload reference document
             This is the quiet version of  'post /api/domains/{domainname}/referencedocuments'
         Args:
@@ -55,15 +55,15 @@
     tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
     metadata (str): Filter by metadata
     file (IOBase): Input document (left document).
     text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
     documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
     color (str): Use this parameter to specify the color for your reference document. Possible values are RED, MAGENTA, AQUA, ORANGE, GREY, or LAVENDER.
     comment (str): Use this parameter to add a comment to your reference document.
-    documentclass (str): 
+    documentclassid (str): 
     addparagraphsasdocuments (bool): Use this parameter to create individual reference documents in the library for each paragraph in your document. The parameter is of type boolean and is set to false by default.
         """
         q_params = {}
         if detectlanguage is not None:
             q_params["detectlanguage"] = detectlanguage
         response = self._session.post(
             url=self._endpoint,
@@ -72,15 +72,15 @@
                 "tags": tags,
                 "metadata": metadata,
                 "file": file,
                 "text": text,
                 "documenttype": documenttype,
                 "color": color,
                 "comment": comment,
-                "documentclass": documentclass,
+                "documentclassid": documentclassid,
                 "addparagraphsasdocuments": addparagraphsasdocuments,
             },
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_references.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkdomains_references.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         synonymousthreshold: float = None,
         marknomatch: bool = None,
         withreferencetext: bool = None,
         withareas: bool = None,
         mode: str = None,
         detectlanguage: bool = None,
         maxreferences: int = None,
-        withcontext: bool = None,
         considertexttype: bool = None,
         resizeparagraphs: bool = None,
     ) -> List[Document]:
         """
         Determine references with several input documents
             Matches several input documents ('file' parameter, as an alternative 'text' can be used) to a set of 'referencedocument' if set or internal library. If you match against internal library the 'tags' parameter can be used to filter the library.
         Args:
@@ -64,16 +63,14 @@
             q_params["withareas"] = withareas
         if mode is not None:
             q_params["mode"] = mode
         if detectlanguage is not None:
             q_params["detectlanguage"] = detectlanguage
         if maxreferences is not None:
             q_params["maxreferences"] = maxreferences
-        if withcontext is not None:
-            q_params["withcontext"] = withcontext
         if considertexttype is not None:
             q_params["considertexttype"] = considertexttype
         if resizeparagraphs is not None:
             q_params["resizeparagraphs"] = resizeparagraphs
         response = self._session.post(
             url=self._endpoint,
             json=DocumentSchema().dump(body),
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_boostwords.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_class.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_classes.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_classes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_dataproperties.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_domain.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from semantha_sdk.api.bulkmodel_boostwords import BulkmodelBoostwordsEndpoint
 from semantha_sdk.api.bulkmodel_classes import BulkmodelClassesEndpoint
 from semantha_sdk.api.bulkmodel_dataproperties import BulkmodelDatapropertiesEndpoint
 from semantha_sdk.api.bulkmodel_instances import BulkmodelInstancesEndpoint
 from semantha_sdk.api.bulkmodel_metadata import BulkmodelMetadataEndpoint
 from semantha_sdk.api.bulkmodel_namedentities import BulkmodelNamedentitiesEndpoint
+from semantha_sdk.api.bulkmodel_rules import BulkmodelRulesEndpoint
 from semantha_sdk.api.bulkmodel_stopwords import BulkmodelStopwordsEndpoint
 from semantha_sdk.api.bulkmodel_synonyms import BulkmodelSynonymsEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
 class BulkmodelDomainEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
@@ -26,14 +27,15 @@
         self._domainname = domainname
         self.__boostwords = BulkmodelBoostwordsEndpoint(session, self._endpoint)
         self.__classes = BulkmodelClassesEndpoint(session, self._endpoint)
         self.__dataproperties = BulkmodelDatapropertiesEndpoint(session, self._endpoint)
         self.__instances = BulkmodelInstancesEndpoint(session, self._endpoint)
         self.__metadata = BulkmodelMetadataEndpoint(session, self._endpoint)
         self.__namedentities = BulkmodelNamedentitiesEndpoint(session, self._endpoint)
+        self.__rules = BulkmodelRulesEndpoint(session, self._endpoint)
         self.__stopwords = BulkmodelStopwordsEndpoint(session, self._endpoint)
         self.__synonyms = BulkmodelSynonymsEndpoint(session, self._endpoint)
 
     @property
     def boostwords(self) -> BulkmodelBoostwordsEndpoint:
         return self.__boostwords
     @property
@@ -48,14 +50,17 @@
     @property
     def metadata(self) -> BulkmodelMetadataEndpoint:
         return self.__metadata
     @property
     def namedentities(self) -> BulkmodelNamedentitiesEndpoint:
         return self.__namedentities
     @property
+    def rules(self) -> BulkmodelRulesEndpoint:
+        return self.__rules
+    @property
     def stopwords(self) -> BulkmodelStopwordsEndpoint:
         return self.__stopwords
     @property
     def synonyms(self) -> BulkmodelSynonymsEndpoint:
         return self.__synonyms
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_domains.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_instances.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_metadata.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_namedentities.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_stopwords.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_synonyms.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodel_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodelclass_instances.py` & `semantha_sdk-5.6.0/semantha_sdk/api/bulkmodelclass_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/clusters.py` & `semantha_sdk-5.6.0/semantha_sdk/api/clusters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/currentuser.py` & `semantha_sdk-5.6.0/semantha_sdk/api/currentuser.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/diff.py` & `semantha_sdk-5.6.0/semantha_sdk/api/diff.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/documentannotations.py` & `semantha_sdk-5.6.0/semantha_sdk/api/documentannotations.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
 
     
-    def post(
+    def post_as_docx(
         self,
         file: IOBase = None,
         document: Document = None,
         similaritythreshold: float = None,
         synonymousthreshold: float = None,
         marknomatch: bool = None,
         withreferencetext: bool = None,
@@ -48,15 +48,50 @@
                 "file": file,
                 "document": document,
                 "similaritythreshold": similaritythreshold,
                 "synonymousthreshold": synonymousthreshold,
                 "marknomatch": marknomatch,
                 "withreferencetext": withreferencetext,
             },
-            headers=RestClient.to_header(MediaType.XLSX),
+            headers=RestClient.to_header(MediaType.DOCX),
+            q_params=q_params
+        ).execute()
+        return response.as_bytesio()
+    def post_as_pdf(
+        self,
+        file: IOBase = None,
+        document: Document = None,
+        similaritythreshold: float = None,
+        synonymousthreshold: float = None,
+        marknomatch: bool = None,
+        withreferencetext: bool = None,
+    ) -> IOBase:
+        """
+        Download the original input document with the referenced document/library matches as annotated comments
+        Args:
+        file (IOBase): Input document (left document).
+    document (Document): 
+    similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
+            In general, the higher the threshold, the more precise the results.
+    synonymousthreshold (float): Threshold for good matches.
+    marknomatch (bool): Marks the paragraphs that have not matched
+    withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
+                "document": document,
+                "similaritythreshold": similaritythreshold,
+                "synonymousthreshold": synonymousthreshold,
+                "marknomatch": marknomatch,
+                "withreferencetext": withreferencetext,
+            },
+            headers=RestClient.to_header(MediaType.PDF),
             q_params=q_params
         ).execute()
         return response.as_bytesio()
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/documentclass.py` & `semantha_sdk-5.6.0/semantha_sdk/api/documentclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/documentclasses.py` & `semantha_sdk-5.6.0/semantha_sdk/api/documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/documentcomparisons.py` & `semantha_sdk-5.6.0/semantha_sdk/api/documentcomparisons.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,25 +18,24 @@
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
 
     
-    def post(
+    def post_as_xlsx(
         self,
         file: IOBase = None,
         referencedocument: IOBase = None,
         similaritythreshold: float = None,
         synonymousthreshold: float = None,
         marknomatch: bool = None,
         withreferencetext: bool = None,
         documenttype: str = None,
         metadata: List[DocumentMetaData] = None,
-        withcontext: bool = None,
         considertexttype: bool = None,
         resizeparagraphs: bool = None,
         xlsxlegalstandard: bool = None,
     ) -> IOBase:
         """
         Determine references (for temporary data)
         Args:
@@ -45,15 +44,14 @@
     similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
             In general, the higher the threshold, the more precise the results.
     synonymousthreshold (float): Threshold for good matches.
     marknomatch (bool): Marks the paragraphs that have not matched
     withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
     documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
     metadata (List[DocumentMetaData]): Filter by metadata
-    withcontext (bool): Creates and saves the context.
     considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
     resizeparagraphs (bool): Automatically resizes paragraphs based on their semantic meaning.
     xlsxlegalstandard (bool): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
@@ -62,15 +60,14 @@
                 "referencedocument": referencedocument,
                 "similaritythreshold": similaritythreshold,
                 "synonymousthreshold": synonymousthreshold,
                 "marknomatch": marknomatch,
                 "withreferencetext": withreferencetext,
                 "documenttype": documenttype,
                 "metadata": metadata,
-                "withcontext": withcontext,
                 "considertexttype": considertexttype,
                 "resizeparagraphs": resizeparagraphs,
                 "xlsxlegalstandard": xlsxlegalstandard,
             },
             headers=RestClient.to_header(MediaType.XLSX),
             q_params=q_params
         ).execute()
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/documents.py` & `semantha_sdk-5.6.0/semantha_sdk/api/similaritymatrix_cluster.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,72 @@
-from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document import Document
-from semantha_sdk.model.document import DocumentSchema
+from semantha_sdk.model.matrix_row import MatrixRow
+from semantha_sdk.model.matrix_row import MatrixRowSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-class DocumentsEndpoint(SemanthaAPIEndpoint):
+class SimilaritymatrixClusterEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/documents"
+        return self._parent_endpoint + "/cluster"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
 
     
     def post(
         self,
-        file: IOBase = None,
-        text: str = None,
-        type: str = None,
-        documenttype: str = None,
-        withareas: bool = None,
-        withcontext: bool = None,
+        tags: str = None,
+        documentids: List[str] = None,
+        documentclassids: List[str] = None,
+        similaritythreshold: float = None,
         mode: str = None,
-        withparagraphtype: bool = None,
-    ) -> List[Document]:
+        considertexttype: bool = None,
+    ) -> List[MatrixRow]:
         """
-        Create a document model
+        Get document clusters
+            Consolidate the documents to clusters based on the results of `post post /api/domains/{domainname}/similaritymatrix`
         Args:
-        file (IOBase): Input document (left document).
-    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
-    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
-    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-    withareas (bool): Gives back the coordinates of referenced area.
-    withcontext (bool): Creates and saves the context.
+        tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    documentids (List[str]): List of document Ids for target. The limit here is 65000 IDs.
+            The IDs are passed as a JSON array.
+    documentclassids (List[str]): List of documentclass IDs for the target. The limit here is 1000 IDs.
+            The IDs are passed as a JSON array.
+            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
+    similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
+            In general, the higher the threshold, the more precise the results.
     mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
             fingerprint: semantic search based on sentences; 
             keyword: keyword: search based on sentences; 
             document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
             document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
             fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
             Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-    withparagraphtype (bool): The type of the paragraph, for example heading, text
+    considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             body={
-                "file": file,
-                "text": text,
-                "type": type,
-                "documenttype": documenttype,
-                "withareas": withareas,
-                "withcontext": withcontext,
+                "tags": tags,
+                "documentids": documentids,
+                "documentclassids": documentclassids,
+                "similaritythreshold": similaritythreshold,
                 "mode": mode,
-                "withparagraphtype": withparagraphtype,
+                "considertexttype": considertexttype,
             },
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
-        return response.to(DocumentSchema)
+        return response.to(MatrixRowSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/domain.py` & `semantha_sdk-5.6.0/semantha_sdk/api/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/domains.py` & `semantha_sdk-5.6.0/semantha_sdk/api/domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/info.py` & `semantha_sdk-5.6.0/semantha_sdk/api/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/languages.py` & `semantha_sdk-5.6.0/semantha_sdk/api/languages.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_boostword.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_boostword.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_boostwords.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_datatypes.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_datatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_domain.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_namedentities.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,69 @@
-from io import IOBase
-from semantha_sdk.api.model_boostwords import ModelBoostwordsEndpoint
-from semantha_sdk.api.model_namedentities import ModelNamedentitiesEndpoint
-from semantha_sdk.api.model_stopwords import ModelStopwordsEndpoint
-from semantha_sdk.api.model_synonyms import ModelSynonymsEndpoint
+from semantha_sdk.api.model_namedentity import ModelNamedentityEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
+from semantha_sdk.model.named_entity import NamedEntity
+from semantha_sdk.model.named_entity import NamedEntitySchema
+from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
+from typing import List
 
-class ModelDomainEndpoint(SemanthaAPIEndpoint):
+class ModelNamedentitiesEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + f"/{self._domainname}"
+        return self._parent_endpoint + "/namedentities"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
-        domainname: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
-        self._domainname = domainname
-        self.__boostwords = ModelBoostwordsEndpoint(session, self._endpoint)
-        self.__namedentities = ModelNamedentitiesEndpoint(session, self._endpoint)
-        self.__stopwords = ModelStopwordsEndpoint(session, self._endpoint)
-        self.__synonyms = ModelSynonymsEndpoint(session, self._endpoint)
 
-    @property
-    def boostwords(self) -> ModelBoostwordsEndpoint:
-        return self.__boostwords
-    @property
-    def namedentities(self) -> ModelNamedentitiesEndpoint:
-        return self.__namedentities
-    @property
-    def stopwords(self) -> ModelStopwordsEndpoint:
-        return self.__stopwords
-    @property
-    def synonyms(self) -> ModelSynonymsEndpoint:
-        return self.__synonyms
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelNamedentityEndpoint:
+        return ModelNamedentityEndpoint(self._session, self._endpoint, id)
 
     def get(
         self,
-    ) -> IOBase:
+    ) -> List[NamedEntity]:
         """
-        Get a domain by domainname
+        Get custom entities
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params).execute().as_bytesio()
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(NamedEntitySchema)
 
-    
-    def patch(
+    def post(
         self,
-        file: IOBase
-    ) -> IOBase:
+        body: NamedEntity = None,
+    ) -> NamedEntity:
         """
-        Update a domain by domainname
+        Create a custom entity
+        Args:
+        body (NamedEntity): 
         """
-        return self._session.patch(
+        q_params = {}
+        response = self._session.post(
             url=self._endpoint,
-            json=file
-        ).execute().as_bytesio()
+            json=NamedEntitySchema().dump(body),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(NamedEntitySchema)
 
     
+    def delete(
+        self,
+    ) -> None:
+        """
+        Delete all custom entities
+        """
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
+
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_domains.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_extractortypes.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_extractortypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_metadatatypes.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_metadatatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_namedentities.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_regexes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from semantha_sdk.api.model_namedentity import ModelNamedentityEndpoint
+from semantha_sdk.api.model_regex import ModelRegexEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.named_entity import NamedEntity
-from semantha_sdk.model.named_entity import NamedEntitySchema
+from semantha_sdk.model.regex import Regex
+from semantha_sdk.model.regex import RegexSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-class ModelNamedentitiesEndpoint(SemanthaAPIEndpoint):
+class ModelRegexesEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/namedentities"
+        return self._parent_endpoint + "/regexes"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
     def __call__(
             self,
             id: str,
-    ) -> ModelNamedentityEndpoint:
-        return ModelNamedentityEndpoint(self._session, self._endpoint, id)
+    ) -> ModelRegexEndpoint:
+        return ModelRegexEndpoint(self._session, self._endpoint, id)
 
     def get(
         self,
-    ) -> List[NamedEntity]:
+    ) -> List[Regex]:
         """
-        Get custom entities
+        Get all regexes
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(NamedEntitySchema)
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(RegexSchema)
 
     def post(
         self,
-        body: NamedEntity = None,
-    ) -> NamedEntity:
+        body: Regex = None,
+    ) -> Regex:
         """
-        Create a custom entity
+        Create a new regex
         Args:
-        body (NamedEntity): 
+        body (Regex): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=NamedEntitySchema().dump(body),
+            json=RegexSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
-        return response.to(NamedEntitySchema)
+        return response.to(RegexSchema)
 
     
     def delete(
         self,
     ) -> None:
         """
-        Delete all custom entities
+        Delete all regexes
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_namedentity.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_namedentity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_stopword.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_stopword.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_stopwords.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_synonym.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/model_synonyms.py` & `semantha_sdk-5.6.0/semantha_sdk/api/model_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/modelclasses.py` & `semantha_sdk-5.6.0/semantha_sdk/api/modelclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/modelinstances.py` & `semantha_sdk-5.6.0/semantha_sdk/api/modelinstances.py`

 * *Files 20% similar despite different names*

```diff
@@ -57,11 +57,51 @@
                 "documentextractor": documentextractor,
                 "applymatchersfordocumentextractor": applymatchersfordocumentextractor,
             },
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(SemanticModelSchema)
+    def post_as_xlsx(
+        self,
+        file: IOBase = None,
+        documentextractor: str = None,
+        applymatchersfordocumentextractor: bool = None,
+        withimages: bool = None,
+        withdocument: bool = None,
+        withadditionalroots: bool = None,
+        documenttype: str = None,
+        uilanguage: str = None,
+    ) -> IOBase:
+        """
+        Extract semantic model for a list of documents
+        Args:
+        file (IOBase): Input document (left document).
+    documentextractor (str): The document extractor you want to be considered.
+    applymatchersfordocumentextractor (bool): 
+        """
+        q_params = {}
+        if withimages is not None:
+            q_params["withimages"] = withimages
+        if withdocument is not None:
+            q_params["withdocument"] = withdocument
+        if withadditionalroots is not None:
+            q_params["withadditionalroots"] = withadditionalroots
+        if documenttype is not None:
+            q_params["documenttype"] = documenttype
+        if uilanguage is not None:
+            q_params["uilanguage"] = uilanguage
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
+                "documentextractor": documentextractor,
+                "applymatchersfordocumentextractor": applymatchersfordocumentextractor,
+            },
+            headers=RestClient.to_header(MediaType.XLSX),
+            q_params=q_params
+        ).execute()
+        return response.as_bytesio()
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/namedentities.py` & `semantha_sdk-5.6.0/semantha_sdk/api/namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/paragraph.py` & `semantha_sdk-5.6.0/semantha_sdk/api/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/paragraphs.py` & `semantha_sdk-5.6.0/semantha_sdk/api/paragraphs.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/referencedocument.py` & `semantha_sdk-5.6.0/semantha_sdk/api/referencedocument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/referencedocuments.py` & `semantha_sdk-5.6.0/semantha_sdk/api/referencedocuments.py`

 * *Files 20% similar despite different names*

```diff
@@ -118,41 +118,119 @@
             q_params["limit"] = limit
         if sort is not None:
             q_params["sort"] = sort
         if fields is not None:
             q_params["fields"] = fields
     
         return self._session.get(self._endpoint, q_params=q_params).execute().to(ReferenceDocumentsResponseContainerSchema)
+    def get_as_xlsx(
+        self,
+        tags: str = None,
+        documentids: str = None,
+        name: str = None,
+        createdafter: int = None,
+        createdbefore: int = None,
+        updatedafter: int = None,
+        updatedbefore: int = None,
+        documentclassids: str = None,
+        withoutdocumentclass: bool = None,
+        mincharacters: int = None,
+        metadata: str = None,
+        comment: str = None,
+        offset: int = None,
+        limit: int = None,
+        sort: str = None,
+        fields: str = None,
+    ) -> IOBase:
+        """
+        Get all reference documents
+            Please be aware that this service is limited: The query parameter ‚tags‘ can only be used in combination with an JSON export.
+        Args:
+        tags str: List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    documentids str: List of document Ids for target. The limit here is 65000 IDs.
+            The IDs are passed as a JSON array.
+    name str: The document name in your library (in contrast to the file name being used during upload).
+    createdafter int: Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdafter filter only works when also using the parameters offset and limit.
+    createdbefore int: Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdbefore filter only works when also using the parameters offset and limit.
+    updatedafter int: 
+    updatedbefore int: 
+    documentclassids str: List of documentclass IDs for the target. The limit here is 1000 IDs.
+            The IDs are passed as a JSON array.
+            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
+    withoutdocumentclass bool: Use this parameter to filter the returned reference documents to include only documents that are not linked to a documentclass. The parameter is of type boolean and is set to false by default.
+    mincharacters int: 
+    metadata str: Filter by metadata
+    comment str: Use this parameter to add a comment to your reference document.
+    offset int: Specify from which number on reference documents should be returned.
+    limit int: Specify the number of reference documents to be returned.
+    sort str: Sort the returned reference documents by name, created, updated and/or metadata. Add a - before the field name to sort in descending order.
+    fields str: Define which fields should be returned by the /referencedocuments endpoints. The following values can be sent as a comma-separated list: id, name, tags, metadata, filename, created, processed, lang, updated.
+        """
+        q_params = {}
+        if tags is not None:
+            q_params["tags"] = tags
+        if documentids is not None:
+            q_params["documentids"] = documentids
+        if name is not None:
+            q_params["name"] = name
+        if createdafter is not None:
+            q_params["createdafter"] = createdafter
+        if createdbefore is not None:
+            q_params["createdbefore"] = createdbefore
+        if updatedafter is not None:
+            q_params["updatedafter"] = updatedafter
+        if updatedbefore is not None:
+            q_params["updatedbefore"] = updatedbefore
+        if documentclassids is not None:
+            q_params["documentclassids"] = documentclassids
+        if withoutdocumentclass is not None:
+            q_params["withoutdocumentclass"] = withoutdocumentclass
+        if mincharacters is not None:
+            q_params["mincharacters"] = mincharacters
+        if metadata is not None:
+            q_params["metadata"] = metadata
+        if comment is not None:
+            q_params["comment"] = comment
+        if offset is not None:
+            q_params["offset"] = offset
+        if limit is not None:
+            q_params["limit"] = limit
+        if sort is not None:
+            q_params["sort"] = sort
+        if fields is not None:
+            q_params["fields"] = fields
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().as_bytesio()
 
     def post(
         self,
         name: str = None,
         tags: str = None,
         metadata: str = None,
         file: IOBase = None,
         text: str = None,
         documenttype: str = None,
         color: str = None,
         comment: str = None,
-        documentclass: str = None,
+        documentclassid: str = None,
         addparagraphsasdocuments: bool = None,
         detectlanguage: bool = None,
     ) -> List[DocumentInformation]:
         """
         Upload reference document
         Args:
         name (str): The document name in your library (in contrast to the file name being used during upload).
     tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
     metadata (str): Filter by metadata
     file (IOBase): Input document (left document).
     text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
     documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
     color (str): Use this parameter to specify the color for your reference document. Possible values are RED, MAGENTA, AQUA, ORANGE, GREY, or LAVENDER.
     comment (str): Use this parameter to add a comment to your reference document.
-    documentclass (str): 
+    documentclassid (str): 
     addparagraphsasdocuments (bool): Use this parameter to create individual reference documents in the library for each paragraph in your document. The parameter is of type boolean and is set to false by default.
         """
         q_params = {}
         if detectlanguage is not None:
             q_params["detectlanguage"] = detectlanguage
         response = self._session.post(
             url=self._endpoint,
@@ -161,15 +239,15 @@
                 "tags": tags,
                 "metadata": metadata,
                 "file": file,
                 "text": text,
                 "documenttype": documenttype,
                 "color": color,
                 "comment": comment,
-                "documentclass": documentclass,
+                "documentclassid": documentclassid,
                 "addparagraphsasdocuments": addparagraphsasdocuments,
             },
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(DocumentInformationSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/references.py` & `semantha_sdk-5.6.0/semantha_sdk/api/documents.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,114 +1,157 @@
 from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.model.document import Document
 from semantha_sdk.model.document import DocumentSchema
-from semantha_sdk.model.document_meta_data import DocumentMetaData
-from semantha_sdk.model.document_meta_data import DocumentMetaDataSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-class ReferencesEndpoint(SemanthaAPIEndpoint):
+class DocumentsEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/references"
+        return self._parent_endpoint + "/documents"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
 
     
     def post(
         self,
         file: IOBase = None,
-        referencedocument: IOBase = None,
-        referencedocumentids: List[str] = None,
-        tags: str = None,
-        documentclassids: List[str] = None,
-        similaritythreshold: float = None,
-        synonymousthreshold: float = None,
-        marknomatch: bool = None,
-        withreferencetext: bool = None,
-        mode: str = None,
-        documenttype: str = None,
-        metadata: List[DocumentMetaData] = None,
-        withcontext: bool = None,
-        considertexttype: bool = None,
-        resizeparagraphs: bool = None,
         text: str = None,
+        type: str = None,
+        documenttype: str = None,
         withareas: bool = None,
-        detectlanguage: bool = None,
-        maxreferences: int = None,
-    ) -> Document:
+        mode: str = None,
+        withparagraphtype: bool = None,
+    ) -> List[Document]:
         """
-        Determine references with one input document
-            Matches one input document ('file' parameter, as an alternative 'text' can be used) to a set of 'referencedocument' if set or internal library. If you match against internal library the 'tags' parameter can be used to filter the library.
+        Create a document model
         Args:
         file (IOBase): Input document (left document).
-    referencedocument (IOBase): Reference document(s) to be used instead of the documents in the domain's library.
-    referencedocumentids (List[str]): To filter for document IDs. The limit here is 65000 IDs.
-            The IDs are passed as a JSON array.
-    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-    documentclassids (List[str]): List of documentclass IDs for the target. The limit here is 1000 IDs.
-            The IDs are passed as a JSON array.
-            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
-    similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-            In general, the higher the threshold, the more precise the results.
-    synonymousthreshold (float): Threshold for good matches.
-    marknomatch (bool): Marks the paragraphs that have not matched
-    withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    withareas (bool): Gives back the coordinates of referenced area.
     mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
             fingerprint: semantic search based on sentences; 
             keyword: keyword: search based on sentences; 
             document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
             document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
             fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
             Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-    metadata (List[DocumentMetaData]): Filter by metadata
-    withcontext (bool): Creates and saves the context.
-    considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
-    resizeparagraphs (bool): Automatically resizes paragraphs based on their semantic meaning.
+    withparagraphtype (bool): The type of the paragraph, for example heading, text
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
+                "text": text,
+                "type": type,
+                "documenttype": documenttype,
+                "withareas": withareas,
+                "mode": mode,
+                "withparagraphtype": withparagraphtype,
+            },
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(DocumentSchema)
+    def post_as_xlsx(
+        self,
+        file: IOBase = None,
+        text: str = None,
+        type: str = None,
+        documenttype: str = None,
+        withareas: bool = None,
+        mode: str = None,
+        withparagraphtype: bool = None,
+    ) -> IOBase:
+        """
+        Create a document model
+        Args:
+        file (IOBase): Input document (left document).
     text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
     withareas (bool): Gives back the coordinates of referenced area.
+    mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
+            fingerprint: semantic search based on sentences; 
+            keyword: keyword: search based on sentences; 
+            document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
+            document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
+            fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    withparagraphtype (bool): The type of the paragraph, for example heading, text
         """
         q_params = {}
-        if detectlanguage is not None:
-            q_params["detectlanguage"] = detectlanguage
-        if maxreferences is not None:
-            q_params["maxreferences"] = maxreferences
         response = self._session.post(
             url=self._endpoint,
             body={
                 "file": file,
-                "referencedocument": referencedocument,
-                "referencedocumentids": referencedocumentids,
-                "tags": tags,
-                "documentclassids": documentclassids,
-                "similaritythreshold": similaritythreshold,
-                "synonymousthreshold": synonymousthreshold,
-                "marknomatch": marknomatch,
-                "withreferencetext": withreferencetext,
-                "mode": mode,
+                "text": text,
+                "type": type,
                 "documenttype": documenttype,
-                "metadata": metadata,
-                "withcontext": withcontext,
-                "considertexttype": considertexttype,
-                "resizeparagraphs": resizeparagraphs,
+                "withareas": withareas,
+                "mode": mode,
+                "withparagraphtype": withparagraphtype,
+            },
+            headers=RestClient.to_header(MediaType.XLSX),
+            q_params=q_params
+        ).execute()
+        return response.as_bytesio()
+    def post_as_docx(
+        self,
+        file: IOBase = None,
+        text: str = None,
+        type: str = None,
+        documenttype: str = None,
+        withareas: bool = None,
+        mode: str = None,
+        withparagraphtype: bool = None,
+    ) -> IOBase:
+        """
+        Create a document model
+        Args:
+        file (IOBase): Input document (left document).
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    withareas (bool): Gives back the coordinates of referenced area.
+    mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
+            fingerprint: semantic search based on sentences; 
+            keyword: keyword: search based on sentences; 
+            document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
+            document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
+            fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    withparagraphtype (bool): The type of the paragraph, for example heading, text
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
                 "text": text,
+                "type": type,
+                "documenttype": documenttype,
                 "withareas": withareas,
+                "mode": mode,
+                "withparagraphtype": withparagraphtype,
             },
-            headers=RestClient.to_header(MediaType.JSON),
+            headers=RestClient.to_header(MediaType.DOCX),
             q_params=q_params
         ).execute()
-        return response.to(DocumentSchema)
+        return response.as_bytesio()
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/roles.py` & `semantha_sdk-5.6.0/semantha_sdk/api/roles.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/semantha_api.py` & `semantha_sdk-5.6.0/semantha_sdk/api/semantha_api.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/sentence.py` & `semantha_sdk-5.6.0/semantha_sdk/api/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/sentences.py` & `semantha_sdk-5.6.0/semantha_sdk/api/sentences.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/settings.py` & `semantha_sdk-5.6.0/semantha_sdk/api/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/similaritymatrix.py` & `semantha_sdk-5.6.0/semantha_sdk/api/similaritymatrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         sourcedocumentids: List[str] = None,
         documentclassids: List[str] = None,
         sourcedocumentclassids: List[str] = None,
         similaritythreshold: float = None,
         mode: str = None,
         documenttype: str = None,
         considertexttype: bool = None,
-        withcontext: bool = None,
     ) -> List[MatrixRow]:
         """
         Get a similarity matrix
         Args:
         file (IOBase): Input document (left document).
     tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
     sourcetags (str): Filters the input library by tags
@@ -64,15 +63,14 @@
             keyword: keyword: search based on sentences; 
             document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
             document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
             fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
             Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
     documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
     considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
-    withcontext (bool): Creates and saves the context.
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             body={
                 "file": file,
                 "tags": tags,
@@ -81,15 +79,14 @@
                 "sourcedocumentids": sourcedocumentids,
                 "documentclassids": documentclassids,
                 "sourcedocumentclassids": sourcedocumentclassids,
                 "similaritythreshold": similaritythreshold,
                 "mode": mode,
                 "documenttype": documenttype,
                 "considertexttype": considertexttype,
-                "withcontext": withcontext,
             },
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(MatrixRowSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/statistic.py` & `semantha_sdk-5.6.0/semantha_sdk/api/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/summarizations.py` & `semantha_sdk-5.6.0/semantha_sdk/api/summarizations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/tag.py` & `semantha_sdk-5.6.0/semantha_sdk/api/tag.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/tag_referencedocuments.py` & `semantha_sdk-5.6.0/semantha_sdk/api/tag_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/tags.py` & `semantha_sdk-5.6.0/semantha_sdk/api/tags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/api/validation.py` & `semantha_sdk-5.6.0/semantha_sdk/api/validation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/__init__.py` & `semantha_sdk-5.6.0/semantha_sdk/model/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """ author semantha, this is a generated file do not change manually! """
 
 from .annotation_cell import AnnotationCell, AnnotationCellSchema
 from .annotation_page import AnnotationPage, AnnotationPageSchema
 from .answer import Answer, AnswerSchema
 from .answer_reference import AnswerReference, AnswerReferenceSchema
+from .argument import Argument, ArgumentSchema
+from .attribute_overview import AttributeOverview, AttributeOverviewSchema
 from .boost_word import BoostWord, BoostWordSchema
 from .class_bulk import ClassBulk, ClassBulkSchema
 from .clustered_document import ClusteredDocument, ClusteredDocumentSchema
 from .clustering_response import ClusteringResponse, ClusteringResponseSchema
+from .column import Column, ColumnSchema
 from .complex_property import ComplexProperty, ComplexPropertySchema
+from .condition import Condition, ConditionSchema
+from .condition_value import ConditionValue, ConditionValueSchema
 from .current_user import CurrentUser, CurrentUserSchema
 from .data_property import DataProperty, DataPropertySchema
 from .difference import Difference, DifferenceSchema
 from .distance import Distance, DistanceSchema
 from .document import Document, DocumentSchema
 from .document_class import DocumentClass, DocumentClassSchema
 from .document_class_bulk import DocumentClassBulk, DocumentClassBulkSchema
@@ -20,52 +25,71 @@
 from .document_cluster import DocumentCluster, DocumentClusterSchema
 from .document_information import DocumentInformation, DocumentInformationSchema
 from .document_meta_data import DocumentMetaData, DocumentMetaDataSchema
 from .document_named_entity import DocumentNamedEntity, DocumentNamedEntitySchema
 from .document_table import DocumentTable, DocumentTableSchema
 from .domain import Domain, DomainSchema
 from .entity import Entity, EntitySchema
+from .expression import Expression, ExpressionSchema
 from .extraction_area import ExtractionArea, ExtractionAreaSchema
 from .extraction_file import ExtractionFile, ExtractionFileSchema
 from .extraction_reference import ExtractionReference, ExtractionReferenceSchema
+from .extractor import Extractor, ExtractorSchema
+from .extractor_attribute import ExtractorAttribute, ExtractorAttributeSchema
+from .extractor_class import ExtractorClass, ExtractorClassSchema
+from .extractor_class_overview import ExtractorClassOverview, ExtractorClassOverviewSchema
+from .extractor_table import ExtractorTable, ExtractorTableSchema
 from .features import Features, FeaturesSchema
+from .field import Field, FieldSchema
 from .file_reference import FileReference, FileReferenceSchema
 from .finding import Finding, FindingSchema
+from .formatter import Formatter, FormatterSchema
 from .info import Info, InfoSchema
 from .instance import Instance, InstanceSchema
 from .instance_child import InstanceChild, InstanceChildSchema
+from .instance_overview import InstanceOverview, InstanceOverviewSchema
 from .label import Label, LabelSchema
 from .language_detection import LanguageDetection, LanguageDetectionSchema
 from .linked_instance import LinkedInstance, LinkedInstanceSchema
 from .linked_value import LinkedValue, LinkedValueSchema
+from .matcher import Matcher, MatcherSchema
 from .matrix_row import MatrixRow, MatrixRowSchema
 from .meta_info_page import MetaInfoPage, MetaInfoPageSchema
 from .metadata import Metadata, MetadataSchema
 from .metadata_value import MetadataValue, MetadataValueSchema
 from .model_class import ModelClass, ModelClassSchema
 from .model_instance import ModelInstance, ModelInstanceSchema
 from .named_entity import NamedEntity, NamedEntitySchema
+from .overview import Overview, OverviewSchema
 from .page import Page, PageSchema
 from .page_content import PageContent, PageContentSchema
 from .paragraph import Paragraph, ParagraphSchema
 from .paragraph_update import ParagraphUpdate, ParagraphUpdateSchema
 from .plotly_chart import PlotlyChart, PlotlyChartSchema
 from .process_information import ProcessInformation, ProcessInformationSchema
+from .range import Range, RangeSchema
 from .rect import Rect, RectSchema
 from .reference import Reference, ReferenceSchema
 from .reference_documents_response_container import ReferenceDocumentsResponseContainer, ReferenceDocumentsResponseContainerSchema
+from .regex import Regex, RegexSchema
+from .relation import Relation, RelationSchema
+from .relation_condition import RelationCondition, RelationConditionSchema
 from .response_meta_info import ResponseMetaInfo, ResponseMetaInfoSchema
 from .row import Row, RowSchema
+from .rule import Rule, RuleSchema
+from .rule_function import RuleFunction, RuleFunctionSchema
+from .rule_overview import RuleOverview, RuleOverviewSchema
 from .semantic_model import SemanticModel, SemanticModelSchema
 from .semi_super_vised_document import SemiSuperVisedDocument, SemiSuperVisedDocumentSchema
 from .sentence import Sentence, SentenceSchema
 from .settings import Settings, SettingsSchema
 from .simple_property import SimpleProperty, SimplePropertySchema
 from .smart_cluster_response_container import SmartClusterResponseContainer, SmartClusterResponseContainerSchema
 from .smart_cluster_semi_supervised_request import SmartClusterSemiSupervisedRequest, SmartClusterSemiSupervisedRequestSchema
 from .statistic import Statistic, StatisticSchema
 from .stop_word import StopWord, StopWordSchema
 from .synonym import Synonym, SynonymSchema
+from .table import Table, TableSchema
 from .table_cell import TableCell, TableCellSchema
 from .table_instance import TableInstance, TableInstanceSchema
 from .tag_docs import TagDocs, TagDocsSchema
 from .version import Version, VersionSchema
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/annotation_cell.py` & `semantha_sdk-5.6.0/semantha_sdk/model/annotation_cell.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e66 6561 7475 7265 7320  .model.features 
 000000d0: 696d 706f 7274 2046 6561 7475 7265 730d  import Features.
-000000e0: 0a0d 0a66 726f 6d20 7365 6d61 6e74 6861  ...from semantha
-000000f0: 5f73 646b 2e6d 6f64 656c 2e72 6563 7420  _sdk.model.rect 
-00000100: 696d 706f 7274 2052 6563 740d 0a0d 0a66  import Rect....f
-00000110: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-00000120: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-00000130: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-00000140: 5472 7565 290d 0a63 6c61 7373 2041 6e6e  True)..class Ann
-00000150: 6f74 6174 696f 6e43 656c 6c28 5365 6d61  otationCell(Sema
-00000160: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
-00000170: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
-00000180: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
-00000190: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
-000001a0: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
-000001b0: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
-000001c0: 220d 0a20 2020 2062 626f 783a 204f 7074  "..    bbox: Opt
-000001d0: 696f 6e61 6c5b 5265 6374 5d0d 0a20 2020  ional[Rect]..   
-000001e0: 2074 7970 653a 204f 7074 696f 6e61 6c5b   type: Optional[
-000001f0: 7374 725d 0d0a 2020 2020 6665 6174 7572  str]..    featur
-00000200: 6573 3a20 4f70 7469 6f6e 616c 5b46 6561  es: Optional[Fea
-00000210: 7475 7265 735d 0d0a 0d0a 416e 6e6f 7461  tures]....Annota
-00000220: 7469 6f6e 4365 6c6c 5363 6865 6d61 203d  tionCellSchema =
-00000230: 2063 6c61 7373 5f73 6368 656d 6128 416e   class_schema(An
-00000240: 6e6f 7461 7469 6f6e 4365 6c6c 2c20 6261  notationCell, ba
-00000250: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
-00000260: 6861 5363 6865 6d61 290d 0a              haSchema)..
+000000e0: 0a66 726f 6d20 7365 6d61 6e74 6861 5f73  .from semantha_s
+000000f0: 646b 2e6d 6f64 656c 2e72 6563 7420 696d  dk.model.rect im
+00000100: 706f 7274 2052 6563 740d 0a66 726f 6d20  port Rect..from 
+00000110: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
+00000120: 7469 6f6e 616c 0d0a 0d0a 0d0a 4064 6174  tional......@dat
+00000130: 6163 6c61 7373 2866 726f 7a65 6e3d 5472  aclass(frozen=Tr
+00000140: 7565 290d 0a63 6c61 7373 2041 6e6e 6f74  ue)..class Annot
+00000150: 6174 696f 6e43 656c 6c28 5365 6d61 6e74  ationCell(Semant
+00000160: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
+00000170: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
+00000180: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
+00000190: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
+000001a0: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
+000001b0: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
+000001c0: 0a20 2020 2062 626f 783a 204f 7074 696f  .    bbox: Optio
+000001d0: 6e61 6c5b 5265 6374 5d0d 0a20 2020 2074  nal[Rect]..    t
+000001e0: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
+000001f0: 725d 0d0a 2020 2020 6665 6174 7572 6573  r]..    features
+00000200: 3a20 4f70 7469 6f6e 616c 5b46 6561 7475  : Optional[Featu
+00000210: 7265 735d 0d0a 0d0a 416e 6e6f 7461 7469  res]....Annotati
+00000220: 6f6e 4365 6c6c 5363 6865 6d61 203d 2063  onCellSchema = c
+00000230: 6c61 7373 5f73 6368 656d 6128 416e 6e6f  lass_schema(Anno
+00000240: 7461 7469 6f6e 4365 6c6c 2c20 6261 7365  tationCell, base
+00000250: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
+00000260: 5363 6865 6d61 290d 0a                   Schema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/annotation_page.py` & `semantha_sdk-5.6.0/semantha_sdk/model/annotation_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e61 6e6e 6f74 6174 696f  .model.annotatio
 000000d0: 6e5f 6365 6c6c 2069 6d70 6f72 7420 416e  n_cell import An
-000000e0: 6e6f 7461 7469 6f6e 4365 6c6c 0d0a 0d0a  notationCell....
-000000f0: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000100: 7274 204c 6973 740d 0a66 726f 6d20 7479  rt List..from ty
-00000110: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
-00000120: 6f6e 616c 0d0a 0d0a 4064 6174 6163 6c61  onal....@datacla
+000000e0: 6e6f 7461 7469 6f6e 4365 6c6c 0d0a 6672  notationCell..fr
+000000f0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000100: 204c 6973 740d 0a66 726f 6d20 7479 7069   List..from typi
+00000110: 6e67 2069 6d70 6f72 7420 4f70 7469 6f6e  ng import Option
+00000120: 616c 0d0a 0d0a 0d0a 4064 6174 6163 6c61  al......@datacla
 00000130: 7373 2866 726f 7a65 6e3d 5472 7565 290d  ss(frozen=True).
 00000140: 0a63 6c61 7373 2041 6e6e 6f74 6174 696f  .class Annotatio
 00000150: 6e50 6167 6528 5365 6d61 6e74 6861 4d6f  nPage(SemanthaMo
 00000160: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
 00000170: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
 00000180: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
 00000190: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/answer.py` & `semantha_sdk-5.6.0/semantha_sdk/model/answer.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.answer_reference import AnswerReference
-
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class Answer(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     answer: Optional[str]
     references: Optional[List[AnswerReference]]
 
 AnswerSchema = class_schema(Answer, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/answer_reference.py` & `semantha_sdk-5.6.0/semantha_sdk/model/answer_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2041 6e73  True)..class Ans
-000000f0: 7765 7252 6566 6572 656e 6365 2853 656d  werReference(Sem
-00000100: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-00000110: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
-00000120: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
-00000130: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
-00000140: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
-00000150: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
-00000160: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
-00000170: 6f6e 616c 5b73 7472 5d0d 0a20 2020 206e  onal[str]..    n
-00000180: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
-00000190: 725d 0d0a 2020 2020 636f 6e74 656e 743a  r]..    content:
-000001a0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-000001b0: 2020 2020 6d65 7461 6461 7461 3a20 4f70      metadata: Op
-000001c0: 7469 6f6e 616c 5b73 7472 5d0d 0a0d 0a41  tional[str]....A
-000001d0: 6e73 7765 7252 6566 6572 656e 6365 5363  nswerReferenceSc
-000001e0: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-000001f0: 656d 6128 416e 7377 6572 5265 6665 7265  ema(AnswerRefere
-00000200: 6e63 652c 2062 6173 655f 7363 6865 6d61  nce, base_schema
-00000210: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
-00000220: 0d0a                                     ..
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2041  n=True)..class A
+000000f0: 6e73 7765 7252 6566 6572 656e 6365 2853  nswerReference(S
+00000100: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
+00000110: 7479 293a 0d0a 2020 2020 2222 2220 6175  ty):..    """ au
+00000120: 7468 6f72 2073 656d 616e 7468 612c 2074  thor semantha, t
+00000130: 6869 7320 6973 2061 2067 656e 6572 6174  his is a generat
+00000140: 6564 2063 6c61 7373 2064 6f20 6e6f 7420  ed class do not 
+00000150: 6368 616e 6765 206d 616e 7561 6c6c 7921  change manually!
+00000160: 2022 2222 0d0a 2020 2020 6964 3a20 4f70   """..    id: Op
+00000170: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000180: 206e 616d 653a 204f 7074 696f 6e61 6c5b   name: Optional[
+00000190: 7374 725d 0d0a 2020 2020 636f 6e74 656e  str]..    conten
+000001a0: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
+000001b0: 0d0a 2020 2020 6d65 7461 6461 7461 3a20  ..    metadata: 
+000001c0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a0d  Optional[str]...
+000001d0: 0a41 6e73 7765 7252 6566 6572 656e 6365  .AnswerReference
+000001e0: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
+000001f0: 6368 656d 6128 416e 7377 6572 5265 6665  chema(AnswerRefe
+00000200: 7265 6e63 652c 2062 6173 655f 7363 6865  rence, base_sche
+00000210: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
+00000220: 6129 0d0a                                a)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/boost_word.py` & `semantha_sdk-5.6.0/semantha_sdk/model/boost_word.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
 000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-000000e0: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
-000000f0: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
-00000100: 636c 6173 7320 426f 6f73 7457 6f72 6428  class BoostWord(
-00000110: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
-00000120: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
-00000130: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
-00000140: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
-00000150: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
-00000160: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
-00000170: 2120 2222 220d 0a20 2020 2069 643a 204f  ! """..    id: O
-00000180: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000190: 2020 776f 7264 3a20 4f70 7469 6f6e 616c    word: Optional
-000001a0: 5b73 7472 5d0d 0a20 2020 2072 6567 6578  [str]..    regex
-000001b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000001c0: 0a20 2020 2074 6167 733a 204f 7074 696f  .    tags: Optio
-000001d0: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 0d0a  nal[List[str]]..
-000001e0: 2020 2020 6c61 6265 6c3a 204f 7074 696f      label: Optio
-000001f0: 6e61 6c5b 7374 725d 0d0a 0d0a 426f 6f73  nal[str]....Boos
-00000200: 7457 6f72 6453 6368 656d 6120 3d20 636c  tWordSchema = cl
-00000210: 6173 735f 7363 6865 6d61 2842 6f6f 7374  ass_schema(Boost
-00000220: 576f 7264 2c20 6261 7365 5f73 6368 656d  Word, base_schem
-00000230: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000240: 290d 0a                                  )..
+000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000100: 0d0a 636c 6173 7320 426f 6f73 7457 6f72  ..class BoostWor
+00000110: 6428 5365 6d61 6e74 6861 4d6f 6465 6c45  d(SemanthaModelE
+00000120: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
+00000130: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
+00000140: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
+00000150: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
+00000160: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
+00000170: 6c79 2120 2222 220d 0a20 2020 2069 643a  ly! """..    id:
+00000180: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
+00000190: 2020 2020 776f 7264 3a20 4f70 7469 6f6e      word: Option
+000001a0: 616c 5b73 7472 5d0d 0a20 2020 2072 6567  al[str]..    reg
+000001b0: 6578 3a20 4f70 7469 6f6e 616c 5b73 7472  ex: Optional[str
+000001c0: 5d0d 0a20 2020 2074 6167 733a 204f 7074  ]..    tags: Opt
+000001d0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
+000001e0: 0d0a 2020 2020 6c61 6265 6c3a 204f 7074  ..    label: Opt
+000001f0: 696f 6e61 6c5b 7374 725d 0d0a 0d0a 426f  ional[str]....Bo
+00000200: 6f73 7457 6f72 6453 6368 656d 6120 3d20  ostWordSchema = 
+00000210: 636c 6173 735f 7363 6865 6d61 2842 6f6f  class_schema(Boo
+00000220: 7374 576f 7264 2c20 6261 7365 5f73 6368  stWord, base_sch
+00000230: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
+00000240: 6d61 290d 0a                             ma)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/class_bulk.py` & `semantha_sdk-5.6.0/semantha_sdk/model/class_bulk.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,56 +7,56 @@
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e6c 6162 656c 2069 6d70  .model.label imp
-000000d0: 6f72 7420 4c61 6265 6c0d 0a0d 0a66 726f  ort Label....fro
-000000e0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000f0: 6f64 656c 2e6d 6574 6164 6174 615f 7661  odel.metadata_va
-00000100: 6c75 6520 696d 706f 7274 204d 6574 6164  lue import Metad
-00000110: 6174 6156 616c 7565 0d0a 0d0a 6672 6f6d  ataValue....from
-00000120: 2074 7970 696e 6720 696d 706f 7274 204c   typing import L
-00000130: 6973 740d 0a66 726f 6d20 7479 7069 6e67  ist..from typing
-00000140: 2069 6d70 6f72 7420 4f70 7469 6f6e 616c   import Optional
-00000150: 0d0a 0d0a 4064 6174 6163 6c61 7373 2866  ....@dataclass(f
-00000160: 726f 7a65 6e3d 5472 7565 290d 0a63 6c61  rozen=True)..cla
-00000170: 7373 2043 6c61 7373 4275 6c6b 2853 656d  ss ClassBulk(Sem
-00000180: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-00000190: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
-000001a0: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
-000001b0: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
-000001c0: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
-000001d0: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
-000001e0: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
-000001f0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 206e  onal[str]..    n
-00000200: 616d 653a 2073 7472 0d0a 2020 2020 7265  ame: str..    re
-00000210: 6164 5f6f 6e6c 793a 204f 7074 696f 6e61  ad_only: Optiona
-00000220: 6c5b 626f 6f6c 5d0d 0a20 2020 2066 756e  l[bool]..    fun
-00000230: 6374 696f 6e61 6c3a 204f 7074 696f 6e61  ctional: Optiona
-00000240: 6c5b 626f 6f6c 5d0d 0a20 2020 206c 6162  l[bool]..    lab
-00000250: 656c 733a 204f 7074 696f 6e61 6c5b 4c69  els: Optional[Li
-00000260: 7374 5b4c 6162 656c 5d5d 0d0a 2020 2020  st[Label]]..    
-00000270: 6d65 7461 6461 7461 3a20 4f70 7469 6f6e  metadata: Option
-00000280: 616c 5b4c 6973 745b 4d65 7461 6461 7461  al[List[Metadata
-00000290: 5661 6c75 655d 5d0d 0a20 2020 2063 6f6d  Value]]..    com
-000002a0: 6d65 6e74 3a20 4f70 7469 6f6e 616c 5b73  ment: Optional[s
-000002b0: 7472 5d0d 0a20 2020 2064 6174 6174 7970  tr]..    datatyp
-000002c0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-000002d0: 0d0a 2020 2020 6174 7472 6962 7574 655f  ..    attribute_
-000002e0: 6964 733a 204f 7074 696f 6e61 6c5b 4c69  ids: Optional[Li
-000002f0: 7374 5b73 7472 5d5d 0d0a 2020 2020 7265  st[str]]..    re
-00000300: 6c65 7661 6e74 5f66 6f72 5f72 656c 6174  levant_for_relat
-00000310: 696f 6e3a 204f 7074 696f 6e61 6c5b 626f  ion: Optional[bo
-00000320: 6f6c 5d0d 0a20 2020 206f 626a 6563 745f  ol]..    object_
-00000330: 7072 6f70 6572 7479 5f69 643a 204f 7074  property_id: Opt
-00000340: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-00000350: 6f62 6a65 6374 5f70 726f 7065 7274 795f  object_property_
-00000360: 7479 7065 5f69 643a 204f 7074 696f 6e61  type_id: Optiona
-00000370: 6c5b 7374 725d 0d0a 2020 2020 7061 7265  l[str]..    pare
-00000380: 6e74 5f69 643a 204f 7074 696f 6e61 6c5b  nt_id: Optional[
-00000390: 7374 725d 0d0a 0d0a 436c 6173 7342 756c  str]....ClassBul
-000003a0: 6b53 6368 656d 6120 3d20 636c 6173 735f  kSchema = class_
-000003b0: 7363 6865 6d61 2843 6c61 7373 4275 6c6b  schema(ClassBulk
-000003c0: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-000003d0: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+000000d0: 6f72 7420 4c61 6265 6c0d 0a66 726f 6d20  ort Label..from 
+000000e0: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
+000000f0: 656c 2e6d 6574 6164 6174 615f 7661 6c75  el.metadata_valu
+00000100: 6520 696d 706f 7274 204d 6574 6164 6174  e import Metadat
+00000110: 6156 616c 7565 0d0a 6672 6f6d 2074 7970  aValue..from typ
+00000120: 696e 6720 696d 706f 7274 204c 6973 740d  ing import List.
+00000130: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+00000140: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
+00000150: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
+00000160: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
+00000170: 2043 6c61 7373 4275 6c6b 2853 656d 616e   ClassBulk(Seman
+00000180: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
+00000190: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
+000001a0: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
+000001b0: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
+000001c0: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
+000001d0: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
+000001e0: 0d0a 2020 2020 6964 3a20 4f70 7469 6f6e  ..    id: Option
+000001f0: 616c 5b73 7472 5d0d 0a20 2020 206e 616d  al[str]..    nam
+00000200: 653a 2073 7472 0d0a 2020 2020 7265 6164  e: str..    read
+00000210: 5f6f 6e6c 793a 204f 7074 696f 6e61 6c5b  _only: Optional[
+00000220: 626f 6f6c 5d0d 0a20 2020 2066 756e 6374  bool]..    funct
+00000230: 696f 6e61 6c3a 204f 7074 696f 6e61 6c5b  ional: Optional[
+00000240: 626f 6f6c 5d0d 0a20 2020 206c 6162 656c  bool]..    label
+00000250: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+00000260: 5b4c 6162 656c 5d5d 0d0a 2020 2020 6d65  [Label]]..    me
+00000270: 7461 6461 7461 3a20 4f70 7469 6f6e 616c  tadata: Optional
+00000280: 5b4c 6973 745b 4d65 7461 6461 7461 5661  [List[MetadataVa
+00000290: 6c75 655d 5d0d 0a20 2020 2063 6f6d 6d65  lue]]..    comme
+000002a0: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
+000002b0: 5d0d 0a20 2020 2064 6174 6174 7970 653a  ]..    datatype:
+000002c0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
+000002d0: 2020 2020 6174 7472 6962 7574 655f 6964      attribute_id
+000002e0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+000002f0: 5b73 7472 5d5d 0d0a 2020 2020 7265 6c65  [str]]..    rele
+00000300: 7661 6e74 5f66 6f72 5f72 656c 6174 696f  vant_for_relatio
+00000310: 6e3a 204f 7074 696f 6e61 6c5b 626f 6f6c  n: Optional[bool
+00000320: 5d0d 0a20 2020 206f 626a 6563 745f 7072  ]..    object_pr
+00000330: 6f70 6572 7479 5f69 643a 204f 7074 696f  operty_id: Optio
+00000340: 6e61 6c5b 7374 725d 0d0a 2020 2020 6f62  nal[str]..    ob
+00000350: 6a65 6374 5f70 726f 7065 7274 795f 7479  ject_property_ty
+00000360: 7065 5f69 643a 204f 7074 696f 6e61 6c5b  pe_id: Optional[
+00000370: 7374 725d 0d0a 2020 2020 7061 7265 6e74  str]..    parent
+00000380: 5f69 643a 204f 7074 696f 6e61 6c5b 7374  _id: Optional[st
+00000390: 725d 0d0a 0d0a 436c 6173 7342 756c 6b53  r]....ClassBulkS
+000003a0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
+000003b0: 6865 6d61 2843 6c61 7373 4275 6c6b 2c20  hema(ClassBulk, 
+000003c0: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
+000003d0: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/clustered_document.py` & `semantha_sdk-5.6.0/semantha_sdk/model/clustered_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2043 6c75  True)..class Clu
-000000f0: 7374 6572 6564 446f 6375 6d65 6e74 2853  steredDocument(S
-00000100: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
-00000110: 7479 293a 0d0a 2020 2020 2222 2220 6175  ty):..    """ au
-00000120: 7468 6f72 2073 656d 616e 7468 612c 2074  thor semantha, t
-00000130: 6869 7320 6973 2061 2067 656e 6572 6174  his is a generat
-00000140: 6564 2063 6c61 7373 2064 6f20 6e6f 7420  ed class do not 
-00000150: 6368 616e 6765 206d 616e 7561 6c6c 7921  change manually!
-00000160: 2022 2222 0d0a 2020 2020 646f 6375 6d65   """..    docume
-00000170: 6e74 5f69 643a 204f 7074 696f 6e61 6c5b  nt_id: Optional[
-00000180: 7374 725d 0d0a 2020 2020 7072 6f62 6162  str]..    probab
-00000190: 696c 6974 793a 204f 7074 696f 6e61 6c5b  ility: Optional[
-000001a0: 666c 6f61 745d 0d0a 0d0a 436c 7573 7465  float]....Cluste
-000001b0: 7265 6444 6f63 756d 656e 7453 6368 656d  redDocumentSchem
-000001c0: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
-000001d0: 2843 6c75 7374 6572 6564 446f 6375 6d65  (ClusteredDocume
-000001e0: 6e74 2c20 6261 7365 5f73 6368 656d 613d  nt, base_schema=
-000001f0: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
-00000200: 0a                                       .
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2043  n=True)..class C
+000000f0: 6c75 7374 6572 6564 446f 6375 6d65 6e74  lusteredDocument
+00000100: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
+00000110: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
+00000120: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
+00000130: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
+00000140: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
+00000150: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
+00000160: 7921 2022 2222 0d0a 2020 2020 646f 6375  y! """..    docu
+00000170: 6d65 6e74 5f69 643a 204f 7074 696f 6e61  ment_id: Optiona
+00000180: 6c5b 7374 725d 0d0a 2020 2020 7072 6f62  l[str]..    prob
+00000190: 6162 696c 6974 793a 204f 7074 696f 6e61  ability: Optiona
+000001a0: 6c5b 666c 6f61 745d 0d0a 0d0a 436c 7573  l[float]....Clus
+000001b0: 7465 7265 6444 6f63 756d 656e 7453 6368  teredDocumentSch
+000001c0: 656d 6120 3d20 636c 6173 735f 7363 6865  ema = class_sche
+000001d0: 6d61 2843 6c75 7374 6572 6564 446f 6375  ma(ClusteredDocu
+000001e0: 6d65 6e74 2c20 6261 7365 5f73 6368 656d  ment, base_schem
+000001f0: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
+00000200: 290d 0a                                  )..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/clustering_response.py` & `semantha_sdk-5.6.0/semantha_sdk/model/clustering_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.document_cluster import DocumentCluster
-
 from semantha_sdk.model.plotly_chart import PlotlyChart
-
 from typing import Dict
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class ClusteringResponse(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     clusters: Optional[List[DocumentCluster]]
     plotly: Optional[Dict[str, PlotlyChart]]
 
 ClusteringResponseSchema = class_schema(ClusteringResponse, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/complex_property.py` & `semantha_sdk-5.6.0/semantha_sdk/model/complex_property.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,69 +8,69 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 696f  .model.extractio
 000000d0: 6e5f 6172 6561 2069 6d70 6f72 7420 4578  n_area import Ex
-000000e0: 7472 6163 7469 6f6e 4172 6561 0d0a 0d0a  tractionArea....
-000000f0: 6672 6f6d 2073 656d 616e 7468 615f 7364  from semantha_sd
-00000100: 6b2e 6d6f 6465 6c2e 6578 7472 6163 7469  k.model.extracti
-00000110: 6f6e 5f72 6566 6572 656e 6365 2069 6d70  on_reference imp
-00000120: 6f72 7420 4578 7472 6163 7469 6f6e 5265  ort ExtractionRe
-00000130: 6665 7265 6e63 650d 0a0d 0a66 726f 6d20  ference....from 
-00000140: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
-00000150: 656c 2e66 696e 6469 6e67 2069 6d70 6f72  el.finding impor
-00000160: 7420 4669 6e64 696e 670d 0a0d 0a66 726f  t Finding....fro
-00000170: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-00000180: 6f64 656c 2e6c 6162 656c 2069 6d70 6f72  odel.label impor
-00000190: 7420 4c61 6265 6c0d 0a0d 0a66 726f 6d20  t Label....from 
-000001a0: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
-000001b0: 656c 2e6d 6574 6164 6174 6120 696d 706f  el.metadata impo
-000001c0: 7274 204d 6574 6164 6174 610d 0a0d 0a66  rt Metadata....f
-000001d0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000001e0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
-000001f0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-00000200: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
-00000210: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
-00000220: 636c 6173 7320 436f 6d70 6c65 7850 726f  class ComplexPro
-00000230: 7065 7274 7928 5365 6d61 6e74 6861 4d6f  perty(SemanthaMo
-00000240: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
-00000250: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
-00000260: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
-00000270: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
-00000280: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
-00000290: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
-000002a0: 206e 616d 653a 2073 7472 0d0a 2020 2020   name: str..    
-000002b0: 7661 6c75 653a 2073 7472 0d0a 2020 2020  value: str..    
-000002c0: 6c61 6265 6c3a 204f 7074 696f 6e61 6c5b  label: Optional[
-000002d0: 7374 725d 0d0a 2020 2020 6964 3a20 4f70  str]..    id: Op
-000002e0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-000002f0: 2063 6c61 7373 5f69 643a 204f 7074 696f   class_id: Optio
-00000300: 6e61 6c5b 7374 725d 0d0a 2020 2020 7265  nal[str]..    re
-00000310: 6c61 7469 6f6e 5f69 643a 204f 7074 696f  lation_id: Optio
-00000320: 6e61 6c5b 7374 725d 0d0a 2020 2020 6f72  nal[str]..    or
-00000330: 6967 696e 616c 5f76 616c 7565 3a20 4f70  iginal_value: Op
-00000340: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000350: 2065 7874 7261 6374 6564 5f76 616c 7565   extracted_value
-00000360: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-00000370: 0a20 2020 2064 6174 6174 7970 653a 204f  .    datatype: O
-00000380: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000390: 2020 6c61 6265 6c73 3a20 4f70 7469 6f6e    labels: Option
-000003a0: 616c 5b4c 6973 745b 4c61 6265 6c5d 5d0d  al[List[Label]].
-000003b0: 0a20 2020 206d 6574 6164 6174 613a 204f  .    metadata: O
-000003c0: 7074 696f 6e61 6c5b 4c69 7374 5b4d 6574  ptional[List[Met
-000003d0: 6164 6174 615d 5d0d 0a20 2020 2065 7874  adata]]..    ext
-000003e0: 7261 6374 696f 6e5f 6172 6561 3a20 4f70  raction_area: Op
-000003f0: 7469 6f6e 616c 5b45 7874 7261 6374 696f  tional[Extractio
-00000400: 6e41 7265 615d 0d0a 2020 2020 6669 6e64  nArea]..    find
-00000410: 696e 6773 3a20 4f70 7469 6f6e 616c 5b4c  ings: Optional[L
-00000420: 6973 745b 4669 6e64 696e 675d 5d0d 0a20  ist[Finding]].. 
-00000430: 2020 2072 6566 6572 656e 6365 733a 204f     references: O
-00000440: 7074 696f 6e61 6c5b 4c69 7374 5b45 7874  ptional[List[Ext
-00000450: 7261 6374 696f 6e52 6566 6572 656e 6365  ractionReference
-00000460: 5d5d 0d0a 0d0a 436f 6d70 6c65 7850 726f  ]]....ComplexPro
-00000470: 7065 7274 7953 6368 656d 6120 3d20 636c  pertySchema = cl
-00000480: 6173 735f 7363 6865 6d61 2843 6f6d 706c  ass_schema(Compl
-00000490: 6578 5072 6f70 6572 7479 2c20 6261 7365  exProperty, base
-000004a0: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
-000004b0: 5363 6865 6d61 290d 0a                   Schema)..
+000000e0: 7472 6163 7469 6f6e 4172 6561 0d0a 6672  tractionArea..fr
+000000f0: 6f6d 2073 656d 616e 7468 615f 7364 6b2e  om semantha_sdk.
+00000100: 6d6f 6465 6c2e 6578 7472 6163 7469 6f6e  model.extraction
+00000110: 5f72 6566 6572 656e 6365 2069 6d70 6f72  _reference impor
+00000120: 7420 4578 7472 6163 7469 6f6e 5265 6665  t ExtractionRefe
+00000130: 7265 6e63 650d 0a66 726f 6d20 7365 6d61  rence..from sema
+00000140: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e66  ntha_sdk.model.f
+00000150: 696e 6469 6e67 2069 6d70 6f72 7420 4669  inding import Fi
+00000160: 6e64 696e 670d 0a66 726f 6d20 7365 6d61  nding..from sema
+00000170: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e6c  ntha_sdk.model.l
+00000180: 6162 656c 2069 6d70 6f72 7420 4c61 6265  abel import Labe
+00000190: 6c0d 0a66 726f 6d20 7365 6d61 6e74 6861  l..from semantha
+000001a0: 5f73 646b 2e6d 6f64 656c 2e6d 6574 6164  _sdk.model.metad
+000001b0: 6174 6120 696d 706f 7274 204d 6574 6164  ata import Metad
+000001c0: 6174 610d 0a66 726f 6d20 7479 7069 6e67  ata..from typing
+000001d0: 2069 6d70 6f72 7420 4c69 7374 0d0a 6672   import List..fr
+000001e0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+000001f0: 204f 7074 696f 6e61 6c0d 0a0d 0a0d 0a40   Optional......@
+00000200: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
+00000210: 3d54 7275 6529 0d0a 636c 6173 7320 436f  =True)..class Co
+00000220: 6d70 6c65 7850 726f 7065 7274 7928 5365  mplexProperty(Se
+00000230: 6d61 6e74 6861 4d6f 6465 6c45 6e74 6974  manthaModelEntit
+00000240: 7929 3a0d 0a20 2020 2022 2222 2061 7574  y):..    """ aut
+00000250: 686f 7220 7365 6d61 6e74 6861 2c20 7468  hor semantha, th
+00000260: 6973 2069 7320 6120 6765 6e65 7261 7465  is is a generate
+00000270: 6420 636c 6173 7320 646f 206e 6f74 2063  d class do not c
+00000280: 6861 6e67 6520 6d61 6e75 616c 6c79 2120  hange manually! 
+00000290: 2222 220d 0a20 2020 206e 616d 653a 2073  """..    name: s
+000002a0: 7472 0d0a 2020 2020 7661 6c75 653a 2073  tr..    value: s
+000002b0: 7472 0d0a 2020 2020 6c61 6265 6c3a 204f  tr..    label: O
+000002c0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+000002d0: 2020 6964 3a20 4f70 7469 6f6e 616c 5b73    id: Optional[s
+000002e0: 7472 5d0d 0a20 2020 2063 6c61 7373 5f69  tr]..    class_i
+000002f0: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
+00000300: 0d0a 2020 2020 7265 6c61 7469 6f6e 5f69  ..    relation_i
+00000310: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
+00000320: 0d0a 2020 2020 6f72 6967 696e 616c 5f76  ..    original_v
+00000330: 616c 7565 3a20 4f70 7469 6f6e 616c 5b73  alue: Optional[s
+00000340: 7472 5d0d 0a20 2020 2065 7874 7261 6374  tr]..    extract
+00000350: 6564 5f76 616c 7565 3a20 4f70 7469 6f6e  ed_value: Option
+00000360: 616c 5b73 7472 5d0d 0a20 2020 2064 6174  al[str]..    dat
+00000370: 6174 7970 653a 204f 7074 696f 6e61 6c5b  atype: Optional[
+00000380: 7374 725d 0d0a 2020 2020 6c61 6265 6c73  str]..    labels
+00000390: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+000003a0: 4c61 6265 6c5d 5d0d 0a20 2020 206d 6574  Label]]..    met
+000003b0: 6164 6174 613a 204f 7074 696f 6e61 6c5b  adata: Optional[
+000003c0: 4c69 7374 5b4d 6574 6164 6174 615d 5d0d  List[Metadata]].
+000003d0: 0a20 2020 2065 7874 7261 6374 696f 6e5f  .    extraction_
+000003e0: 6172 6561 3a20 4f70 7469 6f6e 616c 5b45  area: Optional[E
+000003f0: 7874 7261 6374 696f 6e41 7265 615d 0d0a  xtractionArea]..
+00000400: 2020 2020 6669 6e64 696e 6773 3a20 4f70      findings: Op
+00000410: 7469 6f6e 616c 5b4c 6973 745b 4669 6e64  tional[List[Find
+00000420: 696e 675d 5d0d 0a20 2020 2072 6566 6572  ing]]..    refer
+00000430: 656e 6365 733a 204f 7074 696f 6e61 6c5b  ences: Optional[
+00000440: 4c69 7374 5b45 7874 7261 6374 696f 6e52  List[ExtractionR
+00000450: 6566 6572 656e 6365 5d5d 0d0a 0d0a 436f  eference]]....Co
+00000460: 6d70 6c65 7850 726f 7065 7274 7953 6368  mplexPropertySch
+00000470: 656d 6120 3d20 636c 6173 735f 7363 6865  ema = class_sche
+00000480: 6d61 2843 6f6d 706c 6578 5072 6f70 6572  ma(ComplexProper
+00000490: 7479 2c20 6261 7365 5f73 6368 656d 613d  ty, base_schema=
+000004a0: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+000004b0: 0a                                       .
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/current_user.py` & `semantha_sdk-5.6.0/semantha_sdk/model/current_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
 000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-000000e0: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
-000000f0: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
-00000100: 636c 6173 7320 4375 7272 656e 7455 7365  class CurrentUse
-00000110: 7228 5365 6d61 6e74 6861 4d6f 6465 6c45  r(SemanthaModelE
-00000120: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
-00000130: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
-00000140: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
-00000150: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
-00000160: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
-00000170: 6c79 2120 2222 220d 0a20 2020 206e 616d  ly! """..    nam
-00000180: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-00000190: 0d0a 2020 2020 7661 6c69 645f 756e 7469  ..    valid_unti
-000001a0: 6c3a 204f 7074 696f 6e61 6c5b 696e 745d  l: Optional[int]
-000001b0: 0d0a 2020 2020 726f 6c65 733a 204f 7074  ..    roles: Opt
-000001c0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-000001d0: 0d0a 0d0a 4375 7272 656e 7455 7365 7253  ....CurrentUserS
-000001e0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
-000001f0: 6865 6d61 2843 7572 7265 6e74 5573 6572  hema(CurrentUser
-00000200: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-00000210: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000100: 0d0a 636c 6173 7320 4375 7272 656e 7455  ..class CurrentU
+00000110: 7365 7228 5365 6d61 6e74 6861 4d6f 6465  ser(SemanthaMode
+00000120: 6c45 6e74 6974 7929 3a0d 0a20 2020 2022  lEntity):..    "
+00000130: 2222 2061 7574 686f 7220 7365 6d61 6e74  "" author semant
+00000140: 6861 2c20 7468 6973 2069 7320 6120 6765  ha, this is a ge
+00000150: 6e65 7261 7465 6420 636c 6173 7320 646f  nerated class do
+00000160: 206e 6f74 2063 6861 6e67 6520 6d61 6e75   not change manu
+00000170: 616c 6c79 2120 2222 220d 0a20 2020 206e  ally! """..    n
+00000180: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
+00000190: 725d 0d0a 2020 2020 7661 6c69 645f 756e  r]..    valid_un
+000001a0: 7469 6c3a 204f 7074 696f 6e61 6c5b 696e  til: Optional[in
+000001b0: 745d 0d0a 2020 2020 726f 6c65 733a 204f  t]..    roles: O
+000001c0: 7074 696f 6e61 6c5b 4c69 7374 5b73 7472  ptional[List[str
+000001d0: 5d5d 0d0a 0d0a 4375 7272 656e 7455 7365  ]]....CurrentUse
+000001e0: 7253 6368 656d 6120 3d20 636c 6173 735f  rSchema = class_
+000001f0: 7363 6865 6d61 2843 7572 7265 6e74 5573  schema(CurrentUs
+00000200: 6572 2c20 6261 7365 5f73 6368 656d 613d  er, base_schema=
+00000210: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+00000220: 0a                                       .
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/data_property.py` & `semantha_sdk-5.6.0/semantha_sdk/model/data_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e6c 6162 656c 2069 6d70  .model.label imp
-000000d0: 6f72 7420 4c61 6265 6c0d 0a0d 0a66 726f  ort Label....fro
-000000e0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000f0: 4c69 7374 0d0a 6672 6f6d 2074 7970 696e  List..from typin
-00000100: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
-00000110: 6c0d 0a0d 0a40 6461 7461 636c 6173 7328  l....@dataclass(
+000000d0: 6f72 7420 4c61 6265 6c0d 0a66 726f 6d20  ort Label..from 
+000000e0: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
+000000f0: 7374 0d0a 6672 6f6d 2074 7970 696e 6720  st..from typing 
+00000100: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
+00000110: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
 00000120: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
 00000130: 6173 7320 4461 7461 5072 6f70 6572 7479  ass DataProperty
 00000140: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
 00000150: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
 00000160: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
 00000170: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
 00000180: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/distance.py` & `semantha_sdk-5.6.0/semantha_sdk/model/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2044 6973  True)..class Dis
-000000f0: 7461 6e63 6528 5365 6d61 6e74 6861 4d6f  tance(SemanthaMo
-00000100: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
-00000110: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
-00000120: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
-00000130: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
-00000140: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
-00000150: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
-00000160: 2074 6f70 3a20 4f70 7469 6f6e 616c 5b66   top: Optional[f
-00000170: 6c6f 6174 5d0d 0a20 2020 2062 6f74 746f  loat]..    botto
-00000180: 6d3a 204f 7074 696f 6e61 6c5b 666c 6f61  m: Optional[floa
-00000190: 745d 0d0a 2020 2020 6c65 6674 3a20 4f70  t]..    left: Op
-000001a0: 7469 6f6e 616c 5b66 6c6f 6174 5d0d 0a20  tional[float].. 
-000001b0: 2020 2072 6967 6874 3a20 4f70 7469 6f6e     right: Option
-000001c0: 616c 5b66 6c6f 6174 5d0d 0a0d 0a44 6973  al[float]....Dis
-000001d0: 7461 6e63 6553 6368 656d 6120 3d20 636c  tanceSchema = cl
-000001e0: 6173 735f 7363 6865 6d61 2844 6973 7461  ass_schema(Dista
-000001f0: 6e63 652c 2062 6173 655f 7363 6865 6d61  nce, base_schema
-00000200: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
-00000210: 0d0a                                     ..
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2044  n=True)..class D
+000000f0: 6973 7461 6e63 6528 5365 6d61 6e74 6861  istance(Semantha
+00000100: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
+00000110: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
+00000120: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
+00000130: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
+00000140: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
+00000150: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
+00000160: 2020 2074 6f70 3a20 4f70 7469 6f6e 616c     top: Optional
+00000170: 5b66 6c6f 6174 5d0d 0a20 2020 2062 6f74  [float]..    bot
+00000180: 746f 6d3a 204f 7074 696f 6e61 6c5b 666c  tom: Optional[fl
+00000190: 6f61 745d 0d0a 2020 2020 6c65 6674 3a20  oat]..    left: 
+000001a0: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d0d  Optional[float].
+000001b0: 0a20 2020 2072 6967 6874 3a20 4f70 7469  .    right: Opti
+000001c0: 6f6e 616c 5b66 6c6f 6174 5d0d 0a0d 0a44  onal[float]....D
+000001d0: 6973 7461 6e63 6553 6368 656d 6120 3d20  istanceSchema = 
+000001e0: 636c 6173 735f 7363 6865 6d61 2844 6973  class_schema(Dis
+000001f0: 7461 6e63 652c 2062 6173 655f 7363 6865  tance, base_sche
+00000200: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
+00000210: 6129 0d0a                                a)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/document.py` & `semantha_sdk-5.6.0/semantha_sdk/model/document.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,76 +7,76 @@
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e65 6e74 6974 7920 696d  .model.entity im
-000000d0: 706f 7274 2045 6e74 6974 790d 0a0d 0a66  port Entity....f
-000000e0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000f0: 2e6d 6f64 656c 2e70 6167 6520 696d 706f  .model.page impo
-00000100: 7274 2050 6167 650d 0a0d 0a66 726f 6d20  rt Page....from 
-00000110: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
-00000120: 656c 2e72 6566 6572 656e 6365 2069 6d70  el.reference imp
-00000130: 6f72 7420 5265 6665 7265 6e63 650d 0a0d  ort Reference...
-00000140: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-00000150: 6f72 7420 4c69 7374 0d0a 6672 6f6d 2074  ort List..from t
-00000160: 7970 696e 6720 696d 706f 7274 204f 7074  yping import Opt
-00000170: 696f 6e61 6c0d 0a0d 0a40 6461 7461 636c  ional....@datacl
-00000180: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00000190: 0d0a 636c 6173 7320 446f 6375 6d65 6e74  ..class Document
-000001a0: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
-000001b0: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
-000001c0: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
-000001d0: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
-000001e0: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
-000001f0: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
-00000200: 7921 2022 2222 0d0a 2020 2020 6964 3a20  y! """..    id: 
-00000210: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000220: 2020 206e 616d 653a 204f 7074 696f 6e61     name: Optiona
-00000230: 6c5b 7374 725d 0d0a 2020 2020 7461 6773  l[str]..    tags
-00000240: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00000250: 7374 725d 5d0d 0a20 2020 206d 6574 6164  str]]..    metad
-00000260: 6174 613a 204f 7074 696f 6e61 6c5b 7374  ata: Optional[st
-00000270: 725d 0d0a 2020 2020 6669 6c65 6e61 6d65  r]..    filename
-00000280: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-00000290: 0a20 2020 2063 7265 6174 6564 3a20 4f70  .    created: Op
-000002a0: 7469 6f6e 616c 5b69 6e74 5d0d 0a20 2020  tional[int]..   
-000002b0: 2075 7064 6174 6564 3a20 4f70 7469 6f6e   updated: Option
-000002c0: 616c 5b69 6e74 5d0d 0a20 2020 2070 726f  al[int]..    pro
-000002d0: 6365 7373 6564 3a20 4f70 7469 6f6e 616c  cessed: Optional
-000002e0: 5b62 6f6f 6c5d 0d0a 2020 2020 6c61 6e67  [bool]..    lang
-000002f0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-00000300: 0a20 2020 2063 6f6e 7465 6e74 3a20 4f70  .    content: Op
-00000310: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000320: 2064 6f63 756d 656e 745f 636c 6173 733a   document_class:
-00000330: 204f 7074 696f 6e61 6c5b 456e 7469 7479   Optional[Entity
-00000340: 5d0d 0a20 2020 2064 6572 6976 6564 5f74  ]..    derived_t
-00000350: 6167 733a 204f 7074 696f 6e61 6c5b 4c69  ags: Optional[Li
-00000360: 7374 5b73 7472 5d5d 0d0a 2020 2020 636f  st[str]]..    co
-00000370: 6c6f 723a 204f 7074 696f 6e61 6c5b 7374  lor: Optional[st
-00000380: 725d 0d0a 2020 2020 6465 7269 7665 645f  r]..    derived_
-00000390: 636f 6c6f 723a 204f 7074 696f 6e61 6c5b  color: Optional[
-000003a0: 7374 725d 0d0a 2020 2020 636f 6d6d 656e  str]..    commen
-000003b0: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
-000003c0: 0d0a 2020 2020 6465 7269 7665 645f 636f  ..    derived_co
-000003d0: 6d6d 656e 743a 204f 7074 696f 6e61 6c5b  mment: Optional[
-000003e0: 7374 725d 0d0a 2020 2020 636f 6e74 656e  str]..    conten
-000003f0: 745f 7072 6576 6965 773a 204f 7074 696f  t_preview: Optio
-00000400: 6e61 6c5b 7374 725d 0d0a 2020 2020 7061  nal[str]..    pa
-00000410: 6765 733a 204f 7074 696f 6e61 6c5b 4c69  ges: Optional[Li
-00000420: 7374 5b50 6167 655d 5d0d 0a20 2020 2072  st[Page]]..    r
-00000430: 6566 6572 656e 6365 733a 204f 7074 696f  eferences: Optio
-00000440: 6e61 6c5b 4c69 7374 5b52 6566 6572 656e  nal[List[Referen
-00000450: 6365 5d5d 0d0a 2020 2020 696d 6167 655f  ce]]..    image_
-00000460: 7061 6765 733a 204f 7074 696f 6e61 6c5b  pages: Optional[
-00000470: 4c69 7374 5b73 7472 5d5d 0d0a 2020 2020  List[str]]..    
-00000480: 646f 6375 6d65 6e74 5f63 6c61 7373 5f69  document_class_i
-00000490: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
-000004a0: 0d0a 0d0a 2020 2020 6465 6620 5f5f 6861  ....    def __ha
-000004b0: 7368 5f5f 2873 656c 6629 3a0d 0a20 2020  sh__(self):..   
-000004c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000004d0: 2e69 640d 0a44 6f63 756d 656e 7453 6368  .id..DocumentSch
-000004e0: 656d 6120 3d20 636c 6173 735f 7363 6865  ema = class_sche
-000004f0: 6d61 2844 6f63 756d 656e 742c 2062 6173  ma(Document, bas
-00000500: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
-00000510: 6153 6368 656d 6129 0d0a                 aSchema)..
+000000d0: 706f 7274 2045 6e74 6974 790d 0a66 726f  port Entity..fro
+000000e0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
+000000f0: 6f64 656c 2e70 6167 6520 696d 706f 7274  odel.page import
+00000100: 2050 6167 650d 0a66 726f 6d20 7365 6d61   Page..from sema
+00000110: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e72  ntha_sdk.model.r
+00000120: 6566 6572 656e 6365 2069 6d70 6f72 7420  eference import 
+00000130: 5265 6665 7265 6e63 650d 0a66 726f 6d20  Reference..from 
+00000140: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
+00000150: 7374 0d0a 6672 6f6d 2074 7970 696e 6720  st..from typing 
+00000160: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
+00000170: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
+00000180: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
+00000190: 6173 7320 446f 6375 6d65 6e74 2853 656d  ass Document(Sem
+000001a0: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
+000001b0: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
+000001c0: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
+000001d0: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
+000001e0: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
+000001f0: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
+00000200: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
+00000210: 6f6e 616c 5b73 7472 5d0d 0a20 2020 206e  onal[str]..    n
+00000220: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
+00000230: 725d 0d0a 2020 2020 7461 6773 3a20 4f70  r]..    tags: Op
+00000240: 7469 6f6e 616c 5b4c 6973 745b 7374 725d  tional[List[str]
+00000250: 5d0d 0a20 2020 206d 6574 6164 6174 613a  ]..    metadata:
+00000260: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
+00000270: 2020 2020 6669 6c65 6e61 6d65 3a20 4f70      filename: Op
+00000280: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000290: 2063 7265 6174 6564 3a20 4f70 7469 6f6e   created: Option
+000002a0: 616c 5b69 6e74 5d0d 0a20 2020 2075 7064  al[int]..    upd
+000002b0: 6174 6564 3a20 4f70 7469 6f6e 616c 5b69  ated: Optional[i
+000002c0: 6e74 5d0d 0a20 2020 2070 726f 6365 7373  nt]..    process
+000002d0: 6564 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ed: Optional[boo
+000002e0: 6c5d 0d0a 2020 2020 6c61 6e67 3a20 4f70  l]..    lang: Op
+000002f0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000300: 2063 6f6e 7465 6e74 3a20 4f70 7469 6f6e   content: Option
+00000310: 616c 5b73 7472 5d0d 0a20 2020 2064 6f63  al[str]..    doc
+00000320: 756d 656e 745f 636c 6173 733a 204f 7074  ument_class: Opt
+00000330: 696f 6e61 6c5b 456e 7469 7479 5d0d 0a20  ional[Entity].. 
+00000340: 2020 2064 6572 6976 6564 5f74 6167 733a     derived_tags:
+00000350: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00000360: 7472 5d5d 0d0a 2020 2020 636f 6c6f 723a  tr]]..    color:
+00000370: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
+00000380: 2020 2020 6465 7269 7665 645f 636f 6c6f      derived_colo
+00000390: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
+000003a0: 0d0a 2020 2020 636f 6d6d 656e 743a 204f  ..    comment: O
+000003b0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+000003c0: 2020 6465 7269 7665 645f 636f 6d6d 656e    derived_commen
+000003d0: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
+000003e0: 0d0a 2020 2020 636f 6e74 656e 745f 7072  ..    content_pr
+000003f0: 6576 6965 773a 204f 7074 696f 6e61 6c5b  eview: Optional[
+00000400: 7374 725d 0d0a 2020 2020 7061 6765 733a  str]..    pages:
+00000410: 204f 7074 696f 6e61 6c5b 4c69 7374 5b50   Optional[List[P
+00000420: 6167 655d 5d0d 0a20 2020 2072 6566 6572  age]]..    refer
+00000430: 656e 6365 733a 204f 7074 696f 6e61 6c5b  ences: Optional[
+00000440: 4c69 7374 5b52 6566 6572 656e 6365 5d5d  List[Reference]]
+00000450: 0d0a 2020 2020 696d 6167 655f 7061 6765  ..    image_page
+00000460: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+00000470: 5b73 7472 5d5d 0d0a 2020 2020 646f 6375  [str]]..    docu
+00000480: 6d65 6e74 5f63 6c61 7373 5f69 643a 204f  ment_class_id: O
+00000490: 7074 696f 6e61 6c5b 7374 725d 0d0a 0d0a  ptional[str]....
+000004a0: 2020 2020 6465 6620 5f5f 6861 7368 5f5f      def __hash__
+000004b0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000004c0: 2072 6574 7572 6e20 7365 6c66 2e69 640d   return self.id.
+000004d0: 0a44 6f63 756d 656e 7453 6368 656d 6120  .DocumentSchema 
+000004e0: 3d20 636c 6173 735f 7363 6865 6d61 2844  = class_schema(D
+000004f0: 6f63 756d 656e 742c 2062 6173 655f 7363  ocument, base_sc
+00000500: 6865 6d61 3d53 656d 616e 7468 6153 6368  hema=SemanthaSch
+00000510: 656d 6129 0d0a                           ema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/document_class.py` & `semantha_sdk-5.6.0/semantha_sdk/model/document_class.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e64 6f63 756d 656e 745f  .model.document_
 000000d0: 636c 6173 735f 6e6f 6465 2069 6d70 6f72  class_node impor
 000000e0: 7420 446f 6375 6d65 6e74 436c 6173 734e  t DocumentClassN
-000000f0: 6f64 650d 0a0d 0a66 726f 6d20 7479 7069  ode....from typi
-00000100: 6e67 2069 6d70 6f72 7420 4c69 7374 0d0a  ng import List..
-00000110: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000120: 7274 204f 7074 696f 6e61 6c0d 0a0d 0a40  rt Optional....@
+000000f0: 6f64 650d 0a66 726f 6d20 7479 7069 6e67  ode..from typing
+00000100: 2069 6d70 6f72 7420 4c69 7374 0d0a 6672   import List..fr
+00000110: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000120: 204f 7074 696f 6e61 6c0d 0a0d 0a0d 0a40   Optional......@
 00000130: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
 00000140: 3d54 7275 6529 0d0a 636c 6173 7320 446f  =True)..class Do
 00000150: 6375 6d65 6e74 436c 6173 7328 5365 6d61  cumentClass(Sema
 00000160: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
 00000170: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
 00000180: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
 00000190: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/document_class_bulk.py` & `semantha_sdk-5.6.0/semantha_sdk/model/document_class_bulk.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class DocumentClassBulk(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     id: Optional[str]
     name: str
     document_ids: Optional[List[str]]
     sub_classes: Optional[List["DocumentClassBulk"]]
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/document_class_node.py` & `semantha_sdk-5.6.0/semantha_sdk/model/table_instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2044 6f63  True)..class Doc
-000000f0: 756d 656e 7443 6c61 7373 4e6f 6465 2853  umentClassNode(S
-00000100: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
-00000110: 7479 293a 0d0a 2020 2020 2222 2220 6175  ty):..    """ au
-00000120: 7468 6f72 2073 656d 616e 7468 612c 2074  thor semantha, t
-00000130: 6869 7320 6973 2061 2067 656e 6572 6174  his is a generat
-00000140: 6564 2063 6c61 7373 2064 6f20 6e6f 7420  ed class do not 
-00000150: 6368 616e 6765 206d 616e 7561 6c6c 7921  change manually!
-00000160: 2022 2222 0d0a 2020 2020 6964 3a20 4f70   """..    id: Op
-00000170: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000180: 206e 616d 653a 2073 7472 0d0a 2020 2020   name: str..    
-00000190: 7061 7265 6e74 5f69 643a 204f 7074 696f  parent_id: Optio
-000001a0: 6e61 6c5b 7374 725d 0d0a 2020 2020 6d65  nal[str]..    me
-000001b0: 7461 6461 7461 3a20 4f70 7469 6f6e 616c  tadata: Optional
-000001c0: 5b73 7472 5d0d 0a20 2020 2064 6f63 756d  [str]..    docum
-000001d0: 656e 7473 5f63 6f75 6e74 3a20 4f70 7469  ents_count: Opti
-000001e0: 6f6e 616c 5b69 6e74 5d0d 0a0d 0a44 6f63  onal[int]....Doc
-000001f0: 756d 656e 7443 6c61 7373 4e6f 6465 5363  umentClassNodeSc
-00000200: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-00000210: 656d 6128 446f 6375 6d65 6e74 436c 6173  ema(DocumentClas
-00000220: 734e 6f64 652c 2062 6173 655f 7363 6865  sNode, base_sche
-00000230: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
-00000240: 6129 0d0a                                a)..
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 696f  .model.extractio
+000000d0: 6e5f 6172 6561 2069 6d70 6f72 7420 4578  n_area import Ex
+000000e0: 7472 6163 7469 6f6e 4172 6561 0d0a 6672  tractionArea..fr
+000000f0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000100: 204f 7074 696f 6e61 6c0d 0a0d 0a0d 0a40   Optional......@
+00000110: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
+00000120: 3d54 7275 6529 0d0a 636c 6173 7320 5461  =True)..class Ta
+00000130: 626c 6549 6e73 7461 6e63 6528 5365 6d61  bleInstance(Sema
+00000140: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
+00000150: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
+00000160: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
+00000170: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
+00000180: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
+00000190: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
+000001a0: 220d 0a20 2020 2074 7970 653a 204f 7074  "..    type: Opt
+000001b0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+000001c0: 6578 7472 6163 7469 6f6e 5f61 7265 613a  extraction_area:
+000001d0: 204f 7074 696f 6e61 6c5b 4578 7472 6163   Optional[Extrac
+000001e0: 7469 6f6e 4172 6561 5d0d 0a0d 0a54 6162  tionArea]....Tab
+000001f0: 6c65 496e 7374 616e 6365 5363 6865 6d61  leInstanceSchema
+00000200: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+00000210: 5461 626c 6549 6e73 7461 6e63 652c 2062  TableInstance, b
+00000220: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
+00000230: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/document_cluster.py` & `semantha_sdk-5.6.0/semantha_sdk/model/document_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e63 6c75 7374 6572 6564  .model.clustered
 000000d0: 5f64 6f63 756d 656e 7420 696d 706f 7274  _document import
 000000e0: 2043 6c75 7374 6572 6564 446f 6375 6d65   ClusteredDocume
-000000f0: 6e74 0d0a 0d0a 6672 6f6d 2074 7970 696e  nt....from typin
-00000100: 6720 696d 706f 7274 204c 6973 740d 0a66  g import List..f
-00000110: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-00000120: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
+000000f0: 6e74 0d0a 6672 6f6d 2074 7970 696e 6720  nt..from typing 
+00000100: 696d 706f 7274 204c 6973 740d 0a66 726f  import List..fro
+00000110: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00000120: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
 00000130: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
 00000140: 5472 7565 290d 0a63 6c61 7373 2044 6f63  True)..class Doc
 00000150: 756d 656e 7443 6c75 7374 6572 2853 656d  umentCluster(Sem
 00000160: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
 00000170: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
 00000180: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
 00000190: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/document_information.py` & `semantha_sdk-5.6.0/semantha_sdk/model/document_information.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e65 6e74 6974 7920 696d  .model.entity im
-000000d0: 706f 7274 2045 6e74 6974 790d 0a0d 0a66  port Entity....f
-000000e0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000f0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
-00000100: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-00000110: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
+000000d0: 706f 7274 2045 6e74 6974 790d 0a66 726f  port Entity..fro
+000000e0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+000000f0: 4c69 7374 0d0a 6672 6f6d 2074 7970 696e  List..from typin
+00000100: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
+00000110: 6c0d 0a0d 0a0d 0a40 6461 7461 636c 6173  l......@dataclas
 00000120: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
 00000130: 636c 6173 7320 446f 6375 6d65 6e74 496e  class DocumentIn
 00000140: 666f 726d 6174 696f 6e28 5365 6d61 6e74  formation(Semant
 00000150: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
 00000160: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
 00000170: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
 00000180: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/document_table.py` & `semantha_sdk-5.6.0/semantha_sdk/model/document_table.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.row import Row
-
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class DocumentTable(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     rows: Optional[List[Row]]
 
 DocumentTableSchema = class_schema(DocumentTable, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/domain.py` & `semantha_sdk-5.6.0/semantha_sdk/model/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e73 6574 7469 6e67 7320  .model.settings 
 000000d0: 696d 706f 7274 2053 6574 7469 6e67 730d  import Settings.
-000000e0: 0a0d 0a66 726f 6d20 7479 7069 6e67 2069  ...from typing i
-000000f0: 6d70 6f72 7420 4f70 7469 6f6e 616c 0d0a  mport Optional..
+000000e0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+000000f0: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
 00000100: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
 00000110: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
 00000120: 2044 6f6d 6169 6e28 5365 6d61 6e74 6861   Domain(Semantha
 00000130: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
 00000140: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
 00000150: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
 00000160: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/extraction_area.py` & `semantha_sdk-5.6.0/semantha_sdk/model/extraction_area.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e66 696c 655f 7265 6665  .model.file_refe
 000000d0: 7265 6e63 6520 696d 706f 7274 2046 696c  rence import Fil
-000000e0: 6552 6566 6572 656e 6365 0d0a 0d0a 6672  eReference....fr
-000000f0: 6f6d 2073 656d 616e 7468 615f 7364 6b2e  om semantha_sdk.
-00000100: 6d6f 6465 6c2e 7265 6374 2069 6d70 6f72  model.rect impor
-00000110: 7420 5265 6374 0d0a 0d0a 6672 6f6d 2074  t Rect....from t
-00000120: 7970 696e 6720 696d 706f 7274 204f 7074  yping import Opt
-00000130: 696f 6e61 6c0d 0a0d 0a40 6461 7461 636c  ional....@datacl
-00000140: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00000150: 0d0a 636c 6173 7320 4578 7472 6163 7469  ..class Extracti
-00000160: 6f6e 4172 6561 2853 656d 616e 7468 614d  onArea(SemanthaM
-00000170: 6f64 656c 456e 7469 7479 293a 0d0a 2020  odelEntity):..  
-00000180: 2020 2222 2220 6175 7468 6f72 2073 656d    """ author sem
-00000190: 616e 7468 612c 2074 6869 7320 6973 2061  antha, this is a
-000001a0: 2067 656e 6572 6174 6564 2063 6c61 7373   generated class
-000001b0: 2064 6f20 6e6f 7420 6368 616e 6765 206d   do not change m
-000001c0: 616e 7561 6c6c 7921 2022 2222 0d0a 2020  anually! """..  
-000001d0: 2020 6669 6c65 3a20 4f70 7469 6f6e 616c    file: Optional
-000001e0: 5b46 696c 6552 6566 6572 656e 6365 5d0d  [FileReference].
-000001f0: 0a20 2020 2072 6563 743a 204f 7074 696f  .    rect: Optio
-00000200: 6e61 6c5b 5265 6374 5d0d 0a0d 0a45 7874  nal[Rect]....Ext
-00000210: 7261 6374 696f 6e41 7265 6153 6368 656d  ractionAreaSchem
-00000220: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
-00000230: 2845 7874 7261 6374 696f 6e41 7265 612c  (ExtractionArea,
-00000240: 2062 6173 655f 7363 6865 6d61 3d53 656d   base_schema=Sem
-00000250: 616e 7468 6153 6368 656d 6129 0d0a       anthaSchema)..
+000000e0: 6552 6566 6572 656e 6365 0d0a 6672 6f6d  eReference..from
+000000f0: 2073 656d 616e 7468 615f 7364 6b2e 6d6f   semantha_sdk.mo
+00000100: 6465 6c2e 7265 6374 2069 6d70 6f72 7420  del.rect import 
+00000110: 5265 6374 0d0a 6672 6f6d 2074 7970 696e  Rect..from typin
+00000120: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
+00000130: 6c0d 0a0d 0a0d 0a40 6461 7461 636c 6173  l......@dataclas
+00000140: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
+00000150: 636c 6173 7320 4578 7472 6163 7469 6f6e  class Extraction
+00000160: 4172 6561 2853 656d 616e 7468 614d 6f64  Area(SemanthaMod
+00000170: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
+00000180: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
+00000190: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
+000001a0: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
+000001b0: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
+000001c0: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
+000001d0: 6669 6c65 3a20 4f70 7469 6f6e 616c 5b46  file: Optional[F
+000001e0: 696c 6552 6566 6572 656e 6365 5d0d 0a20  ileReference].. 
+000001f0: 2020 2072 6563 743a 204f 7074 696f 6e61     rect: Optiona
+00000200: 6c5b 5265 6374 5d0d 0a0d 0a45 7874 7261  l[Rect]....Extra
+00000210: 6374 696f 6e41 7265 6153 6368 656d 6120  ctionAreaSchema 
+00000220: 3d20 636c 6173 735f 7363 6865 6d61 2845  = class_schema(E
+00000230: 7874 7261 6374 696f 6e41 7265 612c 2062  xtractionArea, b
+00000240: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
+00000250: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/extraction_file.py` & `semantha_sdk-5.6.0/semantha_sdk/model/extraction_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e64 6f63 756d 656e 7420  .model.document 
 000000d0: 696d 706f 7274 2044 6f63 756d 656e 740d  import Document.
-000000e0: 0a0d 0a66 726f 6d20 7479 7069 6e67 2069  ...from typing i
-000000f0: 6d70 6f72 7420 4f70 7469 6f6e 616c 0d0a  mport Optional..
+000000e0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+000000f0: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
 00000100: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
 00000110: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
 00000120: 2045 7874 7261 6374 696f 6e46 696c 6528   ExtractionFile(
 00000130: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
 00000140: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
 00000150: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
 00000160: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/extraction_reference.py` & `semantha_sdk-5.6.0/semantha_sdk/model/extraction_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2045 7874  True)..class Ext
-000000f0: 7261 6374 696f 6e52 6566 6572 656e 6365  ractionReference
-00000100: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
-00000110: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
-00000120: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
-00000130: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
-00000140: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
-00000150: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
-00000160: 7921 2022 2222 0d0a 2020 2020 646f 6375  y! """..    docu
-00000170: 6d65 6e74 5f69 643a 204f 7074 696f 6e61  ment_id: Optiona
-00000180: 6c5b 7374 725d 0d0a 2020 2020 7369 6d69  l[str]..    simi
-00000190: 6c61 7269 7479 3a20 4f70 7469 6f6e 616c  larity: Optional
-000001a0: 5b66 6c6f 6174 5d0d 0a20 2020 2075 7365  [float]..    use
-000001b0: 643a 204f 7074 696f 6e61 6c5b 626f 6f6c  d: Optional[bool
-000001c0: 5d0d 0a0d 0a45 7874 7261 6374 696f 6e52  ]....ExtractionR
-000001d0: 6566 6572 656e 6365 5363 6865 6d61 203d  eferenceSchema =
-000001e0: 2063 6c61 7373 5f73 6368 656d 6128 4578   class_schema(Ex
-000001f0: 7472 6163 7469 6f6e 5265 6665 7265 6e63  tractionReferenc
-00000200: 652c 2062 6173 655f 7363 6865 6d61 3d53  e, base_schema=S
-00000210: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2045  n=True)..class E
+000000f0: 7874 7261 6374 696f 6e52 6566 6572 656e  xtractionReferen
+00000100: 6365 2853 656d 616e 7468 614d 6f64 656c  ce(SemanthaModel
+00000110: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
+00000120: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
+00000130: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
+00000140: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
+00000150: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
+00000160: 6c6c 7921 2022 2222 0d0a 2020 2020 646f  lly! """..    do
+00000170: 6375 6d65 6e74 5f69 643a 204f 7074 696f  cument_id: Optio
+00000180: 6e61 6c5b 7374 725d 0d0a 2020 2020 7369  nal[str]..    si
+00000190: 6d69 6c61 7269 7479 3a20 4f70 7469 6f6e  milarity: Option
+000001a0: 616c 5b66 6c6f 6174 5d0d 0a20 2020 2075  al[float]..    u
+000001b0: 7365 643a 204f 7074 696f 6e61 6c5b 626f  sed: Optional[bo
+000001c0: 6f6c 5d0d 0a0d 0a45 7874 7261 6374 696f  ol]....Extractio
+000001d0: 6e52 6566 6572 656e 6365 5363 6865 6d61  nReferenceSchema
+000001e0: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+000001f0: 4578 7472 6163 7469 6f6e 5265 6665 7265  ExtractionRefere
+00000200: 6e63 652c 2062 6173 655f 7363 6865 6d61  nce, base_schema
+00000210: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
+00000220: 0d0a                                     ..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/features.py` & `semantha_sdk-5.6.0/semantha_sdk/model/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e64 6973 7461 6e63 6520  .model.distance 
 000000d0: 696d 706f 7274 2044 6973 7461 6e63 650d  import Distance.
-000000e0: 0a0d 0a66 726f 6d20 7479 7069 6e67 2069  ...from typing i
-000000f0: 6d70 6f72 7420 4f70 7469 6f6e 616c 0d0a  mport Optional..
+000000e0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+000000f0: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
 00000100: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
 00000110: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
 00000120: 2046 6561 7475 7265 7328 5365 6d61 6e74   Features(Semant
 00000130: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
 00000140: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
 00000150: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
 00000160: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/file_reference.py` & `semantha_sdk-5.6.0/semantha_sdk/model/file_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2046 696c  True)..class Fil
-000000f0: 6552 6566 6572 656e 6365 2853 656d 616e  eReference(Seman
-00000100: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
-00000110: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
-00000120: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
-00000130: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
-00000140: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
-00000150: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
-00000160: 0d0a 2020 2020 6669 6c65 5f69 643a 204f  ..    file_id: O
-00000170: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000180: 2020 6e61 6d65 3a20 4f70 7469 6f6e 616c    name: Optional
-00000190: 5b73 7472 5d0d 0a20 2020 2070 6167 655f  [str]..    page_
-000001a0: 6e75 6d62 6572 3a20 4f70 7469 6f6e 616c  number: Optional
-000001b0: 5b69 6e74 5d0d 0a0d 0a46 696c 6552 6566  [int]....FileRef
-000001c0: 6572 656e 6365 5363 6865 6d61 203d 2063  erenceSchema = c
-000001d0: 6c61 7373 5f73 6368 656d 6128 4669 6c65  lass_schema(File
-000001e0: 5265 6665 7265 6e63 652c 2062 6173 655f  Reference, base_
-000001f0: 7363 6865 6d61 3d53 656d 616e 7468 6153  schema=SemanthaS
-00000200: 6368 656d 6129 0d0a                      chema)..
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2046  n=True)..class F
+000000f0: 696c 6552 6566 6572 656e 6365 2853 656d  ileReference(Sem
+00000100: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
+00000110: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
+00000120: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
+00000130: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
+00000140: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
+00000150: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
+00000160: 2222 0d0a 2020 2020 6669 6c65 5f69 643a  ""..    file_id:
+00000170: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
+00000180: 2020 2020 6e61 6d65 3a20 4f70 7469 6f6e      name: Option
+00000190: 616c 5b73 7472 5d0d 0a20 2020 2070 6167  al[str]..    pag
+000001a0: 655f 6e75 6d62 6572 3a20 4f70 7469 6f6e  e_number: Option
+000001b0: 616c 5b69 6e74 5d0d 0a0d 0a46 696c 6552  al[int]....FileR
+000001c0: 6566 6572 656e 6365 5363 6865 6d61 203d  eferenceSchema =
+000001d0: 2063 6c61 7373 5f73 6368 656d 6128 4669   class_schema(Fi
+000001e0: 6c65 5265 6665 7265 6e63 652c 2062 6173  leReference, bas
+000001f0: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
+00000200: 6153 6368 656d 6129 0d0a                 aSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/info.py` & `semantha_sdk-5.6.0/semantha_sdk/model/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2049 6e66  True)..class Inf
-000000f0: 6f28 5365 6d61 6e74 6861 4d6f 6465 6c45  o(SemanthaModelE
-00000100: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
-00000110: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
-00000120: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
-00000130: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
-00000140: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
-00000150: 6c79 2120 2222 220d 0a20 2020 2074 6974  ly! """..    tit
-00000160: 6c65 3a20 4f70 7469 6f6e 616c 5b73 7472  le: Optional[str
-00000170: 5d0d 0a20 2020 2076 656e 646f 723a 204f  ]..    vendor: O
-00000180: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000190: 2020 7469 6d65 3a20 4f70 7469 6f6e 616c    time: Optional
-000001a0: 5b73 7472 5d0d 0a20 2020 2067 6974 3a20  [str]..    git: 
-000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-000001c0: 2020 2076 6572 7369 6f6e 3a20 4f70 7469     version: Opti
-000001d0: 6f6e 616c 5b73 7472 5d0d 0a0d 0a49 6e66  onal[str]....Inf
-000001e0: 6f53 6368 656d 6120 3d20 636c 6173 735f  oSchema = class_
-000001f0: 7363 6865 6d61 2849 6e66 6f2c 2062 6173  schema(Info, bas
-00000200: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
-00000210: 6153 6368 656d 6129 0d0a                 aSchema)..
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2049  n=True)..class I
+000000f0: 6e66 6f28 5365 6d61 6e74 6861 4d6f 6465  nfo(SemanthaMode
+00000100: 6c45 6e74 6974 7929 3a0d 0a20 2020 2022  lEntity):..    "
+00000110: 2222 2061 7574 686f 7220 7365 6d61 6e74  "" author semant
+00000120: 6861 2c20 7468 6973 2069 7320 6120 6765  ha, this is a ge
+00000130: 6e65 7261 7465 6420 636c 6173 7320 646f  nerated class do
+00000140: 206e 6f74 2063 6861 6e67 6520 6d61 6e75   not change manu
+00000150: 616c 6c79 2120 2222 220d 0a20 2020 2074  ally! """..    t
+00000160: 6974 6c65 3a20 4f70 7469 6f6e 616c 5b73  itle: Optional[s
+00000170: 7472 5d0d 0a20 2020 2076 656e 646f 723a  tr]..    vendor:
+00000180: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
+00000190: 2020 2020 7469 6d65 3a20 4f70 7469 6f6e      time: Option
+000001a0: 616c 5b73 7472 5d0d 0a20 2020 2067 6974  al[str]..    git
+000001b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+000001c0: 0a20 2020 2076 6572 7369 6f6e 3a20 4f70  .    version: Op
+000001d0: 7469 6f6e 616c 5b73 7472 5d0d 0a0d 0a49  tional[str]....I
+000001e0: 6e66 6f53 6368 656d 6120 3d20 636c 6173  nfoSchema = clas
+000001f0: 735f 7363 6865 6d61 2849 6e66 6f2c 2062  s_schema(Info, b
+00000200: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
+00000210: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/instance.py` & `semantha_sdk-5.6.0/semantha_sdk/model/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,49 +8,49 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e69 6e73 7461 6e63 655f  .model.instance_
 000000d0: 6368 696c 6420 696d 706f 7274 2049 6e73  child import Ins
-000000e0: 7461 6e63 6543 6869 6c64 0d0a 0d0a 6672  tanceChild....fr
-000000f0: 6f6d 2073 656d 616e 7468 615f 7364 6b2e  om semantha_sdk.
-00000100: 6d6f 6465 6c2e 7369 6d70 6c65 5f70 726f  model.simple_pro
-00000110: 7065 7274 7920 696d 706f 7274 2053 696d  perty import Sim
-00000120: 706c 6550 726f 7065 7274 790d 0a0d 0a66  pleProperty....f
-00000130: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-00000140: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
-00000150: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-00000160: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
-00000170: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
-00000180: 636c 6173 7320 496e 7374 616e 6365 2853  class Instance(S
-00000190: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
-000001a0: 7479 293a 0d0a 2020 2020 2222 2220 6175  ty):..    """ au
-000001b0: 7468 6f72 2073 656d 616e 7468 612c 2074  thor semantha, t
-000001c0: 6869 7320 6973 2061 2067 656e 6572 6174  his is a generat
-000001d0: 6564 2063 6c61 7373 2064 6f20 6e6f 7420  ed class do not 
-000001e0: 6368 616e 6765 206d 616e 7561 6c6c 7921  change manually!
-000001f0: 2022 2222 0d0a 2020 2020 6964 3a20 4f70   """..    id: Op
-00000200: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-00000210: 206e 616d 653a 2073 7472 0d0a 2020 2020   name: str..    
-00000220: 636c 6173 735f 6964 3a20 7374 720d 0a20  class_id: str.. 
-00000230: 2020 2072 656c 6174 696f 6e5f 6964 3a20     relation_id: 
-00000240: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000250: 2020 2074 7970 653a 204f 7074 696f 6e61     type: Optiona
-00000260: 6c5b 7374 725d 0d0a 2020 2020 6967 6e6f  l[str]..    igno
-00000270: 7265 5f69 6d70 6f72 743a 204f 7074 696f  re_import: Optio
-00000280: 6e61 6c5b 626f 6f6c 5d0d 0a20 2020 2073  nal[bool]..    s
-00000290: 696d 706c 655f 7072 6f70 6572 7469 6573  imple_properties
-000002a0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-000002b0: 5369 6d70 6c65 5072 6f70 6572 7479 5d5d  SimpleProperty]]
-000002c0: 0d0a 2020 2020 636f 6d6d 656e 743a 204f  ..    comment: O
-000002d0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-000002e0: 2020 696e 7374 616e 6365 733a 204f 7074    instances: Opt
-000002f0: 696f 6e61 6c5b 4c69 7374 5b22 496e 7374  ional[List["Inst
-00000300: 616e 6365 225d 5d0d 0a20 2020 2063 6869  ance"]]..    chi
-00000310: 6c64 733a 204f 7074 696f 6e61 6c5b 4c69  lds: Optional[Li
-00000320: 7374 5b49 6e73 7461 6e63 6543 6869 6c64  st[InstanceChild
-00000330: 5d5d 0d0a 0d0a 496e 7374 616e 6365 5363  ]]....InstanceSc
-00000340: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-00000350: 656d 6128 496e 7374 616e 6365 2c20 6261  ema(Instance, ba
-00000360: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
-00000370: 6861 5363 6865 6d61 290d 0a              haSchema)..
+000000e0: 7461 6e63 6543 6869 6c64 0d0a 6672 6f6d  tanceChild..from
+000000f0: 2073 656d 616e 7468 615f 7364 6b2e 6d6f   semantha_sdk.mo
+00000100: 6465 6c2e 7369 6d70 6c65 5f70 726f 7065  del.simple_prope
+00000110: 7274 7920 696d 706f 7274 2053 696d 706c  rty import Simpl
+00000120: 6550 726f 7065 7274 790d 0a66 726f 6d20  eProperty..from 
+00000130: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
+00000140: 7374 0d0a 6672 6f6d 2074 7970 696e 6720  st..from typing 
+00000150: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
+00000160: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
+00000170: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
+00000180: 6173 7320 496e 7374 616e 6365 2853 656d  ass Instance(Sem
+00000190: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
+000001a0: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
+000001b0: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
+000001c0: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
+000001d0: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
+000001e0: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
+000001f0: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
+00000200: 6f6e 616c 5b73 7472 5d0d 0a20 2020 206e  onal[str]..    n
+00000210: 616d 653a 2073 7472 0d0a 2020 2020 636c  ame: str..    cl
+00000220: 6173 735f 6964 3a20 7374 720d 0a20 2020  ass_id: str..   
+00000230: 2072 656c 6174 696f 6e5f 6964 3a20 4f70   relation_id: Op
+00000240: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000250: 2074 7970 653a 204f 7074 696f 6e61 6c5b   type: Optional[
+00000260: 7374 725d 0d0a 2020 2020 6967 6e6f 7265  str]..    ignore
+00000270: 5f69 6d70 6f72 743a 204f 7074 696f 6e61  _import: Optiona
+00000280: 6c5b 626f 6f6c 5d0d 0a20 2020 2073 696d  l[bool]..    sim
+00000290: 706c 655f 7072 6f70 6572 7469 6573 3a20  ple_properties: 
+000002a0: 4f70 7469 6f6e 616c 5b4c 6973 745b 5369  Optional[List[Si
+000002b0: 6d70 6c65 5072 6f70 6572 7479 5d5d 0d0a  mpleProperty]]..
+000002c0: 2020 2020 636f 6d6d 656e 743a 204f 7074      comment: Opt
+000002d0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+000002e0: 696e 7374 616e 6365 733a 204f 7074 696f  instances: Optio
+000002f0: 6e61 6c5b 4c69 7374 5b22 496e 7374 616e  nal[List["Instan
+00000300: 6365 225d 5d0d 0a20 2020 2063 6869 6c64  ce"]]..    child
+00000310: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+00000320: 5b49 6e73 7461 6e63 6543 6869 6c64 5d5d  [InstanceChild]]
+00000330: 0d0a 0d0a 496e 7374 616e 6365 5363 6865  ....InstanceSche
+00000340: 6d61 203d 2063 6c61 7373 5f73 6368 656d  ma = class_schem
+00000350: 6128 496e 7374 616e 6365 2c20 6261 7365  a(Instance, base
+00000360: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
+00000370: 5363 6865 6d61 290d 0a                   Schema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/instance_child.py` & `semantha_sdk-5.6.0/semantha_sdk/model/instance_child.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2049 6e73  True)..class Ins
-000000f0: 7461 6e63 6543 6869 6c64 2853 656d 616e  tanceChild(Seman
-00000100: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
-00000110: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
-00000120: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
-00000130: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
-00000140: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
-00000150: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
-00000160: 0d0a 2020 2020 6964 3a20 4f70 7469 6f6e  ..    id: Option
-00000170: 616c 5b73 7472 5d0d 0a20 2020 206e 616d  al[str]..    nam
-00000180: 653a 2073 7472 0d0a 2020 2020 7265 6c61  e: str..    rela
-00000190: 7469 6f6e 5f69 643a 2073 7472 0d0a 2020  tion_id: str..  
-000001a0: 2020 636c 6173 735f 6e61 6d65 3a20 4f70    class_name: Op
-000001b0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
-000001c0: 2063 6c61 7373 5f69 643a 2073 7472 0d0a   class_id: str..
-000001d0: 0d0a 496e 7374 616e 6365 4368 696c 6453  ..InstanceChildS
-000001e0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
-000001f0: 6865 6d61 2849 6e73 7461 6e63 6543 6869  hema(InstanceChi
-00000200: 6c64 2c20 6261 7365 5f73 6368 656d 613d  ld, base_schema=
-00000210: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
-00000220: 0a                                       .
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2049  n=True)..class I
+000000f0: 6e73 7461 6e63 6543 6869 6c64 2853 656d  nstanceChild(Sem
+00000100: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
+00000110: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
+00000120: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
+00000130: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
+00000140: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
+00000150: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
+00000160: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
+00000170: 6f6e 616c 5b73 7472 5d0d 0a20 2020 206e  onal[str]..    n
+00000180: 616d 653a 2073 7472 0d0a 2020 2020 7265  ame: str..    re
+00000190: 6c61 7469 6f6e 5f69 643a 2073 7472 0d0a  lation_id: str..
+000001a0: 2020 2020 636c 6173 735f 6e61 6d65 3a20      class_name: 
+000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+000001c0: 2020 2063 6c61 7373 5f69 643a 2073 7472     class_id: str
+000001d0: 0d0a 0d0a 496e 7374 616e 6365 4368 696c  ....InstanceChil
+000001e0: 6453 6368 656d 6120 3d20 636c 6173 735f  dSchema = class_
+000001f0: 7363 6865 6d61 2849 6e73 7461 6e63 6543  schema(InstanceC
+00000200: 6869 6c64 2c20 6261 7365 5f73 6368 656d  hild, base_schem
+00000210: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
+00000220: 290d 0a                                  )..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/linked_instance.py` & `semantha_sdk-5.6.0/semantha_sdk/model/condition_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.linked_value import LinkedValue
-
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
-class LinkedInstance(SemanthaModelEntity):
+class ConditionValue(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
-    instance_id: Optional[str]
-    linked_values: Optional[List[LinkedValue]]
+    function: Optional[str]
+    arguments: Optional[List["Argument"]]
 
-LinkedInstanceSchema = class_schema(LinkedInstance, base_schema=SemanthaSchema)
+from semantha_sdk.model.argument import Argument
+ConditionValueSchema = class_schema(ConditionValue, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/matrix_row.py` & `semantha_sdk-5.6.0/semantha_sdk/model/matrix_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e72 6566 6572 656e 6365  .model.reference
 000000d0: 2069 6d70 6f72 7420 5265 6665 7265 6e63   import Referenc
-000000e0: 650d 0a0d 0a66 726f 6d20 7479 7069 6e67  e....from typing
-000000f0: 2069 6d70 6f72 7420 4c69 7374 0d0a 6672   import List..fr
-00000100: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000110: 204f 7074 696f 6e61 6c0d 0a0d 0a40 6461   Optional....@da
+000000e0: 650d 0a66 726f 6d20 7479 7069 6e67 2069  e..from typing i
+000000f0: 6d70 6f72 7420 4c69 7374 0d0a 6672 6f6d  mport List..from
+00000100: 2074 7970 696e 6720 696d 706f 7274 204f   typing import O
+00000110: 7074 696f 6e61 6c0d 0a0d 0a0d 0a40 6461  ptional......@da
 00000120: 7461 636c 6173 7328 6672 6f7a 656e 3d54  taclass(frozen=T
 00000130: 7275 6529 0d0a 636c 6173 7320 4d61 7472  rue)..class Matr
 00000140: 6978 526f 7728 5365 6d61 6e74 6861 4d6f  ixRow(SemanthaMo
 00000150: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
 00000160: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
 00000170: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
 00000180: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/model_class.py` & `semantha_sdk-5.6.0/semantha_sdk/model/model_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
 000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-000000e0: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
-000000f0: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
-00000100: 636c 6173 7320 4d6f 6465 6c43 6c61 7373  class ModelClass
-00000110: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
-00000120: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
-00000130: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
-00000140: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
-00000150: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
-00000160: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
-00000170: 7921 2022 2222 0d0a 2020 2020 6e61 6d65  y! """..    name
-00000180: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-00000190: 0a20 2020 206c 6162 656c 3a20 4f70 7469  .    label: Opti
-000001a0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2073  onal[str]..    s
-000001b0: 7562 5f6d 6f64 656c 5f63 6c61 7373 6573  ub_model_classes
-000001c0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-000001d0: 224d 6f64 656c 436c 6173 7322 5d5d 0d0a  "ModelClass"]]..
-000001e0: 0d0a 4d6f 6465 6c43 6c61 7373 5363 6865  ..ModelClassSche
-000001f0: 6d61 203d 2063 6c61 7373 5f73 6368 656d  ma = class_schem
-00000200: 6128 4d6f 6465 6c43 6c61 7373 2c20 6261  a(ModelClass, ba
-00000210: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
-00000220: 6861 5363 6865 6d61 290d 0a              haSchema)..
+000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000100: 0d0a 636c 6173 7320 4d6f 6465 6c43 6c61  ..class ModelCla
+00000110: 7373 2853 656d 616e 7468 614d 6f64 656c  ss(SemanthaModel
+00000120: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
+00000130: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
+00000140: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
+00000150: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
+00000160: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
+00000170: 6c6c 7921 2022 2222 0d0a 2020 2020 6e61  lly! """..    na
+00000180: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
+00000190: 5d0d 0a20 2020 206c 6162 656c 3a20 4f70  ]..    label: Op
+000001a0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+000001b0: 2073 7562 5f6d 6f64 656c 5f63 6c61 7373   sub_model_class
+000001c0: 6573 3a20 4f70 7469 6f6e 616c 5b4c 6973  es: Optional[Lis
+000001d0: 745b 224d 6f64 656c 436c 6173 7322 5d5d  t["ModelClass"]]
+000001e0: 0d0a 0d0a 4d6f 6465 6c43 6c61 7373 5363  ....ModelClassSc
+000001f0: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+00000200: 656d 6128 4d6f 6465 6c43 6c61 7373 2c20  ema(ModelClass, 
+00000210: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
+00000220: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/model_instance.py` & `semantha_sdk-5.6.0/semantha_sdk/model/model_instance.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,91 +9,90 @@
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e63 6f6d 706c 6578 5f70  .model.complex_p
 000000d0: 726f 7065 7274 7920 696d 706f 7274 2043  roperty import C
 000000e0: 6f6d 706c 6578 5072 6f70 6572 7479 0d0a  omplexProperty..
-000000f0: 0d0a 6672 6f6d 2073 656d 616e 7468 615f  ..from semantha_
-00000100: 7364 6b2e 6d6f 6465 6c2e 6578 7472 6163  sdk.model.extrac
-00000110: 7469 6f6e 5f72 6566 6572 656e 6365 2069  tion_reference i
-00000120: 6d70 6f72 7420 4578 7472 6163 7469 6f6e  mport Extraction
-00000130: 5265 6665 7265 6e63 650d 0a0d 0a66 726f  Reference....fro
-00000140: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-00000150: 6f64 656c 2e66 696c 655f 7265 6665 7265  odel.file_refere
-00000160: 6e63 6520 696d 706f 7274 2046 696c 6552  nce import FileR
-00000170: 6566 6572 656e 6365 0d0a 0d0a 6672 6f6d  eference....from
-00000180: 2073 656d 616e 7468 615f 7364 6b2e 6d6f   semantha_sdk.mo
-00000190: 6465 6c2e 6669 6e64 696e 6720 696d 706f  del.finding impo
-000001a0: 7274 2046 696e 6469 6e67 0d0a 0d0a 6672  rt Finding....fr
-000001b0: 6f6d 2073 656d 616e 7468 615f 7364 6b2e  om semantha_sdk.
-000001c0: 6d6f 6465 6c2e 6c61 6265 6c20 696d 706f  model.label impo
-000001d0: 7274 204c 6162 656c 0d0a 0d0a 6672 6f6d  rt Label....from
-000001e0: 2073 656d 616e 7468 615f 7364 6b2e 6d6f   semantha_sdk.mo
-000001f0: 6465 6c2e 6c69 6e6b 6564 5f69 6e73 7461  del.linked_insta
-00000200: 6e63 6520 696d 706f 7274 204c 696e 6b65  nce import Linke
-00000210: 6449 6e73 7461 6e63 650d 0a0d 0a66 726f  dInstance....fro
-00000220: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-00000230: 6f64 656c 2e6d 6574 6164 6174 6120 696d  odel.metadata im
-00000240: 706f 7274 204d 6574 6164 6174 610d 0a0d  port Metadata...
-00000250: 0a66 726f 6d20 7365 6d61 6e74 6861 5f73  .from semantha_s
-00000260: 646b 2e6d 6f64 656c 2e73 696d 706c 655f  dk.model.simple_
-00000270: 7072 6f70 6572 7479 2069 6d70 6f72 7420  property import 
-00000280: 5369 6d70 6c65 5072 6f70 6572 7479 0d0a  SimpleProperty..
-00000290: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
-000002a0: 706f 7274 204c 6973 740d 0a66 726f 6d20  port List..from 
-000002b0: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
-000002c0: 7469 6f6e 616c 0d0a 0d0a 4064 6174 6163  tional....@datac
-000002d0: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
-000002e0: 290d 0a63 6c61 7373 204d 6f64 656c 496e  )..class ModelIn
-000002f0: 7374 616e 6365 2853 656d 616e 7468 614d  stance(SemanthaM
-00000300: 6f64 656c 456e 7469 7479 293a 0d0a 2020  odelEntity):..  
-00000310: 2020 2222 2220 6175 7468 6f72 2073 656d    """ author sem
-00000320: 616e 7468 612c 2074 6869 7320 6973 2061  antha, this is a
-00000330: 2067 656e 6572 6174 6564 2063 6c61 7373   generated class
-00000340: 2064 6f20 6e6f 7420 6368 616e 6765 206d   do not change m
-00000350: 616e 7561 6c6c 7921 2022 2222 0d0a 2020  anually! """..  
-00000360: 2020 6964 3a20 4f70 7469 6f6e 616c 5b73    id: Optional[s
-00000370: 7472 5d0d 0a20 2020 206e 616d 653a 204f  tr]..    name: O
-00000380: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-00000390: 2020 636c 6173 735f 6964 3a20 7374 720d    class_id: str.
-000003a0: 0a20 2020 2072 656c 6174 696f 6e5f 6964  .    relation_id
-000003b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000003c0: 0a20 2020 2074 7970 653a 204f 7074 696f  .    type: Optio
-000003d0: 6e61 6c5b 7374 725d 0d0a 2020 2020 6967  nal[str]..    ig
-000003e0: 6e6f 7265 5f69 6d70 6f72 743a 204f 7074  nore_import: Opt
-000003f0: 696f 6e61 6c5b 626f 6f6c 5d0d 0a20 2020  ional[bool]..   
-00000400: 2073 696d 706c 655f 7072 6f70 6572 7469   simple_properti
-00000410: 6573 3a20 4f70 7469 6f6e 616c 5b4c 6973  es: Optional[Lis
-00000420: 745b 5369 6d70 6c65 5072 6f70 6572 7479  t[SimpleProperty
-00000430: 5d5d 0d0a 2020 2020 6d65 7461 6461 7461  ]]..    metadata
-00000440: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00000450: 4d65 7461 6461 7461 5d5d 0d0a 2020 2020  Metadata]]..    
-00000460: 7175 616c 6966 6965 645f 6e61 6d65 3a20  qualified_name: 
-00000470: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000480: 2020 2065 7874 7261 6374 6f72 5f63 6c61     extractor_cla
-00000490: 7373 5f69 6473 3a20 4f70 7469 6f6e 616c  ss_ids: Optional
-000004a0: 5b4c 6973 745b 7374 725d 5d0d 0a20 2020  [List[str]]..   
-000004b0: 206c 6162 656c 3a20 4f70 7469 6f6e 616c   label: Optional
-000004c0: 5b73 7472 5d0d 0a20 2020 206c 6162 656c  [str]..    label
-000004d0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-000004e0: 5b4c 6162 656c 5d5d 0d0a 2020 2020 6669  [Label]]..    fi
-000004f0: 6c65 3a20 4f70 7469 6f6e 616c 5b46 696c  le: Optional[Fil
-00000500: 6552 6566 6572 656e 6365 5d0d 0a20 2020  eReference]..   
-00000510: 2063 6f6d 706c 6578 5f70 726f 7065 7274   complex_propert
-00000520: 6965 733a 204f 7074 696f 6e61 6c5b 4c69  ies: Optional[Li
-00000530: 7374 5b43 6f6d 706c 6578 5072 6f70 6572  st[ComplexProper
-00000540: 7479 5d5d 0d0a 2020 2020 6669 6e64 696e  ty]]..    findin
-00000550: 6773 3a20 4f70 7469 6f6e 616c 5b4c 6973  gs: Optional[Lis
-00000560: 745b 4669 6e64 696e 675d 5d0d 0a20 2020  t[Finding]]..   
-00000570: 2072 6566 6572 656e 6365 733a 204f 7074   references: Opt
-00000580: 696f 6e61 6c5b 4c69 7374 5b45 7874 7261  ional[List[Extra
-00000590: 6374 696f 6e52 6566 6572 656e 6365 5d5d  ctionReference]]
-000005a0: 0d0a 2020 2020 6c69 6e6b 6564 5f69 6e73  ..    linked_ins
-000005b0: 7461 6e63 6573 3a20 4f70 7469 6f6e 616c  tances: Optional
-000005c0: 5b4c 6973 745b 4c69 6e6b 6564 496e 7374  [List[LinkedInst
-000005d0: 616e 6365 5d5d 0d0a 0d0a 4d6f 6465 6c49  ance]]....ModelI
-000005e0: 6e73 7461 6e63 6553 6368 656d 6120 3d20  nstanceSchema = 
-000005f0: 636c 6173 735f 7363 6865 6d61 284d 6f64  class_schema(Mod
-00000600: 656c 496e 7374 616e 6365 2c20 6261 7365  elInstance, base
-00000610: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
-00000620: 5363 6865 6d61 290d 0a                   Schema)..
+000000f0: 6672 6f6d 2073 656d 616e 7468 615f 7364  from semantha_sd
+00000100: 6b2e 6d6f 6465 6c2e 6578 7472 6163 7469  k.model.extracti
+00000110: 6f6e 5f72 6566 6572 656e 6365 2069 6d70  on_reference imp
+00000120: 6f72 7420 4578 7472 6163 7469 6f6e 5265  ort ExtractionRe
+00000130: 6665 7265 6e63 650d 0a66 726f 6d20 7365  ference..from se
+00000140: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000150: 2e66 696c 655f 7265 6665 7265 6e63 6520  .file_reference 
+00000160: 696d 706f 7274 2046 696c 6552 6566 6572  import FileRefer
+00000170: 656e 6365 0d0a 6672 6f6d 2073 656d 616e  ence..from seman
+00000180: 7468 615f 7364 6b2e 6d6f 6465 6c2e 6669  tha_sdk.model.fi
+00000190: 6e64 696e 6720 696d 706f 7274 2046 696e  nding import Fin
+000001a0: 6469 6e67 0d0a 6672 6f6d 2073 656d 616e  ding..from seman
+000001b0: 7468 615f 7364 6b2e 6d6f 6465 6c2e 6c61  tha_sdk.model.la
+000001c0: 6265 6c20 696d 706f 7274 204c 6162 656c  bel import Label
+000001d0: 0d0a 6672 6f6d 2073 656d 616e 7468 615f  ..from semantha_
+000001e0: 7364 6b2e 6d6f 6465 6c2e 6c69 6e6b 6564  sdk.model.linked
+000001f0: 5f69 6e73 7461 6e63 6520 696d 706f 7274  _instance import
+00000200: 204c 696e 6b65 6449 6e73 7461 6e63 650d   LinkedInstance.
+00000210: 0a66 726f 6d20 7365 6d61 6e74 6861 5f73  .from semantha_s
+00000220: 646b 2e6d 6f64 656c 2e6d 6574 6164 6174  dk.model.metadat
+00000230: 6120 696d 706f 7274 204d 6574 6164 6174  a import Metadat
+00000240: 610d 0a66 726f 6d20 7365 6d61 6e74 6861  a..from semantha
+00000250: 5f73 646b 2e6d 6f64 656c 2e73 696d 706c  _sdk.model.simpl
+00000260: 655f 7072 6f70 6572 7479 2069 6d70 6f72  e_property impor
+00000270: 7420 5369 6d70 6c65 5072 6f70 6572 7479  t SimpleProperty
+00000280: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
+00000290: 706f 7274 204c 6973 740d 0a66 726f 6d20  port List..from 
+000002a0: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
+000002b0: 7469 6f6e 616c 0d0a 0d0a 0d0a 4064 6174  tional......@dat
+000002c0: 6163 6c61 7373 2866 726f 7a65 6e3d 5472  aclass(frozen=Tr
+000002d0: 7565 290d 0a63 6c61 7373 204d 6f64 656c  ue)..class Model
+000002e0: 496e 7374 616e 6365 2853 656d 616e 7468  Instance(Semanth
+000002f0: 614d 6f64 656c 456e 7469 7479 293a 0d0a  aModelEntity):..
+00000300: 2020 2020 2222 2220 6175 7468 6f72 2073      """ author s
+00000310: 656d 616e 7468 612c 2074 6869 7320 6973  emantha, this is
+00000320: 2061 2067 656e 6572 6174 6564 2063 6c61   a generated cla
+00000330: 7373 2064 6f20 6e6f 7420 6368 616e 6765  ss do not change
+00000340: 206d 616e 7561 6c6c 7921 2022 2222 0d0a   manually! """..
+00000350: 2020 2020 6964 3a20 4f70 7469 6f6e 616c      id: Optional
+00000360: 5b73 7472 5d0d 0a20 2020 206e 616d 653a  [str]..    name:
+00000370: 2073 7472 0d0a 2020 2020 636c 6173 735f   str..    class_
+00000380: 6964 3a20 7374 720d 0a20 2020 2072 656c  id: str..    rel
+00000390: 6174 696f 6e5f 6964 3a20 4f70 7469 6f6e  ation_id: Option
+000003a0: 616c 5b73 7472 5d0d 0a20 2020 2074 7970  al[str]..    typ
+000003b0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+000003c0: 0d0a 2020 2020 6967 6e6f 7265 5f69 6d70  ..    ignore_imp
+000003d0: 6f72 743a 204f 7074 696f 6e61 6c5b 626f  ort: Optional[bo
+000003e0: 6f6c 5d0d 0a20 2020 2073 696d 706c 655f  ol]..    simple_
+000003f0: 7072 6f70 6572 7469 6573 3a20 4f70 7469  properties: Opti
+00000400: 6f6e 616c 5b4c 6973 745b 5369 6d70 6c65  onal[List[Simple
+00000410: 5072 6f70 6572 7479 5d5d 0d0a 2020 2020  Property]]..    
+00000420: 6d65 7461 6461 7461 3a20 4f70 7469 6f6e  metadata: Option
+00000430: 616c 5b4c 6973 745b 4d65 7461 6461 7461  al[List[Metadata
+00000440: 5d5d 0d0a 2020 2020 7175 616c 6966 6965  ]]..    qualifie
+00000450: 645f 6e61 6d65 3a20 4f70 7469 6f6e 616c  d_name: Optional
+00000460: 5b73 7472 5d0d 0a20 2020 2065 7874 7261  [str]..    extra
+00000470: 6374 6f72 5f63 6c61 7373 5f69 6473 3a20  ctor_class_ids: 
+00000480: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+00000490: 725d 5d0d 0a20 2020 206c 6162 656c 3a20  r]]..    label: 
+000004a0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+000004b0: 2020 206c 6162 656c 733a 204f 7074 696f     labels: Optio
+000004c0: 6e61 6c5b 4c69 7374 5b4c 6162 656c 5d5d  nal[List[Label]]
+000004d0: 0d0a 2020 2020 6669 6c65 3a20 4f70 7469  ..    file: Opti
+000004e0: 6f6e 616c 5b46 696c 6552 6566 6572 656e  onal[FileReferen
+000004f0: 6365 5d0d 0a20 2020 2063 6f6d 706c 6578  ce]..    complex
+00000500: 5f70 726f 7065 7274 6965 733a 204f 7074  _properties: Opt
+00000510: 696f 6e61 6c5b 4c69 7374 5b43 6f6d 706c  ional[List[Compl
+00000520: 6578 5072 6f70 6572 7479 5d5d 0d0a 2020  exProperty]]..  
+00000530: 2020 6669 6e64 696e 6773 3a20 4f70 7469    findings: Opti
+00000540: 6f6e 616c 5b4c 6973 745b 4669 6e64 696e  onal[List[Findin
+00000550: 675d 5d0d 0a20 2020 2072 6566 6572 656e  g]]..    referen
+00000560: 6365 733a 204f 7074 696f 6e61 6c5b 4c69  ces: Optional[Li
+00000570: 7374 5b45 7874 7261 6374 696f 6e52 6566  st[ExtractionRef
+00000580: 6572 656e 6365 5d5d 0d0a 2020 2020 6c69  erence]]..    li
+00000590: 6e6b 6564 5f69 6e73 7461 6e63 6573 3a20  nked_instances: 
+000005a0: 4f70 7469 6f6e 616c 5b4c 6973 745b 4c69  Optional[List[Li
+000005b0: 6e6b 6564 496e 7374 616e 6365 5d5d 0d0a  nkedInstance]]..
+000005c0: 0d0a 4d6f 6465 6c49 6e73 7461 6e63 6553  ..ModelInstanceS
+000005d0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
+000005e0: 6865 6d61 284d 6f64 656c 496e 7374 616e  hema(ModelInstan
+000005f0: 6365 2c20 6261 7365 5f73 6368 656d 613d  ce, base_schema=
+00000600: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+00000610: 0a                                       .
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/page.py` & `semantha_sdk-5.6.0/semantha_sdk/model/page.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.annotation_page import AnnotationPage
-
 from semantha_sdk.model.document_table import DocumentTable
-
 from semantha_sdk.model.page_content import PageContent
-
 from semantha_sdk.model.paragraph import Paragraph
-
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class Page(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     contents: Optional[List[PageContent]]
     paragraphs: Optional[List[Paragraph]]
     tables: Optional[List[DocumentTable]]
     annotation_page: Optional[AnnotationPage]
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/page_content.py` & `semantha_sdk-5.6.0/semantha_sdk/model/page_content.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.paragraph import Paragraph
-
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class PageContent(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     paragraphs: Optional[List[Paragraph]]
 
 PageContentSchema = class_schema(PageContent, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/paragraph.py` & `semantha_sdk-5.6.0/semantha_sdk/model/paragraph.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,59 +7,58 @@
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e72 6563 7420 696d 706f  .model.rect impo
-000000d0: 7274 2052 6563 740d 0a0d 0a66 726f 6d20  rt Rect....from 
-000000e0: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
-000000f0: 656c 2e72 6566 6572 656e 6365 2069 6d70  el.reference imp
-00000100: 6f72 7420 5265 6665 7265 6e63 650d 0a0d  ort Reference...
-00000110: 0a66 726f 6d20 7365 6d61 6e74 6861 5f73  .from semantha_s
-00000120: 646b 2e6d 6f64 656c 2e73 656e 7465 6e63  dk.model.sentenc
-00000130: 6520 696d 706f 7274 2053 656e 7465 6e63  e import Sentenc
-00000140: 650d 0a0d 0a66 726f 6d20 7479 7069 6e67  e....from typing
-00000150: 2069 6d70 6f72 7420 4469 6374 0d0a 6672   import Dict..fr
-00000160: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000170: 204c 6973 740d 0a66 726f 6d20 7479 7069   List..from typi
-00000180: 6e67 2069 6d70 6f72 7420 4f70 7469 6f6e  ng import Option
-00000190: 616c 0d0a 0d0a 4064 6174 6163 6c61 7373  al....@dataclass
-000001a0: 2866 726f 7a65 6e3d 5472 7565 290d 0a63  (frozen=True)..c
-000001b0: 6c61 7373 2050 6172 6167 7261 7068 2853  lass Paragraph(S
-000001c0: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
-000001d0: 7479 293a 0d0a 2020 2020 2222 2220 6175  ty):..    """ au
-000001e0: 7468 6f72 2073 656d 616e 7468 612c 2074  thor semantha, t
-000001f0: 6869 7320 6973 2061 2067 656e 6572 6174  his is a generat
-00000200: 6564 2063 6c61 7373 2064 6f20 6e6f 7420  ed class do not 
-00000210: 6368 616e 6765 206d 616e 7561 6c6c 7921  change manually!
-00000220: 2022 2222 0d0a 2020 2020 7465 7874 3a20   """..    text: 
-00000230: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000240: 2020 2074 7970 653a 204f 7074 696f 6e61     type: Optiona
-00000250: 6c5b 7374 725d 0d0a 2020 2020 6964 3a20  l[str]..    id: 
-00000260: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-00000270: 2020 2064 6f63 756d 656e 745f 6e61 6d65     document_name
-00000280: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-00000290: 0a20 2020 2073 656e 7465 6e63 6573 3a20  .    sentences: 
-000002a0: 4f70 7469 6f6e 616c 5b4c 6973 745b 5365  Optional[List[Se
-000002b0: 6e74 656e 6365 5d5d 0d0a 2020 2020 7265  ntence]]..    re
-000002c0: 6665 7265 6e63 6573 3a20 4f70 7469 6f6e  ferences: Option
-000002d0: 616c 5b4c 6973 745b 5265 6665 7265 6e63  al[List[Referenc
-000002e0: 655d 5d0d 0a20 2020 2063 6f6e 7465 7874  e]]..    context
-000002f0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-00000300: 7374 722c 2073 7472 5d5d 0d0a 2020 2020  str, str]]..    
-00000310: 6172 6561 733a 204f 7074 696f 6e61 6c5b  areas: Optional[
-00000320: 4c69 7374 5b52 6563 745d 5d0d 0a20 2020  List[Rect]]..   
-00000330: 2063 6f6d 6d65 6e74 3a20 4f70 7469 6f6e   comment: Option
-00000340: 616c 5b73 7472 5d0d 0a20 2020 2076 6572  al[str]..    ver
-00000350: 6966 6965 643a 204f 7074 696f 6e61 6c5b  ified: Optional[
-00000360: 626f 6f6c 5d0d 0a20 2020 2064 6174 615f  bool]..    data_
-00000370: 7572 6c5f 696d 6167 653a 204f 7074 696f  url_image: Optio
-00000380: 6e61 6c5b 7374 725d 0d0a 2020 2020 7265  nal[str]..    re
-00000390: 6665 7265 6e63 6573 5f73 6166 653a 204f  ferences_safe: O
-000003a0: 7074 696f 6e61 6c5b 4c69 7374 5b52 6566  ptional[List[Ref
-000003b0: 6572 656e 6365 5d5d 0d0a 0d0a 5061 7261  erence]]....Para
-000003c0: 6772 6170 6853 6368 656d 6120 3d20 636c  graphSchema = cl
-000003d0: 6173 735f 7363 6865 6d61 2850 6172 6167  ass_schema(Parag
-000003e0: 7261 7068 2c20 6261 7365 5f73 6368 656d  raph, base_schem
-000003f0: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000400: 290d 0a                                  )..
+000000d0: 7274 2052 6563 740d 0a66 726f 6d20 7365  rt Rect..from se
+000000e0: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+000000f0: 2e72 6566 6572 656e 6365 2069 6d70 6f72  .reference impor
+00000100: 7420 5265 6665 7265 6e63 650d 0a66 726f  t Reference..fro
+00000110: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
+00000120: 6f64 656c 2e73 656e 7465 6e63 6520 696d  odel.sentence im
+00000130: 706f 7274 2053 656e 7465 6e63 650d 0a66  port Sentence..f
+00000140: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+00000150: 7420 4469 6374 0d0a 6672 6f6d 2074 7970  t Dict..from typ
+00000160: 696e 6720 696d 706f 7274 204c 6973 740d  ing import List.
+00000170: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+00000180: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
+00000190: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
+000001a0: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
+000001b0: 2050 6172 6167 7261 7068 2853 656d 616e   Paragraph(Seman
+000001c0: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
+000001d0: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
+000001e0: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
+000001f0: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
+00000200: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
+00000210: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
+00000220: 0d0a 2020 2020 7465 7874 3a20 4f70 7469  ..    text: Opti
+00000230: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2074  onal[str]..    t
+00000240: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
+00000250: 725d 0d0a 2020 2020 6964 3a20 4f70 7469  r]..    id: Opti
+00000260: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2064  onal[str]..    d
+00000270: 6f63 756d 656e 745f 6e61 6d65 3a20 4f70  ocument_name: Op
+00000280: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000290: 2073 656e 7465 6e63 6573 3a20 4f70 7469   sentences: Opti
+000002a0: 6f6e 616c 5b4c 6973 745b 5365 6e74 656e  onal[List[Senten
+000002b0: 6365 5d5d 0d0a 2020 2020 7265 6665 7265  ce]]..    refere
+000002c0: 6e63 6573 3a20 4f70 7469 6f6e 616c 5b4c  nces: Optional[L
+000002d0: 6973 745b 5265 6665 7265 6e63 655d 5d0d  ist[Reference]].
+000002e0: 0a20 2020 2063 6f6e 7465 7874 3a20 4f70  .    context: Op
+000002f0: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00000300: 2073 7472 5d5d 0d0a 2020 2020 6172 6561   str]]..    area
+00000310: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+00000320: 5b52 6563 745d 5d0d 0a20 2020 2063 6f6d  [Rect]]..    com
+00000330: 6d65 6e74 3a20 4f70 7469 6f6e 616c 5b73  ment: Optional[s
+00000340: 7472 5d0d 0a20 2020 2076 6572 6966 6965  tr]..    verifie
+00000350: 643a 204f 7074 696f 6e61 6c5b 626f 6f6c  d: Optional[bool
+00000360: 5d0d 0a20 2020 2064 6174 615f 7572 6c5f  ]..    data_url_
+00000370: 696d 6167 653a 204f 7074 696f 6e61 6c5b  image: Optional[
+00000380: 7374 725d 0d0a 2020 2020 7265 6665 7265  str]..    refere
+00000390: 6e63 6573 5f73 6166 653a 204f 7074 696f  nces_safe: Optio
+000003a0: 6e61 6c5b 4c69 7374 5b52 6566 6572 656e  nal[List[Referen
+000003b0: 6365 5d5d 0d0a 0d0a 5061 7261 6772 6170  ce]]....Paragrap
+000003c0: 6853 6368 656d 6120 3d20 636c 6173 735f  hSchema = class_
+000003d0: 7363 6865 6d61 2850 6172 6167 7261 7068  schema(Paragraph
+000003e0: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+000003f0: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/plotly_chart.py` & `semantha_sdk-5.6.0/semantha_sdk/model/plotly_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from typing import Any
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class PlotlyChart(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     data: Optional[List[Any]]
     layout: Optional[Any]
 
 PlotlyChartSchema = class_schema(PlotlyChart, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/process_information.py` & `semantha_sdk-5.6.0/semantha_sdk/model/rule_overview.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
-000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e76 6572 7369 6f6e 2069  .model.version i
-000000d0: 6d70 6f72 7420 5665 7273 696f 6e0d 0a0d  mport Version...
-000000e0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-000000f0: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
-00000100: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-00000110: 6e3d 5472 7565 290d 0a63 6c61 7373 2050  n=True)..class P
-00000120: 726f 6365 7373 496e 666f 726d 6174 696f  rocessInformatio
-00000130: 6e28 5365 6d61 6e74 6861 4d6f 6465 6c45  n(SemanthaModelE
-00000140: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
-00000150: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
-00000160: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
-00000170: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
-00000180: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
-00000190: 6c79 2120 2222 220d 0a20 2020 2063 7265  ly! """..    cre
-000001a0: 6174 6564 3a20 4f70 7469 6f6e 616c 5b73  ated: Optional[s
-000001b0: 7472 5d0d 0a20 2020 2065 6469 7465 643a  tr]..    edited:
-000001c0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-000001d0: 2020 2020 7665 7273 696f 6e3a 204f 7074      version: Opt
-000001e0: 696f 6e61 6c5b 5665 7273 696f 6e5d 0d0a  ional[Version]..
-000001f0: 0d0a 5072 6f63 6573 7349 6e66 6f72 6d61  ..ProcessInforma
-00000200: 7469 6f6e 5363 6865 6d61 203d 2063 6c61  tionSchema = cla
-00000210: 7373 5f73 6368 656d 6128 5072 6f63 6573  ss_schema(Proces
-00000220: 7349 6e66 6f72 6d61 7469 6f6e 2c20 6261  sInformation, ba
-00000230: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
-00000240: 6861 5363 6865 6d61 290d 0a              haSchema)..
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000100: 0d0a 636c 6173 7320 5275 6c65 4f76 6572  ..class RuleOver
+00000110: 7669 6577 2853 656d 616e 7468 614d 6f64  view(SemanthaMod
+00000120: 656c 456e 7469 7479 293a 0d0a 2020 2020  elEntity):..    
+00000130: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
+00000140: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
+00000150: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
+00000160: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
+00000170: 7561 6c6c 7921 2022 2222 0d0a 2020 2020  ually! """..    
+00000180: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
+00000190: 5d0d 0a20 2020 206e 616d 653a 2073 7472  ]..    name: str
+000001a0: 0d0a 2020 2020 7265 6164 5f6f 6e6c 793a  ..    read_only:
+000001b0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
+000001c0: 0a20 2020 2072 756c 655f 7374 7269 6e67  .    rule_string
+000001d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+000001e0: 0a20 2020 2074 6167 733a 204f 7074 696f  .    tags: Optio
+000001f0: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 0d0a  nal[List[str]]..
+00000200: 0d0a 5275 6c65 4f76 6572 7669 6577 5363  ..RuleOverviewSc
+00000210: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+00000220: 656d 6128 5275 6c65 4f76 6572 7669 6577  ema(RuleOverview
+00000230: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+00000240: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/reference.py` & `semantha_sdk-5.6.0/semantha_sdk/model/reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,45 +8,45 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4469 6374 0d0a 6672 6f6d 2074 7970  t Dict..from typ
 000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-000000e0: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
-000000f0: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
-00000100: 636c 6173 7320 5265 6665 7265 6e63 6528  class Reference(
-00000110: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
-00000120: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
-00000130: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
-00000140: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
-00000150: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
-00000160: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
-00000170: 2120 2222 220d 0a20 2020 2064 6f63 756d  ! """..    docum
-00000180: 656e 745f 6964 3a20 4f70 7469 6f6e 616c  ent_id: Optional
-00000190: 5b73 7472 5d0d 0a20 2020 2064 6f63 756d  [str]..    docum
-000001a0: 656e 745f 6e61 6d65 3a20 4f70 7469 6f6e  ent_name: Option
-000001b0: 616c 5b73 7472 5d0d 0a20 2020 2070 6167  al[str]..    pag
-000001c0: 655f 6e75 6d62 6572 3a20 4f70 7469 6f6e  e_number: Option
-000001d0: 616c 5b69 6e74 5d0d 0a20 2020 2070 6172  al[int]..    par
-000001e0: 6167 7261 7068 5f69 643a 204f 7074 696f  agraph_id: Optio
-000001f0: 6e61 6c5b 7374 725d 0d0a 2020 2020 7365  nal[str]..    se
-00000200: 6e74 656e 6365 5f69 643a 204f 7074 696f  ntence_id: Optio
-00000210: 6e61 6c5b 7374 725d 0d0a 2020 2020 7369  nal[str]..    si
-00000220: 6d69 6c61 7269 7479 3a20 4f70 7469 6f6e  milarity: Option
-00000230: 616c 5b66 6c6f 6174 5d0d 0a20 2020 2074  al[float]..    t
-00000240: 6578 743a 204f 7074 696f 6e61 6c5b 7374  ext: Optional[st
-00000250: 725d 0d0a 2020 2020 636f 6e74 6578 743a  r]..    context:
-00000260: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
-00000270: 7472 2c20 7374 725d 5d0d 0a20 2020 2074  tr, str]]..    t
-00000280: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
-00000290: 725d 0d0a 2020 2020 636f 6c6f 723a 204f  r]..    color: O
-000002a0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
-000002b0: 2020 636f 6d6d 656e 743a 204f 7074 696f    comment: Optio
-000002c0: 6e61 6c5b 7374 725d 0d0a 2020 2020 6861  nal[str]..    ha
-000002d0: 735f 6f70 706f 7369 7465 5f6d 6561 6e69  s_opposite_meani
-000002e0: 6e67 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ng: Optional[boo
-000002f0: 6c5d 0d0a 0d0a 5265 6665 7265 6e63 6553  l]....ReferenceS
-00000300: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
-00000310: 6865 6d61 2852 6566 6572 656e 6365 2c20  hema(Reference, 
-00000320: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
-00000330: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
+000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000100: 0d0a 636c 6173 7320 5265 6665 7265 6e63  ..class Referenc
+00000110: 6528 5365 6d61 6e74 6861 4d6f 6465 6c45  e(SemanthaModelE
+00000120: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
+00000130: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
+00000140: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
+00000150: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
+00000160: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
+00000170: 6c79 2120 2222 220d 0a20 2020 2064 6f63  ly! """..    doc
+00000180: 756d 656e 745f 6964 3a20 4f70 7469 6f6e  ument_id: Option
+00000190: 616c 5b73 7472 5d0d 0a20 2020 2064 6f63  al[str]..    doc
+000001a0: 756d 656e 745f 6e61 6d65 3a20 4f70 7469  ument_name: Opti
+000001b0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2070  onal[str]..    p
+000001c0: 6167 655f 6e75 6d62 6572 3a20 4f70 7469  age_number: Opti
+000001d0: 6f6e 616c 5b69 6e74 5d0d 0a20 2020 2070  onal[int]..    p
+000001e0: 6172 6167 7261 7068 5f69 643a 204f 7074  aragraph_id: Opt
+000001f0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+00000200: 7365 6e74 656e 6365 5f69 643a 204f 7074  sentence_id: Opt
+00000210: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+00000220: 7369 6d69 6c61 7269 7479 3a20 4f70 7469  similarity: Opti
+00000230: 6f6e 616c 5b66 6c6f 6174 5d0d 0a20 2020  onal[float]..   
+00000240: 2074 6578 743a 204f 7074 696f 6e61 6c5b   text: Optional[
+00000250: 7374 725d 0d0a 2020 2020 636f 6e74 6578  str]..    contex
+00000260: 743a 204f 7074 696f 6e61 6c5b 4469 6374  t: Optional[Dict
+00000270: 5b73 7472 2c20 7374 725d 5d0d 0a20 2020  [str, str]]..   
+00000280: 2074 7970 653a 204f 7074 696f 6e61 6c5b   type: Optional[
+00000290: 7374 725d 0d0a 2020 2020 636f 6c6f 723a  str]..    color:
+000002a0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
+000002b0: 2020 2020 636f 6d6d 656e 743a 204f 7074      comment: Opt
+000002c0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+000002d0: 6861 735f 6f70 706f 7369 7465 5f6d 6561  has_opposite_mea
+000002e0: 6e69 6e67 3a20 4f70 7469 6f6e 616c 5b62  ning: Optional[b
+000002f0: 6f6f 6c5d 0d0a 0d0a 5265 6665 7265 6e63  ool]....Referenc
+00000300: 6553 6368 656d 6120 3d20 636c 6173 735f  eSchema = class_
+00000310: 7363 6865 6d61 2852 6566 6572 656e 6365  schema(Reference
+00000320: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+00000330: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/reference_documents_response_container.py` & `semantha_sdk-5.6.0/semantha_sdk/model/reference_documents_response_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.document_information import DocumentInformation
-
 from semantha_sdk.model.response_meta_info import ResponseMetaInfo
-
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class ReferenceDocumentsResponseContainer(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     meta: Optional[ResponseMetaInfo]
     data: Optional[List[DocumentInformation]]
 
 ReferenceDocumentsResponseContainerSchema = class_schema(ReferenceDocumentsResponseContainer, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/response_meta_info.py` & `semantha_sdk-5.6.0/semantha_sdk/model/response_meta_info.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.meta_info_page import MetaInfoPage
-
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class ResponseMetaInfo(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     info: Optional[str]
     parameters: Optional[Dict[str, Any]]
     warnings: Optional[List[str]]
     page: Optional[MetaInfoPage]
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/row.py` & `semantha_sdk-5.6.0/semantha_sdk/model/row.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.table_cell import TableCell
-
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class Row(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     cells: Optional[List[TableCell]]
 
 RowSchema = class_schema(Row, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/semantha_entity.py` & `semantha_sdk-5.6.0/semantha_sdk/model/semantha_entity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/semantic_model.py` & `semantha_sdk-5.6.0/semantha_sdk/model/semantic_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.extraction_file import ExtractionFile
-
 from semantha_sdk.model.model_instance import ModelInstance
-
 from semantha_sdk.model.process_information import ProcessInformation
-
 from semantha_sdk.model.table_instance import TableInstance
-
 from typing import List
 from typing import Optional
 
+
 @dataclass(frozen=True)
 class SemanticModel(SemanthaModelEntity):
     """ author semantha, this is a generated class do not change manually! """
     files: Optional[List[ExtractionFile]]
     instances: Optional[List[ModelInstance]]
     tables: Optional[List[TableInstance]]
     process_information: Optional[ProcessInformation]
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/semi_super_vised_document.py` & `semantha_sdk-5.6.0/semantha_sdk/model/semi_super_vised_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2053 656d  True)..class Sem
-000000f0: 6953 7570 6572 5669 7365 6444 6f63 756d  iSuperVisedDocum
-00000100: 656e 7428 5365 6d61 6e74 6861 4d6f 6465  ent(SemanthaMode
-00000110: 6c45 6e74 6974 7929 3a0d 0a20 2020 2022  lEntity):..    "
-00000120: 2222 2061 7574 686f 7220 7365 6d61 6e74  "" author semant
-00000130: 6861 2c20 7468 6973 2069 7320 6120 6765  ha, this is a ge
-00000140: 6e65 7261 7465 6420 636c 6173 7320 646f  nerated class do
-00000150: 206e 6f74 2063 6861 6e67 6520 6d61 6e75   not change manu
-00000160: 616c 6c79 2120 2222 220d 0a20 2020 2064  ally! """..    d
-00000170: 6f63 756d 656e 745f 6964 3a20 4f70 7469  ocument_id: Opti
-00000180: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2074  onal[str]..    t
-00000190: 6f70 6963 5f69 643a 204f 7074 696f 6e61  opic_id: Optiona
-000001a0: 6c5b 696e 745d 0d0a 0d0a 5365 6d69 5375  l[int]....SemiSu
-000001b0: 7065 7256 6973 6564 446f 6375 6d65 6e74  perVisedDocument
-000001c0: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
-000001d0: 6368 656d 6128 5365 6d69 5375 7065 7256  chema(SemiSuperV
-000001e0: 6973 6564 446f 6375 6d65 6e74 2c20 6261  isedDocument, ba
-000001f0: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
-00000200: 6861 5363 6865 6d61 290d 0a              haSchema)..
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2053  n=True)..class S
+000000f0: 656d 6953 7570 6572 5669 7365 6444 6f63  emiSuperVisedDoc
+00000100: 756d 656e 7428 5365 6d61 6e74 6861 4d6f  ument(SemanthaMo
+00000110: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
+00000120: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
+00000130: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
+00000140: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
+00000150: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
+00000160: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
+00000170: 2064 6f63 756d 656e 745f 6964 3a20 4f70   document_id: Op
+00000180: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000190: 2074 6f70 6963 5f69 643a 204f 7074 696f   topic_id: Optio
+000001a0: 6e61 6c5b 696e 745d 0d0a 0d0a 5365 6d69  nal[int]....Semi
+000001b0: 5375 7065 7256 6973 6564 446f 6375 6d65  SuperVisedDocume
+000001c0: 6e74 5363 6865 6d61 203d 2063 6c61 7373  ntSchema = class
+000001d0: 5f73 6368 656d 6128 5365 6d69 5375 7065  _schema(SemiSupe
+000001e0: 7256 6973 6564 446f 6375 6d65 6e74 2c20  rVisedDocument, 
+000001f0: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
+00000200: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/sentence.py` & `semantha_sdk-5.6.0/semantha_sdk/model/sentence.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,45 +9,44 @@
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e64 6f63 756d 656e 745f  .model.document_
 000000d0: 6e61 6d65 645f 656e 7469 7479 2069 6d70  named_entity imp
 000000e0: 6f72 7420 446f 6375 6d65 6e74 4e61 6d65  ort DocumentName
-000000f0: 6445 6e74 6974 790d 0a0d 0a66 726f 6d20  dEntity....from 
-00000100: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
-00000110: 656c 2e72 6563 7420 696d 706f 7274 2052  el.rect import R
-00000120: 6563 740d 0a0d 0a66 726f 6d20 7365 6d61  ect....from sema
-00000130: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e72  ntha_sdk.model.r
-00000140: 6566 6572 656e 6365 2069 6d70 6f72 7420  eference import 
-00000150: 5265 6665 7265 6e63 650d 0a0d 0a66 726f  Reference....fro
-00000160: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-00000170: 4c69 7374 0d0a 6672 6f6d 2074 7970 696e  List..from typin
-00000180: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
-00000190: 6c0d 0a0d 0a40 6461 7461 636c 6173 7328  l....@dataclass(
-000001a0: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
-000001b0: 6173 7320 5365 6e74 656e 6365 2853 656d  ass Sentence(Sem
-000001c0: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-000001d0: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
-000001e0: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
-000001f0: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
-00000200: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
-00000210: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
-00000220: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
-00000230: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2074  onal[str]..    t
-00000240: 6578 743a 204f 7074 696f 6e61 6c5b 7374  ext: Optional[st
-00000250: 725d 0d0a 2020 2020 646f 6375 6d65 6e74  r]..    document
-00000260: 5f6e 616d 653a 204f 7074 696f 6e61 6c5b  _name: Optional[
-00000270: 7374 725d 0d0a 2020 2020 6e61 6d65 645f  str]..    named_
-00000280: 656e 7469 7469 6573 3a20 4f70 7469 6f6e  entities: Option
-00000290: 616c 5b4c 6973 745b 446f 6375 6d65 6e74  al[List[Document
-000002a0: 4e61 6d65 6445 6e74 6974 795d 5d0d 0a20  NamedEntity]].. 
-000002b0: 2020 2072 6566 6572 656e 6365 733a 204f     references: O
-000002c0: 7074 696f 6e61 6c5b 4c69 7374 5b52 6566  ptional[List[Ref
-000002d0: 6572 656e 6365 5d5d 0d0a 2020 2020 6172  erence]]..    ar
-000002e0: 6561 733a 204f 7074 696f 6e61 6c5b 4c69  eas: Optional[Li
-000002f0: 7374 5b52 6563 745d 5d0d 0a0d 0a53 656e  st[Rect]]....Sen
-00000300: 7465 6e63 6553 6368 656d 6120 3d20 636c  tenceSchema = cl
-00000310: 6173 735f 7363 6865 6d61 2853 656e 7465  ass_schema(Sente
-00000320: 6e63 652c 2062 6173 655f 7363 6865 6d61  nce, base_schema
-00000330: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
-00000340: 0d0a                                     ..
+000000f0: 6445 6e74 6974 790d 0a66 726f 6d20 7365  dEntity..from se
+00000100: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000110: 2e72 6563 7420 696d 706f 7274 2052 6563  .rect import Rec
+00000120: 740d 0a66 726f 6d20 7365 6d61 6e74 6861  t..from semantha
+00000130: 5f73 646b 2e6d 6f64 656c 2e72 6566 6572  _sdk.model.refer
+00000140: 656e 6365 2069 6d70 6f72 7420 5265 6665  ence import Refe
+00000150: 7265 6e63 650d 0a66 726f 6d20 7479 7069  rence..from typi
+00000160: 6e67 2069 6d70 6f72 7420 4c69 7374 0d0a  ng import List..
+00000170: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000180: 7274 204f 7074 696f 6e61 6c0d 0a0d 0a0d  rt Optional.....
+00000190: 0a40 6461 7461 636c 6173 7328 6672 6f7a  .@dataclass(froz
+000001a0: 656e 3d54 7275 6529 0d0a 636c 6173 7320  en=True)..class 
+000001b0: 5365 6e74 656e 6365 2853 656d 616e 7468  Sentence(Semanth
+000001c0: 614d 6f64 656c 456e 7469 7479 293a 0d0a  aModelEntity):..
+000001d0: 2020 2020 2222 2220 6175 7468 6f72 2073      """ author s
+000001e0: 656d 616e 7468 612c 2074 6869 7320 6973  emantha, this is
+000001f0: 2061 2067 656e 6572 6174 6564 2063 6c61   a generated cla
+00000200: 7373 2064 6f20 6e6f 7420 6368 616e 6765  ss do not change
+00000210: 206d 616e 7561 6c6c 7921 2022 2222 0d0a   manually! """..
+00000220: 2020 2020 6964 3a20 4f70 7469 6f6e 616c      id: Optional
+00000230: 5b73 7472 5d0d 0a20 2020 2074 6578 743a  [str]..    text:
+00000240: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
+00000250: 2020 2020 646f 6375 6d65 6e74 5f6e 616d      document_nam
+00000260: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+00000270: 0d0a 2020 2020 6e61 6d65 645f 656e 7469  ..    named_enti
+00000280: 7469 6573 3a20 4f70 7469 6f6e 616c 5b4c  ties: Optional[L
+00000290: 6973 745b 446f 6375 6d65 6e74 4e61 6d65  ist[DocumentName
+000002a0: 6445 6e74 6974 795d 5d0d 0a20 2020 2072  dEntity]]..    r
+000002b0: 6566 6572 656e 6365 733a 204f 7074 696f  eferences: Optio
+000002c0: 6e61 6c5b 4c69 7374 5b52 6566 6572 656e  nal[List[Referen
+000002d0: 6365 5d5d 0d0a 2020 2020 6172 6561 733a  ce]]..    areas:
+000002e0: 204f 7074 696f 6e61 6c5b 4c69 7374 5b52   Optional[List[R
+000002f0: 6563 745d 5d0d 0a0d 0a53 656e 7465 6e63  ect]]....Sentenc
+00000300: 6553 6368 656d 6120 3d20 636c 6173 735f  eSchema = class_
+00000310: 7363 6865 6d61 2853 656e 7465 6e63 652c  schema(Sentence,
+00000320: 2062 6173 655f 7363 6865 6d61 3d53 656d   base_schema=Sem
+00000330: 616e 7468 6153 6368 656d 6129 0d0a       anthaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/settings.py` & `semantha_sdk-5.6.0/semantha_sdk/model/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,105 +6,105 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2053 6574  True)..class Set
-000000f0: 7469 6e67 7328 5365 6d61 6e74 6861 4d6f  tings(SemanthaMo
-00000100: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
-00000110: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
-00000120: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
-00000130: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
-00000140: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
-00000150: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
-00000160: 2073 696d 696c 6172 6974 795f 6d6f 6465   similarity_mode
-00000170: 6c5f 6964 3a20 4f70 7469 6f6e 616c 5b73  l_id: Optional[s
-00000180: 7472 5d0d 0a20 2020 2073 6d61 7274 5f63  tr]..    smart_c
-00000190: 6c75 7374 6572 5f73 696d 696c 6172 6974  luster_similarit
-000001a0: 795f 6d6f 6465 6c5f 6964 3a20 4f70 7469  y_model_id: Opti
-000001b0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 206b  onal[str]..    k
-000001c0: 6565 705f 6e75 6d62 6572 733a 204f 7074  eep_numbers: Opt
-000001d0: 696f 6e61 6c5b 626f 6f6c 5d0d 0a20 2020  ional[bool]..   
-000001e0: 206d 696e 5f74 6f6b 656e 733a 204f 7074   min_tokens: Opt
-000001f0: 696f 6e61 6c5b 696e 745d 0d0a 2020 2020  ional[int]..    
-00000200: 7369 6d69 6c61 7269 7479 5f6d 6561 7375  similarity_measu
-00000210: 7265 3a20 4f70 7469 6f6e 616c 5b73 7472  re: Optional[str
-00000220: 5d0d 0a20 2020 2063 6f6e 7465 7874 5f77  ]..    context_w
-00000230: 6569 6768 743a 204f 7074 696f 6e61 6c5b  eight: Optional[
-00000240: 666c 6f61 745d 0d0a 2020 2020 656e 6162  float]..    enab
-00000250: 6c65 5f73 7472 696e 675f 636f 6d70 6172  le_string_compar
-00000260: 6973 6f6e 3a20 4f70 7469 6f6e 616c 5b62  ison: Optional[b
-00000270: 6f6f 6c5d 0d0a 2020 2020 6465 6661 756c  ool]..    defaul
-00000280: 745f 646f 6375 6d65 6e74 5f74 7970 653a  t_document_type:
-00000290: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-000002a0: 2020 2020 656e 6162 6c65 5f70 6172 6167      enable_parag
-000002b0: 7261 7068 5f73 6f72 7469 6e67 3a20 4f70  raph_sorting: Op
-000002c0: 7469 6f6e 616c 5b62 6f6f 6c5d 0d0a 2020  tional[bool]..  
-000002d0: 2020 656e 6162 6c65 5f70 6172 6167 7261    enable_paragra
-000002e0: 7068 5f65 6e64 5f64 6574 6563 7469 6f6e  ph_end_detection
-000002f0: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
-00000300: 0d0a 2020 2020 656e 6162 6c65 5f62 6f6f  ..    enable_boo
-00000310: 7374 5f77 6f72 645f 6669 6c74 6572 696e  st_word_filterin
-00000320: 675f 666f 725f 696e 7075 745f 646f 6375  g_for_input_docu
-00000330: 6d65 6e74 733a 204f 7074 696f 6e61 6c5b  ments: Optional[
-00000340: 626f 6f6c 5d0d 0a20 2020 2074 6167 6769  bool]..    taggi
-00000350: 6e67 5f73 696d 696c 6172 6974 795f 6d6f  ng_similarity_mo
-00000360: 6465 3a20 4f70 7469 6f6e 616c 5b73 7472  de: Optional[str
-00000370: 5d0d 0a20 2020 2065 6e61 626c 655f 7570  ]..    enable_up
-00000380: 6461 7469 6e67 5f66 696e 6765 7270 7269  dating_fingerpri
-00000390: 6e74 735f 6f6e 5f74 6167 5f75 7064 6174  nts_on_tag_updat
-000003a0: 6573 3a20 4f70 7469 6f6e 616c 5b62 6f6f  es: Optional[boo
-000003b0: 6c5d 0d0a 2020 2020 656e 6162 6c65 5f70  l]..    enable_p
-000003c0: 6172 6167 7261 7068 5f6d 6572 6769 6e67  aragraph_merging
-000003d0: 5f62 6173 6564 5f6f 6e5f 666f 726d 6174  _based_on_format
-000003e0: 7469 6e67 3a20 4f70 7469 6f6e 616c 5b62  ting: Optional[b
-000003f0: 6f6f 6c5d 0d0a 2020 2020 7573 655f 6372  ool]..    use_cr
-00000400: 6561 7469 6f6e 5f64 6174 655f 6672 6f6d  eation_date_from
-00000410: 5f69 6e70 7574 5f64 6f63 756d 656e 743a  _input_document:
-00000420: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
-00000430: 0a20 2020 2065 6e61 626c 655f 7361 7475  .    enable_satu
-00000440: 7261 7465 645f 6d61 7463 685f 636f 6c6f  rated_match_colo
-00000450: 7273 3a20 4f70 7469 6f6e 616c 5b62 6f6f  rs: Optional[boo
-00000460: 6c5d 0d0a 2020 2020 656e 6162 6c65 5f6e  l]..    enable_n
-00000470: 6f5f 6d61 7463 685f 636f 6c6f 725f 7265  o_match_color_re
-00000480: 643a 204f 7074 696f 6e61 6c5b 626f 6f6c  d: Optional[bool
-00000490: 5d0d 0a20 2020 2065 6e61 626c 655f 636f  ]..    enable_co
-000004a0: 6e74 6578 745f 636f 6e73 6964 6572 6174  ntext_considerat
-000004b0: 696f 6e3a 204f 7074 696f 6e61 6c5b 626f  ion: Optional[bo
-000004c0: 6f6c 5d0d 0a20 2020 2065 6e61 626c 655f  ol]..    enable_
-000004d0: 7061 7261 6772 6170 685f 7265 7369 7a69  paragraph_resizi
-000004e0: 6e67 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ng: Optional[boo
-000004f0: 6c5d 0d0a 2020 2020 7369 6d69 6c61 7269  l]..    similari
-00000500: 7479 5f6d 6174 6368 6572 3a20 4f70 7469  ty_matcher: Opti
-00000510: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2073  onal[str]..    s
-00000520: 696d 696c 6172 6974 795f 6d61 785f 6465  imilarity_max_de
-00000530: 7669 6174 696f 6e3a 204f 7074 696f 6e61  viation: Optiona
-00000540: 6c5b 696e 745d 0d0a 2020 2020 7369 6d69  l[int]..    simi
-00000550: 6c61 7269 7479 5f74 6872 6573 686f 6c64  larity_threshold
-00000560: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-00000570: 5d0d 0a20 2020 2065 6e61 626c 655f 7461  ]..    enable_ta
-00000580: 6767 696e 673a 204f 7074 696f 6e61 6c5b  gging: Optional[
-00000590: 626f 6f6c 5d0d 0a20 2020 2074 6167 6769  bool]..    taggi
-000005a0: 6e67 5f74 6872 6573 686f 6c64 3a20 4f70  ng_threshold: Op
-000005b0: 7469 6f6e 616c 5b66 6c6f 6174 5d0d 0a20  tional[float].. 
-000005c0: 2020 2074 6167 6769 6e67 5f73 7472 6174     tagging_strat
-000005d0: 6567 793a 204f 7074 696f 6e61 6c5b 7374  egy: Optional[st
-000005e0: 725d 0d0a 2020 2020 6578 7472 6163 7469  r]..    extracti
-000005f0: 6f6e 5f74 6872 6573 686f 6c64 3a20 4f70  on_threshold: Op
-00000600: 7469 6f6e 616c 5b66 6c6f 6174 5d0d 0a20  tional[float].. 
-00000610: 2020 2065 7874 7261 6374 696f 6e5f 7374     extraction_st
-00000620: 7261 7465 6779 3a20 4f70 7469 6f6e 616c  rategy: Optional
-00000630: 5b73 7472 5d0d 0a20 2020 2072 6573 697a  [str]..    resiz
-00000640: 655f 7061 7261 6772 6170 6873 5f6f 6e5f  e_paragraphs_on_
-00000650: 6578 7472 6163 7469 6f6e 3a20 4f70 7469  extraction: Opti
-00000660: 6f6e 616c 5b62 6f6f 6c5d 0d0a 2020 2020  onal[bool]..    
-00000670: 7265 6c65 7661 6e74 5f70 6167 655f 636f  relevant_page_co
-00000680: 756e 743a 204f 7074 696f 6e61 6c5b 696e  unt: Optional[in
-00000690: 745d 0d0a 0d0a 5365 7474 696e 6773 5363  t]....SettingsSc
-000006a0: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-000006b0: 656d 6128 5365 7474 696e 6773 2c20 6261  ema(Settings, ba
-000006c0: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
-000006d0: 6861 5363 6865 6d61 290d 0a              haSchema)..
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
+000000d0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+000000e0: 6e3d 5472 7565 290d 0a63 6c61 7373 2053  n=True)..class S
+000000f0: 6574 7469 6e67 7328 5365 6d61 6e74 6861  ettings(Semantha
+00000100: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
+00000110: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
+00000120: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
+00000130: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
+00000140: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
+00000150: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
+00000160: 2020 2073 696d 696c 6172 6974 795f 6d6f     similarity_mo
+00000170: 6465 6c5f 6964 3a20 4f70 7469 6f6e 616c  del_id: Optional
+00000180: 5b73 7472 5d0d 0a20 2020 2073 6d61 7274  [str]..    smart
+00000190: 5f63 6c75 7374 6572 5f73 696d 696c 6172  _cluster_similar
+000001a0: 6974 795f 6d6f 6465 6c5f 6964 3a20 4f70  ity_model_id: Op
+000001b0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+000001c0: 206b 6565 705f 6e75 6d62 6572 733a 204f   keep_numbers: O
+000001d0: 7074 696f 6e61 6c5b 626f 6f6c 5d0d 0a20  ptional[bool].. 
+000001e0: 2020 206d 696e 5f74 6f6b 656e 733a 204f     min_tokens: O
+000001f0: 7074 696f 6e61 6c5b 696e 745d 0d0a 2020  ptional[int]..  
+00000200: 2020 7369 6d69 6c61 7269 7479 5f6d 6561    similarity_mea
+00000210: 7375 7265 3a20 4f70 7469 6f6e 616c 5b73  sure: Optional[s
+00000220: 7472 5d0d 0a20 2020 2063 6f6e 7465 7874  tr]..    context
+00000230: 5f77 6569 6768 743a 204f 7074 696f 6e61  _weight: Optiona
+00000240: 6c5b 666c 6f61 745d 0d0a 2020 2020 656e  l[float]..    en
+00000250: 6162 6c65 5f73 7472 696e 675f 636f 6d70  able_string_comp
+00000260: 6172 6973 6f6e 3a20 4f70 7469 6f6e 616c  arison: Optional
+00000270: 5b62 6f6f 6c5d 0d0a 2020 2020 6465 6661  [bool]..    defa
+00000280: 756c 745f 646f 6375 6d65 6e74 5f74 7970  ult_document_typ
+00000290: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+000002a0: 0d0a 2020 2020 656e 6162 6c65 5f70 6172  ..    enable_par
+000002b0: 6167 7261 7068 5f73 6f72 7469 6e67 3a20  agraph_sorting: 
+000002c0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 0d0a  Optional[bool]..
+000002d0: 2020 2020 656e 6162 6c65 5f70 6172 6167      enable_parag
+000002e0: 7261 7068 5f65 6e64 5f64 6574 6563 7469  raph_end_detecti
+000002f0: 6f6e 3a20 4f70 7469 6f6e 616c 5b62 6f6f  on: Optional[boo
+00000300: 6c5d 0d0a 2020 2020 656e 6162 6c65 5f62  l]..    enable_b
+00000310: 6f6f 7374 5f77 6f72 645f 6669 6c74 6572  oost_word_filter
+00000320: 696e 675f 666f 725f 696e 7075 745f 646f  ing_for_input_do
+00000330: 6375 6d65 6e74 733a 204f 7074 696f 6e61  cuments: Optiona
+00000340: 6c5b 626f 6f6c 5d0d 0a20 2020 2074 6167  l[bool]..    tag
+00000350: 6769 6e67 5f73 696d 696c 6172 6974 795f  ging_similarity_
+00000360: 6d6f 6465 3a20 4f70 7469 6f6e 616c 5b73  mode: Optional[s
+00000370: 7472 5d0d 0a20 2020 2065 6e61 626c 655f  tr]..    enable_
+00000380: 7570 6461 7469 6e67 5f66 696e 6765 7270  updating_fingerp
+00000390: 7269 6e74 735f 6f6e 5f74 6167 5f75 7064  rints_on_tag_upd
+000003a0: 6174 6573 3a20 4f70 7469 6f6e 616c 5b62  ates: Optional[b
+000003b0: 6f6f 6c5d 0d0a 2020 2020 656e 6162 6c65  ool]..    enable
+000003c0: 5f70 6172 6167 7261 7068 5f6d 6572 6769  _paragraph_mergi
+000003d0: 6e67 5f62 6173 6564 5f6f 6e5f 666f 726d  ng_based_on_form
+000003e0: 6174 7469 6e67 3a20 4f70 7469 6f6e 616c  atting: Optional
+000003f0: 5b62 6f6f 6c5d 0d0a 2020 2020 7573 655f  [bool]..    use_
+00000400: 6372 6561 7469 6f6e 5f64 6174 655f 6672  creation_date_fr
+00000410: 6f6d 5f69 6e70 7574 5f64 6f63 756d 656e  om_input_documen
+00000420: 743a 204f 7074 696f 6e61 6c5b 626f 6f6c  t: Optional[bool
+00000430: 5d0d 0a20 2020 2065 6e61 626c 655f 7361  ]..    enable_sa
+00000440: 7475 7261 7465 645f 6d61 7463 685f 636f  turated_match_co
+00000450: 6c6f 7273 3a20 4f70 7469 6f6e 616c 5b62  lors: Optional[b
+00000460: 6f6f 6c5d 0d0a 2020 2020 656e 6162 6c65  ool]..    enable
+00000470: 5f6e 6f5f 6d61 7463 685f 636f 6c6f 725f  _no_match_color_
+00000480: 7265 643a 204f 7074 696f 6e61 6c5b 626f  red: Optional[bo
+00000490: 6f6c 5d0d 0a20 2020 2065 6e61 626c 655f  ol]..    enable_
+000004a0: 636f 6e74 6578 745f 636f 6e73 6964 6572  context_consider
+000004b0: 6174 696f 6e3a 204f 7074 696f 6e61 6c5b  ation: Optional[
+000004c0: 626f 6f6c 5d0d 0a20 2020 2065 6e61 626c  bool]..    enabl
+000004d0: 655f 7061 7261 6772 6170 685f 7265 7369  e_paragraph_resi
+000004e0: 7a69 6e67 3a20 4f70 7469 6f6e 616c 5b62  zing: Optional[b
+000004f0: 6f6f 6c5d 0d0a 2020 2020 7369 6d69 6c61  ool]..    simila
+00000500: 7269 7479 5f6d 6174 6368 6572 3a20 4f70  rity_matcher: Op
+00000510: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000520: 2073 696d 696c 6172 6974 795f 6d61 785f   similarity_max_
+00000530: 6465 7669 6174 696f 6e3a 204f 7074 696f  deviation: Optio
+00000540: 6e61 6c5b 696e 745d 0d0a 2020 2020 7369  nal[int]..    si
+00000550: 6d69 6c61 7269 7479 5f74 6872 6573 686f  milarity_thresho
+00000560: 6c64 3a20 4f70 7469 6f6e 616c 5b66 6c6f  ld: Optional[flo
+00000570: 6174 5d0d 0a20 2020 2065 6e61 626c 655f  at]..    enable_
+00000580: 7461 6767 696e 673a 204f 7074 696f 6e61  tagging: Optiona
+00000590: 6c5b 626f 6f6c 5d0d 0a20 2020 2074 6167  l[bool]..    tag
+000005a0: 6769 6e67 5f74 6872 6573 686f 6c64 3a20  ging_threshold: 
+000005b0: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d0d  Optional[float].
+000005c0: 0a20 2020 2074 6167 6769 6e67 5f73 7472  .    tagging_str
+000005d0: 6174 6567 793a 204f 7074 696f 6e61 6c5b  ategy: Optional[
+000005e0: 7374 725d 0d0a 2020 2020 6578 7472 6163  str]..    extrac
+000005f0: 7469 6f6e 5f74 6872 6573 686f 6c64 3a20  tion_threshold: 
+00000600: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d0d  Optional[float].
+00000610: 0a20 2020 2065 7874 7261 6374 696f 6e5f  .    extraction_
+00000620: 7374 7261 7465 6779 3a20 4f70 7469 6f6e  strategy: Option
+00000630: 616c 5b73 7472 5d0d 0a20 2020 2072 6573  al[str]..    res
+00000640: 697a 655f 7061 7261 6772 6170 6873 5f6f  ize_paragraphs_o
+00000650: 6e5f 6578 7472 6163 7469 6f6e 3a20 4f70  n_extraction: Op
+00000660: 7469 6f6e 616c 5b62 6f6f 6c5d 0d0a 2020  tional[bool]..  
+00000670: 2020 7265 6c65 7661 6e74 5f70 6167 655f    relevant_page_
+00000680: 636f 756e 743a 204f 7074 696f 6e61 6c5b  count: Optional[
+00000690: 696e 745d 0d0a 0d0a 5365 7474 696e 6773  int]....Settings
+000006a0: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
+000006b0: 6368 656d 6128 5365 7474 696e 6773 2c20  chema(Settings, 
+000006c0: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
+000006d0: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/smart_cluster_response_container.py` & `semantha_sdk-5.6.0/semantha_sdk/model/smart_cluster_response_container.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,36 +9,36 @@
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e63 6c75 7374 6572 696e  .model.clusterin
 000000d0: 675f 7265 7370 6f6e 7365 2069 6d70 6f72  g_response impor
 000000e0: 7420 436c 7573 7465 7269 6e67 5265 7370  t ClusteringResp
-000000f0: 6f6e 7365 0d0a 0d0a 6672 6f6d 2073 656d  onse....from sem
-00000100: 616e 7468 615f 7364 6b2e 6d6f 6465 6c2e  antha_sdk.model.
-00000110: 7265 7370 6f6e 7365 5f6d 6574 615f 696e  response_meta_in
-00000120: 666f 2069 6d70 6f72 7420 5265 7370 6f6e  fo import Respon
-00000130: 7365 4d65 7461 496e 666f 0d0a 0d0a 6672  seMetaInfo....fr
-00000140: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000150: 204f 7074 696f 6e61 6c0d 0a0d 0a40 6461   Optional....@da
-00000160: 7461 636c 6173 7328 6672 6f7a 656e 3d54  taclass(frozen=T
-00000170: 7275 6529 0d0a 636c 6173 7320 536d 6172  rue)..class Smar
-00000180: 7443 6c75 7374 6572 5265 7370 6f6e 7365  tClusterResponse
-00000190: 436f 6e74 6169 6e65 7228 5365 6d61 6e74  Container(Semant
-000001a0: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
-000001b0: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
-000001c0: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
-000001d0: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
-000001e0: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
-000001f0: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
-00000200: 0a20 2020 206d 6574 613a 204f 7074 696f  .    meta: Optio
-00000210: 6e61 6c5b 5265 7370 6f6e 7365 4d65 7461  nal[ResponseMeta
-00000220: 496e 666f 5d0d 0a20 2020 2064 6174 613a  Info]..    data:
-00000230: 204f 7074 696f 6e61 6c5b 436c 7573 7465   Optional[Cluste
-00000240: 7269 6e67 5265 7370 6f6e 7365 5d0d 0a0d  ringResponse]...
-00000250: 0a53 6d61 7274 436c 7573 7465 7252 6573  .SmartClusterRes
-00000260: 706f 6e73 6543 6f6e 7461 696e 6572 5363  ponseContainerSc
-00000270: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-00000280: 656d 6128 536d 6172 7443 6c75 7374 6572  ema(SmartCluster
-00000290: 5265 7370 6f6e 7365 436f 6e74 6169 6e65  ResponseContaine
-000002a0: 722c 2062 6173 655f 7363 6865 6d61 3d53  r, base_schema=S
-000002b0: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
+000000f0: 6f6e 7365 0d0a 6672 6f6d 2073 656d 616e  onse..from seman
+00000100: 7468 615f 7364 6b2e 6d6f 6465 6c2e 7265  tha_sdk.model.re
+00000110: 7370 6f6e 7365 5f6d 6574 615f 696e 666f  sponse_meta_info
+00000120: 2069 6d70 6f72 7420 5265 7370 6f6e 7365   import Response
+00000130: 4d65 7461 496e 666f 0d0a 6672 6f6d 2074  MetaInfo..from t
+00000140: 7970 696e 6720 696d 706f 7274 204f 7074  yping import Opt
+00000150: 696f 6e61 6c0d 0a0d 0a0d 0a40 6461 7461  ional......@data
+00000160: 636c 6173 7328 6672 6f7a 656e 3d54 7275  class(frozen=Tru
+00000170: 6529 0d0a 636c 6173 7320 536d 6172 7443  e)..class SmartC
+00000180: 6c75 7374 6572 5265 7370 6f6e 7365 436f  lusterResponseCo
+00000190: 6e74 6169 6e65 7228 5365 6d61 6e74 6861  ntainer(Semantha
+000001a0: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
+000001b0: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
+000001c0: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
+000001d0: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
+000001e0: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
+000001f0: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
+00000200: 2020 206d 6574 613a 204f 7074 696f 6e61     meta: Optiona
+00000210: 6c5b 5265 7370 6f6e 7365 4d65 7461 496e  l[ResponseMetaIn
+00000220: 666f 5d0d 0a20 2020 2064 6174 613a 204f  fo]..    data: O
+00000230: 7074 696f 6e61 6c5b 436c 7573 7465 7269  ptional[Clusteri
+00000240: 6e67 5265 7370 6f6e 7365 5d0d 0a0d 0a53  ngResponse]....S
+00000250: 6d61 7274 436c 7573 7465 7252 6573 706f  martClusterRespo
+00000260: 6e73 6543 6f6e 7461 696e 6572 5363 6865  nseContainerSche
+00000270: 6d61 203d 2063 6c61 7373 5f73 6368 656d  ma = class_schem
+00000280: 6128 536d 6172 7443 6c75 7374 6572 5265  a(SmartClusterRe
+00000290: 7370 6f6e 7365 436f 6e74 6169 6e65 722c  sponseContainer,
+000002a0: 2062 6173 655f 7363 6865 6d61 3d53 656d   base_schema=Sem
+000002b0: 616e 7468 6153 6368 656d 6129 0d0a       anthaSchema)..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py` & `semantha_sdk-5.6.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e73 656d 695f 7375 7065  .model.semi_supe
 000000d0: 725f 7669 7365 645f 646f 6375 6d65 6e74  r_vised_document
 000000e0: 2069 6d70 6f72 7420 5365 6d69 5375 7065   import SemiSupe
 000000f0: 7256 6973 6564 446f 6375 6d65 6e74 0d0a  rVisedDocument..
-00000100: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
-00000110: 706f 7274 204c 6973 740d 0a66 726f 6d20  port List..from 
-00000120: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
-00000130: 7469 6f6e 616c 0d0a 0d0a 4064 6174 6163  tional....@datac
+00000100: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000110: 7274 204c 6973 740d 0a66 726f 6d20 7479  rt List..from ty
+00000120: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
+00000130: 6f6e 616c 0d0a 0d0a 0d0a 4064 6174 6163  onal......@datac
 00000140: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
 00000150: 290d 0a63 6c61 7373 2053 6d61 7274 436c  )..class SmartCl
 00000160: 7573 7465 7253 656d 6953 7570 6572 7669  usterSemiSupervi
 00000170: 7365 6452 6571 7565 7374 2853 656d 616e  sedRequest(Seman
 00000180: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
 00000190: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
 000001a0: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/statistic.py` & `semantha_sdk-5.6.0/semantha_sdk/model/statistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
 000000c0: 2e6d 6f64 656c 2e74 6167 5f64 6f63 7320  .model.tag_docs 
 000000d0: 696d 706f 7274 2054 6167 446f 6373 0d0a  import TagDocs..
-000000e0: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
-000000f0: 706f 7274 204c 6973 740d 0a66 726f 6d20  port List..from 
-00000100: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
-00000110: 7469 6f6e 616c 0d0a 0d0a 4064 6174 6163  tional....@datac
+000000e0: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+000000f0: 7274 204c 6973 740d 0a66 726f 6d20 7479  rt List..from ty
+00000100: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
+00000110: 6f6e 616c 0d0a 0d0a 0d0a 4064 6174 6163  onal......@datac
 00000120: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
 00000130: 290d 0a63 6c61 7373 2053 7461 7469 7374  )..class Statist
 00000140: 6963 2853 656d 616e 7468 614d 6f64 656c  ic(SemanthaModel
 00000150: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
 00000160: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
 00000170: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
 00000180: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/synonym.py` & `semantha_sdk-5.6.0/semantha_sdk/model/synonym.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
 000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
 000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-000000e0: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
-000000f0: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
-00000100: 636c 6173 7320 5379 6e6f 6e79 6d28 5365  class Synonym(Se
-00000110: 6d61 6e74 6861 4d6f 6465 6c45 6e74 6974  manthaModelEntit
-00000120: 7929 3a0d 0a20 2020 2022 2222 2061 7574  y):..    """ aut
-00000130: 686f 7220 7365 6d61 6e74 6861 2c20 7468  hor semantha, th
-00000140: 6973 2069 7320 6120 6765 6e65 7261 7465  is is a generate
-00000150: 6420 636c 6173 7320 646f 206e 6f74 2063  d class do not c
-00000160: 6861 6e67 6520 6d61 6e75 616c 6c79 2120  hange manually! 
-00000170: 2222 220d 0a20 2020 2069 643a 204f 7074  """..    id: Opt
-00000180: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-00000190: 776f 7264 3a20 4f70 7469 6f6e 616c 5b73  word: Optional[s
-000001a0: 7472 5d0d 0a20 2020 2072 6567 6578 3a20  tr]..    regex: 
-000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
-000001c0: 2020 2073 796e 6f6e 796d 3a20 4f70 7469     synonym: Opti
-000001d0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2074  onal[str]..    t
-000001e0: 6167 733a 204f 7074 696f 6e61 6c5b 4c69  ags: Optional[Li
-000001f0: 7374 5b73 7472 5d5d 0d0a 0d0a 5379 6e6f  st[str]]....Syno
-00000200: 6e79 6d53 6368 656d 6120 3d20 636c 6173  nymSchema = clas
-00000210: 735f 7363 6865 6d61 2853 796e 6f6e 796d  s_schema(Synonym
-00000220: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-00000230: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+000000e0: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
+000000f0: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000100: 0d0a 636c 6173 7320 5379 6e6f 6e79 6d28  ..class Synonym(
+00000110: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
+00000120: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
+00000130: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
+00000140: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
+00000150: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
+00000160: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
+00000170: 2120 2222 220d 0a20 2020 2069 643a 204f  ! """..    id: O
+00000180: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+00000190: 2020 776f 7264 3a20 4f70 7469 6f6e 616c    word: Optional
+000001a0: 5b73 7472 5d0d 0a20 2020 2072 6567 6578  [str]..    regex
+000001b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+000001c0: 0a20 2020 2073 796e 6f6e 796d 3a20 4f70  .    synonym: Op
+000001d0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+000001e0: 2074 6167 733a 204f 7074 696f 6e61 6c5b   tags: Optional[
+000001f0: 4c69 7374 5b73 7472 5d5d 0d0a 0d0a 5379  List[str]]....Sy
+00000200: 6e6f 6e79 6d53 6368 656d 6120 3d20 636c  nonymSchema = cl
+00000210: 6173 735f 7363 6865 6d61 2853 796e 6f6e  ass_schema(Synon
+00000220: 796d 2c20 6261 7365 5f73 6368 656d 613d  ym, base_schema=
+00000230: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+00000240: 0a                                       .
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/model/table_instance.py` & `semantha_sdk-5.6.0/semantha_sdk/model/argument.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,31 +6,37 @@
 00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
 00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
 00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
 00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
 00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
 000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
 000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 696f  .model.extractio
-000000d0: 6e5f 6172 6561 2069 6d70 6f72 7420 4578  n_area import Ex
-000000e0: 7472 6163 7469 6f6e 4172 6561 0d0a 0d0a  tractionArea....
-000000f0: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000100: 7274 204f 7074 696f 6e61 6c0d 0a0d 0a40  rt Optional....@
-00000110: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
-00000120: 3d54 7275 6529 0d0a 636c 6173 7320 5461  =True)..class Ta
-00000130: 626c 6549 6e73 7461 6e63 6528 5365 6d61  bleInstance(Sema
-00000140: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
-00000150: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
-00000160: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
-00000170: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
-00000180: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
-00000190: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
-000001a0: 220d 0a20 2020 2074 7970 653a 204f 7074  "..    type: Opt
-000001b0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
-000001c0: 6578 7472 6163 7469 6f6e 5f61 7265 613a  extraction_area:
-000001d0: 204f 7074 696f 6e61 6c5b 4578 7472 6163   Optional[Extrac
-000001e0: 7469 6f6e 4172 6561 5d0d 0a0d 0a54 6162  tionArea]....Tab
-000001f0: 6c65 496e 7374 616e 6365 5363 6865 6d61  leInstanceSchema
-00000200: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
-00000210: 5461 626c 6549 6e73 7461 6e63 652c 2062  TableInstance, b
-00000220: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
-00000230: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
+000000c0: 2e6d 6f64 656c 2e66 6965 6c64 2069 6d70  .model.field imp
+000000d0: 6f72 7420 4669 656c 640d 0a66 726f 6d20  ort Field..from 
+000000e0: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
+000000f0: 7374 0d0a 6672 6f6d 2074 7970 696e 6720  st..from typing 
+00000100: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
+00000110: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
+00000120: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
+00000130: 6173 7320 4172 6775 6d65 6e74 2853 656d  ass Argument(Sem
+00000140: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
+00000150: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
+00000160: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
+00000170: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
+00000180: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
+00000190: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
+000001a0: 2222 0d0a 2020 2020 7661 6c75 653a 204f  ""..    value: O
+000001b0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+000001c0: 2020 6669 656c 6473 3a20 4f70 7469 6f6e    fields: Option
+000001d0: 616c 5b4c 6973 745b 4669 656c 645d 5d0d  al[List[Field]].
+000001e0: 0a20 2020 2063 6f6e 6469 7469 6f6e 3a20  .    condition: 
+000001f0: 4f70 7469 6f6e 616c 5b22 436f 6e64 6974  Optional["Condit
+00000200: 696f 6e56 616c 7565 225d 0d0a 0d0a 6672  ionValue"]....fr
+00000210: 6f6d 2073 656d 616e 7468 615f 7364 6b2e  om semantha_sdk.
+00000220: 6d6f 6465 6c2e 636f 6e64 6974 696f 6e5f  model.condition_
+00000230: 7661 6c75 6520 696d 706f 7274 2043 6f6e  value import Con
+00000240: 6469 7469 6f6e 5661 6c75 650d 0a41 7267  ditionValue..Arg
+00000250: 756d 656e 7453 6368 656d 6120 3d20 636c  umentSchema = cl
+00000260: 6173 735f 7363 6865 6d61 2841 7267 756d  ass_schema(Argum
+00000270: 656e 742c 2062 6173 655f 7363 6865 6d61  ent, base_schema
+00000280: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
+00000290: 0d0a                                     ..
```

### Comparing `semantha_sdk-5.5.0/semantha_sdk/request/semantha_request.py` & `semantha_sdk-5.6.0/semantha_sdk/request/semantha_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/response/semantha_response.py` & `semantha_sdk-5.6.0/semantha_sdk/response/semantha_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/semantha_sdk/rest/rest_client.py` & `semantha_sdk-5.6.0/semantha_sdk/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.5.0/PKG-INFO` & `semantha_sdk-5.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantha-sdk
-Version: 5.5.0
+Version: 5.6.0
 Summary: This is a python client sdk for accessing semantha (the semantic platform)
 Home-page: https://semantha.de
 License: Apache-2.0
 Author: Sebastian Weigelt
 Author-email: sebastian.weigelt@semantha.ai
 Maintainer: semantha support
 Maintainer-email: support@semantha.de
@@ -39,14 +39,17 @@
 ### Disclaimer
 
 **IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
 Use with caution and on own risk.
 
 ## Update Notes
 
+### Version 5.6.0
+Adde most endpoints in **/api/models/* **
+
 ### Version 5.5.0
 Removed language parameter on **/api/domains/{domainname}/references**
 Fixed bug on serialization of **/api/domains/{domainname}/modelinstances** response.
 Fixed return of binary responses of bulk services.
 
 ### Version 5.4.0
 Added **new** service: 
@@ -150,15 +153,15 @@
 - [x] **/bulk/domains/{domainname}** -> BulkdomainsDomainEndpoint
 - [x] **/bulk/domains/{domainname}/documentclasses** -> BulkdomainsDocumentclassesEndpoint
     - [x] **GET** -> List[DocumentClassBulk]
     - [x] **POST** -> None
 - [x] **/bulk/domains/{domainname}/referencedocuments** -> BulkdomainsReferencedocumentsEndpoint
     - [x] **GET** -> List[Document]
     - [x] **POST** -> None
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/bulk/domains/{domainname}/references** -> BulkdomainsReferencesEndpoint
     - [x] **POST** -> List[Document]
 - [x] **/bulk/model** -> BulkModelEndpoint
 - [x] **/bulk/model/domains** -> BulkmodelDomainsEndpoint
 - [x] **/bulk/model/domains/{domainname}** -> BulkmodelDomainEndpoint
 - [x] **/bulk/model/domains/{domainname}/boostwords** -> BulkmodelBoostwordsEndpoint
     - [x] **POST** -> None
@@ -175,15 +178,17 @@
     - [x] **GET** -> List[Instance]
     - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/metadata** -> BulkmodelMetadataEndpoint
     - [x] **GET** -> List[Metadata]
     - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/namedentities** -> BulkmodelNamedentitiesEndpoint
     - [x] **POST** -> None
-- [ ] **/bulk/model/domains/{domainname}/rules** 
+- [x] **/bulk/model/domains/{domainname}/rules** -> BulkmodelRulesEndpoint
+    - [x] **GET** -> List[Rule]
+    - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/stopwords** -> BulkmodelStopwordsEndpoint
     - [x] **POST** -> None
 - [x] **/bulk/model/domains/{domainname}/synonyms** -> BulkmodelSynonymsEndpoint
     - [x] **POST** -> None
 - [x] **/currentuser** -> CurrentuserEndpoint
     - [x] **GET** -> CurrentUser
 - [x] **/currentuser/roles** -> RolesEndpoint
@@ -193,144 +198,209 @@
 - [x] **/domains** -> DomainsEndpoint
     - [x] **GET** -> List[Domain]
 - [x] **/domains/{domainname}** -> DomainEndpoint
     - [x] **GET** -> Domain
 - [x] **/domains/{domainname}/answers** -> AnswersEndpoint
     - [x] **POST** -> Answer
 - [x] **/domains/{domainname}/documentannotations** -> DocumentannotationsEndpoint
-    - [x] **POST** -> IOBase
+    - [x] **POST** (Accept: docx) -> IOBase
+    - [x] **POST** (Accept: pdf) -> IOBase
 - [x] **/domains/{domainname}/documentclasses** -> DocumentclassesEndpoint
     - [x] **GET** -> List[DocumentClass]
     - [x] **POST** -> DocumentClass
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/domains/{domainname}/documentclasses/{id}** -> DocumentclassEndpoint
     - [x] **GET** -> DocumentClass
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PUT** -> DocumentClass
 - [ ] **/domains/{domainname}/documentclasses/{id}/documentclasses** 
 - [ ] **/domains/{domainname}/documentclasses/{id}/referencedocuments** 
 - [x] **/domains/{domainname}/documentcomparisons** -> DocumentcomparisonsEndpoint
-    - [x] **POST** -> IOBase
+    - [x] **POST** (Accept: xlsx) -> IOBase
 - [x] **/domains/{domainname}/documents** -> DocumentsEndpoint
     - [x] **POST** -> List[Document]
+    - [x] **POST** (Accept: xlsx) -> IOBase
+    - [x] **POST** (Accept: docx) -> IOBase
 - [x] **/domains/{domainname}/modelclasses** -> ModelclassesEndpoint
     - [x] **GET** -> List[ModelClass]
 - [x] **/domains/{domainname}/modelinstances** -> ModelinstancesEndpoint
     - [x] **POST** -> SemanticModel
+    - [x] **POST** (Accept: xlsx) -> IOBase
 - [x] **/domains/{domainname}/referencedocuments** -> ReferencedocumentsEndpoint
     - [x] **GET** -> ReferenceDocumentsResponseContainer
+    - [x] **GET** (Accept: xlsx) -> IOBase
     - [x] **POST** -> List[DocumentInformation]
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/domains/{domainname}/referencedocuments/clusters** -> ClustersEndpoint
     - [x] **GET** -> SmartClusterResponseContainer
     - [x] **PUT** -> SmartClusterResponseContainer
 - [x] **/domains/{domainname}/referencedocuments/namedentities** -> NamedentitiesEndpoint
     - [x] **GET** -> List[DocumentNamedEntity]
 - [x] **/domains/{domainname}/referencedocuments/statistic** -> StatisticEndpoint
     - [x] **GET** -> Statistic
 - [x] **/domains/{domainname}/referencedocuments/{documentid}** -> ReferencedocumentEndpoint
     - [x] **GET** -> Document
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PATCH** -> DocumentInformation
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs** -> ParagraphsEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs/{id}** -> ParagraphEndpoint
     - [x] **GET** -> Paragraph
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PATCH** -> Paragraph
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences** -> SentencesEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences/{id}** -> SentenceEndpoint
     - [x] **GET** -> Sentence
 - [x] **/domains/{domainname}/references** -> ReferencesEndpoint
     - [x] **POST** -> Document
+    - [x] **POST** (Accept: xlsx) -> IOBase
+    - [x] **POST** (Accept: docx) -> IOBase
+    - [x] **POST** (Accept: pdf) -> IOBase
 - [x] **/domains/{domainname}/settings** -> SettingsEndpoint
     - [x] **GET** -> Settings
     - [x] **PATCH** -> Settings
 - [x] **/domains/{domainname}/similaritymatrix** -> SimilaritymatrixEndpoint
     - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/similaritymatrix/cluster** -> SimilaritymatrixClusterEndpoint
     - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/summarizations** -> SummarizationsEndpoint
     - [x] **POST** -> str
 - [x] **/domains/{domainname}/tags** -> TagsEndpoint
     - [x] **GET** -> List[str]
 - [x] **/domains/{domainname}/tags/{tagname}** -> TagEndpoint
 - [x] **/domains/{domainname}/tags/{tagname}/referencedocuments** -> TagReferencedocumentsEndpoint
     - [x] **GET** -> List[DocumentInformation]
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/domains/{domainname}/validation** -> ValidationEndpoint
     - [x] **POST** -> SemanticModel
 - [x] **/info** -> InfoEndpoint
     - [x] **GET** -> Info
 - [x] **/languages** -> LanguagesEndpoint
     - [x] **POST** -> LanguageDetection
 - [x] **/model** -> ModelEndpoint
 - [x] **/model/datatypes** -> ModelDatatypesEndpoint
     - [x] **GET** -> List[str]
 - [x] **/model/domains** -> ModelDomainsEndpoint
 - [x] **/model/domains/{domainname}** -> ModelDomainEndpoint
-    - [x] **GET** -> IOBase
+    - [x] **GET** (Accept: xlsx) -> IOBase
     - [x] **PATCH** -> IOBase
-- [ ] **/model/domains/{domainname}/attributes** 
+- [x] **/model/domains/{domainname}/attributes** -> ModelAttributesEndpoint
+    - [x] **GET** -> List[AttributeOverview]
 - [ ] **/model/domains/{domainname}/backups** 
 - [x] **/model/domains/{domainname}/boostwords** -> ModelBoostwordsEndpoint
     - [x] **GET** -> List[BoostWord]
     - [x] **POST** -> BoostWord
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/boostwords/{id}** -> ModelBoostwordEndpoint
     - [x] **GET** -> BoostWord
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PUT** -> BoostWord
 - [ ] **/model/domains/{domainname}/classes** 
 - [ ] **/model/domains/{domainname}/classes/{classid}** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/attributes** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/attributes/{id}** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/instances** 
-- [ ] **/model/domains/{domainname}/dataproperties** 
-- [ ] **/model/domains/{domainname}/dataproperties/{id}** 
-- [ ] **/model/domains/{domainname}/extractorclasses** 
-- [ ] **/model/domains/{domainname}/extractorclasses/{id}** 
-- [ ] **/model/domains/{domainname}/extractorclasses/{id}/extractorclasses** 
-- [ ] **/model/domains/{domainname}/extractors** 
-- [ ] **/model/domains/{domainname}/extractortables** 
-- [ ] **/model/domains/{domainname}/extractortables/{id}** 
-- [ ] **/model/domains/{domainname}/formatters** 
-- [ ] **/model/domains/{domainname}/instances** 
-- [ ] **/model/domains/{domainname}/instances/{id}** 
-- [ ] **/model/domains/{domainname}/metadata** 
-- [ ] **/model/domains/{domainname}/metadata/{id}** 
+- [x] **/model/domains/{domainname}/dataproperties** -> ModelDatapropertiesEndpoint
+    - [x] **GET** -> List[Overview]
+    - [x] **POST** -> DataProperty
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/dataproperties/{id}** -> ModelDatapropertyEndpoint
+    - [x] **GET** -> DataProperty
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> DataProperty
+- [x] **/model/domains/{domainname}/extractorclasses** -> ModelExtractorclassesEndpoint
+    - [x] **GET** -> List[ExtractorClassOverview]
+    - [x] **POST** -> ExtractorClass
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> None
+- [x] **/model/domains/{domainname}/extractorclasses/{id}** -> ModelExtractorclassEndpoint
+    - [x] **GET** -> ExtractorClass
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> ExtractorClass
+- [x] **/model/domains/{domainname}/extractorclasses/{id}/extractorclasses** -> ChildExtractorclassesEndpoint
+    - [x] **POST** -> ExtractorClass
+- [x] **/model/domains/{domainname}/extractors** -> ModelExtractorsEndpoint
+    - [x] **GET** -> List[Entity]
+- [x] **/model/domains/{domainname}/extractortables** -> ModelExtractortablesEndpoint
+    - [x] **GET** -> List[Table]
+    - [x] **POST** -> ExtractorTable
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/extractortables/{id}** -> ModelExtractortableEndpoint
+    - [x] **GET** -> ExtractorTable
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> ExtractorTable
+- [x] **/model/domains/{domainname}/formatters** -> ModelFormattersEndpoint
+    - [x] **GET** -> List[Formatter]
+- [x] **/model/domains/{domainname}/instances** -> ModelontInstancesEndpoint
+    - [x] **GET** -> List[InstanceOverview]
+    - [x] **GET** (Accept: xlsx) -> IOBase
+    - [x] **POST** -> Instance
+    - [x] **DELETE** -> None
+    - [x] **PATCH** -> None
+- [x] **/model/domains/{domainname}/instances/{id}** -> ModelontInstanceEndpoint
+    - [x] **GET** -> Instance
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Instance
+- [x] **/model/domains/{domainname}/metadata** -> ModelMetadataEndpoint
+    - [x] **GET** -> List[Metadata]
+    - [x] **POST** -> Metadata
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/metadata/{id}** -> ModelOnemetadataEndpoint
+    - [x] **GET** -> Metadata
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Metadata
 - [x] **/model/domains/{domainname}/namedentities** -> ModelNamedentitiesEndpoint
     - [x] **GET** -> List[NamedEntity]
     - [x] **POST** -> NamedEntity
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/namedentities/{id}** -> ModelNamedentityEndpoint
     - [x] **GET** -> NamedEntity
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PUT** -> NamedEntity
-- [ ] **/model/domains/{domainname}/objectproperties** 
-- [ ] **/model/domains/{domainname}/regexes** 
-- [ ] **/model/domains/{domainname}/regexes/{id}** 
-- [ ] **/model/domains/{domainname}/relations** 
-- [ ] **/model/domains/{domainname}/relations/{id}** 
-- [ ] **/model/domains/{domainname}/rulefunctions** 
-- [ ] **/model/domains/{domainname}/rules** 
-- [ ] **/model/domains/{domainname}/rules/{id}** 
+- [x] **/model/domains/{domainname}/objectproperties** -> ModelObjectpropertiesEndpoint
+    - [x] **GET** -> List[Overview]
+- [x] **/model/domains/{domainname}/regexes** -> ModelRegexesEndpoint
+    - [x] **GET** -> List[Regex]
+    - [x] **POST** -> Regex
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/regexes/{id}** -> ModelRegexEndpoint
+    - [x] **GET** -> Regex
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Regex
+- [x] **/model/domains/{domainname}/relations** -> ModelRelationsEndpoint
+    - [x] **GET** -> List[Relation]
+    - [x] **POST** -> Relation
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/relations/{id}** -> ModelRelationEndpoint
+    - [x] **GET** -> Relation
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Relation
+- [x] **/model/domains/{domainname}/rulefunctions** -> ModelRulefunctionsEndpoint
+    - [x] **GET** -> List[RuleFunction]
+- [x] **/model/domains/{domainname}/rules** -> ModelRulesEndpoint
+    - [x] **GET** -> List[RuleOverview]
+    - [x] **POST** -> Rule
+    - [x] **DELETE** -> None
+- [x] **/model/domains/{domainname}/rules/{id}** -> ModelRuleEndpoint
+    - [x] **GET** -> Rule
+    - [x] **DELETE** -> None
+    - [x] **PUT** -> Rule
 - [x] **/model/domains/{domainname}/stopwords** -> ModelStopwordsEndpoint
     - [x] **GET** -> List[StopWord]
     - [x] **POST** -> StopWord
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/stopwords/{id}** -> ModelStopwordEndpoint
     - [x] **GET** -> StopWord
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PUT** -> StopWord
 - [x] **/model/domains/{domainname}/synonyms** -> ModelSynonymsEndpoint
     - [x] **GET** -> List[Synonym]
     - [x] **POST** -> Synonym
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
 - [x] **/model/domains/{domainname}/synonyms/{id}** -> ModelSynonymEndpoint
     - [x] **GET** -> Synonym
-    - [x] **DELETE** -> void
+    - [x] **DELETE** -> None
     - [x] **PUT** -> Synonym
 - [x] **/model/extractortypes** -> ModelExtractortypesEndpoint
     - [x] **GET** -> List[str]
 - [x] **/model/metadatatypes** -> ModelMetadatatypesEndpoint
     - [x] **GET** -> List[str]
```

