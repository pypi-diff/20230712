# Comparing `tmp/gpt_index-0.7.5.tar.gz` & `tmp/gpt_index-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_index-0.7.5.tar", last modified: Wed Jul 12 01:48:31 2023, max compression
+gzip compressed data, was "gpt_index-0.7.6.tar", last modified: Wed Jul 12 17:39:34 2023, max compression
```

## Comparing `gpt_index-0.7.5.tar` & `gpt_index-0.7.6.tar`

### file list

```diff
@@ -1,656 +1,672 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.706850 gpt_index-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-12 01:48:16.000000 gpt_index-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 01:48:16.000000 gpt_index-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-12 01:48:31.706850 gpt_index-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-12 01:48:16.000000 gpt_index-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.578849 gpt_index-0.7.5/gpt_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-12 01:48:31.000000 gpt_index-0.7.5/gpt_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-07-12 01:48:31.000000 gpt_index-0.7.5/gpt_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:48:31.000000 gpt_index-0.7.5/gpt_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 01:48:31.000000 gpt_index-0.7.5/gpt_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 01:48:31.000000 gpt_index-0.7.5/gpt_index.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.582849 gpt_index-0.7.5/llama_index/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.582849 gpt_index-0.7.5/llama_index/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/agent/context_retriever_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    18290 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/agent/openai_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/agent/retriever_openai_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.582849 gpt_index-0.7.5/llama_index/bridge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/bridge/langchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.582849 gpt_index-0.7.5/llama_index/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/callbacks/aim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/callbacks/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/callbacks/token_counting.py
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/callbacks/wandb_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.582849 gpt_index-0.7.5/llama_index/chat_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/chat_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/chat_engine/condense_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/chat_engine/react.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/chat_engine/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/chat_engine/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/chat_engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.582849 gpt_index-0.7.5/llama_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.582849 gpt_index-0.7.5/llama_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/data_structs/document_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/data_structs/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.586849 gpt_index-0.7.5/llama_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/embeddings/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.586849 gpt_index-0.7.5/llama_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/evaluation/guideline_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.586849 gpt_index-0.7.5/llama_index/graph_stores/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/graph_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16582 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/graph_stores/nebulagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/graph_stores/registery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/graph_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/graph_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.586849 gpt_index-0.7.5/llama_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14414 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.586849 gpt_index-0.7.5/llama_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.586849 gpt_index-0.7.5/llama_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.586849 gpt_index-0.7.5/llama_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.586849 gpt_index-0.7.5/llama_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.590849 gpt_index-0.7.5/llama_index/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/document_summary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/document_summary/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.590849 gpt_index-0.7.5/llama_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.590849 gpt_index-0.7.5/llama_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.590849 gpt_index-0.7.5/llama_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/knowledge_graph/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.590849 gpt_index-0.7.5/llama_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.590849 gpt_index-0.7.5/llama_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/postprocessor/cohere_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/postprocessor/llm_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/postprocessor/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/postprocessor/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.590849 gpt_index-0.7.5/llama_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.594849 gpt_index-0.7.5/llama_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/query/query_transform/feedback_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.594849 gpt_index-0.7.5/llama_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/struct_store/json_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.594849 gpt_index-0.7.5/llama_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/tree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.594849 gpt_index-0.7.5/llama_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/vector_store/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.594849 gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.594849 gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.594849 gpt_index-0.7.5/llama_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.598849 gpt_index-0.7.5/llama_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/langchain_helpers/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.598849 gpt_index-0.7.5/llama_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/structured.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.598849 gpt_index-0.7.5/llama_index/llm_predictor/vellum/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/vellum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/vellum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/vellum/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/vellum/prompt_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/vellum/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llm_predictor/vellum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.602849 gpt_index-0.7.5/llama_index/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/anthropic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/azure_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/langchain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/llms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.606849 gpt_index-0.7.5/llama_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.606849 gpt_index-0.7.5/llama_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/node_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.606849 gpt_index-0.7.5/llama_index/node_parser/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/node_parser/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/node_parser/extractors/metadata_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.606849 gpt_index-0.7.5/llama_index/objects/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/objects/base_node_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/objects/table_node_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/objects/tool_node_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.606849 gpt_index-0.7.5/llama_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/output_parsers/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/output_parsers/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/output_parsers/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/output_parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.610849 gpt_index-0.7.5/llama_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.610849 gpt_index-0.7.5/llama_index/program/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/base_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/guidance_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/llm_program.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/llm_prompt_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/openai_program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.610849 gpt_index-0.7.5/llama_index/program/predefined/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/predefined/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/predefined/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.610849 gpt_index-0.7.5/llama_index/program/predefined/evaporate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/predefined/evaporate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/predefined/evaporate/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/predefined/evaporate/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/program/predefined/evaporate/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.614849 gpt_index-0.7.5/llama_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/choice_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/guidance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/prompt_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/prompts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.618849 gpt_index-0.7.5/llama_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/citation_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.618849 gpt_index-0.7.5/llama_index/query_engine/flare/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/flare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/flare/answer_inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/flare/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/flare/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/flare/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/pandas_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/retry_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/retry_source_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/sql_join_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/sql_vector_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/sub_question_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.618849 gpt_index-0.7.5/llama_index/question_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/question_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/question_gen/guidance_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/question_gen/llm_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/question_gen/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/question_gen/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/question_gen/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.622850 gpt_index-0.7.5/llama_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.626850 gpt_index-0.7.5/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.626850 gpt_index-0.7.5/llama_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/docs_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/epub_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/image_caption_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/image_vision_llm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/ipynb_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/markdown_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/mbox_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/slides_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/tabular_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/file/video_audio_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.630849 gpt_index-0.7.5/llama_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.630849 gpt_index-0.7.5/llama_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.630849 gpt_index-0.7.5/llama_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/psychic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.630849 gpt_index-0.7.5/llama_index/readers/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.630849 gpt_index-0.7.5/llama_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.630849 gpt_index-0.7.5/llama_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.630849 gpt_index-0.7.5/llama_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.630849 gpt_index-0.7.5/llama_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response/pprint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.634850 gpt_index-0.7.5/llama_index/response_synthesizers/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/accumulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/compact_and_accumulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/compact_and_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/no_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/simple_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/tree_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/response_synthesizers/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.634850 gpt_index-0.7.5/llama_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/retrievers/recursive_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.638850 gpt_index-0.7.5/llama_index/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/selectors/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/selectors/pydantic_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/selectors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.638850 gpt_index-0.7.5/llama_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.638850 gpt_index-0.7.5/llama_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/docstore/dynamodb_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/docstore/redis_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.642850 gpt_index-0.7.5/llama_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/index_store/dynamodb_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/index_store/redis_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.642850 gpt_index-0.7.5/llama_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/kvstore/dynamodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/kvstore/redis_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/kvstore/s3_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.642850 gpt_index-0.7.5/llama_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.642850 gpt_index-0.7.5/llama_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/function_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/ondemand_loader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/query_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.646850 gpt_index-0.7.5/llama_index/tools/tool_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/tool_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/tool_spec/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.646850 gpt_index-0.7.5/llama_index/tools/tool_spec/notion/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/tool_spec/notion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/tool_spec/notion/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.646850 gpt_index-0.7.5/llama_index/tools/tool_spec/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/tool_spec/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/tool_spec/slack/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.646850 gpt_index-0.7.5/llama_index/tts/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tts/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/tts/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.650850 gpt_index-0.7.5/llama_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/deeplake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.654850 gpt_index-0.7.5/llama_index/vector_stores/docarray/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/docarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/docarray/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/docarray/hnsw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/docarray/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/lancedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)    17241 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/supabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/tair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/typesense.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-12 01:48:17.000000 gpt_index-0.7.5/llama_index/vector_stores/weaviate_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-12 01:48:17.000000 gpt_index-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:48:31.706850 gpt_index-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-12 01:48:17.000000 gpt_index-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.654850 gpt_index-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.654850 gpt_index-0.7.5/tests/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/callbacks/test_llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/callbacks/test_token_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.654850 gpt_index-0.7.5/tests/chat_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/chat_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/chat_engine/test_condense_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/chat_engine/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.654850 gpt_index-0.7.5/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.654850 gpt_index-0.7.5/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.658850 gpt_index-0.7.5/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.658850 gpt_index-0.7.5/tests/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/document_summary/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/document_summary/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.658850 gpt_index-0.7.5/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.658850 gpt_index-0.7.5/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.658850 gpt_index-0.7.5/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.658850 gpt_index-0.7.5/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.662850 gpt_index-0.7.5/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/postprocessor/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/postprocessor/test_llm_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/postprocessor/test_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.666850 gpt_index-0.7.5/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.666850 gpt_index-0.7.5/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/query/test_embedding_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.670850 gpt_index-0.7.5/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/struct_store/test_json_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.670850 gpt_index-0.7.5/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.674850 gpt_index-0.7.5/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.674850 gpt_index-0.7.5/tests/indices/vector_store/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/auto_retriever/test_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.678850 gpt_index-0.7.5/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.678850 gpt_index-0.7.5/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.678850 gpt_index-0.7.5/tests/llm_predictor/vellum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llm_predictor/vellum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llm_predictor/vellum/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llm_predictor/vellum/test_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llm_predictor/vellum/test_prompt_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llm_predictor/vellum/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.682850 gpt_index-0.7.5/tests/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llms/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llms/test_anthropic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llms/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llms/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llms/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llms/test_openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/llms/test_palm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.686850 gpt_index-0.7.5/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.686850 gpt_index-0.7.5/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.686850 gpt_index-0.7.5/tests/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/objects/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/objects/test_node_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.690850 gpt_index-0.7.5/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/output_parsers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/output_parsers/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/output_parsers/test_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.690850 gpt_index-0.7.5/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.690850 gpt_index-0.7.5/tests/program/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/program/test_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/program/test_llm_program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.694850 gpt_index-0.7.5/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/prompts/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/prompts/test_guidance_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.694850 gpt_index-0.7.5/tests/question_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/question_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/question_gen/test_guidance_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/question_gen/test_llm_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.698850 gpt_index-0.7.5/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.698850 gpt_index-0.7.5/tests/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.698850 gpt_index-0.7.5/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.702850 gpt_index-0.7.5/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/storage/docstore/test_dynamodb_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/storage/docstore/test_redis_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/storage/test_storage_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.702850 gpt_index-0.7.5/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.702850 gpt_index-0.7.5/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/tools/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/tools/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/tools/test_ondemand_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/tools/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.702850 gpt_index-0.7.5/tests/tools/tool_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/tools/tool_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/tools/tool_spec/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:31.706850 gpt_index-0.7.5/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/vector_stores/test_docarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/vector_stores/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/vector_stores/test_qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/vector_stores/test_tair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-12 01:48:17.000000 gpt_index-0.7.5/tests/vector_stores/test_weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.268658 gpt_index-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-12 17:39:19.000000 gpt_index-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 17:39:19.000000 gpt_index-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-12 17:39:34.268658 gpt_index-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-12 17:39:19.000000 gpt_index-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.200659 gpt_index-0.7.6/gpt_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-12 17:39:34.000000 gpt_index-0.7.6/gpt_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21400 2023-07-12 17:39:34.000000 gpt_index-0.7.6/gpt_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:39:34.000000 gpt_index-0.7.6/gpt_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 17:39:34.000000 gpt_index-0.7.6/gpt_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 17:39:34.000000 gpt_index-0.7.6/gpt_index.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.200659 gpt_index-0.7.6/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.200659 gpt_index-0.7.6/llama_index/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/context_retriever_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18652 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/openai_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.200659 gpt_index-0.7.6/llama_index/agent/react/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/react/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/react/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/react/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/react/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/react/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/react/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/retriever_openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/agent/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.200659 gpt_index-0.7.6/llama_index/bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/bridge/langchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.204659 gpt_index-0.7.6/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/callbacks/aim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/callbacks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/callbacks/token_counting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/callbacks/wandb_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.204659 gpt_index-0.7.6/llama_index/chat_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/chat_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/chat_engine/condense_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/chat_engine/react.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/chat_engine/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/chat_engine/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/chat_engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.204659 gpt_index-0.7.6/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.204659 gpt_index-0.7.6/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/data_structs/document_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/data_structs/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.204659 gpt_index-0.7.6/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.204659 gpt_index-0.7.6/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/evaluation/guideline_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.204659 gpt_index-0.7.6/llama_index/graph_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16582 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/graph_stores/nebulagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/graph_stores/registery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/graph_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/graph_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.208659 gpt_index-0.7.6/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14414 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.208659 gpt_index-0.7.6/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.208659 gpt_index-0.7.6/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.208659 gpt_index-0.7.6/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.208659 gpt_index-0.7.6/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.208659 gpt_index-0.7.6/llama_index/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/document_summary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/document_summary/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.208659 gpt_index-0.7.6/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.208659 gpt_index-0.7.6/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.208659 gpt_index-0.7.6/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/knowledge_graph/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.208659 gpt_index-0.7.6/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.212659 gpt_index-0.7.6/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/postprocessor/cohere_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/postprocessor/llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/postprocessor/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/postprocessor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.212659 gpt_index-0.7.6/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.212659 gpt_index-0.7.6/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/query/query_transform/feedback_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.212659 gpt_index-0.7.6/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/struct_store/json_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.212659 gpt_index-0.7.6/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/tree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.212659 gpt_index-0.7.6/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/vector_store/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.212659 gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.216658 gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.216658 gpt_index-0.7.6/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.216658 gpt_index-0.7.6/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/langchain_helpers/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.216658 gpt_index-0.7.6/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.216658 gpt_index-0.7.6/llama_index/llm_predictor/vellum/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/vellum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/vellum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/vellum/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/vellum/prompt_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/vellum/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llm_predictor/vellum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.220658 gpt_index-0.7.6/llama_index/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/anthropic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/azure_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/langchain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/llms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.220658 gpt_index-0.7.6/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.220658 gpt_index-0.7.6/llama_index/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/memory/chat_memory_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/memory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.220658 gpt_index-0.7.6/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/node_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.220658 gpt_index-0.7.6/llama_index/node_parser/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/node_parser/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/node_parser/extractors/metadata_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.220658 gpt_index-0.7.6/llama_index/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/objects/base_node_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/objects/table_node_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/objects/tool_node_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.220658 gpt_index-0.7.6/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/output_parsers/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/output_parsers/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/output_parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.220658 gpt_index-0.7.6/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.220658 gpt_index-0.7.6/llama_index/program/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/base_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/guidance_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/llm_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/llm_prompt_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/openai_program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.224659 gpt_index-0.7.6/llama_index/program/predefined/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/predefined/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/predefined/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.224659 gpt_index-0.7.6/llama_index/program/predefined/evaporate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/predefined/evaporate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/predefined/evaporate/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/predefined/evaporate/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/program/predefined/evaporate/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.224659 gpt_index-0.7.6/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/choice_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/guidance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/prompt_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/prompts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.228659 gpt_index-0.7.6/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/citation_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.228659 gpt_index-0.7.6/llama_index/query_engine/flare/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/flare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/flare/answer_inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/flare/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/flare/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/flare/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/pandas_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/retry_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/retry_source_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/sql_join_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/sql_vector_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/sub_question_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.228659 gpt_index-0.7.6/llama_index/question_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/question_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/question_gen/guidance_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/question_gen/llm_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/question_gen/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/question_gen/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/question_gen/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.232658 gpt_index-0.7.6/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.232658 gpt_index-0.7.6/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.232658 gpt_index-0.7.6/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/docs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/epub_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/image_caption_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/image_vision_llm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/ipynb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/markdown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/mbox_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/slides_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/tabular_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/file/video_audio_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.232658 gpt_index-0.7.6/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.232658 gpt_index-0.7.6/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.236658 gpt_index-0.7.6/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/psychic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.236658 gpt_index-0.7.6/llama_index/readers/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.236658 gpt_index-0.7.6/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.236658 gpt_index-0.7.6/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.236658 gpt_index-0.7.6/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.236658 gpt_index-0.7.6/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response/pprint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.236658 gpt_index-0.7.6/llama_index/response_synthesizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/compact_and_accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/compact_and_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/no_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/simple_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/tree_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/response_synthesizers/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.236658 gpt_index-0.7.6/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/retrievers/recursive_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.240658 gpt_index-0.7.6/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/selectors/pydantic_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.240658 gpt_index-0.7.6/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.240658 gpt_index-0.7.6/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/docstore/dynamodb_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/docstore/redis_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.240658 gpt_index-0.7.6/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/index_store/dynamodb_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/index_store/redis_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.240658 gpt_index-0.7.6/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/kvstore/dynamodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/kvstore/redis_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/kvstore/s3_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.244658 gpt_index-0.7.6/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.244658 gpt_index-0.7.6/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/function_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/ondemand_loader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/query_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.244658 gpt_index-0.7.6/llama_index/tools/tool_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/tool_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/tool_spec/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.244658 gpt_index-0.7.6/llama_index/tools/tool_spec/load_and_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/tool_spec/load_and_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/tool_spec/load_and_search/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.244658 gpt_index-0.7.6/llama_index/tools/tool_spec/notion/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/tool_spec/notion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/tool_spec/notion/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.244658 gpt_index-0.7.6/llama_index/tools/tool_spec/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/tool_spec/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/tool_spec/slack/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.244658 gpt_index-0.7.6/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.248659 gpt_index-0.7.6/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/deeplake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.248659 gpt_index-0.7.6/llama_index/vector_stores/docarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/docarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/docarray/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/docarray/hnsw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/docarray/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17241 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/supabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/tair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/typesense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-12 17:39:20.000000 gpt_index-0.7.6/llama_index/vector_stores/weaviate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-12 17:39:20.000000 gpt_index-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:39:34.268658 gpt_index-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-12 17:39:20.000000 gpt_index-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.248659 gpt_index-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.252658 gpt_index-0.7.6/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/callbacks/test_token_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.252658 gpt_index-0.7.6/tests/chat_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/chat_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/chat_engine/test_condense_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/chat_engine/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.252658 gpt_index-0.7.6/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.252658 gpt_index-0.7.6/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.252658 gpt_index-0.7.6/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.252658 gpt_index-0.7.6/tests/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/document_summary/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/document_summary/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.252658 gpt_index-0.7.6/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.252658 gpt_index-0.7.6/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.252658 gpt_index-0.7.6/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.252658 gpt_index-0.7.6/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.256658 gpt_index-0.7.6/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/postprocessor/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/postprocessor/test_llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/postprocessor/test_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.256658 gpt_index-0.7.6/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.256658 gpt_index-0.7.6/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/query/test_embedding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.256658 gpt_index-0.7.6/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/struct_store/test_json_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.256658 gpt_index-0.7.6/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.260658 gpt_index-0.7.6/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.260658 gpt_index-0.7.6/tests/indices/vector_store/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/auto_retriever/test_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.260658 gpt_index-0.7.6/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.260658 gpt_index-0.7.6/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.260658 gpt_index-0.7.6/tests/llm_predictor/vellum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llm_predictor/vellum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llm_predictor/vellum/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llm_predictor/vellum/test_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llm_predictor/vellum/test_prompt_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llm_predictor/vellum/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.260658 gpt_index-0.7.6/tests/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llms/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llms/test_anthropic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llms/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llms/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llms/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llms/test_openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/llms/test_palm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.260658 gpt_index-0.7.6/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.260658 gpt_index-0.7.6/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/objects/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/objects/test_node_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/output_parsers/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/output_parsers/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/output_parsers/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/program/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/program/test_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/program/test_llm_program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/prompts/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/prompts/test_guidance_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/question_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/question_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/question_gen/test_guidance_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/question_gen/test_llm_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/storage/docstore/test_dynamodb_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/storage/docstore/test_redis_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/storage/test_storage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.264658 gpt_index-0.7.6/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.268658 gpt_index-0.7.6/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/tools/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/tools/test_ondemand_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/tools/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.268658 gpt_index-0.7.6/tests/tools/tool_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/tools/tool_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/tools/tool_spec/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:34.268658 gpt_index-0.7.6/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/vector_stores/test_docarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/vector_stores/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/vector_stores/test_tair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-12 17:39:20.000000 gpt_index-0.7.6/tests/vector_stores/test_weaviate.py
```

### Comparing `gpt_index-0.7.5/LICENSE` & `gpt_index-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/PKG-INFO` & `gpt_index-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_index
-Version: 0.7.5
+Version: 0.7.6
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 Author: Jerry Liu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gpt_index-0.7.5/README.md` & `gpt_index-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/gpt_index.egg-info/PKG-INFO` & `gpt_index-0.7.6/gpt_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-index
-Version: 0.7.5
+Version: 0.7.6
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 Author: Jerry Liu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gpt_index-0.7.5/gpt_index.egg-info/SOURCES.txt` & `gpt_index-0.7.6/gpt_index.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 llama_index/schema.py
 llama_index/types.py
 llama_index/utils.py
 llama_index/agent/__init__.py
 llama_index/agent/context_retriever_agent.py
 llama_index/agent/openai_agent.py
 llama_index/agent/retriever_openai_agent.py
