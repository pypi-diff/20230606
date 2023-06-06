# Comparing `tmp/langflow-0.0.81.tar.gz` & `tmp/langflow-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-0.0.81.tar", max compression
+gzip compressed data, was "langflow-0.0.83.tar", max compression
```

## Comparing `langflow-0.0.81.tar` & `langflow-0.0.83.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1065 2023-06-02 22:24:10.421499 langflow-0.0.81/LICENSE
--rw-r--r--   0        0        0    10199 2023-06-02 22:24:10.421499 langflow-0.0.81/README.md
--rw-r--r--   0        0        0     2042 2023-06-02 22:24:10.441500 langflow-0.0.81/pyproject.toml
--rw-r--r--   0        0        0      152 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/__init__.py
--rw-r--r--   0        0        0     3851 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/__main__.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/api/__init__.py
--rw-r--r--   0        0        0     2032 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/api/base.py
--rw-r--r--   0        0        0     1124 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/api/callback.py
--rw-r--r--   0        0        0      776 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/api/chat.py
--rw-r--r--   0        0        0     8558 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/api/chat_manager.py
--rw-r--r--   0        0        0     1246 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/api/endpoints.py
--rw-r--r--   0        0        0     1443 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/api/schemas.py
--rw-r--r--   0        0        0     1765 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/api/validate.py
--rw-r--r--   0        0        0       57 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/cache/__init__.py
--rw-r--r--   0        0        0     4329 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/cache/base.py
--rw-r--r--   0        0        0     4478 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/cache/manager.py
--rw-r--r--   0        0        0     2580 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/config.yaml
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/custom/__init__.py
--rw-r--r--   0        0        0     1213 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/custom/customs.py
--rw-r--r--   0        0        0      889 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg
--rw-r--r--   0        0        0     2521 2023-06-02 22:25:07.582097 langflow-0.0.81/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg
--rw-r--r--   0        0        0     3513 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg
--rw-r--r--   0        0        0     1578 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg
--rw-r--r--   0        0        0     1705 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg
--rw-r--r--   0        0        0     7249 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg
--rw-r--r--   0        0        0     1106 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg
--rw-r--r--   0        0        0     2007 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg
--rw-r--r--   0        0        0     6783 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/bing-60c0c591.svg
--rw-r--r--   0        0        0      622 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/chroma-65ceac37.svg
--rw-r--r--   0        0        0     1450 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/cohere-f09153b9.svg
--rw-r--r--   0        0        0     1667 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg
--rw-r--r--   0        0        0    11568 2023-06-02 22:25:07.582097 langflow-0.0.81/src/backend/langflow/frontend/assets/froze-flow-494453cf.png
--rw-r--r--   0        0        0     1111 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg
--rw-r--r--   0        0        0      688 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/google-0cf576a5.svg
--rw-r--r--   0        0        0    35286 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg
--rw-r--r--   0        0        0      789 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg
--rw-r--r--   0        0        0  4102332 2023-06-02 22:25:07.582097 langflow-0.0.81/src/backend/langflow/frontend/assets/index-8d4095bd.js
--rw-r--r--   0        0        0    82705 2023-06-02 22:25:07.582097 langflow-0.0.81/src/backend/langflow/frontend/assets/index-c2ccece6.css
--rw-r--r--   0        0        0     2212 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg
--rw-r--r--   0        0        0     2509 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/openAI-2c85883b.svg
--rw-r--r--   0        0        0     1539 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg
--rw-r--r--   0        0        0     4310 2023-06-02 22:25:07.582097 langflow-0.0.81/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
--rw-r--r--   0        0        0   104188 2023-06-02 22:25:07.578097 langflow-0.0.81/src/backend/langflow/frontend/favicon.ico
--rw-r--r--   0        0        0      622 2023-06-02 22:25:07.582097 langflow-0.0.81/src/backend/langflow/frontend/index.html
--rw-r--r--   0        0        0      119 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/graph/__init__.py
--rw-r--r--   0        0        0    11139 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/graph/base.py
--rw-r--r--   0        0        0       72 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/graph/constants.py
--rw-r--r--   0        0        0     6217 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/graph/graph.py
--rw-r--r--   0        0        0     6444 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/graph/nodes.py
--rw-r--r--   0        0        0      420 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/graph/utils.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/__init__.py
--rw-r--r--   0        0        0       84 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/agents/__init__.py
--rw-r--r--   0        0        0     1843 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/agents/base.py
--rw-r--r--   0        0        0    10017 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/agents/custom.py
--rw-r--r--   0        0        0     1447 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/agents/prebuilt.py
--rw-r--r--   0        0        0     2991 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/base.py
--rw-r--r--   0        0        0       84 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/chains/__init__.py
--rw-r--r--   0        0        0     2008 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/chains/base.py
--rw-r--r--   0        0        0     4084 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/chains/custom.py
--rw-r--r--   0        0        0     1979 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/custom_lists.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/document_loaders/__init__.py
--rw-r--r--   0        0        0     5759 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/document_loaders/base.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/embeddings/__init__.py
--rw-r--r--   0        0        0     1445 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/embeddings/base.py
--rw-r--r--   0        0        0      171 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/importing/__init__.py
--rw-r--r--   0        0        0     4811 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/importing/utils.py
--rw-r--r--   0        0        0     1668 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/listing.py
--rw-r--r--   0        0        0       78 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/llms/__init__.py
--rw-r--r--   0        0        0     1355 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/llms/base.py
--rw-r--r--   0        0        0    13821 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/loading.py
--rw-r--r--   0        0        0       88 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/memories/__init__.py
--rw-r--r--   0        0        0     1541 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/memories/base.py
--rw-r--r--   0        0        0       87 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/prompts/__init__.py
--rw-r--r--   0        0        0     2459 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/prompts/base.py
--rw-r--r--   0        0        0     2618 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/prompts/custom.py
--rw-r--r--   0        0        0    10020 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/run.py
--rw-r--r--   0        0        0      106 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/text_splitters/__init__.py
--rw-r--r--   0        0        0     2309 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/text_splitters/base.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/toolkits/__init__.py
--rw-r--r--   0        0        0     2447 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/toolkits/base.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/toolkits/custom.py
--rw-r--r--   0        0        0       81 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/tools/__init__.py
--rw-r--r--   0        0        0     5402 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/tools/base.py
--rw-r--r--   0        0        0      823 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/tools/constants.py
--rw-r--r--   0        0        0      811 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/tools/custom.py
--rw-r--r--   0        0        0     4328 2023-06-02 22:24:10.441500 langflow-0.0.81/src/backend/langflow/interface/tools/util.py
--rw-r--r--   0        0        0     1813 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/interface/types.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/interface/utilities/__init__.py
--rw-r--r--   0        0        0     2294 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/interface/utilities/base.py
--rw-r--r--   0        0        0     1569 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/interface/utils.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/interface/vector_store/__init__.py
--rw-r--r--   0        0        0     1813 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/interface/vector_store/base.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/interface/wrappers/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/interface/wrappers/base.py
--rw-r--r--   0        0        0       29 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/jcloud.yml
--rw-r--r--   0        0        0      362 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/lcserve.py
--rw-r--r--   0        0        0      816 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/main.py
--rw-r--r--   0        0        0      579 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/server.py
--rw-r--r--   0        0        0     2128 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/settings.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/field/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/field/base.py
--rw-r--r--   0        0        0      291 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/__init__.py
--rw-r--r--   0        0        0     6631 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/agents.py
--rw-r--r--   0        0        0     7516 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/base.py
--rw-r--r--   0        0        0     4720 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/chains.py
--rw-r--r--   0        0        0      683 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/constants.py
--rw-r--r--   0        0        0     1680 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/embeddings.py
--rw-r--r--   0        0        0     1889 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/llms.py
--rw-r--r--   0        0        0      648 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/memories.py
--rw-r--r--   0        0        0     3535 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/prompts.py
--rw-r--r--   0        0        0     2374 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/tools.py
--rw-r--r--   0        0        0      823 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/utilities.py
--rw-r--r--   0        0        0     2648 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/frontend_node/vectorstores.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/template/__init__.py
--rw-r--r--   0        0        0      819 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/template/template/base.py
--rw-r--r--   0        0        0        0 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/utils/__init__.py
--rw-r--r--   0        0        0      364 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/utils/constants.py
--rw-r--r--   0        0        0      914 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/utils/logger.py
--rw-r--r--   0        0        0     3169 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/utils/payload.py
--rw-r--r--   0        0        0    10983 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/utils/util.py
--rw-r--r--   0        0        0     5311 2023-06-02 22:24:10.445500 langflow-0.0.81/src/backend/langflow/utils/validate.py
--rw-r--r--   0        0        0    12544 1970-01-01 00:00:00.000000 langflow-0.0.81/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-06 10:55:55.228335 langflow-0.0.83/LICENSE
+-rw-r--r--   0        0        0    10199 2023-06-06 10:55:55.228335 langflow-0.0.83/README.md
+-rw-r--r--   0        0        0     2042 2023-06-06 10:55:55.244335 langflow-0.0.83/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/__init__.py
+-rw-r--r--   0        0        0     3851 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/api/__init__.py
+-rw-r--r--   0        0        0     2032 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/api/base.py
+-rw-r--r--   0        0        0     1124 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/api/callback.py
+-rw-r--r--   0        0        0      776 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/api/chat.py
+-rw-r--r--   0        0        0     8558 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/api/chat_manager.py
+-rw-r--r--   0        0        0     1246 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/api/endpoints.py
+-rw-r--r--   0        0        0     1443 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/api/schemas.py
+-rw-r--r--   0        0        0     1765 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/api/validate.py
+-rw-r--r--   0        0        0       57 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/cache/__init__.py
+-rw-r--r--   0        0        0     4329 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/cache/base.py
+-rw-r--r--   0        0        0     4478 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/cache/manager.py
+-rw-r--r--   0        0        0     2580 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/config.yaml
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/custom/__init__.py
+-rw-r--r--   0        0        0     1213 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/custom/customs.py
+-rw-r--r--   0        0        0      889 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg
+-rw-r--r--   0        0        0     2521 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg
+-rw-r--r--   0        0        0     3513 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg
+-rw-r--r--   0        0        0     1578 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg
+-rw-r--r--   0        0        0     1705 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg
+-rw-r--r--   0        0        0     7249 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg
+-rw-r--r--   0        0        0     1106 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg
+-rw-r--r--   0        0        0     2007 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg
+-rw-r--r--   0        0        0     6783 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/bing-60c0c591.svg
+-rw-r--r--   0        0        0      622 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/chroma-65ceac37.svg
+-rw-r--r--   0        0        0     1450 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/cohere-f09153b9.svg
+-rw-r--r--   0        0        0     1667 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg
+-rw-r--r--   0        0        0    11568 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/froze-flow-494453cf.png
+-rw-r--r--   0        0        0     1111 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg
+-rw-r--r--   0        0        0      688 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/google-0cf576a5.svg
+-rw-r--r--   0        0        0    35286 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg
+-rw-r--r--   0        0        0      789 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg
+-rw-r--r--   0        0        0  4102332 2023-06-06 10:57:10.945357 langflow-0.0.83/src/backend/langflow/frontend/assets/index-8d4095bd.js
+-rw-r--r--   0        0        0    82705 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/index-c2ccece6.css
+-rw-r--r--   0        0        0     2212 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg
+-rw-r--r--   0        0        0     2509 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/openAI-2c85883b.svg
+-rw-r--r--   0        0        0     1539 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg
+-rw-r--r--   0        0        0     4310 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
+-rw-r--r--   0        0        0   104188 2023-06-06 10:57:10.941357 langflow-0.0.83/src/backend/langflow/frontend/favicon.ico
+-rw-r--r--   0        0        0      622 2023-06-06 10:57:10.945357 langflow-0.0.83/src/backend/langflow/frontend/index.html
+-rw-r--r--   0        0        0      119 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/graph/__init__.py
+-rw-r--r--   0        0        0    11139 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/graph/base.py
+-rw-r--r--   0        0        0       72 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/graph/constants.py
+-rw-r--r--   0        0        0     6217 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/graph/graph.py
+-rw-r--r--   0        0        0     6444 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/graph/nodes.py
+-rw-r--r--   0        0        0      420 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/graph/utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/agents/__init__.py
+-rw-r--r--   0        0        0     1843 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/agents/base.py
+-rw-r--r--   0        0        0    10017 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/agents/custom.py
+-rw-r--r--   0        0        0     1447 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/agents/prebuilt.py
+-rw-r--r--   0        0        0     2991 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/base.py
+-rw-r--r--   0        0        0       84 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/chains/__init__.py
+-rw-r--r--   0        0        0     2008 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/chains/base.py
+-rw-r--r--   0        0        0     4084 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/chains/custom.py
+-rw-r--r--   0        0        0     1979 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/custom_lists.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/document_loaders/__init__.py
+-rw-r--r--   0        0        0     5759 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/document_loaders/base.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/embeddings/__init__.py
+-rw-r--r--   0        0        0     1445 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/embeddings/base.py
+-rw-r--r--   0        0        0      171 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/importing/__init__.py
+-rw-r--r--   0        0        0     4811 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/importing/utils.py
+-rw-r--r--   0        0        0     1668 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/listing.py
+-rw-r--r--   0        0        0       78 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/llms/__init__.py
+-rw-r--r--   0        0        0     1355 2023-06-06 10:55:55.244335 langflow-0.0.83/src/backend/langflow/interface/llms/base.py
+-rw-r--r--   0        0        0    13821 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/loading.py
+-rw-r--r--   0        0        0       88 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/memories/__init__.py
+-rw-r--r--   0        0        0     1541 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/memories/base.py
+-rw-r--r--   0        0        0       87 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/prompts/__init__.py
+-rw-r--r--   0        0        0     2459 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/prompts/base.py
+-rw-r--r--   0        0        0     2618 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/prompts/custom.py
+-rw-r--r--   0        0        0    10020 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/run.py
+-rw-r--r--   0        0        0      106 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/text_splitters/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/text_splitters/base.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/toolkits/__init__.py
+-rw-r--r--   0        0        0     2447 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/toolkits/custom.py
+-rw-r--r--   0        0        0       81 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/tools/__init__.py
+-rw-r--r--   0        0        0     5402 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/tools/base.py
+-rw-r--r--   0        0        0      823 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/tools/constants.py
+-rw-r--r--   0        0        0      811 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/tools/custom.py
+-rw-r--r--   0        0        0     4328 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/tools/util.py
+-rw-r--r--   0        0        0     1813 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/types.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/utilities/__init__.py
+-rw-r--r--   0        0        0     2294 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/utilities/base.py
+-rw-r--r--   0        0        0     1569 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/utils.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/vector_store/__init__.py
+-rw-r--r--   0        0        0     1813 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/vector_store/base.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/wrappers/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/interface/wrappers/base.py
+-rw-r--r--   0        0        0       29 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/jcloud.yml
+-rw-r--r--   0        0        0      362 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/lcserve.py
+-rw-r--r--   0        0        0      816 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/main.py
+-rw-r--r--   0        0        0      579 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/server.py
+-rw-r--r--   0        0        0     2128 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/settings.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/field/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/field/base.py
+-rw-r--r--   0        0        0      291 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/__init__.py
+-rw-r--r--   0        0        0     6631 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/agents.py
+-rw-r--r--   0        0        0     7516 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/base.py
+-rw-r--r--   0        0        0     4720 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/chains.py
+-rw-r--r--   0        0        0      683 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/constants.py
+-rw-r--r--   0        0        0     1680 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/embeddings.py
+-rw-r--r--   0        0        0     1889 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/llms.py
+-rw-r--r--   0        0        0      648 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/memories.py
+-rw-r--r--   0        0        0     3535 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/prompts.py
+-rw-r--r--   0        0        0     2374 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/tools.py
+-rw-r--r--   0        0        0      823 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/utilities.py
+-rw-r--r--   0        0        0     2648 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/frontend_node/vectorstores.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/template/__init__.py
+-rw-r--r--   0        0        0      819 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/template/template/base.py
+-rw-r--r--   0        0        0        0 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/utils/__init__.py
+-rw-r--r--   0        0        0      364 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/utils/constants.py
+-rw-r--r--   0        0        0      914 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/utils/logger.py
+-rw-r--r--   0        0        0     3169 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/utils/payload.py
+-rw-r--r--   0        0        0    10983 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/utils/util.py
+-rw-r--r--   0        0        0     5311 2023-06-06 10:55:55.248335 langflow-0.0.83/src/backend/langflow/utils/validate.py
+-rw-r--r--   0        0        0    12535 1970-01-01 00:00:00.000000 langflow-0.0.83/PKG-INFO
```

### Comparing `langflow-0.0.81/LICENSE` & `langflow-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/README.md` & `langflow-0.0.83/README.md`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/pyproject.toml` & `langflow-0.0.83/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "0.0.81"
+version = "0.0.83"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Ibis Prevedello <ibiscp@gmail.com>",
     "Lucas Eduoli <lucaseduoli@gmail.com>",
     "Otávio Anovazzi <otavio2204@gmail.com>",
@@ -45,15 +45,15 @@
 pysrt = "^1.1.2"
 fake-useragent = "^1.1.3"
 docstring-parser = "^0.15"
 psycopg2-binary = "^2.9.6"
 pyarrow = "^11.0.0"
 tiktoken = "^0.3.3"
 wikipedia = "^1.4.0"
-langchain-serve = { version = "^0.0.38", optional = true }
+langchain-serve = { version = ">0.0.39", optional = true }
 qdrant-client = "^1.2.0"
 websockets = "^11.0.3"
 weaviate-client = "^3.19.2"
 jina = "3.15.2"
 sentence-transformers = "^2.2.2"
 ctransformers = "^0.2.2"
 cohere = "^4.6.0"
```