+llama_index/agent/types.py
+llama_index/agent/react/__init__.py
+llama_index/agent/react/base.py
+llama_index/agent/react/formatter.py
+llama_index/agent/react/output_parser.py
+llama_index/agent/react/prompts.py
+llama_index/agent/react/types.py
 llama_index/bridge/__init__.py
 llama_index/bridge/langchain.py
 llama_index/callbacks/__init__.py
 llama_index/callbacks/aim.py
 llama_index/callbacks/base.py
 llama_index/callbacks/llama_debug.py
 llama_index/callbacks/schema.py
@@ -167,14 +174,17 @@
 llama_index/llms/mock.py
 llama_index/llms/openai.py
 llama_index/llms/openai_utils.py
 llama_index/llms/palm.py
 llama_index/llms/utils.py
 llama_index/logger/__init__.py
 llama_index/logger/base.py
+llama_index/memory/__init__.py
+llama_index/memory/chat_memory_buffer.py
+llama_index/memory/types.py
 llama_index/node_parser/__init__.py
 llama_index/node_parser/interface.py
 llama_index/node_parser/node_utils.py
 llama_index/node_parser/simple.py
 llama_index/node_parser/extractors/__init__.py
 llama_index/node_parser/extractors/metadata_extractors.py
 llama_index/objects/__init__.py
@@ -356,14 +366,16 @@
 llama_index/tools/ondemand_loader_tool.py
 llama_index/tools/query_engine.py
 llama_index/tools/query_plan.py
 llama_index/tools/types.py
 llama_index/tools/utils.py
 llama_index/tools/tool_spec/__init__.py
 llama_index/tools/tool_spec/base.py
+llama_index/tools/tool_spec/load_and_search/__init__.py
+llama_index/tools/tool_spec/load_and_search/base.py
 llama_index/tools/tool_spec/notion/__init__.py
 llama_index/tools/tool_spec/notion/base.py
 llama_index/tools/tool_spec/slack/__init__.py
 llama_index/tools/tool_spec/slack/base.py
 llama_index/tts/__init__.py
 llama_index/tts/bark.py
 llama_index/tts/base.py
@@ -495,14 +507,15 @@
 tests/objects/__init__.py
 tests/objects/test_base.py
 tests/objects/test_node_mapping.py
 tests/output_parsers/__init__.py
 tests/output_parsers/test_base.py
 tests/output_parsers/test_pydantic.py
 tests/output_parsers/test_selection.py
+tests/output_parsers/test_utils.py
 tests/playground/__init__.py
 tests/playground/test_base.py
 tests/program/__init__.py
 tests/program/test_guidance.py
 tests/program/test_llm_program.py
 tests/prompts/__init__.py
 tests/prompts/test_base.py
```

### Comparing `gpt_index-0.7.5/llama_index/__init__.py` & `gpt_index-0.7.6/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/agent/context_retriever_agent.py` & `gpt_index-0.7.6/llama_index/agent/context_retriever_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Context retriever agent."""
 
-from typing import List, Optional
+from typing import List, Type, Optional
 
 from llama_index.agent.openai_agent import (
     DEFAULT_MAX_FUNCTION_CALLS,
     DEFAULT_MODEL_NAME,
     SUPPORTED_MODEL_NAMES,
     BaseOpenAIAgent,
 )
 from llama_index.bridge.langchain import print_text
+from llama_index.chat_engine.types import AgentChatResponse
 from llama_index.callbacks.base import CallbackManager
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.llms.base import ChatMessage
 from llama_index.llms.openai import OpenAI
+from llama_index.memory import BaseMemory, ChatMemoryBuffer
 from llama_index.prompts.prompts import QuestionAnswerPrompt
-from llama_index.response.schema import RESPONSE_TYPE
 from llama_index.schema import NodeWithScore
 from llama_index.tools import BaseTool
 
 # inspired by DEFAULT_QA_PROMPT_TMPL from llama_index/prompts/default_prompts.py
 DEFAULT_QA_PROMPT_TMPL = (
     "Context information is below.\n"
     "---------------------\n"
@@ -55,23 +56,23 @@
     def __init__(
         self,
         tools: List[BaseTool],
         retriever: BaseRetriever,
         qa_prompt: QuestionAnswerPrompt,
         context_separator: str,
         llm: OpenAI,
-        chat_history: List[ChatMessage],
+        memory: BaseMemory,
         prefix_messages: List[ChatMessage],
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         super().__init__(
             llm=llm,
-            chat_history=chat_history,
+            memory=memory,
             prefix_messages=prefix_messages,
             verbose=verbose,
             max_function_calls=max_function_calls,
             callback_manager=callback_manager,
         )
         self._tools = tools
         self._qa_prompt = qa_prompt
@@ -83,14 +84,16 @@
         cls,
         tools: List[BaseTool],
         retriever: BaseRetriever,
         qa_prompt: Optional[QuestionAnswerPrompt] = None,
         context_separator: str = "\n",
         llm: Optional[OpenAI] = None,
         chat_history: Optional[List[ChatMessage]] = None,
+        memory: Optional[BaseMemory] = None,
+        memory_cls: Type[BaseMemory] = ChatMemoryBuffer,
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
         prefix_messages: Optional[List[ChatMessage]] = None,
     ) -> "ContextRetrieverOpenAIAgent":
         """Create a ContextRetrieverOpenAIAgent from a retriever.
@@ -104,14 +107,15 @@
             verbose (bool): Whether to print debug statements.
             max_function_calls (int): Maximum number of function calls.
             callback_manager (Optional[CallbackManager]): A callback manager.
 
         """
         qa_prompt = qa_prompt or DEFAULT_QA_PROMPT
         chat_history = chat_history or []
+        memory = memory or memory_cls.from_defaults(chat_history=chat_history)
         llm = llm or OpenAI(model=DEFAULT_MODEL_NAME)
         if not isinstance(llm, OpenAI):
             raise ValueError("llm must be a OpenAI instance")
 
         if llm.model not in SUPPORTED_MODEL_NAMES:
             raise ValueError(
                 f"Model name {llm.model} not supported. "
@@ -128,28 +132,28 @@
 
         return cls(
             tools=tools,
             retriever=retriever,
             qa_prompt=qa_prompt,
             context_separator=context_separator,
             llm=llm,
-            chat_history=chat_history,
+            memory=memory,
             prefix_messages=prefix_messages,
             verbose=verbose,
             max_function_calls=max_function_calls,
             callback_manager=callback_manager,
         )
 
     def _get_tools(self, message: str) -> List[BaseTool]:
         """Get tools."""
         return self._tools
 
     def chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> RESPONSE_TYPE:
+    ) -> AgentChatResponse:
         """Chat."""
         # augment user message
         retrieved_nodes_w_scores: List[NodeWithScore] = self._retriever.retrieve(
             message
         )
         retrieved_nodes = [node.node for node in retrieved_nodes_w_scores]
         retrieved_texts = [node.get_content() for node in retrieved_nodes]
```

### Comparing `gpt_index-0.7.5/llama_index/agent/openai_agent.py` & `gpt_index-0.7.6/llama_index/agent/openai_agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import asyncio
 import json
 import time
 from abc import abstractmethod
 from threading import Thread
 from typing import (
-    AsyncGenerator,
     Callable,
-    Generator,
     List,
     Tuple,
+    Type,
     Optional,
 )
 
-from llama_index.callbacks.base import CallbackManager
 from llama_index.chat_engine.types import (
-    BaseChatEngine,
-    StreamingChatResponse,
-    STREAMING_CHAT_RESPONSE_TYPE,
+    AgentChatResponse,
+    StreamingAgentChatResponse,
 )
+from llama_index.callbacks.base import CallbackManager
 from llama_index.indices.base_retriever import BaseRetriever
-from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.llms.base import (
     ChatMessage,
     MessageRole,
 )
 from llama_index.llms.openai import OpenAI
+from llama_index.memory import BaseMemory, ChatMemoryBuffer
 from llama_index.response.schema import RESPONSE_TYPE, Response
 from llama_index.schema import BaseNode, NodeWithScore
-from llama_index.tools import BaseTool
+from llama_index.agent.types import BaseAgent
+from llama_index.tools import BaseTool, ToolOutput
 
 DEFAULT_MAX_FUNCTION_CALLS = 5
 DEFAULT_MODEL_NAME = "gpt-3.5-turbo-0613"
 SUPPORTED_MODEL_NAMES = [
     "gpt-3.5-turbo-0613",
     "gpt-4-0613",
 ]
@@ -44,341 +43,353 @@
     if name not in name_to_tool:
         raise ValueError(f"Tool with name {name} not found")
     return name_to_tool[name]
 
 
 def call_function(
     tools: List[BaseTool], function_call: dict, verbose: bool = False
-) -> ChatMessage:
+) -> Tuple[ChatMessage, ToolOutput]:
     """Call a function and return the output as a string."""
     name = function_call["name"]
     arguments_str = function_call["arguments"]
     if verbose:
         print("=== Calling Function ===")
         print(f"Calling function: {name} with args: {arguments_str}")
     tool = get_function_by_name(tools, name)
     argument_dict = json.loads(arguments_str)
     output = tool(**argument_dict)
     if verbose:
-        print(f"Got output: {output}")
+        print(f"Got output: {str(output)}")
         print("========================")
-    return ChatMessage(
-        content=str(output),
-        role=MessageRole.FUNCTION,
-        additional_kwargs={
-            "name": function_call["name"],
-        },
+    return (
+        ChatMessage(
+            content=str(output),
+            role=MessageRole.FUNCTION,
+            additional_kwargs={
+                "name": function_call["name"],
+            },
+        ),
+        output,
     )
 
 
-class BaseOpenAIAgent(BaseChatEngine, BaseQueryEngine):
+class BaseOpenAIAgent(BaseAgent):
     """Base OpenAI Agent."""
 
     def __init__(
         self,
         llm: OpenAI,
-        chat_history: List[ChatMessage],
+        memory: BaseMemory,
         prefix_messages: List[ChatMessage],
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         self._llm = llm
-        self._chat_history = chat_history
+        self._memory = memory
         self._prefix_messages = prefix_messages
         self._verbose = verbose
         self._max_function_calls = max_function_calls
         self.callback_manager = callback_manager or CallbackManager([])
 
     @property
     def chat_history(self) -> List[ChatMessage]:
-        return self._chat_history
+        return self._memory.get_all()
 
     def reset(self) -> None:
-        self._chat_history.clear()
+        self._memory.reset()
 
     @abstractmethod
     def _get_tools(self, message: str) -> List[BaseTool]:
         """Get tools."""
 
     def _get_latest_function_call(
         self, chat_history: List[ChatMessage]
     ) -> Optional[dict]:
         """Get latest function call from chat history."""
         return chat_history[-1].additional_kwargs.get("function_call", None)
 
-    def _init_chat(
-        self, chat_history: List[ChatMessage], message: str
-    ) -> Tuple[List[BaseTool], List[dict]]:
+    def _init_chat(self, message: str) -> Tuple[List[BaseTool], List[dict]]:
         """Add user message to chat history and get tools and functions."""
-        chat_history.append(ChatMessage(content=message, role=MessageRole.USER))
+        self._memory.put(ChatMessage(content=message, role=MessageRole.USER))
         tools = self._get_tools(message)
         functions = [tool.metadata.to_openai_function() for tool in tools]
         return tools, functions
 
     def chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> RESPONSE_TYPE:
-        chat_history = chat_history or self._chat_history
-        tools, functions = self._init_chat(chat_history, message)
+    ) -> AgentChatResponse:
+        if chat_history is not None:
+            self._memory.set(chat_history)
+
+        tools, functions = self._init_chat(message)
+        sources = []
 
         # TODO: Support forced function call
-        all_messages = self._prefix_messages + chat_history
+        all_messages = self._prefix_messages + self._memory.get()
         chat_response = self._llm.chat(all_messages, functions=functions)
         ai_message = chat_response.message
-        chat_history.append(ai_message)
+        self._memory.put(ai_message)
 
         n_function_calls = 0
-        function_call = self._get_latest_function_call(chat_history)
+        function_call = self._get_latest_function_call(self._memory.get_all())
         while function_call is not None:
             if n_function_calls >= self._max_function_calls:
                 print(f"Exceeded max function calls: {self._max_function_calls}.")
                 break
 
-            function_message = call_function(
+            function_message, tool_output = call_function(
                 tools, function_call, verbose=self._verbose
             )
-            chat_history.append(function_message)
+            sources.append(tool_output)
+            self._memory.put(function_message)
             n_function_calls += 1
 
             # send function call & output back to get another response
-            all_messages = self._prefix_messages + chat_history
+            all_messages = self._prefix_messages + self._memory.get()
             chat_response = self._llm.chat(all_messages, functions=functions)
             ai_message = chat_response.message
-            chat_history.append(ai_message)
-            function_call = self._get_latest_function_call(chat_history)
+            self._memory.put(ai_message)
+            function_call = self._get_latest_function_call(self._memory.get_all())
 
-        return Response(ai_message.content)
+        return AgentChatResponse(response=str(ai_message.content), sources=sources)
 
     def stream_chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> STREAMING_CHAT_RESPONSE_TYPE:
-        chat_history = chat_history or self._chat_history
-        tools, functions = self._init_chat(chat_history, message)
-
-        def gen(
-            chat_history: List[ChatMessage],
-        ) -> Generator[StreamingChatResponse, None, None]:
-            # TODO: Support forced function call
-            all_messages = self._prefix_messages + chat_history
-            chat_stream_response = StreamingChatResponse(
-                self._llm.stream_chat(all_messages, functions=functions)
+    ) -> StreamingAgentChatResponse:
+        if chat_history is not None:
+            self._memory.set(chat_history)
+        tools, functions = self._init_chat(message)
+        all_messages = self._prefix_messages + self._memory.get()
+        sources = []
+
+        # TODO: Support forced function call
+        chat_stream_response = StreamingAgentChatResponse(
+            chat_stream=self._llm.stream_chat(all_messages, functions=functions)
+        )
+
+        # Get the response in a separate thread so we can yield the response
+        thread = Thread(
+            target=chat_stream_response.write_response_to_history,
+            args=(self._memory,),
+        )
+        thread.start()
+
+        while chat_stream_response._is_function is None:
+            # Wait until we know if the response is a function call or not
+            time.sleep(0.05)
+            if chat_stream_response._is_function is False:
+                return chat_stream_response
+
+        thread.join()
+
+        n_function_calls = 0
+        function_call = self._get_latest_function_call(self._memory.get_all())
+        while function_call is not None:
+            if n_function_calls >= self._max_function_calls:
+                print(f"Exceeded max function calls: {self._max_function_calls}.")
+                break
+
+            function_message, tool_output = call_function(
+                tools, function_call, verbose=self._verbose
+            )
+            sources.append(tool_output)
+            self._memory.put(function_message)
+            n_function_calls += 1
+
+            # send function call & output back to get another response
+            all_messages = self._prefix_messages + self._memory.get()
+            chat_stream_response = StreamingAgentChatResponse(
+                chat_stream=self._llm.stream_chat(all_messages, functions=functions),
+                sources=sources,
             )
 
             # Get the response in a separate thread so we can yield the response
             thread = Thread(
                 target=chat_stream_response.write_response_to_history,
-                args=(chat_history,),
+                args=(self._memory,),
             )
             thread.start()
-            yield chat_stream_response
-
             while chat_stream_response._is_function is None:
                 # Wait until we know if the response is a function call or not
                 time.sleep(0.05)
                 if chat_stream_response._is_function is False:
-                    return
+                    return chat_stream_response
 
             thread.join()
+            function_call = self._get_latest_function_call(self._memory.get_all())
 
-            n_function_calls = 0
-            function_call = self._get_latest_function_call(chat_history)
-            while function_call is not None:
-                if n_function_calls >= self._max_function_calls:
-                    print(f"Exceeded max function calls: {self._max_function_calls}.")
-                    break
-
-                function_message = call_function(
-                    tools, function_call, verbose=self._verbose
-                )
-                chat_history.append(function_message)
-                n_function_calls += 1
-
-                all_messages = self._prefix_messages + chat_history
-                # send function call & output back to get another response
-                chat_stream_response = StreamingChatResponse(
-                    self._llm.stream_chat(all_messages, functions=functions)
-                )
-
-                # Get the response in a separate thread so we can yield the response
-                thread = Thread(
-                    target=chat_stream_response.write_response_to_history,
-                    args=(chat_history,),
-                )
-                thread.start()
-                yield chat_stream_response
-
-                while chat_stream_response._is_function is None:
-                    # Wait until we know if the response is a function call or not
-                    time.sleep(0.05)
-                    if chat_stream_response._is_function is False:
-                        return
-
-                thread.join()
-                function_call = self._get_latest_function_call(chat_history)
-
-        return gen(chat_history)
+        return chat_stream_response
 
     async def achat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> RESPONSE_TYPE:
-        chat_history = chat_history or self._chat_history
-        tools, functions = self._init_chat(chat_history, message)
+    ) -> AgentChatResponse:
+        if chat_history is not None:
+            self._memory.set(chat_history)
+        all_messages = self._prefix_messages + self._memory.get()
+        tools, functions = self._init_chat(message)
+        sources = []
 
         # TODO: Support forced function call
-        all_messages = self._prefix_messages + chat_history
         chat_response = await self._llm.achat(all_messages, functions=functions)
         ai_message = chat_response.message
-        chat_history.append(ai_message)
+        self._memory.put(ai_message)
 
         n_function_calls = 0
-        function_call = self._get_latest_function_call(chat_history)
+        function_call = self._get_latest_function_call(self._memory.get_all())
         while function_call is not None:
             if n_function_calls >= self._max_function_calls:
                 print(f"Exceeded max function calls: {self._max_function_calls}.")
                 continue
 
-            function_message = call_function(
+            function_message, tool_output = call_function(
                 tools, function_call, verbose=self._verbose
             )
-            chat_history.append(function_message)
+            sources.append(tool_output)
+            self._memory.put(function_message)
             n_function_calls += 1
 
             # send function call & output back to get another response
             response = await self._llm.achat(
-                self._prefix_messages + chat_history, functions=functions
+                self._prefix_messages + self._memory.get(), functions=functions
             )
             ai_message = response.message
-            chat_history.append(ai_message)
-            function_call = self._get_latest_function_call(chat_history)
+            self._memory.put(ai_message)
+            function_call = self._get_latest_function_call(self._memory.get_all())
 
-        return Response(ai_message.content)
+        return AgentChatResponse(response=str(ai_message.content), sources=sources)
 
     async def astream_chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> STREAMING_CHAT_RESPONSE_TYPE:
-        chat_history = chat_history or self._chat_history
-        tools, functions = self._init_chat(chat_history, message)
-
-        async def gen(
-            chat_history: List[ChatMessage],
-        ) -> AsyncGenerator[StreamingChatResponse, None]:
-            all_messages = self._prefix_messages + chat_history
-            # TODO: Support forced function call
-            chat_stream_response = StreamingChatResponse(
-                await self._llm.astream_chat(all_messages, functions=functions)
+    ) -> StreamingAgentChatResponse:
+        if chat_history is not None:
+            self._memory.set(chat_history)
+        tools, functions = self._init_chat(message)
+        all_messages = self._prefix_messages + self._memory.get()
+        sources = []
+
+        # TODO: Support forced function call
+        chat_stream_response = StreamingAgentChatResponse(
+            achat_stream=await self._llm.astream_chat(all_messages, functions=functions)
+        )
+
+        # Get the response in a separate thread so we can yield the response
+        thread = Thread(
+            target=lambda x: asyncio.run(
+                chat_stream_response.awrite_response_to_history(x)
+            ),
+            args=(self._memory,),
+        )
+        thread.start()
+
+        while chat_stream_response._is_function is None:
+            # Wait until we know if the response is a function call or not
+            time.sleep(0.05)
+            if chat_stream_response._is_function is False:
+                return chat_stream_response
+
+        thread.join()
+
+        n_function_calls = 0
+        function_call = self._get_latest_function_call(self._memory.get_all())
+        while function_call is not None:
+            if n_function_calls >= self._max_function_calls:
+                print(f"Exceeded max function calls: {self._max_function_calls}.")
+                break
+
+            function_message, tool_output = call_function(
+                tools, function_call, verbose=self._verbose
+            )
+            sources.append(tool_output)
+            self._memory.put(function_message)
+            n_function_calls += 1
+
+            # send function call & output back to get another response
+            all_messages = self._prefix_messages + self._memory.get()
+            chat_stream_response = StreamingAgentChatResponse(
+                achat_stream=await self._llm.astream_chat(
+                    all_messages, functions=functions
+                ),
+                sources=sources,
             )
 
             # Get the response in a separate thread so we can yield the response
             thread = Thread(
                 target=lambda x: asyncio.run(
                     chat_stream_response.awrite_response_to_history(x)
                 ),
-                args=(chat_history,),
+                args=(self._memory,),
             )
             thread.start()
-            yield chat_stream_response
 
             while chat_stream_response._is_function is None:
                 # Wait until we know if the response is a function call or not
                 time.sleep(0.05)
                 if chat_stream_response._is_function is False:
-                    return
+                    return chat_stream_response
 
             thread.join()
+            function_call = self._get_latest_function_call(self._memory.get_all())
 
-            n_function_calls = 0
-            function_call = self._get_latest_function_call(chat_history)
-            while function_call is not None:
-                if n_function_calls >= self._max_function_calls:
-                    print(f"Exceeded max function calls: {self._max_function_calls}.")
-                    break
-
-                function_message = call_function(
-                    tools, function_call, verbose=self._verbose
-                )
-                chat_history.append(function_message)
-                n_function_calls += 1
-
-                # send function call & output back to get another response
-                all_messages = self._prefix_messages + chat_history
-                chat_stream_response = StreamingChatResponse(
-                    await self._llm.astream_chat(all_messages, functions=functions)
-                )
-
-                # Get the response in a separate thread so we can yield the response
-                thread = Thread(
-                    target=lambda x: asyncio.run(
-                        chat_stream_response.awrite_response_to_history(x)
-                    ),
-                    args=(chat_history,),
-                )
-                thread.start()
-                yield chat_stream_response
-
-                while chat_stream_response._is_function is None:
-                    # Wait until we know if the response is a function call or not
-                    time.sleep(0.05)
-                    if chat_stream_response._is_function is False:
-                        return
-
-                thread.join()
-                function_call = self._get_latest_function_call(chat_history)
-
-        return gen(chat_history)
+        return chat_stream_response
 
     # ===== Query Engine Interface =====
     def _query(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
-        return self.chat(
+        agent_response = self.chat(
             query_bundle.query_str,
             chat_history=[],
         )
+        return Response(response=str(agent_response))
 
     async def _aquery(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
-        return await self.achat(
+        agent_response = await self.achat(
             query_bundle.query_str,
             chat_history=[],
         )
+        return Response(response=str(agent_response))
 
 
 class OpenAIAgent(BaseOpenAIAgent):
     def __init__(
         self,
         tools: List[BaseTool],
         llm: OpenAI,
-        chat_history: List[ChatMessage],
+        memory: BaseMemory,
         prefix_messages: List[ChatMessage],
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         super().__init__(
             llm=llm,
-            chat_history=chat_history,
+            memory=memory,
             prefix_messages=prefix_messages,
             verbose=verbose,
             max_function_calls=max_function_calls,
             callback_manager=callback_manager,
         )
         self._tools = tools
 
     @classmethod
     def from_tools(
         cls,
         tools: Optional[List[BaseTool]] = None,
         llm: Optional[OpenAI] = None,
         chat_history: Optional[List[ChatMessage]] = None,
+        memory: Optional[BaseMemory] = None,
+        memory_cls: Type[BaseMemory] = ChatMemoryBuffer,
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
         prefix_messages: Optional[List[ChatMessage]] = None,
     ) -> "OpenAIAgent":
         tools = tools or []
         chat_history = chat_history or []
+        memory = memory or memory_cls.from_defaults(chat_history)
         llm = llm or OpenAI(model=DEFAULT_MODEL_NAME)
         if not isinstance(llm, OpenAI):
             raise ValueError("llm must be a OpenAI instance")
 
         if llm.model not in SUPPORTED_MODEL_NAMES:
             raise ValueError(
                 f"Model name {llm.model} not supported. "
@@ -393,15 +404,15 @@
             prefix_messages = [ChatMessage(content=system_prompt, role="system")]
 
         prefix_messages = prefix_messages or []
 
         return cls(
             tools=tools,
             llm=llm,
-            chat_history=chat_history,
+            memory=memory,
             prefix_messages=prefix_messages,
             verbose=verbose,
             max_function_calls=max_function_calls,
             callback_manager=callback_manager,
         )
 
     def _get_tools(self, message: str) -> List[BaseTool]:
@@ -424,23 +435,23 @@
     """
 
     def __init__(
         self,
         retriever: BaseRetriever,
         node_to_tool_fn: Callable[[BaseNode], BaseTool],
         llm: OpenAI,
-        chat_history: List[ChatMessage],
+        memory: BaseMemory,
         prefix_messages: List[ChatMessage],
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         super().__init__(
             llm=llm,
-            chat_history=chat_history,
+            memory=memory,
             prefix_messages=prefix_messages,
             verbose=verbose,
             max_function_calls=max_function_calls,
             callback_manager=callback_manager,
         )
         self._retriever = retriever
         self._node_to_tool_fn = node_to_tool_fn
@@ -448,21 +459,25 @@
     @classmethod
     def from_retriever(
         cls,
         retriever: BaseRetriever,
         node_to_tool_fn: Callable[[BaseNode], BaseTool],
         llm: Optional[OpenAI] = None,
         chat_history: Optional[List[ChatMessage]] = None,
+        memory: Optional[BaseMemory] = None,
+        memory_cls: Type[BaseMemory] = ChatMemoryBuffer,
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
         prefix_messages: Optional[List[ChatMessage]] = None,
     ) -> "RetrieverOpenAIAgent":
-        lc_chat_history = chat_history or []
+        chat_history = chat_history or []
+        memory = memory or memory_cls.from_defaults(chat_history)
+
         llm = llm or OpenAI(model=DEFAULT_MODEL_NAME)
         if not isinstance(llm, OpenAI):
             raise ValueError("llm must be a OpenAI instance")
 
         if llm.model not in SUPPORTED_MODEL_NAMES:
             raise ValueError(
                 f"Model name {llm.model} not supported. "
@@ -478,15 +493,15 @@
 
         prefix_messages = prefix_messages or []
 
         return cls(
             retriever=retriever,
             node_to_tool_fn=node_to_tool_fn,
             llm=llm,
-            chat_history=lc_chat_history,
+            memory=memory,
             prefix_messages=prefix_messages,
             verbose=verbose,
             max_function_calls=max_function_calls,
             callback_manager=callback_manager,
         )
 
     def _get_tools(self, message: str) -> List[BaseTool]:
```

### Comparing `gpt_index-0.7.5/llama_index/agent/retriever_openai_agent.py` & `gpt_index-0.7.6/llama_index/agent/retriever_openai_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Retriever OpenAI agent."""
 
-from typing import List, Optional
+from typing import List, Type, Optional
 
 from llama_index.agent.openai_agent import (
     DEFAULT_MAX_FUNCTION_CALLS,
     DEFAULT_MODEL_NAME,
     SUPPORTED_MODEL_NAMES,
     BaseOpenAIAgent,
 )
 from llama_index.callbacks.base import CallbackManager
 from llama_index.llms.base import ChatMessage
 from llama_index.llms.openai import OpenAI
+from llama_index.memory import BaseMemory, ChatMemoryBuffer
 from llama_index.objects.base import ObjectRetriever
 from llama_index.tools.types import BaseTool
 
 
 class FnRetrieverOpenAIAgent(BaseOpenAIAgent):
     """Function Retriever OpenAI Agent.
 
@@ -22,43 +23,46 @@
 
     """
 
     def __init__(
         self,
         retriever: ObjectRetriever[BaseTool],
         llm: OpenAI,
-        chat_history: List[ChatMessage],
+        memory: BaseMemory,
         prefix_messages: List[ChatMessage],
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         super().__init__(
             llm=llm,
-            chat_history=chat_history,
+            memory=memory,
             prefix_messages=prefix_messages,
             verbose=verbose,
             max_function_calls=max_function_calls,
             callback_manager=callback_manager,
         )
         self._retriever = retriever
 
     @classmethod
     def from_retriever(
         cls,
         retriever: ObjectRetriever[BaseTool],
         llm: Optional[OpenAI] = None,
         chat_history: Optional[List[ChatMessage]] = None,
+        memory: Optional[BaseMemory] = None,
+        memory_cls: Type[BaseMemory] = ChatMemoryBuffer,
         verbose: bool = False,
         max_function_calls: int = DEFAULT_MAX_FUNCTION_CALLS,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
         prefix_messages: Optional[List[ChatMessage]] = None,
     ) -> "FnRetrieverOpenAIAgent":
         chat_history = chat_history or []
+        memory = memory or memory_cls.from_defaults(chat_history=chat_history)
         llm = llm or OpenAI(model=DEFAULT_MODEL_NAME)
         if not isinstance(llm, OpenAI):
             raise ValueError("llm must be a OpenAI instance")
 
         if llm.model not in SUPPORTED_MODEL_NAMES:
             raise ValueError(
                 f"Model name {llm.model} not supported. "
@@ -72,15 +76,15 @@
             prefix_messages = [ChatMessage(content=system_prompt, role="system")]
 
         prefix_messages = prefix_messages or []
 
         return cls(
             retriever=retriever,
             llm=llm,
-            chat_history=chat_history,
+            memory=memory,
             prefix_messages=prefix_messages,
             verbose=verbose,
             max_function_calls=max_function_calls,
             callback_manager=callback_manager,
         )
 
     def _get_tools(self, message: str) -> List[BaseTool]:
```

### Comparing `gpt_index-0.7.5/llama_index/async_utils.py` & `gpt_index-0.7.6/llama_index/async_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/bridge/langchain.py` & `gpt_index-0.7.6/llama_index/bridge/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/callbacks/aim.py` & `gpt_index-0.7.6/llama_index/callbacks/aim.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/callbacks/base.py` & `gpt_index-0.7.6/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/callbacks/llama_debug.py` & `gpt_index-0.7.6/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/callbacks/schema.py` & `gpt_index-0.7.6/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/callbacks/token_counting.py` & `gpt_index-0.7.6/llama_index/callbacks/token_counting.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/callbacks/wandb_callback.py` & `gpt_index-0.7.6/llama_index/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/chat_engine/condense_question.py` & `gpt_index-0.7.6/llama_index/chat_engine/condense_question.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import logging
-from typing import Any, List, Optional
+from typing import Any, List, Type, Optional
 
-from llama_index.chat_engine.types import BaseChatEngine, STREAMING_CHAT_RESPONSE_TYPE
+from llama_index.chat_engine.types import (
+    BaseChatEngine,
+    AgentChatResponse,
+    StreamingAgentChatResponse,
+)
 from llama_index.chat_engine.utils import response_gen_with_chat_history
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.service_context import ServiceContext
 from llama_index.llms.base import ChatMessage, MessageRole
 from llama_index.llms.generic_utils import messages_to_history_str
+from llama_index.memory import BaseMemory, ChatMemoryBuffer
 from llama_index.prompts.base import Prompt
-from llama_index.response.schema import RESPONSE_TYPE, StreamingResponse
+from llama_index.response.schema import StreamingResponse, RESPONSE_TYPE
+from llama_index.tools import ToolOutput
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_TEMPLATE = """\
 Given a conversation (between Human and Assistant) and a follow up message from Human, \
 rewrite the message to be a standalone question that captures all relevant context \
@@ -37,54 +43,57 @@
     then query the query engine for a response.
     """
 
     def __init__(
         self,
         query_engine: BaseQueryEngine,
         condense_question_prompt: Prompt,
-        chat_history: List[ChatMessage],
+        memory: BaseMemory,
         service_context: ServiceContext,
         verbose: bool = False,
     ) -> None:
         self._query_engine = query_engine
         self._condense_question_prompt = condense_question_prompt
-        self._chat_history = chat_history
+        self._memory = memory
         self._service_context = service_context
         self._verbose = verbose
 
     @classmethod
     def from_defaults(
         cls,
         query_engine: BaseQueryEngine,
         condense_question_prompt: Optional[Prompt] = None,
         chat_history: Optional[List[ChatMessage]] = None,
+        memory: Optional[BaseMemory] = None,
+        memory_cls: Type[BaseMemory] = ChatMemoryBuffer,
         service_context: Optional[ServiceContext] = None,
         verbose: bool = False,
         system_prompt: Optional[str] = None,
         prefix_messages: Optional[List[ChatMessage]] = None,
         **kwargs: Any,
     ) -> "CondenseQuestionChatEngine":
         """Initialize a CondenseQuestionChatEngine from default parameters."""
         condense_question_prompt = condense_question_prompt or DEFAULT_PROMPT
         chat_history = chat_history or []
+        memory = memory or memory_cls.from_defaults(chat_history=chat_history)
         service_context = service_context or ServiceContext.from_defaults()
 
         if system_prompt is not None:
             raise NotImplementedError(
                 "system_prompt is not supported for CondenseQuestionChatEngine."
             )
         if prefix_messages is not None:
             raise NotImplementedError(
                 "prefix_messages is not supported for CondenseQuestionChatEngine."
             )
 
         return cls(
             query_engine,
             condense_question_prompt,
-            chat_history,
+            memory,
             service_context,
             verbose=verbose,
         )
 
     def _condense_question(
         self, chat_history: List[ChatMessage], last_message: str
     ) -> str:
@@ -115,132 +124,150 @@
         response = await self._service_context.llm_predictor.apredict(
             self._condense_question_prompt,
             question=last_message,
             chat_history=chat_history_str,
         )
         return response
 
+    def _get_tool_output_from_response(
+        self, query: str, response: RESPONSE_TYPE
+    ) -> ToolOutput:
+        return ToolOutput(
+            content=str(response),
+            tool_name="query_engine",
+            raw_input={"query": query},
+            raw_output=response,
+        )
+
     def chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> RESPONSE_TYPE:
-        chat_history = chat_history or self._chat_history
+    ) -> AgentChatResponse:
+        chat_history = chat_history or self._memory.get()
 
         # Generate standalone question from conversation context and last message
         condensed_question = self._condense_question(chat_history, message)
 
         log_str = f"Querying with: {condensed_question}"
         logger.info(log_str)
         if self._verbose:
             print(log_str)
 
         # Query with standalone question
-        response = self._query_engine.query(condensed_question)
+        query_response = self._query_engine.query(condensed_question)
+        tool_output = self._get_tool_output_from_response(
+            condensed_question, query_response
+        )
 
         # Record response
-        chat_history.extend(
-            [
-                ChatMessage(role=MessageRole.USER, content=message),
-                ChatMessage(role=MessageRole.ASSISTANT, content=str(response)),
-            ]
+        self._memory.put(ChatMessage(role=MessageRole.USER, content=message))
+        self._memory.put(
+            ChatMessage(role=MessageRole.ASSISTANT, content=str(query_response))
         )
-        return response
+
+        return AgentChatResponse(response=str(query_response), sources=[tool_output])
 
     def stream_chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> STREAMING_CHAT_RESPONSE_TYPE:
-        chat_history = chat_history or self._chat_history
+    ) -> StreamingAgentChatResponse:
+        chat_history = chat_history or self._memory.get()
 
         # Generate standalone question from conversation context and last message
         condensed_question = self._condense_question(chat_history, message)
 
         log_str = f"Querying with: {condensed_question}"
         logger.info(log_str)
         if self._verbose:
             print(log_str)
 
         # Query with standalone question
-        response = self._query_engine.query(condensed_question)
+        query_response = self._query_engine.query(condensed_question)
+        tool_output = self._get_tool_output_from_response(
+            condensed_question, query_response
+        )
 
         # Record response
         if (
-            isinstance(response, StreamingResponse)
-            and response.response_gen is not None
+            isinstance(query_response, StreamingResponse)
+            and query_response.response_gen is not None
         ):
             # override the generator to include writing to chat history
-            response = StreamingResponse(
-                response_gen_with_chat_history(
-                    message, chat_history, response.response_gen
+            response = StreamingAgentChatResponse(
+                chat_stream=response_gen_with_chat_history(
+                    message, self._memory, query_response.response_gen
                 ),
-                source_nodes=response.source_nodes,
-                metadata=response.metadata,
+                sources=[tool_output],
             )
         else:
             raise ValueError("Streaming is not enabled. Please use chat() instead.")
         return response
 
     async def achat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> RESPONSE_TYPE:
-        chat_history = chat_history or self._chat_history
+    ) -> AgentChatResponse:
+        chat_history = chat_history or self._memory.get()
 
         # Generate standalone question from conversation context and last message
         condensed_question = await self._acondense_question(chat_history, message)
 
         log_str = f"Querying with: {condensed_question}"
         logger.info(log_str)
         if self._verbose:
             print(log_str)
 
         # Query with standalone question
-        response = await self._query_engine.aquery(condensed_question)
+        query_response = await self._query_engine.aquery(condensed_question)
+        tool_output = self._get_tool_output_from_response(
+            condensed_question, query_response
+        )
 
         # Record response
-        chat_history.extend(
-            [
-                ChatMessage(role=MessageRole.USER, content=message),
-                ChatMessage(role=MessageRole.ASSISTANT, content=str(response)),
-            ]
+        self._memory.put(ChatMessage(role=MessageRole.USER, content=message))
+        self._memory.put(
+            ChatMessage(role=MessageRole.ASSISTANT, content=str(query_response))
         )
 
-        return response
+        return AgentChatResponse(response=str(query_response), sources=[tool_output])
 
     async def astream_chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> STREAMING_CHAT_RESPONSE_TYPE:
-        chat_history = chat_history or self._chat_history
+    ) -> StreamingAgentChatResponse:
+        chat_history = chat_history or self._memory.get()
 
         # Generate standalone question from conversation context and last message
         condensed_question = await self._acondense_question(chat_history, message)
 
         log_str = f"Querying with: {condensed_question}"
         logger.info(log_str)
         if self._verbose:
             print(log_str)
 
         # Query with standalone question
-        response = await self._query_engine.aquery(condensed_question)
+        query_response = await self._query_engine.aquery(condensed_question)
+        tool_output = self._get_tool_output_from_response(
+            condensed_question, query_response
+        )
 
         # Record response
         if (
-            isinstance(response, StreamingResponse)
-            and response.response_gen is not None
+            isinstance(query_response, StreamingResponse)
+            and query_response.response_gen is not None
         ):
             # override the generator to include writing to chat history
-            response = StreamingResponse(
-                response_gen_with_chat_history(
-                    message, chat_history, response.response_gen
+            # TODO: query engine does not support async generator yet
+            response = StreamingAgentChatResponse(
+                chat_stream=response_gen_with_chat_history(
+                    message, self._memory, query_response.response_gen
                 ),
-                source_nodes=response.source_nodes,
-                metadata=response.metadata,
+                sources=[tool_output],
             )
         else:
             raise ValueError("Streaming is not enabled. Please use achat() instead.")
         return response
 
     def reset(self) -> None:
         # Clear chat history
-        self._chat_history = []
+        self._memory.reset()
 
     @property
     def chat_history(self) -> List[ChatMessage]:
-        """Get chat history as human and ai message pairs."""
-        return self._chat_history
+        """Get chat history."""
+        return self._memory.get_all()
```

### Comparing `gpt_index-0.7.5/llama_index/chat_engine/react.py` & `gpt_index-0.7.6/llama_index/chat_engine/react.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from typing import Any, List, Optional, Sequence
 
 from llama_index.bridge.langchain import (
     BaseChatMemory,
     ChatMessageHistory,
     ConversationBufferMemory,
 )
-from llama_index.chat_engine.types import BaseChatEngine, STREAMING_CHAT_RESPONSE_TYPE
+from llama_index.chat_engine.types import (
+    BaseChatEngine,
+    AgentChatResponse,
+    StreamingAgentChatResponse,
+)
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.service_context import ServiceContext
 from llama_index.langchain_helpers.agents.agents import (
     AgentExecutor,
     AgentType,
     initialize_agent,
 )
@@ -17,15 +21,14 @@
 from llama_index.llms.base import ChatMessage
 from llama_index.llms.langchain import LangChainLLM
 from llama_index.llms.langchain_utils import (
     from_lc_messages,
     is_chat_model,
     to_lc_messages,
 )
-from llama_index.response.schema import RESPONSE_TYPE, Response
 from llama_index.tools.query_engine import QueryEngineTool
 
 
 class ReActChatEngine(BaseChatEngine):
     """ReAct Chat Engine.
 
     Use a ReAct agent loop with query engine tools. Implemented via LangChain agent.
@@ -144,42 +147,42 @@
     @property
     def chat_history(self) -> List[ChatMessage]:
         assert isinstance(self._memory, ConversationBufferMemory)
         return from_lc_messages(self._memory.chat_memory.messages)
 
     def chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> RESPONSE_TYPE:
+    ) -> AgentChatResponse:
         if chat_history is not None:
             raise NotImplementedError(
                 "chat_history argument is not supported for ReActChatEngine."
             )
 
         response = self._agent.run(input=message)
-        return Response(response=response)
+        return AgentChatResponse(response=response)
 
     async def achat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> RESPONSE_TYPE:
+    ) -> AgentChatResponse:
         if chat_history is not None:
             raise NotImplementedError(
                 "chat_history argument is not supported for ReActChatEngine."
             )
 
         response = await self._agent.arun(input=message)