### Comparing `langflow-0.0.81/src/backend/langflow/__main__.py` & `langflow-0.0.83/src/backend/langflow/__main__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/api/base.py` & `langflow-0.0.83/src/backend/langflow/api/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/api/callback.py` & `langflow-0.0.83/src/backend/langflow/api/callback.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/api/chat.py` & `langflow-0.0.83/src/backend/langflow/api/chat.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/api/chat_manager.py` & `langflow-0.0.83/src/backend/langflow/api/chat_manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/api/endpoints.py` & `langflow-0.0.83/src/backend/langflow/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/api/schemas.py` & `langflow-0.0.83/src/backend/langflow/api/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/api/validate.py` & `langflow-0.0.83/src/backend/langflow/api/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/cache/base.py` & `langflow-0.0.83/src/backend/langflow/cache/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/cache/manager.py` & `langflow-0.0.83/src/backend/langflow/cache/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/config.yaml` & `langflow-0.0.83/src/backend/langflow/config.yaml`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/custom/customs.py` & `langflow-0.0.83/src/backend/langflow/custom/customs.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/bing-60c0c591.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/bing-60c0c591.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/chroma-65ceac37.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/chroma-65ceac37.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/cohere-f09153b9.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/cohere-f09153b9.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/froze-flow-494453cf.png` & `langflow-0.0.83/src/backend/langflow/frontend/assets/froze-flow-494453cf.png`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/google-0cf576a5.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/google-0cf576a5.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/index-8d4095bd.js` & `langflow-0.0.83/src/backend/langflow/frontend/assets/index-8d4095bd.js`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/index-c2ccece6.css` & `langflow-0.0.83/src/backend/langflow/frontend/assets/index-c2ccece6.css`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/openAI-2c85883b.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/openAI-2c85883b.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg` & `langflow-0.0.83/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js` & `langflow-0.0.83/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/favicon.ico` & `langflow-0.0.83/src/backend/langflow/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/frontend/index.html` & `langflow-0.0.83/src/backend/langflow/frontend/index.html`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/graph/base.py` & `langflow-0.0.83/src/backend/langflow/graph/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/graph/graph.py` & `langflow-0.0.83/src/backend/langflow/graph/graph.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/graph/nodes.py` & `langflow-0.0.83/src/backend/langflow/graph/nodes.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/agents/base.py` & `langflow-0.0.83/src/backend/langflow/interface/agents/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/agents/custom.py` & `langflow-0.0.83/src/backend/langflow/interface/agents/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/agents/prebuilt.py` & `langflow-0.0.83/src/backend/langflow/interface/agents/prebuilt.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/base.py` & `langflow-0.0.83/src/backend/langflow/interface/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/chains/base.py` & `langflow-0.0.83/src/backend/langflow/interface/chains/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/chains/custom.py` & `langflow-0.0.83/src/backend/langflow/interface/chains/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/custom_lists.py` & `langflow-0.0.83/src/backend/langflow/interface/custom_lists.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/document_loaders/base.py` & `langflow-0.0.83/src/backend/langflow/interface/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/embeddings/base.py` & `langflow-0.0.83/src/backend/langflow/interface/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/importing/utils.py` & `langflow-0.0.83/src/backend/langflow/interface/importing/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/listing.py` & `langflow-0.0.83/src/backend/langflow/interface/listing.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/llms/base.py` & `langflow-0.0.83/src/backend/langflow/interface/llms/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/loading.py` & `langflow-0.0.83/src/backend/langflow/interface/loading.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/memories/base.py` & `langflow-0.0.83/src/backend/langflow/interface/memories/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/prompts/base.py` & `langflow-0.0.83/src/backend/langflow/interface/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/prompts/custom.py` & `langflow-0.0.83/src/backend/langflow/interface/prompts/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/run.py` & `langflow-0.0.83/src/backend/langflow/interface/run.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/text_splitters/base.py` & `langflow-0.0.83/src/backend/langflow/interface/text_splitters/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/toolkits/base.py` & `langflow-0.0.83/src/backend/langflow/interface/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/tools/base.py` & `langflow-0.0.83/src/backend/langflow/interface/tools/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/tools/constants.py` & `langflow-0.0.83/src/backend/langflow/interface/tools/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/tools/custom.py` & `langflow-0.0.83/src/backend/langflow/interface/tools/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/tools/util.py` & `langflow-0.0.83/src/backend/langflow/interface/tools/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/types.py` & `langflow-0.0.83/src/backend/langflow/interface/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/utilities/base.py` & `langflow-0.0.83/src/backend/langflow/interface/utilities/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/utils.py` & `langflow-0.0.83/src/backend/langflow/interface/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/vector_store/base.py` & `langflow-0.0.83/src/backend/langflow/interface/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/interface/wrappers/base.py` & `langflow-0.0.83/src/backend/langflow/interface/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/main.py` & `langflow-0.0.83/src/backend/langflow/main.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/server.py` & `langflow-0.0.83/src/backend/langflow/server.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/settings.py` & `langflow-0.0.83/src/backend/langflow/settings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/field/base.py` & `langflow-0.0.83/src/backend/langflow/template/field/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/agents.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/agents.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/base.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/chains.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/chains.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/constants.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/embeddings.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/embeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/llms.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/llms.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/memories.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/memories.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/prompts.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/prompts.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/tools.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/tools.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/utilities.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/utilities.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/frontend_node/vectorstores.py` & `langflow-0.0.83/src/backend/langflow/template/frontend_node/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/template/template/base.py` & `langflow-0.0.83/src/backend/langflow/template/template/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/utils/logger.py` & `langflow-0.0.83/src/backend/langflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/utils/payload.py` & `langflow-0.0.83/src/backend/langflow/utils/payload.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/utils/util.py` & `langflow-0.0.83/src/backend/langflow/utils/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/src/backend/langflow/utils/validate.py` & `langflow-0.0.83/src/backend/langflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.81/PKG-INFO` & `langflow-0.0.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 0.0.81
+Version: 0.0.83
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Gabriel Almeida
@@ -27,15 +27,15 @@
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: google-api-python-client (>=2.79.0,<3.0.0)
 Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: huggingface-hub (>=0.13.3,<0.14.0)
 Requires-Dist: jina (==3.15.2)
 Requires-Dist: langchain (>=0.0.186,<0.0.187)