-        return Response(response=response)
+        return AgentChatResponse(response=response)
 
     def stream_chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> STREAMING_CHAT_RESPONSE_TYPE:
+    ) -> StreamingAgentChatResponse:
         raise NotImplementedError("stream_chat() is not supported for ReActChatEngine.")
 
     async def astream_chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> STREAMING_CHAT_RESPONSE_TYPE:
+    ) -> StreamingAgentChatResponse:
         raise NotImplementedError(
             "astream_chat() is not supported for ReActChatEngine."
         )
 
     def reset(self) -> None:
         self._memory.clear()
         self._agent = self._create_agent()
```

### Comparing `gpt_index-0.7.5/llama_index/chat_engine/types.py` & `gpt_index-0.7.6/llama_index/chat_engine/types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,128 +1,134 @@
 import logging
 import queue
 from abc import ABC, abstractmethod
+from dataclasses import dataclass, field
 from enum import Enum
-from typing import AsyncGenerator, Generator, List, Optional, Union
+from typing import Generator, List, Optional
 
+from llama_index.tools import ToolOutput
 from llama_index.llms.base import ChatMessage, ChatResponseGen, ChatResponseAsyncGen
-from llama_index.response.schema import RESPONSE_TYPE, StreamingResponse
+from llama_index.memory import BaseMemory
 
 logger = logging.getLogger(__name__)
 
 
-class StreamingChatResponse:
+@dataclass
+class AgentChatResponse:
+    """Agent chat response."""
+
+    response: str = ""
+    sources: List[ToolOutput] = field(default_factory=list)
+
+    def __str__(self) -> str:
+        return self.response
+
+
+@dataclass
+class StreamingAgentChatResponse:
     """Streaming chat response to user and writing to chat history."""
 
-    def __init__(
-        self, chat_stream: Union[ChatResponseGen, ChatResponseAsyncGen]
-    ) -> None:
-        self._chat_stream = chat_stream
-        self._queue: queue.Queue = queue.Queue()
-        self._is_done = False
-        self._is_function: Optional[bool] = None
-        self.response_str = ""
+    response: str = ""
+    sources: List[ToolOutput] = field(default_factory=list)
+    chat_stream: Optional[ChatResponseGen] = None
+    achat_stream: Optional[ChatResponseAsyncGen] = None
+    _queue: queue.Queue = queue.Queue()
+    _is_done = False
+    _is_function: Optional[bool] = None
 
     def __str__(self) -> str:
         if self._is_done and not self._queue.empty() and not self._is_function:
             for delta in self._queue.queue:
-                self.response_str += delta
-        return self.response_str
+                self.response += delta
+        return self.response
 
-    def write_response_to_history(self, chat_history: List[ChatMessage]) -> None:
-        if isinstance(self._chat_stream, AsyncGenerator):
+    def write_response_to_history(self, memory: BaseMemory) -> None:
+        if self.chat_stream is None:
             raise ValueError(
-                "Cannot write to history with async generator in sync function."
+                "chat_stream is None. Cannot write to history without chat_stream."
             )
 
         final_message = None
-        for chat in self._chat_stream:
+        for chat in self.chat_stream:
             final_message = chat.message
             self._is_function = (
                 final_message.additional_kwargs.get("function_call", None) is not None
             )
             self._queue.put_nowait(chat.delta)
 
         if final_message is not None:
-            chat_history.append(final_message)
+            memory.put(final_message)
 
         self._is_done = True
 
-    async def awrite_response_to_history(self, chat_history: List[ChatMessage]) -> None:
-        if isinstance(self._chat_stream, Generator):
+    async def awrite_response_to_history(self, memory: BaseMemory) -> None:
+        if self.achat_stream is None:
             raise ValueError(
-                "Cannot write to history with sync generator in async function."
+                "achat_stream is None. Cannot asynchronously write to "
+                "history without achat_stream."
             )
 
         final_message = None
-        async for chat in self._chat_stream:
+        async for chat in self.achat_stream:
             final_message = chat.message
             self._is_function = (
                 final_message.additional_kwargs.get("function_call", None) is not None
             )
             self._queue.put_nowait(chat.delta)
 
         if final_message is not None:
-            chat_history.append(final_message)
+            memory.put(final_message)
 
         self._is_done = True
 
     @property
     def response_gen(self) -> Generator[str, None, None]:
         while not self._is_done or not self._queue.empty():
             try:
                 delta = self._queue.get(block=False)
-                self.response_str += delta
+                self.response += delta
                 yield delta
             except queue.Empty:
                 # Queue is empty, but we're not done yet
                 continue
 
 
-STREAMING_CHAT_RESPONSE_TYPE = Union[
-    StreamingResponse,
-    StreamingChatResponse,
-    Generator[StreamingChatResponse, None, None],
-    AsyncGenerator[StreamingChatResponse, None],
-]
-
-
 class BaseChatEngine(ABC):
     """Base Chat Engine."""
 
     @abstractmethod
     def reset(self) -> None:
         """Reset conversation state."""
         pass
 
     @abstractmethod
     def chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> RESPONSE_TYPE:
+    ) -> AgentChatResponse:
         """Main chat interface."""
         pass
 
     @abstractmethod
     def stream_chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> STREAMING_CHAT_RESPONSE_TYPE:
+    ) -> StreamingAgentChatResponse:
         """Stream chat interface."""
         pass
 
     @abstractmethod
     async def achat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> RESPONSE_TYPE:
+    ) -> AgentChatResponse:
         """Async version of main chat interface."""
         pass
 
     @abstractmethod
     async def astream_chat(
         self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> STREAMING_CHAT_RESPONSE_TYPE:
+    ) -> StreamingAgentChatResponse:
         """Async version of main chat interface."""
         pass
 
     def chat_repl(self) -> None:
         """Enter interactive chat REPL."""
         print("===== Entering Chat REPL =====")
         print('Type "exit" to exit.\n')
```

### Comparing `gpt_index-0.7.5/llama_index/chat_engine/utils.py` & `gpt_index-0.7.6/llama_index/chat_engine/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from typing import List
-
-from llama_index.llms.base import ChatMessage, MessageRole
+from llama_index.llms.base import (
+    ChatMessage,
+    MessageRole,
+    ChatResponse,
+    ChatResponseGen,
+)
+from llama_index.memory import BaseMemory
 from llama_index.types import TokenGen
 
 
 def response_gen_with_chat_history(
-    message: str, chat_history: List[ChatMessage], response_gen: TokenGen
-) -> TokenGen:
+    message: str, memory: BaseMemory, response_gen: TokenGen
+) -> ChatResponseGen:
     response_str = ""
     for token in response_gen:
         response_str += token
-        yield token
+        yield ChatResponse(
+            role=MessageRole.ASSISTANT, content=response_str, delta=token
+        )
 