-Requires-Dist: langchain-serve (>=0.0.38,<0.0.39) ; extra == "deploy"
+Requires-Dist: langchain-serve (>0.0.39) ; extra == "deploy"
 Requires-Dist: llama-cpp-python (>=0.1.50,<0.2.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langflow Version: 0.0.81 Summary: A Python package
+Metadata-Version: 2.1 Name: langflow Version: 0.0.83 Summary: A Python package
 with a built-in web application Home-page: https://github.com/logspace-ai/
 langflow License: MIT Keywords: nlp,langchain,openai,gpt,gui Author: Logspace
 Author-email: contact@logspace.ai Maintainer: Gabriel Almeida Maintainer-email:
 gabriel@logspace.ai Requires-Python: >=3.9,<3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -11,18 +11,18 @@
 (>=4.6.0,<5.0.0) Requires-Dist: ctransformers (>=0.2.2,<0.3.0) Requires-Dist:
 dill (>=0.3.6,<0.4.0) Requires-Dist: docstring-parser (>=0.15,<0.16) Requires-
 Dist: faiss-cpu (>=1.7.4,<2.0.0) Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0) Requires-Dist: google-api-python-
 client (>=2.79.0,<3.0.0) Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist: huggingface-hub
 (>=0.13.3,<0.14.0) Requires-Dist: jina (==3.15.2) Requires-Dist: langchain