-    chat_history.extend(
-        [
-            ChatMessage(role=MessageRole.USER, content=message),
-            ChatMessage(role=MessageRole.ASSISTANT, content=response_str),
-        ]
-    )
+    # Record response
+    memory.put(ChatMessage(role=MessageRole.USER, content=message))
+    memory.put(ChatMessage(role=MessageRole.ASSISTANT, content=response_str))
```

### Comparing `gpt_index-0.7.5/llama_index/composability/joint_qa_summary.py` & `gpt_index-0.7.6/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/data_structs/data_structs.py` & `gpt_index-0.7.6/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/data_structs/document_summary.py` & `gpt_index-0.7.6/llama_index/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/data_structs/registry.py` & `gpt_index-0.7.6/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/data_structs/struct_type.py` & `gpt_index-0.7.6/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/data_structs/table.py` & `gpt_index-0.7.6/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/embeddings/base.py` & `gpt_index-0.7.6/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/embeddings/google.py` & `gpt_index-0.7.6/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/embeddings/langchain.py` & `gpt_index-0.7.6/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/embeddings/openai.py` & `gpt_index-0.7.6/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/embeddings/utils.py` & `gpt_index-0.7.6/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/evaluation/base.py` & `gpt_index-0.7.6/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/evaluation/dataset_generation.py` & `gpt_index-0.7.6/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/evaluation/guideline_eval.py` & `gpt_index-0.7.6/llama_index/evaluation/guideline_eval.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/graph_stores/nebulagraph.py` & `gpt_index-0.7.6/llama_index/graph_stores/nebulagraph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/graph_stores/registery.py` & `gpt_index-0.7.6/llama_index/graph_stores/registery.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/graph_stores/simple.py` & `gpt_index-0.7.6/llama_index/graph_stores/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/graph_stores/types.py` & `gpt_index-0.7.6/llama_index/graph_stores/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/img_utils.py` & `gpt_index-0.7.6/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/__init__.py` & `gpt_index-0.7.6/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/base.py` & `gpt_index-0.7.6/llama_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/base_retriever.py` & `gpt_index-0.7.6/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/common/struct_store/base.py` & `gpt_index-0.7.6/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/common/struct_store/schema.py` & `gpt_index-0.7.6/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/common/struct_store/sql.py` & `gpt_index-0.7.6/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/common_tree/base.py` & `gpt_index-0.7.6/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/composability/graph.py` & `gpt_index-0.7.6/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/document_summary/base.py` & `gpt_index-0.7.6/llama_index/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/document_summary/retrievers.py` & `gpt_index-0.7.6/llama_index/indices/document_summary/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/empty/base.py` & `gpt_index-0.7.6/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/empty/retrievers.py` & `gpt_index-0.7.6/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/keyword_table/__init__.py` & `gpt_index-0.7.6/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/keyword_table/base.py` & `gpt_index-0.7.6/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/keyword_table/rake_base.py` & `gpt_index-0.7.6/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/keyword_table/retrievers.py` & `gpt_index-0.7.6/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/keyword_table/simple_base.py` & `gpt_index-0.7.6/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/keyword_table/utils.py` & `gpt_index-0.7.6/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/knowledge_graph/base.py` & `gpt_index-0.7.6/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/knowledge_graph/retriever.py` & `gpt_index-0.7.6/llama_index/indices/knowledge_graph/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/list/base.py` & `gpt_index-0.7.6/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/list/retrievers.py` & `gpt_index-0.7.6/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/loading.py` & `gpt_index-0.7.6/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/postprocessor/__init__.py` & `gpt_index-0.7.6/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/postprocessor/cohere_rerank.py` & `gpt_index-0.7.6/llama_index/indices/postprocessor/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/postprocessor/llm_rerank.py` & `gpt_index-0.7.6/llama_index/indices/postprocessor/llm_rerank.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/postprocessor/node.py` & `gpt_index-0.7.6/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/postprocessor/node_recency.py` & `gpt_index-0.7.6/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/postprocessor/optimizer.py` & `gpt_index-0.7.6/llama_index/indices/postprocessor/optimizer.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/postprocessor/pii.py` & `gpt_index-0.7.6/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/prompt_helper.py` & `gpt_index-0.7.6/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/query/base.py` & `gpt_index-0.7.6/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/query/embedding_utils.py` & `gpt_index-0.7.6/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/query/query_transform/base.py` & `gpt_index-0.7.6/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/query/query_transform/feedback_transform.py` & `gpt_index-0.7.6/llama_index/indices/query/query_transform/feedback_transform.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/query/query_transform/prompts.py` & `gpt_index-0.7.6/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/query/schema.py` & `gpt_index-0.7.6/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/registry.py` & `gpt_index-0.7.6/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/service_context.py` & `gpt_index-0.7.6/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/struct_store/__init__.py` & `gpt_index-0.7.6/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/struct_store/base.py` & `gpt_index-0.7.6/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/struct_store/container_builder.py` & `gpt_index-0.7.6/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/struct_store/json_query.py` & `gpt_index-0.7.6/llama_index/indices/struct_store/json_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/struct_store/pandas.py` & `gpt_index-0.7.6/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/struct_store/sql.py` & `gpt_index-0.7.6/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/struct_store/sql_query.py` & `gpt_index-0.7.6/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/tree/__init__.py` & `gpt_index-0.7.6/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/tree/all_leaf_retriever.py` & `gpt_index-0.7.6/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/tree/base.py` & `gpt_index-0.7.6/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/tree/inserter.py` & `gpt_index-0.7.6/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `gpt_index-0.7.6/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/tree/select_leaf_retriever.py` & `gpt_index-0.7.6/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/tree/tree_root_retriever.py` & `gpt_index-0.7.6/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/tree/utils.py` & `gpt_index-0.7.6/llama_index/indices/tree/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/utils.py` & `gpt_index-0.7.6/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/vector_store/base.py` & `gpt_index-0.7.6/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py` & `gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py` & `gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py` & `gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/indices/vector_store/retrievers/retriever.py` & `gpt_index-0.7.6/llama_index/indices/vector_store/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/langchain_helpers/agents/__init__.py` & `gpt_index-0.7.6/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/langchain_helpers/agents/agents.py` & `gpt_index-0.7.6/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/langchain_helpers/agents/toolkits.py` & `gpt_index-0.7.6/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/langchain_helpers/agents/tools.py` & `gpt_index-0.7.6/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/langchain_helpers/memory_wrapper.py` & `gpt_index-0.7.6/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/langchain_helpers/sql_wrapper.py` & `gpt_index-0.7.6/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/langchain_helpers/streaming.py` & `gpt_index-0.7.6/llama_index/langchain_helpers/streaming.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/langchain_helpers/text_splitter.py` & `gpt_index-0.7.6/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llm_predictor/base.py` & `gpt_index-0.7.6/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llm_predictor/mock.py` & `gpt_index-0.7.6/llama_index/llm_predictor/mock.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llm_predictor/structured.py` & `gpt_index-0.7.6/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llm_predictor/utils.py` & `gpt_index-0.7.6/llama_index/llm_predictor/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llm_predictor/vellum/predictor.py` & `gpt_index-0.7.6/llama_index/llm_predictor/vellum/predictor.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llm_predictor/vellum/prompt_registry.py` & `gpt_index-0.7.6/llama_index/llm_predictor/vellum/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llm_predictor/vellum/types.py` & `gpt_index-0.7.6/llama_index/llm_predictor/vellum/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/__init__.py` & `gpt_index-0.7.6/llama_index/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/anthropic.py` & `gpt_index-0.7.6/llama_index/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/anthropic_utils.py` & `gpt_index-0.7.6/llama_index/llms/anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/azure_openai.py` & `gpt_index-0.7.6/llama_index/llms/azure_openai.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/base.py` & `gpt_index-0.7.6/llama_index/llms/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/custom.py` & `gpt_index-0.7.6/llama_index/llms/custom.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/generic_utils.py` & `gpt_index-0.7.6/llama_index/llms/generic_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/huggingface.py` & `gpt_index-0.7.6/llama_index/llms/huggingface.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/langchain.py` & `gpt_index-0.7.6/llama_index/llms/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/langchain_utils.py` & `gpt_index-0.7.6/llama_index/llms/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/mock.py` & `gpt_index-0.7.6/llama_index/llms/mock.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/openai.py` & `gpt_index-0.7.6/llama_index/llms/openai.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/openai_utils.py` & `gpt_index-0.7.6/llama_index/llms/openai_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/llms/palm.py` & `gpt_index-0.7.6/llama_index/llms/palm.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/logger/base.py` & `gpt_index-0.7.6/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/node_parser/extractors/metadata_extractors.py` & `gpt_index-0.7.6/llama_index/node_parser/extractors/metadata_extractors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/node_parser/interface.py` & `gpt_index-0.7.6/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/node_parser/node_utils.py` & `gpt_index-0.7.6/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/node_parser/simple.py` & `gpt_index-0.7.6/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/objects/__init__.py` & `gpt_index-0.7.6/llama_index/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/objects/base.py` & `gpt_index-0.7.6/llama_index/objects/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/objects/base_node_mapping.py` & `gpt_index-0.7.6/llama_index/objects/base_node_mapping.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/objects/table_node_mapping.py` & `gpt_index-0.7.6/llama_index/objects/table_node_mapping.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/objects/tool_node_mapping.py` & `gpt_index-0.7.6/llama_index/objects/tool_node_mapping.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/output_parsers/guardrails.py` & `gpt_index-0.7.6/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/output_parsers/langchain.py` & `gpt_index-0.7.6/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/output_parsers/pydantic.py` & `gpt_index-0.7.6/llama_index/output_parsers/pydantic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Pydantic output parser."""
 
+from llama_index.output_parsers.utils import extract_json_str
 from llama_index.types import BaseOutputParser, Model
 from typing import Type, Optional, List, Any
-import re
 import json
 
 PYDANTIC_FORMAT_TMPL = """
 Please use the following JSON schema to format your query:
 {schema}
 """
 
@@ -32,23 +32,16 @@
 
     @property
     def output_cls(self) -> Type[Model]:
         return self._output_cls
 
     def parse(self, text: str) -> Any:
         """Parse, validate, and correct errors programmatically."""
-        # NOTE: this regex parsing is taken from langchain.output_parsers.pydantic
-        match = re.search(
-            r"\{.*\}", text.strip(), re.MULTILINE | re.IGNORECASE | re.DOTALL
-        )
-        if match:
-            json_str = match.group()
-            return self._output_cls.parse_raw(json_str)
-        else:
-            raise ValueError(f"Could not parse output: {text}")
+        json_str = extract_json_str(text)
+        return self._output_cls.parse_raw(json_str)
 
     def format(self, query: str) -> str:
         """Format a query with structured output formatting instructions."""
         schema_dict = self._output_cls.schema()
         for key in self._excluded_schema_keys_from_format:
             del schema_dict[key]
```

### Comparing `gpt_index-0.7.5/llama_index/output_parsers/selection.py` & `gpt_index-0.7.6/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/output_parsers/utils.py` & `gpt_index-0.7.6/llama_index/output_parsers/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import re
 from typing import Any
 
 import yaml
 
 from llama_index.output_parsers.base import OutputParserException
 
 
@@ -25,7 +26,17 @@
             json_obj = yaml.safe_load(json_string)
         except yaml.YAMLError as e_yaml:
             raise OutputParserException(
                 f"Got invalid JSON object. Error: {e_json} {e_yaml}"
             )
 
     return json_obj
+
+
+def extract_json_str(text: str) -> str:
+    """Extract JSON string from text."""
+    # NOTE: this regex parsing is taken from langchain.output_parsers.pydantic
+    match = re.search(r"\{.*\}", text.strip(), re.MULTILINE | re.IGNORECASE | re.DOTALL)
+    if not match:
+        raise ValueError(f"Could not extract json string from output: {text}")
+
+    return match.group()
```

### Comparing `gpt_index-0.7.5/llama_index/playground/base.py` & `gpt_index-0.7.6/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/program/__init__.py` & `gpt_index-0.7.6/llama_index/program/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/program/guidance_program.py` & `gpt_index-0.7.6/llama_index/program/guidance_program.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/program/llm_program.py` & `gpt_index-0.7.6/llama_index/program/llm_program.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/program/llm_prompt_program.py` & `gpt_index-0.7.6/llama_index/program/llm_prompt_program.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/program/openai_program.py` & `gpt_index-0.7.6/llama_index/program/openai_program.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/program/predefined/df.py` & `gpt_index-0.7.6/llama_index/program/predefined/df.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/program/predefined/evaporate/base.py` & `gpt_index-0.7.6/llama_index/program/predefined/evaporate/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/program/predefined/evaporate/extractor.py` & `gpt_index-0.7.6/llama_index/program/predefined/evaporate/extractor.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/program/predefined/evaporate/prompts.py` & `gpt_index-0.7.6/llama_index/program/predefined/evaporate/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/base.py` & `gpt_index-0.7.6/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/chat_prompts.py` & `gpt_index-0.7.6/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/choice_select.py` & `gpt_index-0.7.6/llama_index/prompts/choice_select.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/default_prompt_selectors.py` & `gpt_index-0.7.6/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/default_prompts.py` & `gpt_index-0.7.6/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/guidance_utils.py` & `gpt_index-0.7.6/llama_index/prompts/guidance_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/prompt_selector.py` & `gpt_index-0.7.6/llama_index/prompts/prompt_selector.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/prompt_type.py` & `gpt_index-0.7.6/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/prompts.py` & `gpt_index-0.7.6/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/system.py` & `gpt_index-0.7.6/llama_index/prompts/system.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/prompts/utils.py` & `gpt_index-0.7.6/llama_index/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/__init__.py` & `gpt_index-0.7.6/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/citation_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/citation_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/flare/answer_inserter.py` & `gpt_index-0.7.6/llama_index/query_engine/flare/answer_inserter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/flare/base.py` & `gpt_index-0.7.6/llama_index/query_engine/flare/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/flare/output_parser.py` & `gpt_index-0.7.6/llama_index/query_engine/flare/output_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/graph_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/multistep_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/pandas_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/pandas_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/retriever_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/retry_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/retry_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/retry_source_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/retry_source_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/router_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/sql_join_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/sql_join_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/sql_vector_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/sql_vector_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/sub_question_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/sub_question_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/query_engine/transform_query_engine.py` & `gpt_index-0.7.6/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/question_gen/guidance_generator.py` & `gpt_index-0.7.6/llama_index/question_gen/guidance_generator.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/question_gen/llm_generators.py` & `gpt_index-0.7.6/llama_index/question_gen/llm_generators.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/question_gen/output_parser.py` & `gpt_index-0.7.6/llama_index/question_gen/output_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/question_gen/prompts.py` & `gpt_index-0.7.6/llama_index/question_gen/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/question_gen/types.py` & `gpt_index-0.7.6/llama_index/question_gen/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/__init__.py` & `gpt_index-0.7.6/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/base.py` & `gpt_index-0.7.6/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/chatgpt_plugin/base.py` & `gpt_index-0.7.6/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/chroma.py` & `gpt_index-0.7.6/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/database.py` & `gpt_index-0.7.6/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/deeplake.py` & `gpt_index-0.7.6/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/discord_reader.py` & `gpt_index-0.7.6/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/download.py` & `gpt_index-0.7.6/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/elasticsearch.py` & `gpt_index-0.7.6/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/faiss.py` & `gpt_index-0.7.6/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/base.py` & `gpt_index-0.7.6/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/docs_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/docs_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/epub_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/epub_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/image_caption_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/image_caption_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/image_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/image_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/image_vision_llm_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/image_vision_llm_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/ipynb_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/ipynb_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/markdown_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/markdown_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/mbox_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/mbox_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/slides_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/slides_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/tabular_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/tabular_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/file/video_audio_reader.py` & `gpt_index-0.7.6/llama_index/readers/file/video_audio_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/github_readers/github_api_client.py` & `gpt_index-0.7.6/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/github_readers/github_repository_reader.py` & `gpt_index-0.7.6/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/github_readers/utils.py` & `gpt_index-0.7.6/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/google_readers/gdocs.py` & `gpt_index-0.7.6/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/google_readers/gsheets.py` & `gpt_index-0.7.6/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/json.py` & `gpt_index-0.7.6/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/make_com/wrapper.py` & `gpt_index-0.7.6/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/mbox.py` & `gpt_index-0.7.6/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/metal.py` & `gpt_index-0.7.6/llama_index/readers/metal.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/milvus.py` & `gpt_index-0.7.6/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/mongo.py` & `gpt_index-0.7.6/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/myscale.py` & `gpt_index-0.7.6/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/notion.py` & `gpt_index-0.7.6/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/obsidian.py` & `gpt_index-0.7.6/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/pinecone.py` & `gpt_index-0.7.6/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/psychic.py` & `gpt_index-0.7.6/llama_index/readers/psychic.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/qdrant.py` & `gpt_index-0.7.6/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/redis/utils.py` & `gpt_index-0.7.6/llama_index/readers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/slack.py` & `gpt_index-0.7.6/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/steamship/file_reader.py` & `gpt_index-0.7.6/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/string_iterable.py` & `gpt_index-0.7.6/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/twitter.py` & `gpt_index-0.7.6/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/weaviate/reader.py` & `gpt_index-0.7.6/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/web.py` & `gpt_index-0.7.6/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/wikipedia.py` & `gpt_index-0.7.6/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/readers/youtube_transcript.py` & `gpt_index-0.7.6/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response/notebook_utils.py` & `gpt_index-0.7.6/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response/pprint_utils.py` & `gpt_index-0.7.6/llama_index/response/pprint_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response/schema.py` & `gpt_index-0.7.6/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/__init__.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/accumulate.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/accumulate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/base.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/compact_and_accumulate.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/compact_and_accumulate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/compact_and_refine.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/compact_and_refine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/factory.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/factory.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/generation.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/generation.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/no_text.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/no_text.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/refine.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/refine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/simple_summarize.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/simple_summarize.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/tree_summarize.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/response_synthesizers/type.py` & `gpt_index-0.7.6/llama_index/response_synthesizers/type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/retrievers/__init__.py` & `gpt_index-0.7.6/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/retrievers/recursive_retriever.py` & `gpt_index-0.7.6/llama_index/retrievers/recursive_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/retrievers/transform_retriever.py` & `gpt_index-0.7.6/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/schema.py` & `gpt_index-0.7.6/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/selectors/llm_selectors.py` & `gpt_index-0.7.6/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/selectors/prompts.py` & `gpt_index-0.7.6/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/selectors/pydantic_selectors.py` & `gpt_index-0.7.6/llama_index/selectors/pydantic_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/selectors/types.py` & `gpt_index-0.7.6/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/docstore/__init__.py` & `gpt_index-0.7.6/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/docstore/dynamodb_docstore.py` & `gpt_index-0.7.6/llama_index/storage/docstore/dynamodb_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/docstore/keyval_docstore.py` & `gpt_index-0.7.6/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/docstore/mongo_docstore.py` & `gpt_index-0.7.6/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/docstore/redis_docstore.py` & `gpt_index-0.7.6/llama_index/storage/docstore/redis_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/docstore/registry.py` & `gpt_index-0.7.6/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/docstore/simple_docstore.py` & `gpt_index-0.7.6/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/docstore/types.py` & `gpt_index-0.7.6/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/docstore/utils.py` & `gpt_index-0.7.6/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/index_store/dynamodb_index_store.py` & `gpt_index-0.7.6/llama_index/storage/index_store/dynamodb_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/index_store/keyval_index_store.py` & `gpt_index-0.7.6/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/index_store/mongo_index_store.py` & `gpt_index-0.7.6/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/index_store/redis_index_store.py` & `gpt_index-0.7.6/llama_index/storage/index_store/redis_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/index_store/simple_index_store.py` & `gpt_index-0.7.6/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/index_store/types.py` & `gpt_index-0.7.6/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/index_store/utils.py` & `gpt_index-0.7.6/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/kvstore/dynamodb_kvstore.py` & `gpt_index-0.7.6/llama_index/storage/kvstore/dynamodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/kvstore/mongodb_kvstore.py` & `gpt_index-0.7.6/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/kvstore/redis_kvstore.py` & `gpt_index-0.7.6/llama_index/storage/kvstore/redis_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/kvstore/s3_kvstore.py` & `gpt_index-0.7.6/llama_index/storage/kvstore/s3_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/kvstore/simple_kvstore.py` & `gpt_index-0.7.6/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/kvstore/types.py` & `gpt_index-0.7.6/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/storage/storage_context.py` & `gpt_index-0.7.6/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/token_counter/mock_embed_model.py` & `gpt_index-0.7.6/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/token_counter/utils.py` & `gpt_index-0.7.6/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/tools/function_tool.py` & `gpt_index-0.7.6/llama_index/tools/function_tool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Optional, Callable, Type
 
 from pydantic import BaseModel
-from llama_index.tools.types import BaseTool, ToolMetadata
+from llama_index.tools.types import BaseTool, ToolMetadata, ToolOutput
 from llama_index.bridge.langchain import Tool, StructuredTool
 from inspect import signature
 from llama_index.tools.utils import create_schema_from_function
 
 
 class FunctionTool(BaseTool):
     """Function Tool.
@@ -46,17 +46,23 @@
         return self._metadata
 
     @property
     def fn(self) -> Callable[..., Any]:
         """Function."""
         return self._fn
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    def __call__(self, *args: Any, **kwargs: Any) -> ToolOutput:
         """Call."""
-        return self._fn(*args, **kwargs)
+        tool_output = self._fn(*args, **kwargs)
+        return ToolOutput(
+            content=str(tool_output),
+            tool_name=self.metadata.name,
+            raw_input={"args": args, "kwargs": kwargs},
+            raw_output=tool_output,
+        )
 
     def to_langchain_tool(
         self,
         **langchain_tool_kwargs: Any,
     ) -> Tool:
         """To langchain tool."""
         langchain_tool_kwargs = self._process_langchain_tool_kwargs(
```

### Comparing `gpt_index-0.7.5/llama_index/tools/ondemand_loader_tool.py` & `gpt_index-0.7.6/llama_index/tools/ondemand_loader_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Ad-hoc data loader tool.
 
 Tool that wraps any data loader, and is able to load data on-demand.
 
 """
 
 
-from llama_index.tools.types import BaseTool, ToolMetadata
+from llama_index.tools.types import BaseTool, ToolMetadata, ToolOutput
 from llama_index.readers.base import BaseReader
 from typing import Any, Optional, Dict, Type, Callable, List
 from llama_index.readers.schema.base import Document
 from llama_index.indices.base import BaseIndex
 from llama_index.indices.vector_store import VectorStoreIndex
 from llama_index.tools.utils import create_schema_from_function
 from pydantic import BaseModel
@@ -103,23 +103,23 @@
             description = f"Tool to load data from {tool.__class__.__name__}"
         if fn_schema is None:
             fn_schema = create_schema_from_function(
                 name or "LoadData", tool._fn, [(query_str_kwargs_key, str, None)]
             )
         metadata = ToolMetadata(name=name, description=description, fn_schema=fn_schema)
         return cls(
-            loader=tool,
+            loader=tool._fn,
             index_cls=index_cls,
             index_kwargs=index_kwargs,
             use_query_str_in_loader=use_query_str_in_loader,
             query_str_kwargs_key=query_str_kwargs_key,
             metadata=metadata,
         )
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    def __call__(self, *args: Any, **kwargs: Any) -> ToolOutput:
         """Call."""
         if self._query_str_kwargs_key not in kwargs:
             raise ValueError(
                 "Missing query_str in kwargs with parameter name: "
                 f"{self._query_str_kwargs_key}"
             )
         if self._use_query_str_in_loader:
@@ -129,8 +129,13 @@
 
         docs = self._loader(*args, **kwargs)
 
         index = self._index_cls.from_documents(docs, **self._index_kwargs)
         # TODO: add query kwargs
         query_engine = index.as_query_engine()
         response = query_engine.query(query_str)
-        return str(response)
+        return ToolOutput(
+            content=str(response),
+            tool_name=self.metadata.name,
+            raw_input={"query": query_str},
+            raw_output=response,
+        )
```

### Comparing `gpt_index-0.7.5/llama_index/tools/query_engine.py` & `gpt_index-0.7.6/llama_index/tools/query_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Optional, cast
 
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.langchain_helpers.agents.tools import IndexToolConfig, LlamaIndexTool
-from llama_index.tools.types import BaseTool, ToolMetadata
+from llama_index.tools.types import BaseTool, ToolMetadata, ToolOutput
 
 DEFAULT_NAME = "Query Engine Tool"
 DEFAULT_DESCRIPTION = """Useful for running a natural language query
 against a knowledge base and get back a natural language response.
 """
 
 
@@ -33,29 +33,35 @@
         cls,
         query_engine: BaseQueryEngine,
         name: Optional[str] = None,
         description: Optional[str] = None,
     ) -> "QueryEngineTool":
         name = name or DEFAULT_NAME
         description = description or DEFAULT_DESCRIPTION
+
         metadata = ToolMetadata(name=name, description=description)
         return cls(query_engine=query_engine, metadata=metadata)
 
     @property
     def query_engine(self) -> BaseQueryEngine:
         return self._query_engine
 
     @property
     def metadata(self) -> ToolMetadata:
         return self._metadata
 
-    def __call__(self, input: Any) -> Any:
+    def __call__(self, input: Any) -> ToolOutput:
         query_str = cast(str, input)
         response = self._query_engine.query(query_str)
-        return str(response)
+        return ToolOutput(
+            content=str(response),
+            tool_name=self.metadata.name,
+            raw_input={"input": input},
+            raw_output=response,
+        )
 
     def as_langchain_tool(self) -> LlamaIndexTool:
         tool_config = IndexToolConfig(
             query_engine=self.query_engine,
             name=self.metadata.name,
             description=self.metadata.description,
         )
```

### Comparing `gpt_index-0.7.5/llama_index/tools/query_plan.py` & `gpt_index-0.7.6/llama_index/tools/query_plan.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 from llama_index.bridge.langchain import print_text
 from pydantic import BaseModel, Field
 from typing import Dict, List, Any, Optional
 
 from llama_index.response_synthesizers import BaseSynthesizer, get_response_synthesizer
 from llama_index.schema import NodeWithScore, TextNode
-from llama_index.tools.types import BaseTool
-from llama_index.tools.types import ToolMetadata
+from llama_index.tools.types import BaseTool, ToolMetadata, ToolOutput
 
 
 DEFAULT_NAME = "query_plan_tool"
 
 QUERYNODE_QUERY_STR_DESC = """\
 Question we are asking. This is the query string that will be executed. \
 """