-(>=0.0.186,<0.0.187) Requires-Dist: langchain-serve (>=0.0.38,<0.0.39) ; extra
-== "deploy" Requires-Dist: llama-cpp-python (>=0.1.50,<0.2.0) Requires-Dist:
-lxml (>=4.9.2,<5.0.0) Requires-Dist: networkx (>=3.1,<4.0) Requires-Dist:
-openai (>=0.27.7,<0.28.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist:
+(>=0.0.186,<0.0.187) Requires-Dist: langchain-serve (>0.0.39) ; extra ==
+"deploy" Requires-Dist: llama-cpp-python (>=0.1.50,<0.2.0) Requires-Dist: lxml
+(>=4.9.2,<5.0.0) Requires-Dist: networkx (>=3.1,<4.0) Requires-Dist: openai
+(>=0.27.7,<0.28.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist:
 psycopg2-binary (>=2.9.6,<3.0.0) Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: pypdf (>=3.7.1,<4.0.0) Requires-Dist: pysrt (>=1.1.2,<2.0.0)
 Requires-Dist: qdrant-client (>=1.2.0,<2.0.0) Requires-Dist: rich
 (>=13.3.3,<14.0.0) Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0) Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: types-pyyaml (>=6.0.12.8,<7.0.0.0) Requires-Dist: unstructured
 (>=0.5.11,<0.6.0) Requires-Dist: uvicorn (>=0.20.0,<0.21.0) Requires-Dist:
```