@@ -133,58 +132,65 @@
         {self._description_prefix}\n\n
         {tools_description}
         """
         metadata = ToolMetadata(description, self._name, fn_schema=QueryPlan)
 
         return metadata
 
-    def _execute_node(self, node: QueryNode, nodes_dict: Dict[int, QueryNode]) -> str:
+    def _execute_node(
+        self, node: QueryNode, nodes_dict: Dict[int, QueryNode]
+    ) -> ToolOutput:
         """Execute node."""
         print_text(f"Executing node {node.json()}\n", color="blue")
         if len(node.dependencies) > 0:
             print_text(
                 f"Executing {len(node.dependencies)} child nodes\n", color="pink"
             )
             child_query_nodes: List[QueryNode] = [
                 nodes_dict[dep] for dep in node.dependencies
             ]
             # execute the child nodes first
-            child_responses: List[str] = [
+            child_responses: List[ToolOutput] = [
                 self._execute_node(child, nodes_dict) for child in child_query_nodes
             ]
             # form the child Node/NodeWithScore objects
             child_nodes = []
             for child_query_node, child_response in zip(
                 child_query_nodes, child_responses
             ):
                 node_text = (
                     f"Query: {child_query_node.query_str}\n"
-                    f"Response: {child_response}\n"
+                    f"Response: {str(child_response)}\n"
                 )
                 child_node = TextNode(text=node_text)
                 child_nodes.append(child_node)
             # use response synthesizer to combine results
             child_nodes_with_scores = [
                 NodeWithScore(node=n, score=1.0) for n in child_nodes
             ]
             response_obj = self._response_synthesizer.synthesize(
                 query=node.query_str,
                 nodes=child_nodes_with_scores,
             )
-            response = str(response_obj)
+            response = ToolOutput(
+                content=str(response_obj),
+                tool_name=node.query_str,
+                raw_input={"query": node.query_str},
+                raw_output=response_obj,
+            )
 
         else:
             # this is a leaf request, execute the query string using the specified tool
             tool = self._query_tools_dict[node.tool_name]
             print_text(f"Selected Tool: {tool.metadata}\n", color="pink")
             response = tool(node.query_str)
         print_text(
             "Executed query, got response.\n"
             f"Query: {node.query_str}\n"
-            f"Response: {response}\n",
+            f"Response: {str(response)}\n",
             color="blue",
         )
         return response
 
     def _find_root_nodes(self, nodes_dict: Dict[int, QueryNode]) -> List[QueryNode]:
         """Find root node."""
         # the root node is the one that isn't a dependency of any other node
@@ -193,15 +199,15 @@
             for dep in node.dependencies:
                 node_counts[dep] += 1
         root_node_ids = [
             node_id for node_id, count in node_counts.items() if count == 0
         ]
         return [nodes_dict[node_id] for node_id in root_node_ids]
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    def __call__(self, *args: Any, **kwargs: Any) -> ToolOutput:
         """Call."""
         # the kwargs represented as a JSON object
         # should be a QueryPlan object
         query_plan = QueryPlan(**kwargs)
 
         nodes_dict = {node.id: node for node in query_plan.nodes}
         root_nodes = self._find_root_nodes(nodes_dict)
```

### Comparing `gpt_index-0.7.5/llama_index/tools/tool_spec/base.py` & `gpt_index-0.7.6/llama_index/tools/tool_spec/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/tools/tool_spec/notion/base.py` & `gpt_index-0.7.6/llama_index/tools/tool_spec/notion/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/tools/tool_spec/slack/base.py` & `gpt_index-0.7.6/llama_index/tools/tool_spec/slack/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/tools/types.py` & `gpt_index-0.7.6/llama_index/tools/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,38 @@
 from dataclasses import dataclass
 from typing import Any, Dict, Optional, Type
 
 from llama_index.bridge.langchain import StructuredTool, Tool
 from pydantic import BaseModel
 
 
+class DefaultToolFnSchema(BaseModel):
+    """Default tool function Schema."""
+
+    input: str
+
+
 @dataclass
 class ToolMetadata:
     description: str
     name: Optional[str] = None
-    fn_schema: Optional[Type[BaseModel]] = None
+    fn_schema: Optional[Type[BaseModel]] = DefaultToolFnSchema
+
+    @property
+    def fn_schema_str(self) -> str:
+        """Get fn schema as string."""
+        if self.fn_schema is None:
+            raise ValueError("fn_schema is None.")
+        return str(self.fn_schema.schema())
+
+    def get_name(self) -> str:
+        """Get name."""
+        if self.name is None:
+            raise ValueError("name is None.")
+        return self.name
 
     def to_openai_function(self) -> Dict[str, Any]:
         """To OpenAI function."""
         if self.fn_schema is None:
             parameters = {
                 "properties": {
                     "input": {"title": "input query string", "type": "string"},
@@ -28,22 +47,35 @@
         return {
             "name": self.name,
             "description": self.description,
             "parameters": parameters,
         }
 
 
+class ToolOutput(BaseModel):
+    """Tool output."""
+
+    content: str
+    tool_name: str
+    raw_input: Dict[str, Any]
+    raw_output: Any
+
+    def __str__(self) -> str:
+        """String."""
+        return str(self.content)
+
+
 class BaseTool:
     @property
     @abstractmethod
     def metadata(self) -> ToolMetadata:
         pass
 
     @abstractmethod
-    def __call__(self, input: Any) -> Any:
+    def __call__(self, input: Any) -> ToolOutput:
         pass
 
     def _process_langchain_tool_kwargs(
         self,
         langchain_tool_kwargs: Any,
     ) -> Dict[str, Any]:
         """Process langchain tool kwargs."""
```

### Comparing `gpt_index-0.7.5/llama_index/tools/utils.py` & `gpt_index-0.7.6/llama_index/tools/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/tts/bark.py` & `gpt_index-0.7.6/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/tts/base.py` & `gpt_index-0.7.6/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/tts/elevenlabs.py` & `gpt_index-0.7.6/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/types.py` & `gpt_index-0.7.6/llama_index/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/utils.py` & `gpt_index-0.7.6/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/__init__.py` & `gpt_index-0.7.6/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/chatgpt_plugin.py` & `gpt_index-0.7.6/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/chroma.py` & `gpt_index-0.7.6/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/deeplake.py` & `gpt_index-0.7.6/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/docarray/base.py` & `gpt_index-0.7.6/llama_index/vector_stores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/docarray/hnsw.py` & `gpt_index-0.7.6/llama_index/vector_stores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/docarray/in_memory.py` & `gpt_index-0.7.6/llama_index/vector_stores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/dynamodb.py` & `gpt_index-0.7.6/llama_index/vector_stores/dynamodb.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/faiss.py` & `gpt_index-0.7.6/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/lancedb.py` & `gpt_index-0.7.6/llama_index/vector_stores/lancedb.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/metal.py` & `gpt_index-0.7.6/llama_index/vector_stores/metal.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/milvus.py` & `gpt_index-0.7.6/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/mongodb.py` & `gpt_index-0.7.6/llama_index/vector_stores/mongodb.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/myscale.py` & `gpt_index-0.7.6/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/opensearch.py` & `gpt_index-0.7.6/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/pinecone.py` & `gpt_index-0.7.6/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/postgres.py` & `gpt_index-0.7.6/llama_index/vector_stores/postgres.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/qdrant.py` & `gpt_index-0.7.6/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/redis.py` & `gpt_index-0.7.6/llama_index/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/registry.py` & `gpt_index-0.7.6/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/simple.py` & `gpt_index-0.7.6/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/supabase.py` & `gpt_index-0.7.6/llama_index/vector_stores/supabase.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/tair.py` & `gpt_index-0.7.6/llama_index/vector_stores/tair.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/types.py` & `gpt_index-0.7.6/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/typesense.py` & `gpt_index-0.7.6/llama_index/vector_stores/typesense.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/utils.py` & `gpt_index-0.7.6/llama_index/vector_stores/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,17 @@
     metadata.pop(text_key, None)
     metadata.pop("id", None)
     metadata.pop("document_id", None)
     metadata.pop("doc_id", None)
     metadata.pop("ref_doc_id", None)
 
     # remaining metadata is metadata or node_info
-    metadata = {}
+    new_metadata = {}
     for key, val in metadata.items():
         # NOTE: right now we enforce metadata to be dict of simple types.
         #       dump anything that's not a simple type into node_info.
         if isinstance(val, (str, int, float, type(None))):
-            metadata[key] = val
+            new_metadata[key] = val
         else:
             node_info[key] = val
 
-    return metadata, node_info, relationships
+    return new_metadata, node_info, relationships
```

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/weaviate.py` & `gpt_index-0.7.6/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/llama_index/vector_stores/weaviate_utils.py` & `gpt_index-0.7.6/llama_index/vector_stores/weaviate_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/setup.py` & `gpt_index-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/callbacks/test_llama_debug.py` & `gpt_index-0.7.6/tests/callbacks/test_llama_debug.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/callbacks/test_token_counter.py` & `gpt_index-0.7.6/tests/callbacks/test_token_counter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/chat_engine/test_condense_question.py` & `gpt_index-0.7.6/tests/chat_engine/test_condense_question.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/chat_engine/test_simple.py` & `gpt_index-0.7.6/tests/chat_engine/test_simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/conftest.py` & `gpt_index-0.7.6/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -74,7 +74,12 @@
 
 
 @pytest.fixture()
 def mock_service_context(
     patch_token_text_splitter: Any, patch_llm_predictor: Any
 ) -> ServiceContext:
     return ServiceContext.from_defaults(embed_model=MockEmbedding())
+
+
+@pytest.fixture()
+def mock_llm() -> MockLLM:
+    return MockLLM()
```

### Comparing `gpt_index-0.7.5/tests/embeddings/test_base.py` & `gpt_index-0.7.6/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/composability/test_utils.py` & `gpt_index-0.7.6/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/conftest.py` & `gpt_index-0.7.6/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/document_summary/test_index.py` & `gpt_index-0.7.6/tests/indices/document_summary/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/empty/test_base.py` & `gpt_index-0.7.6/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/keyword_table/test_base.py` & `gpt_index-0.7.6/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/keyword_table/test_retrievers.py` & `gpt_index-0.7.6/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/keyword_table/test_utils.py` & `gpt_index-0.7.6/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/knowledge_graph/test_base.py` & `gpt_index-0.7.6/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/knowledge_graph/test_retrievers.py` & `gpt_index-0.7.6/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/list/test_index.py` & `gpt_index-0.7.6/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/list/test_retrievers.py` & `gpt_index-0.7.6/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/postprocessor/test_base.py` & `gpt_index-0.7.6/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/postprocessor/test_llm_rerank.py` & `gpt_index-0.7.6/tests/indices/postprocessor/test_llm_rerank.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/postprocessor/test_optimizer.py` & `gpt_index-0.7.6/tests/indices/postprocessor/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/query/conftest.py` & `gpt_index-0.7.6/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/query/query_transform/test_base.py` & `gpt_index-0.7.6/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/query/test_compose.py` & `gpt_index-0.7.6/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/query/test_compose_vector.py` & `gpt_index-0.7.6/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/query/test_embedding_utils.py` & `gpt_index-0.7.6/tests/indices/query/test_embedding_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/query/test_query_bundle.py` & `gpt_index-0.7.6/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/struct_store/conftest.py` & `gpt_index-0.7.6/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/struct_store/test_base.py` & `gpt_index-0.7.6/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/struct_store/test_json_query.py` & `gpt_index-0.7.6/tests/indices/struct_store/test_json_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/struct_store/test_sql_query.py` & `gpt_index-0.7.6/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/test_loading.py` & `gpt_index-0.7.6/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/test_loading_graph.py` & `gpt_index-0.7.6/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/test_node_utils.py` & `gpt_index-0.7.6/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/test_prompt_helper.py` & `gpt_index-0.7.6/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/tree/conftest.py` & `gpt_index-0.7.6/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/tree/test_embedding_retriever.py` & `gpt_index-0.7.6/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/tree/test_index.py` & `gpt_index-0.7.6/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/tree/test_retrievers.py` & `gpt_index-0.7.6/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/vector_store/auto_retriever/test_output_parser.py` & `gpt_index-0.7.6/tests/indices/vector_store/auto_retriever/test_output_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/vector_store/conftest.py` & `gpt_index-0.7.6/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/vector_store/mock_faiss.py` & `gpt_index-0.7.6/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/vector_store/mock_services.py` & `gpt_index-0.7.6/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/vector_store/test_faiss.py` & `gpt_index-0.7.6/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/vector_store/test_myscale.py` & `gpt_index-0.7.6/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/vector_store/test_pinecone.py` & `gpt_index-0.7.6/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/vector_store/test_retrievers.py` & `gpt_index-0.7.6/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/vector_store/test_simple.py` & `gpt_index-0.7.6/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/indices/vector_store/utils.py` & `gpt_index-0.7.6/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/langchain_helpers/test_text_splitter.py` & `gpt_index-0.7.6/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/llm_predictor/test_base.py` & `gpt_index-0.7.6/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/llm_predictor/vellum/conftest.py` & `gpt_index-0.7.6/tests/llm_predictor/vellum/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/llm_predictor/vellum/test_predictor.py` & `gpt_index-0.7.6/tests/llm_predictor/vellum/test_predictor.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/llm_predictor/vellum/test_prompt_registry.py` & `gpt_index-0.7.6/tests/llm_predictor/vellum/test_prompt_registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/llms/test_anthropic.py` & `gpt_index-0.7.6/tests/llms/test_anthropic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from llama_index.llms.anthropic import Anthropic
 from llama_index.llms.base import ChatMessage
 
 try:
     import anthropic
 except ImportError:
-    anthropic = None
+    anthropic = None  # type: ignore
 
 
 @pytest.mark.skipif(anthropic is None, reason="anthropic not installed")
 def test_basic() -> None:
     llm = Anthropic(model="test")
     test_prompt = "test prompt"
     response = llm.complete(test_prompt)
```

### Comparing `gpt_index-0.7.5/tests/llms/test_anthropic_utils.py` & `gpt_index-0.7.6/tests/llms/test_anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/llms/test_custom.py` & `gpt_index-0.7.6/tests/llms/test_custom.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/llms/test_langchain.py` & `gpt_index-0.7.6/tests/llms/test_langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/llms/test_openai.py` & `gpt_index-0.7.6/tests/llms/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/llms/test_openai_utils.py` & `gpt_index-0.7.6/tests/llms/test_openai_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/llms/test_palm.py` & `gpt_index-0.7.6/tests/llms/test_palm.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/logger/test_base.py` & `gpt_index-0.7.6/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/mock_utils/mock_predict.py` & `gpt_index-0.7.6/tests/mock_utils/mock_predict.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/mock_utils/mock_prompts.py` & `gpt_index-0.7.6/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/mock_utils/mock_text_splitter.py` & `gpt_index-0.7.6/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/mock_utils/mock_utils.py` & `gpt_index-0.7.6/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/objects/test_base.py` & `gpt_index-0.7.6/tests/objects/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/objects/test_node_mapping.py` & `gpt_index-0.7.6/tests/objects/test_node_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         "Tool name: test_tool\n" "Tool description: test\n"
     ) in node_mapping.to_node(tool1).get_text()
     assert node_mapping.from_node(node_mapping.to_node(tool1)) == tool1
     assert (
         "Tool name: test_tool2\n" "Tool description: test\n"
     ) in node_mapping.to_node(tool2).get_text()
     recon_tool2 = node_mapping.from_node(node_mapping.to_node(tool2))
-    assert recon_tool2(1, 2) == 3
+    assert recon_tool2(1, 2).raw_output == 3
 
     tool3 = FunctionTool.from_defaults(
         fn=lambda x, y: x * y, name="test_tool3", description="test3"
     )
     node_mapping.add_object(tool3)
     assert (
         "Tool name: test_tool3\n" "Tool description: test3\n"
```

### Comparing `gpt_index-0.7.5/tests/output_parsers/test_base.py` & `gpt_index-0.7.6/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/output_parsers/test_pydantic.py` & `gpt_index-0.7.6/tests/output_parsers/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/output_parsers/test_selection.py` & `gpt_index-0.7.6/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/playground/test_base.py` & `gpt_index-0.7.6/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/program/test_guidance.py` & `gpt_index-0.7.6/tests/program/test_guidance.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/program/test_llm_program.py` & `gpt_index-0.7.6/tests/program/test_llm_program.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/prompts/test_base.py` & `gpt_index-0.7.6/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/prompts/test_guidance_utils.py` & `gpt_index-0.7.6/tests/prompts/test_guidance_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/question_gen/test_guidance_generator.py` & `gpt_index-0.7.6/tests/question_gen/test_guidance_generator.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/question_gen/test_llm_generators.py` & `gpt_index-0.7.6/tests/question_gen/test_llm_generators.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/readers/test_file.py` & `gpt_index-0.7.6/tests/readers/test_file.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/readers/test_json.py` & `gpt_index-0.7.6/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/readers/test_mongo.py` & `gpt_index-0.7.6/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/selectors/test_llm_selectors.py` & `gpt_index-0.7.6/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/storage/conftest.py` & `gpt_index-0.7.6/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/storage/docstore/test_dynamodb_docstore.py` & `gpt_index-0.7.6/tests/storage/docstore/test_dynamodb_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/storage/docstore/test_mongo_docstore.py` & `gpt_index-0.7.6/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/storage/docstore/test_redis_docstore.py` & `gpt_index-0.7.6/tests/storage/docstore/test_redis_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/storage/docstore/test_simple_docstore.py` & `gpt_index-0.7.6/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/storage/test_storage_context.py` & `gpt_index-0.7.6/tests/storage/test_storage_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/test_utils.py` & `gpt_index-0.7.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/token_predictor/test_base.py` & `gpt_index-0.7.6/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/tools/test_base.py` & `gpt_index-0.7.6/tests/tools/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     assert function_tool.metadata.description == "bar"
     assert function_tool.metadata.fn_schema is not None
     actual_schema = function_tool.metadata.fn_schema.schema()
     # note: no type
     assert "x" in actual_schema["properties"]
 
     result = function_tool(1)
-    assert result == "1"
+    assert str(result) == "1"
 
     # test adding typing to function
     def tmp_function(x: int) -> str:
         return str(x)
 
     function_tool = FunctionTool.from_defaults(
         tmp_function, name="foo", description="bar"
@@ -44,11 +44,11 @@
 
     function_tool = FunctionTool.from_defaults(
         lambda x, y: str(x) + "," + str(y),
         name="foo",
         description="bar",
         fn_schema=TestSchema,
     )
-    assert function_tool(1, 2) == "1,2"
+    assert str(function_tool(1, 2)) == "1,2"
     langchain_tool2 = function_tool.to_langchain_structured_tool()
     assert langchain_tool2.run({"x": 1, "y": 2}) == "1,2"
     assert langchain_tool2.args_schema == TestSchema
```

### Comparing `gpt_index-0.7.5/tests/tools/test_ondemand_loader.py` & `gpt_index-0.7.6/tests/tools/test_ondemand_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,14 @@
         index_cls=VectorStoreIndex,
         index_kwargs={"service_context": mock_service_context},
         name="ondemand_loader_tool",
         description="ondemand_loader_tool_desc",
         fn_schema=TestSchemaSpec,
     )
     response = tool(["Hello world."], query_str="What is?")
-    assert response == "What is?:Hello world."
+    assert str(response) == "What is?:Hello world."
 
     # convert tool to structured langchain tool
     lc_tool = tool.to_langchain_structured_tool()
     assert lc_tool.args_schema == TestSchemaSpec
     response = lc_tool.run({"texts": ["Hello world."], "query_str": "What is?"})
-    assert response == "What is?:Hello world."
+    assert str(response) == "What is?:Hello world."
```

### Comparing `gpt_index-0.7.5/tests/tools/test_utils.py` & `gpt_index-0.7.6/tests/tools/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/tools/tool_spec/test_base.py` & `gpt_index-0.7.6/tests/tools/tool_spec/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,30 +53,33 @@
     tools = tool_spec.to_tool_list()
     assert len(tools) == 3
     assert tools[0].metadata.name == "foo"
     assert tools[0].metadata.description == "foo(arg1: str, arg2: int) -> str\nFoo."
     assert tools[0].fn("hello", 1) == "foo hello 1"
     assert tools[1].metadata.name == "bar"
     assert tools[1].metadata.description == "bar(arg1: bool) -> str\nBar."
-    assert tools[1](True) == "bar True"
+    assert str(tools[1](True)) == "bar True"
     assert tools[2].metadata.name == "abc"
     assert tools[2].metadata.description == "abc(arg1: str) -> str\n"
     assert tools[2].metadata.fn_schema == AbcSchema
 
     # test metadata mapping
     tools = tool_spec.to_tool_list(
         func_to_metadata_mapping={
-            "foo": ToolMetadata("foo_description", name="foo_name"),
+            "foo": ToolMetadata(
+                "foo_description", name="foo_name", fn_schema=FooSchema
+            ),
         }
     )
     assert len(tools) == 3
     assert tools[0].metadata.name == "foo_name"
     assert tools[0].metadata.description == "foo_description"
     assert tools[0].metadata.fn_schema is not None
     fn_schema = tools[0].metadata.fn_schema.schema()
+    print(fn_schema)
     assert fn_schema["properties"]["arg1"]["type"] == "string"
     assert fn_schema["properties"]["arg2"]["type"] == "integer"
     assert tools[1].metadata.name == "bar"
     assert tools[1].metadata.description == "bar(arg1: bool) -> str\nBar."
     assert tools[1].metadata.fn_schema is not None
     fn_schema = tools[1].metadata.fn_schema.schema()
     assert fn_schema["properties"]["arg1"]["type"] == "boolean"
```

### Comparing `gpt_index-0.7.5/tests/vector_stores/test_docarray.py` & `gpt_index-0.7.6/tests/vector_stores/test_docarray.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/vector_stores/test_postgres.py` & `gpt_index-0.7.6/tests/vector_stores/test_postgres.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/vector_stores/test_qdrant.py` & `gpt_index-0.7.6/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/vector_stores/test_tair.py` & `gpt_index-0.7.6/tests/vector_stores/test_tair.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.7.5/tests/vector_stores/test_weaviate.py` & `gpt_index-0.7.6/tests/vector_stores/test_weaviate.py`

 * *Files identical despite different names*

