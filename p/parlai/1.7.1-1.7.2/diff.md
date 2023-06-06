# Comparing `tmp/parlai-1.7.1.tar.gz` & `tmp/parlai-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parlai-1.7.1.tar", last modified: Fri Sep 16 16:27:41 2022, max compression
+gzip compressed data, was "dist/parlai-1.7.2.tar", last modified: Tue Jun  6 20:17:51 2023, max compression
```

## Comparing `parlai-1.7.1.tar` & `parlai-1.7.2.tar`

### file list

```diff
@@ -1,1417 +1,1647 @@
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.979542 parlai-1.7.1/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1086 2022-08-23 20:50:09.000000 parlai-1.7.1/LICENSE
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10106 2022-09-16 16:27:37.978435 parlai-1.7.1/PKG-INFO
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10919 2022-08-23 20:50:09.000000 parlai-1.7.1/README.md
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:32.946829 parlai-1.7.1/example_parlai_internal/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:09.000000 parlai-1.7.1/example_parlai_internal/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:32.952917 parlai-1.7.1/parlai/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      222 2022-09-16 16:20:54.000000 parlai-1.7.1/parlai/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      547 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/__main__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:32.978743 parlai-1.7.1/parlai/agents/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:32.987792 parlai-1.7.1/parlai/agents/alice/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/alice/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2114 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/alice/alice.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.007788 parlai-1.7.1/parlai/agents/bart/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bart/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6036 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bart/bart.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    18448 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bart/convert_fairseq_to_parlai.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2824 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bart/modules.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.017620 parlai-1.7.1/parlai/agents/bert_classifier/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bert_classifier/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8642 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bert_classifier/bert_classifier.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.052161 parlai-1.7.1/parlai/agents/bert_ranker/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bert_ranker/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2599 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bert_ranker/bert_dictionary.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      840 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bert_ranker/bert_ranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10030 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bert_ranker/bi_encoder_ranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5336 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bert_ranker/both_encoder_ranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3421 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bert_ranker/cross_encoder_ranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7284 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/bert_ranker/helpers.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.070229 parlai-1.7.1/parlai/agents/examples/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/examples/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7495 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/examples/seq2seq.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3572 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/examples/tra.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6891 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/examples/transformer_variant.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.079847 parlai-1.7.1/parlai/agents/fid/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/fid/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    18942 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/fid/fid.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.089372 parlai-1.7.1/parlai/agents/fixed_response/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/fixed_response/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1320 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/fixed_response/fixed_response.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.103233 parlai-1.7.1/parlai/agents/hred/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/hred/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6521 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/hred/hred.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9697 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/hred/modules.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.131032 parlai-1.7.1/parlai/agents/hugging_face/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/hugging_face/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4067 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/hugging_face/dialogpt.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7932 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/hugging_face/dict.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    12801 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/hugging_face/gpt2.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      960 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/hugging_face/hugging_face.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    12969 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/hugging_face/t5.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.225261 parlai-1.7.1/parlai/agents/image_seq2seq/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/image_seq2seq/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8317 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/image_seq2seq/image_seq2seq.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    15611 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/image_seq2seq/modules.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.233978 parlai-1.7.1/parlai/agents/ir_baseline/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/ir_baseline/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9673 2022-08-23 20:50:09.000000 parlai-1.7.1/parlai/agents/ir_baseline/ir_baseline.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.246115 parlai-1.7.1/parlai/agents/local_human/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/local_human/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3011 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/local_human/local_human.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.259799 parlai-1.7.1/parlai/agents/memnn/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/memnn/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8089 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/memnn/memnn.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7626 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/memnn/modules.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.313868 parlai-1.7.1/parlai/agents/rag/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    12531 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/args.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6130 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/conversion_utils.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10212 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/dpr.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    15598 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/indexers.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    48820 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/model_types.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    21182 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/modules.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3456 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/polyfaiss.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    34716 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/rag.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5245 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/retrieve_api.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    50690 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/retrievers.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.327159 parlai-1.7.1/parlai/agents/rag/scripts/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/scripts/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7678 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/scripts/generate_dense_embeddings.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4832 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/rag/scripts/index_dense_embeddings.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.336452 parlai-1.7.1/parlai/agents/random_candidate/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/random_candidate/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2698 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/random_candidate/random_candidate.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.345466 parlai-1.7.1/parlai/agents/repeat_label/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/repeat_label/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3041 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/repeat_label/repeat_label.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.354383 parlai-1.7.1/parlai/agents/repeat_query/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/repeat_query/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1328 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/repeat_query/repeat_query.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.374246 parlai-1.7.1/parlai/agents/reranker/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/reranker/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      849 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/reranker/classifier_gpt2_reranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3899 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/reranker/classifier_reranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    22618 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/reranker/reranker.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.384449 parlai-1.7.1/parlai/agents/retriever_reader/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/retriever_reader/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3905 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/retriever_reader/retriever_reader.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.394013 parlai-1.7.1/parlai/agents/safe_local_human/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/safe_local_human/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4597 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/safe_local_human/safe_local_human.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.408970 parlai-1.7.1/parlai/agents/seq2seq/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/seq2seq/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    24820 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/seq2seq/modules.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9302 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/seq2seq/seq2seq.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.423333 parlai-1.7.1/parlai/agents/starspace/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/starspace/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2661 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/starspace/modules.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    20522 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/starspace/starspace.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.453717 parlai-1.7.1/parlai/agents/test_agents/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/test_agents/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3451 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/test_agents/counter.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      807 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/test_agents/null.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4375 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/test_agents/test_agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      971 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/test_agents/transformer_generator_prefix.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1387 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/test_agents/unigram.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.478498 parlai-1.7.1/parlai/agents/tfidf_retriever/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6267 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/build_tfidf.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2100 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/doc_db.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3573 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/tfidf_doc_ranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9999 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/tfidf_retriever.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.501396 parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/
--rwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)      718 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/__init__.py
--rwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)     3970 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/regexp_tokenizer.py
--rwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)     1630 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/simple_tokenizer.py
--rwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)     2103 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/spacy_tokenizer.py
--rwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)     2129 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/tokenizer.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4505 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/tfidf_retriever/utils.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.545833 parlai-1.7.1/parlai/agents/transformer/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5244 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/biencoder.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      343 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/classifier.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3755 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/crossencoder.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3329 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/decoder.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4429 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/dropout_poly.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      345 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/generator.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7810 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/image_polyencoder.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.594404 parlai-1.7.1/parlai/agents/transformer/modules/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      973 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10039 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/attention.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      248 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/constants.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    27590 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/decoder.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    14521 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/encoder.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1712 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/ffn.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1802 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/functions.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4674 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/generator.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6176 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/mem_net.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4897 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/modular.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1560 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/modules/wrappers.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    22684 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/polyencoder.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      335 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/ranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    15643 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/transformer/transformer.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.602534 parlai-1.7.1/parlai/agents/unigram/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/unigram/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3913 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/agents/unigram/unigram.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.607049 parlai-1.7.1/parlai/chat_service/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.626527 parlai-1.7.1/parlai/chat_service/core/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/core/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4946 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/core/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    30802 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/core/chat_service_manager.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.630769 parlai-1.7.1/parlai/chat_service/core/server/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/core/server/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5922 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/core/socket.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7095 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/core/world_runner.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.634405 parlai-1.7.1/parlai/chat_service/services/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.660019 parlai-1.7.1/parlai/chat_service/services/browser_chat/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/browser_chat/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      320 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/browser_chat/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      464 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/browser_chat/browser_manager.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5420 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/browser_chat/client.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1408 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/browser_chat/run.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.690971 parlai-1.7.1/parlai/chat_service/services/messenger/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      489 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/messenger/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5685 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/messenger/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11419 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/messenger/message_sender.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11193 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/messenger/messenger_manager.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1109 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/messenger/run.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1262 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/messenger/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.739155 parlai-1.7.1/parlai/chat_service/services/terminal_chat/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/terminal_chat/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      321 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/terminal_chat/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3646 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/terminal_chat/client.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1418 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/terminal_chat/run.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      458 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/terminal_chat/terminal_manager.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.761551 parlai-1.7.1/parlai/chat_service/services/websocket/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/websocket/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2424 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/websocket/agents.py
--rwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)     1110 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/websocket/run.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2318 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/websocket/sockets.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10414 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/services/websocket/websocket_manager.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.765793 parlai-1.7.1/parlai/chat_service/tasks/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/tasks/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.773913 parlai-1.7.1/parlai/chat_service/tasks/chatbot/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/tasks/chatbot/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4333 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/tasks/chatbot/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.781820 parlai-1.7.1/parlai/chat_service/tasks/overworld_demo/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/tasks/overworld_demo/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8536 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/tasks/overworld_demo/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.791018 parlai-1.7.1/parlai/chat_service/tasks/qa_data_collection/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/tasks/qa_data_collection/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3338 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/tasks/qa_data_collection/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.821208 parlai-1.7.1/parlai/chat_service/utils/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/utils/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2449 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/utils/config.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3869 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/utils/image.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1066 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/utils/logging.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6342 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/utils/misc.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10239 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/utils/server.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2763 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/chat_service/utils/timeout.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.825355 parlai-1.7.1/parlai/clib/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/clib/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.829115 parlai-1.7.1/parlai/clib/cuda/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/clib/cuda/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.931214 parlai-1.7.1/parlai/core/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      411 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    18269 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    24798 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/build_data.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    29950 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/dict.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      292 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/exceptions.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9312 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/image_featurizers.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13189 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/loader.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8933 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/logs.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1883 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/message.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    35003 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/metrics.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8263 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/mutators.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6204 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/opt.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    49975 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/params.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10294 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/script.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    99494 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/teachers.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.962972 parlai-1.7.1/parlai/core/tod/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/tod/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4994 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/tod/teacher_metrics.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    32366 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/tod/tod_agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8951 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/tod/tod_core.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.971817 parlai-1.7.1/parlai/core/tod/tod_test_utils/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/tod/tod_test_utils/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6573 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/tod/tod_test_utils/test_agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13188 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/tod/tod_world.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4584 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/tod/world_metrics.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6448 2022-08-23 20:50:10.000000 parlai-1.7.1/parlai/core/tod/world_metrics_handlers.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    91548 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/core/torch_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    26840 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/core/torch_classifier_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    72853 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/core/torch_generator_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3581 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/core/torch_image_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    43701 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/core/torch_ranker_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    48703 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/core/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.975728 parlai-1.7.1/parlai/crowdsourcing/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:33.979572 parlai-1.7.1/parlai/crowdsourcing/tasks/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.035738 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1103 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/acute_eval_agent_state.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6689 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/acute_eval_blueprint.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2890 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/acute_eval_builder.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    17630 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/acute_eval_runner.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    31320 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/analysis.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4189 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/dump_task_to_acute_format.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3265 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/fast_acute_blueprint.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    21588 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/fast_eval.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2314 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/run.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7419 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/util.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.044437 parlai-1.7.1/parlai/crowdsourcing/tasks/chat_demo/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/chat_demo/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2465 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/chat_demo/run.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.056697 parlai-1.7.1/parlai/crowdsourcing/tasks/dialcrowd/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/dialcrowd/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3743 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/dialcrowd/dialcrowd_blueprint.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.062370 parlai-1.7.1/parlai/crowdsourcing/tasks/dialcrowd/images/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/dialcrowd/images/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1350 2022-08-23 20:50:11.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/dialcrowd/run.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.104262 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:12.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.113124 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/analysis/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:12.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/analysis/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    18886 2022-08-23 20:50:12.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/analysis/compile_results.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4940 2022-08-23 20:50:12.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/bot_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      362 2022-08-23 20:50:12.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/constants.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1973 2022-08-23 20:50:12.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/impl.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    24035 2022-08-23 20:50:12.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/model_chat_blueprint.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1349 2022-08-23 20:50:12.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/run.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.121838 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/scripts/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:12.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/scripts/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2901 2022-08-23 20:50:12.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/scripts/save_image_contexts.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    19639 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/utils.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    27409 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/worlds.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5659 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/worlds_image_chat.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.145850 parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.153337 parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/analysis/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/analysis/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    24077 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/analysis/compile_results.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1840 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/bot_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2036 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/impl.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7337 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/per_turn_eval_blueprint.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1529 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/run.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    22952 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.171274 parlai-1.7.1/parlai/crowdsourcing/tasks/qa_data_collection/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/qa_data_collection/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2699 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/qa_data_collection/run.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      779 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/qa_data_collection/util.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2355 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/qa_data_collection/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.183934 parlai-1.7.1/parlai/crowdsourcing/tasks/turn_annotations_static/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/turn_annotations_static/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.192602 parlai-1.7.1/parlai/crowdsourcing/tasks/turn_annotations_static/analysis/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/turn_annotations_static/analysis/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    24682 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/turn_annotations_static/analysis/compile_results.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1505 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/turn_annotations_static/run.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    17547 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/tasks/turn_annotations_static/turn_annotations_blueprint.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.223477 parlai-1.7.1/parlai/crowdsourcing/utils/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/utils/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5080 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/utils/acceptability.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8802 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/utils/analysis.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1206 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/utils/frontend.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4024 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/utils/mturk.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    17182 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/utils/tests.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3648 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/crowdsourcing/utils/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.260555 parlai-1.7.1/parlai/mutators/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/mutators/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1001 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/mutators/context_shuffle.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1842 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/mutators/episode_reverse.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1836 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/mutators/episode_shuffle.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      935 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/mutators/flatten.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5493 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/mutators/flip_labels.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1518 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/mutators/last_turn.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1172 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/mutators/word_reverse.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1167 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/mutators/word_shuffle.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.272740 parlai-1.7.1/parlai/nn/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/nn/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      547 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/nn/checkpoint.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    17643 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/nn/lr_scheduler.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.281618 parlai-1.7.1/parlai/ops/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/ops/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2462 2022-09-16 16:17:54.000000 parlai-1.7.1/parlai/ops/ngram_repeat_block.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.288878 parlai-1.7.1/parlai/opt_presets/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/opt_presets/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2133 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/opt_presets/docs.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.437704 parlai-1.7.1/parlai/scripts/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3237 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/build_candidates.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5014 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/build_dict.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3049 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/compare_opts.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      954 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/convert_data_to_json_format.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3245 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/convert_data_to_parlai_format.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10549 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/convo_render.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5963 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/data_stats.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4517 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/detect_offensive_language.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3582 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/display_data.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2968 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/display_model.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1615 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/distributed_eval.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      972 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/distributed_tod_world_script.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1677 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/distributed_train.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9628 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/eval_model.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9590 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/eval_wordstat.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2038 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/extract_image_feature.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1360 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/flask.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    60325 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/generate_model_card.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3911 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/interactive.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10378 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/interactive_web.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2855 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/multiprocessing_eval.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3351 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/multiprocessing_train.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10248 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/party.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2758 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/profile_interactive.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2526 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/profile_train.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2667 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/safe_interactive.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5642 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/self_chat.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    17304 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/tod_world_script.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3714 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/token_stats.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4315 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/torchscript.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    37980 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/train_model.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2427 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/vacuum.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5106 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/scripts/verify_data.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.451743 parlai-1.7.1/parlai/tasks/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/tasks/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.469487 parlai-1.7.1/parlai/tasks/airdialogue/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/tasks/airdialogue/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3384 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/tasks/airdialogue/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1105 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/tasks/airdialogue/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      406 2022-08-23 20:50:13.000000 parlai-1.7.1/parlai/tasks/airdialogue/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.484002 parlai-1.7.1/parlai/tasks/amazon_qa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/amazon_qa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3690 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/amazon_qa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10704 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/amazon_qa/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.505787 parlai-1.7.1/parlai/tasks/anli/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/anli/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5829 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/anli/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1183 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/anli/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      326 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/anli/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.522557 parlai-1.7.1/parlai/tasks/aqua/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/aqua/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1922 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/aqua/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1241 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/aqua/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      312 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/aqua/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.539153 parlai-1.7.1/parlai/tasks/babi/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/babi/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3541 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/babi/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1158 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/babi/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      448 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/babi/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.562557 parlai-1.7.1/parlai/tasks/blended_skill_talk/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/blended_skill_talk/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    23214 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/blended_skill_talk/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7608 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/blended_skill_talk/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      431 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/blended_skill_talk/test.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7028 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/blended_skill_talk/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.574952 parlai-1.7.1/parlai/tasks/booktest/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/booktest/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1090 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/booktest/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1172 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/booktest/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.593759 parlai-1.7.1/parlai/tasks/bot_adversarial_dialogue/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/bot_adversarial_dialogue/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11317 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/bot_adversarial_dialogue/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3597 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/bot_adversarial_dialogue/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      987 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/bot_adversarial_dialogue/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.610651 parlai-1.7.1/parlai/tasks/c3/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/c3/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      624 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/c3/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1509 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/c3/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      369 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/c3/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.628467 parlai-1.7.1/parlai/tasks/casino/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/casino/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13981 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/casino/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1722 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/casino/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      328 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/casino/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.645923 parlai-1.7.1/parlai/tasks/cbt/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cbt/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1786 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cbt/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1150 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cbt/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      325 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cbt/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.658754 parlai-1.7.1/parlai/tasks/ccpe/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/ccpe/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5177 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/ccpe/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1211 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/ccpe/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.673058 parlai-1.7.1/parlai/tasks/clevr/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/clevr/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2236 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/clevr/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1167 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/clevr/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.694568 parlai-1.7.1/parlai/tasks/cmu_dog/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cmu_dog/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13286 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cmu_dog/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5770 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cmu_dog/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      329 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cmu_dog/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.705116 parlai-1.7.1/parlai/tasks/cnn_dm/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cnn_dm/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2986 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cnn_dm/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4296 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cnn_dm/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.725532 parlai-1.7.1/parlai/tasks/coco_caption/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/coco_caption/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13934 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/coco_caption/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2469 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/coco_caption/build_2014.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2106 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/coco_caption/build_2015.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2805 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/coco_caption/build_2017.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.737868 parlai-1.7.1/parlai/tasks/commonsenseqa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/commonsenseqa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2744 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/commonsenseqa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1269 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/commonsenseqa/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.760153 parlai-1.7.1/parlai/tasks/convai2/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai2/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7372 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai2/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1188 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai2/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      628 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai2/test.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4008 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai2/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.771407 parlai-1.7.1/parlai/tasks/convai2_wild_evaluation/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai2_wild_evaluation/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      764 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai2_wild_evaluation/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2522 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai2_wild_evaluation/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.784310 parlai-1.7.1/parlai/tasks/convai_chitchat/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      222 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai_chitchat/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3276 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai_chitchat/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1352 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/convai_chitchat/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.796695 parlai-1.7.1/parlai/tasks/copa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/copa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2081 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/copa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1131 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/copa/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.808621 parlai-1.7.1/parlai/tasks/coqa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/coqa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      854 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/coqa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2939 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/coqa/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.825745 parlai-1.7.1/parlai/tasks/cornell_movie/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cornell_movie/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2448 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cornell_movie/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1222 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cornell_movie/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      412 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/cornell_movie/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.849084 parlai-1.7.1/parlai/tasks/dailydialog/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dailydialog/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4169 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dailydialog/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1186 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dailydialog/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3123 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dailydialog/parse.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      412 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dailydialog/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.865749 parlai-1.7.1/parlai/tasks/dbll_babi/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dbll_babi/__init__.py
--rwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)     2100 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dbll_babi/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1148 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dbll_babi/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      331 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dbll_babi/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.881780 parlai-1.7.1/parlai/tasks/dbll_movie/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dbll_movie/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2339 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dbll_movie/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      756 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dbll_movie/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      399 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dbll_movie/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.897829 parlai-1.7.1/parlai/tasks/dealnodeal/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dealnodeal/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7383 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dealnodeal/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1217 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dealnodeal/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      332 2022-08-23 20:50:14.000000 parlai-1.7.1/parlai/tasks/dealnodeal/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.904887 parlai-1.7.1/parlai/tasks/decanlp/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/decanlp/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2011 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/decanlp/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.921035 parlai-1.7.1/parlai/tasks/decode/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/decode/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3029 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/decode/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1255 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/decode/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      328 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/decode/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.937600 parlai-1.7.1/parlai/tasks/dialog_babi/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialog_babi/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2222 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialog_babi/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1182 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialog_babi/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      333 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialog_babi/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.953068 parlai-1.7.1/parlai/tasks/dialog_babi_plus/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialog_babi_plus/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1641 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialog_babi_plus/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1094 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialog_babi_plus/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      411 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialog_babi_plus/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.969434 parlai-1.7.1/parlai/tasks/dialogue_nli/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_nli/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4378 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_nli/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1256 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_nli/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      334 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_nli/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:34.986339 parlai-1.7.1/parlai/tasks/dialogue_qe/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      222 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_qe/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2654 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_qe/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1395 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_qe/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      319 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_qe/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.004820 parlai-1.7.1/parlai/tasks/dialogue_safety/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_safety/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13726 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_safety/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3059 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_safety/base_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1377 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dialogue_safety/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.025538 parlai-1.7.1/parlai/tasks/dream/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dream/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2512 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dream/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1506 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dream/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      385 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dream/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.042737 parlai-1.7.1/parlai/tasks/dstc7/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dstc7/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4895 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dstc7/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1107 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dstc7/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      327 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/dstc7/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.055718 parlai-1.7.1/parlai/tasks/eli5/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2635 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4358 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.088639 parlai-1.7.1/parlai/tasks/eli5/data_creation/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/data_creation/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9191 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/data_creation/data_utils.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    21150 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/data_creation/download_reddit_qalist.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13468 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/data_creation/download_support_docs.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2215 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/data_creation/finalize_qda.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3441 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/data_creation/merge_support_docs.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5700 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/data_creation/select_sentences_tfidf.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.093955 parlai-1.7.1/parlai/tasks/eli5/data_creation/slurm_scripts/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/eli5/data_creation/slurm_scripts/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.117752 parlai-1.7.1/parlai/tasks/empathetic_dialogues/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/empathetic_dialogues/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6462 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/empathetic_dialogues/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1216 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/empathetic_dialogues/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      342 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/empathetic_dialogues/test.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      367 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/empathetic_dialogues/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.143837 parlai-1.7.1/parlai/tasks/fits/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/fits/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    27863 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/fits/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1639 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/fits/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      631 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/fits/constants.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11361 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/fits/mutators.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      585 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/fits/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.156686 parlai-1.7.1/parlai/tasks/flickr30k/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/flickr30k/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6178 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/flickr30k/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1175 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/flickr30k/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.173769 parlai-1.7.1/parlai/tasks/friends/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/friends/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11265 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/friends/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3241 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/friends/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      844 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/friends/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.181742 parlai-1.7.1/parlai/tasks/fromfile/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/fromfile/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5082 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/fromfile/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.199093 parlai-1.7.1/parlai/tasks/funpedia/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/funpedia/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5122 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/funpedia/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1203 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/funpedia/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      695 2022-08-23 20:50:15.000000 parlai-1.7.1/parlai/tasks/funpedia/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.212151 parlai-1.7.1/parlai/tasks/fvqa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/fvqa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5895 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/fvqa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1129 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/fvqa/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.229918 parlai-1.7.1/parlai/tasks/genderation_bias/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/genderation_bias/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10633 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/genderation_bias/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1461 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/genderation_bias/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4481 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/genderation_bias/utils.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.242969 parlai-1.7.1/parlai/tasks/glue/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/glue/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4224 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/glue/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      893 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/glue/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.260508 parlai-1.7.1/parlai/tasks/google_sgd/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/google_sgd/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    12932 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/google_sgd/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1651 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/google_sgd/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      509 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/google_sgd/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.280610 parlai-1.7.1/parlai/tasks/google_sgd_simulation_splits/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/google_sgd_simulation_splits/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6141 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/google_sgd_simulation_splits/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4950 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/google_sgd_simulation_splits/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      745 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/google_sgd_simulation_splits/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.299970 parlai-1.7.1/parlai/tasks/holl_e/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/holl_e/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5553 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/holl_e/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1435 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/holl_e/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      384 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/holl_e/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.326451 parlai-1.7.1/parlai/tasks/hotpotqa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/hotpotqa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1331 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/hotpotqa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3280 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/hotpotqa/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      474 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/hotpotqa/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.335687 parlai-1.7.1/parlai/tasks/huggingface/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/huggingface/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4686 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/huggingface/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.347232 parlai-1.7.1/parlai/tasks/igc/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/igc/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11014 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/igc/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.368802 parlai-1.7.1/parlai/tasks/image_chat/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/image_chat/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    14335 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/image_chat/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1382 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/image_chat/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      781 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/image_chat/download_data.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.387488 parlai-1.7.1/parlai/tasks/insuranceqa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/insuranceqa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1293 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/insuranceqa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8456 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/insuranceqa/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      455 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/insuranceqa/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.395453 parlai-1.7.1/parlai/tasks/integration_tests/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/integration_tests/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    16616 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/integration_tests/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.408331 parlai-1.7.1/parlai/tasks/interactive/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/interactive/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      346 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/interactive/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2993 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/interactive/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.424330 parlai-1.7.1/parlai/tasks/iwslt14/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/iwslt14/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1657 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/iwslt14/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1164 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/iwslt14/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      329 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/iwslt14/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.445007 parlai-1.7.1/parlai/tasks/jericho_world/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/jericho_world/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    21968 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/jericho_world/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1468 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/jericho_world/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1150 2022-08-23 20:50:16.000000 parlai-1.7.1/parlai/tasks/jericho_world/constants.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      706 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/jericho_world/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.453228 parlai-1.7.1/parlai/tasks/jsonfile/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/jsonfile/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2286 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/jsonfile/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.470569 parlai-1.7.1/parlai/tasks/lccc/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/lccc/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1445 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/lccc/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2104 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/lccc/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      312 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/lccc/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.496443 parlai-1.7.1/parlai/tasks/light_dialog/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10120 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2835 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13835 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog/builder.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      320 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog/test.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4531 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.520069 parlai-1.7.1/parlai/tasks/light_dialog_wild/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog_wild/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    17210 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog_wild/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3576 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog_wild/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    28587 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog_wild/builder.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      325 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_dialog_wild/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.532529 parlai-1.7.1/parlai/tasks/light_genderation_bias/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_genderation_bias/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    12975 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_genderation_bias/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1183 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/light_genderation_bias/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.550119 parlai-1.7.1/parlai/tasks/mctest/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mctest/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      971 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mctest/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3391 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mctest/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      328 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mctest/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.606812 parlai-1.7.1/parlai/tasks/md_gender/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1717 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1170 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10426 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/convai2.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4296 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/funpedia.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5835 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/image_chat.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7525 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/light.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3524 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/new_data.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      449 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/opensubtitles.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8635 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/utils.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9828 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/wikipedia.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4487 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/wizard.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5048 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/worlds.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8921 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/md_gender/yelp.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.624154 parlai-1.7.1/parlai/tasks/metalwoz/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/metalwoz/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4462 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/metalwoz/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1527 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/metalwoz/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      410 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/metalwoz/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.641011 parlai-1.7.1/parlai/tasks/mnist_qa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mnist_qa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2285 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mnist_qa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1160 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mnist_qa/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      330 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mnist_qa/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.656456 parlai-1.7.1/parlai/tasks/moviedialog/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/moviedialog/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3239 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/moviedialog/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2270 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/moviedialog/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.668677 parlai-1.7.1/parlai/tasks/ms_marco/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/ms_marco/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1817 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/ms_marco/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4321 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/ms_marco/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.696094 parlai-1.7.1/parlai/tasks/msc/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/msc/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    30947 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/msc/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1342 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/msc/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2312 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/msc/constants.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1088 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/msc/mutators.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      619 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/msc/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.713361 parlai-1.7.1/parlai/tasks/msr_e2e/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/msr_e2e/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9993 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/msr_e2e/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1772 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/msr_e2e/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      421 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/msr_e2e/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.725548 parlai-1.7.1/parlai/tasks/mturkwikimovies/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mturkwikimovies/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      999 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mturkwikimovies/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1354 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mturkwikimovies/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.741309 parlai-1.7.1/parlai/tasks/multidogo/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multidogo/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6005 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multidogo/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    12446 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multidogo/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      479 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multidogo/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.756904 parlai-1.7.1/parlai/tasks/multinli/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multinli/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5682 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multinli/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1127 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multinli/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      316 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multinli/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.772341 parlai-1.7.1/parlai/tasks/multiwoz_v20/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v20/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4210 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v20/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1065 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v20/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      402 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v20/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.788986 parlai-1.7.1/parlai/tasks/multiwoz_v21/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v21/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4210 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v21/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1069 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v21/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      402 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v21/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.810165 parlai-1.7.1/parlai/tasks/multiwoz_v22/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v22/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    23467 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v22/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7958 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v22/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2198 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v22/build_sha_check_script.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      517 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/multiwoz_v22/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.822887 parlai-1.7.1/parlai/tasks/mutualfriends/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mutualfriends/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3287 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mutualfriends/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1235 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mutualfriends/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.833889 parlai-1.7.1/parlai/tasks/mwsc/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mwsc/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1458 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mwsc/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3331 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/mwsc/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.846316 parlai-1.7.1/parlai/tasks/narrative_qa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/narrative_qa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4471 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/narrative_qa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5668 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/narrative_qa/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.865886 parlai-1.7.1/parlai/tasks/natural_questions/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/natural_questions/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    14049 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/natural_questions/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4281 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/natural_questions/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2178 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/natural_questions/build_open.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      487 2022-08-23 20:50:17.000000 parlai-1.7.1/parlai/tasks/natural_questions/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.874562 parlai-1.7.1/parlai/tasks/natural_questions/utils/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/natural_questions/utils/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5999 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/natural_questions/utils/text_utils.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.882978 parlai-1.7.1/parlai/tasks/nli/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/nli/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2123 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/nli/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.895457 parlai-1.7.1/parlai/tasks/nlvr/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/nlvr/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1880 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/nlvr/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1142 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/nlvr/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.907343 parlai-1.7.1/parlai/tasks/onecommon/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/onecommon/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8582 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/onecommon/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1156 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/onecommon/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.922989 parlai-1.7.1/parlai/tasks/opensubtitles/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/opensubtitles/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5991 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/opensubtitles/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/opensubtitles/build_2009.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11397 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/opensubtitles/build_2018.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.939351 parlai-1.7.1/parlai/tasks/personachat/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personachat/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2629 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personachat/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1149 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personachat/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1141 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personachat/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.956570 parlai-1.7.1/parlai/tasks/personality_captions/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personality_captions/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9285 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personality_captions/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1310 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personality_captions/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2368 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personality_captions/download_images.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.968413 parlai-1.7.1/parlai/tasks/personalized_dialog/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personalized_dialog/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3758 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personalized_dialog/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1232 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/personalized_dialog/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.984366 parlai-1.7.1/parlai/tasks/qacnn/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qacnn/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      685 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qacnn/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2282 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qacnn/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:35.996231 parlai-1.7.1/parlai/tasks/qadailymail/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qadailymail/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      691 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qadailymail/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2263 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qadailymail/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.009513 parlai-1.7.1/parlai/tasks/qangaroo/
--rwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qangaroo/__init__.py
--rwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)     3121 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qangaroo/agents.py
--rwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)     1181 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qangaroo/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.020534 parlai-1.7.1/parlai/tasks/qasrl/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qasrl/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2721 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qasrl/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1635 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qasrl/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.031614 parlai-1.7.1/parlai/tasks/qazre/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qazre/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1781 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qazre/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1192 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/qazre/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.049206 parlai-1.7.1/parlai/tasks/quac/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/quac/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      854 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/quac/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3553 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/quac/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      312 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/quac/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.066838 parlai-1.7.1/parlai/tasks/redial/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/redial/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4401 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/redial/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1014 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/redial/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      386 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/redial/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.084468 parlai-1.7.1/parlai/tasks/saferdialogues/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/saferdialogues/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3213 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/saferdialogues/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1298 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/saferdialogues/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      437 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/saferdialogues/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.102896 parlai-1.7.1/parlai/tasks/safety_mix/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/safety_mix/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3941 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/safety_mix/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    15347 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/safety_mix/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      506 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/safety_mix/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.120178 parlai-1.7.1/parlai/tasks/scan/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/scan/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      684 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/scan/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2213 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/scan/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      326 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/scan/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.133438 parlai-1.7.1/parlai/tasks/self_chat/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/self_chat/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      460 2022-08-23 20:50:18.000000 parlai-1.7.1/parlai/tasks/self_chat/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6981 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/self_chat/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.144929 parlai-1.7.1/parlai/tasks/sensitive_topics_evaluation/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/sensitive_topics_evaluation/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1387 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/sensitive_topics_evaluation/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1256 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/sensitive_topics_evaluation/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.161519 parlai-1.7.1/parlai/tasks/simplequestions/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/simplequestions/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      715 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/simplequestions/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1198 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/simplequestions/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      337 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/simplequestions/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.178041 parlai-1.7.1/parlai/tasks/snli/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/snli/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2514 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/snli/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1116 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/snli/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      312 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/snli/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.193497 parlai-1.7.1/parlai/tasks/spolin/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/spolin/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2301 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/spolin/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1695 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/spolin/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      362 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/spolin/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.210131 parlai-1.7.1/parlai/tasks/squad/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/squad/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    14423 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/squad/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2204 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/squad/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      691 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/squad/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.226795 parlai-1.7.1/parlai/tasks/squad2/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/squad2/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    15503 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/squad2/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1436 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/squad2/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      730 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/squad2/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.245544 parlai-1.7.1/parlai/tasks/sst/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/sst/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2118 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/sst/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1830 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/sst/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      375 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/sst/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.262086 parlai-1.7.1/parlai/tasks/style_gen/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/style_gen/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5933 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/style_gen/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2485 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/style_gen/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      658 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/style_gen/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.274069 parlai-1.7.1/parlai/tasks/superglue/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/superglue/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2133 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/superglue/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      525 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/superglue/test.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    60496 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/task_list.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.294405 parlai-1.7.1/parlai/tasks/taskmaster/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/taskmaster/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    19615 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/taskmaster/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1625 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/taskmaster/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      773 2022-08-23 20:50:19.000000 parlai-1.7.1/parlai/tasks/taskmaster/test.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5584 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskmaster/tm_utils.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.310815 parlai-1.7.1/parlai/tasks/taskmaster2/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskmaster2/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7886 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskmaster2/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4014 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskmaster2/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      416 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskmaster2/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.329064 parlai-1.7.1/parlai/tasks/taskmaster3/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskmaster3/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7046 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskmaster3/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5232 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskmaster3/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      429 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskmaster3/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.341998 parlai-1.7.1/parlai/tasks/taskntalk/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskntalk/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3737 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskntalk/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4163 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/taskntalk/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1795 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/tasks.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.350595 parlai-1.7.1/parlai/tasks/tod_json/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/tod_json/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9036 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/tod_json/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.363071 parlai-1.7.1/parlai/tasks/triviaqa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/triviaqa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6284 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/triviaqa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3822 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/triviaqa/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.379941 parlai-1.7.1/parlai/tasks/twitter/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/twitter/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      695 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/twitter/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3851 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/twitter/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      329 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/twitter/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.396524 parlai-1.7.1/parlai/tasks/ubuntu/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/ubuntu/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3898 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/ubuntu/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1163 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/ubuntu/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      405 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/ubuntu/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.409813 parlai-1.7.1/parlai/tasks/visdial/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/visdial/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3332 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/visdial/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2812 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/visdial/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.422035 parlai-1.7.1/parlai/tasks/vqa_v1/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/vqa_v1/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    17758 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/vqa_v1/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2109 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/vqa_v1/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.434401 parlai-1.7.1/parlai/tasks/vqa_v2/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/vqa_v2/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5937 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/vqa_v2/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2135 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/vqa_v2/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.446239 parlai-1.7.1/parlai/tasks/webquestions/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/webquestions/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      692 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/webquestions/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2414 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/webquestions/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.463654 parlai-1.7.1/parlai/tasks/wikimovies/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikimovies/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1895 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikimovies/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1178 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikimovies/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      332 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikimovies/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.476220 parlai-1.7.1/parlai/tasks/wikipedia/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikipedia/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6906 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikipedia/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1295 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikipedia/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.492855 parlai-1.7.1/parlai/tasks/wikiqa/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikiqa/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      979 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikiqa/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2789 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikiqa/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      328 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikiqa/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.509805 parlai-1.7.1/parlai/tasks/wikisql/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikisql/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3495 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikisql/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1403 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikisql/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      392 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wikisql/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.534707 parlai-1.7.1/parlai/tasks/wizard_of_internet/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wizard_of_internet/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    24880 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wizard_of_internet/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1212 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wizard_of_internet/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2368 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wizard_of_internet/constants.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9597 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wizard_of_internet/mutators.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      954 2022-08-23 20:50:20.000000 parlai-1.7.1/parlai/tasks/wizard_of_internet/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.560569 parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    45682 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1091 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5943 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/mutators.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1253 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/test.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8657 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/worlds.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.576946 parlai-1.7.1/parlai/tasks/wmt/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wmt/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      842 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wmt/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3419 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wmt/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      376 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wmt/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.592073 parlai-1.7.1/parlai/tasks/woz/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/woz/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1915 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/woz/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1735 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/woz/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      374 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/woz/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.600035 parlai-1.7.1/parlai/tasks/wrapper/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wrapper/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6305 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/wrapper/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.616963 parlai-1.7.1/parlai/tasks/xpersona/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/xpersona/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1435 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/xpersona/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8152 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/xpersona/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      785 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/tasks/xpersona/test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.633216 parlai-1.7.1/parlai/torchscript/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/torchscript/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2242 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/torchscript/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    21156 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/torchscript/modules.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.641465 parlai-1.7.1/parlai/torchscript/scripts/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/torchscript/scripts/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1350 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/torchscript/scripts/test_exported_model.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    22843 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/torchscript/tokenizer.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.727424 parlai-1.7.1/parlai/utils/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    31618 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/bpe.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10369 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/conversations.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6033 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/curated_response.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6447 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/data.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11398 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/distributed.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3423 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/flake8.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    31338 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/fp16.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3162 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/fsdp.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      901 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/io.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4916 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/logging.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    23309 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/misc.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1714 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/pickle.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8816 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/safety.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5006 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/strings.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13534 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/testing.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    22580 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/torch.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      944 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/typing.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5957 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/utils/world_logging.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.735766 parlai-1.7.1/parlai/zoo/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.746036 parlai-1.7.1/parlai/zoo/bart/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bart/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2295 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bart/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.762663 parlai-1.7.1/parlai/zoo/bb3/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bb3/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      678 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bb3/bb3_3B.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.766911 parlai-1.7.1/parlai/zoo/bb3/images/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bb3/images/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      690 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bb3/persona_summarizer.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.775178 parlai-1.7.1/parlai/zoo/bert/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bert/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1222 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bert/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.804731 parlai-1.7.1/parlai/zoo/blended_skill_talk/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blended_skill_talk/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      677 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blended_skill_talk/bst_single_task.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      672 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blended_skill_talk/convai2_single_task.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      679 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blended_skill_talk/ed_single_task.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      718 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blended_skill_talk/multi_task.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      763 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blended_skill_talk/multi_task_bst_tuned.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      683 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blended_skill_talk/wizard_single_task.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.849638 parlai-1.7.1/parlai/zoo/blender/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      539 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/blender_1Bdistill.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      421 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/blender_3B.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      543 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/blender_400Mdistill.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      421 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/blender_90M.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      421 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/blender_9B.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      882 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      436 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/dict_3B.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      439 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/dict_90M.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      425 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/reddit_3B.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      425 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blender/reddit_9B.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.868755 parlai-1.7.1/parlai/zoo/blenderbot2/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blenderbot2/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      724 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blenderbot2/blenderbot2_3B.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      728 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blenderbot2/blenderbot2_400M.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      739 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blenderbot2/memory_decoder.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      741 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/blenderbot2/query_generator.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.880594 parlai-1.7.1/parlai/zoo/bot_adversarial_dialogue/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bot_adversarial_dialogue/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      801 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bot_adversarial_dialogue/multi_turn.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      803 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/bot_adversarial_dialogue/multi_turn_v0.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.900721 parlai-1.7.1/parlai/zoo/dialogue_bias/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_bias/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      752 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_bias/gender__ctrl_gen_tokens.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      689 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_bias/gender__name_scrambling.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      724 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_bias/gender__unlikelihood_sequence_level.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      718 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_bias/gender_ethnicity__name_scrambling.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.912291 parlai-1.7.1/parlai/zoo/dialogue_safety/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_safety/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      559 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_safety/multi_turn.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      581 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_safety/single_turn.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:36.972485 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      719 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      511 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_convai2_ctxt.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      541 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_convai2_ctxt_and_label.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      511 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_convai2_label.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      463 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_eli5_ctxt.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      532 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_eli5_ctxt_and_label.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      477 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_eli5_label.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      478 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_wiki_ctxt.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      547 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_wiki_ctxt_and_label.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      492 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_wiki_label.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      465 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/vocab_alpha1e0.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      465 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/vocab_alpha1e1.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      465 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/vocab_alpha1e2.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      465 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/vocab_alpha1e3.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.031393 parlai-1.7.1/parlai/zoo/dodecadialogue/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      318 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/all_tasks_mt.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1209 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      316 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/convai2_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      322 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/cornell_movie_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      321 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/daily_dialog_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      313 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/eli5_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      329 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/empathetic_dialogues_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      312 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/igc_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      319 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/image_chat_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      321 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/light_dialog_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      315 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/reddit_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      316 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/twitter_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      315 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/ubuntu_ft.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      328 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/dodecadialogue/wizard_of_wikipedia_ft.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.039347 parlai-1.7.1/parlai/zoo/fasttext_cc_vectors/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fasttext_cc_vectors/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      618 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fasttext_cc_vectors/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.047507 parlai-1.7.1/parlai/zoo/fasttext_vectors/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fasttext_vectors/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      574 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fasttext_vectors/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.079708 parlai-1.7.1/parlai/zoo/fits/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fits/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      744 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fits/bart_sq_gen.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      734 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fits/bb2_module_supervision.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      731 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fits/director_bb2_module.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      723 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fits/director_seeker_module.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      723 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fits/response_satisfaction.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      723 2022-08-23 20:50:21.000000 parlai-1.7.1/parlai/zoo/fits/seeker_module_supervision.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.092677 parlai-1.7.1/parlai/zoo/glove_vectors/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/glove_vectors/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      493 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/glove_vectors/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.155905 parlai-1.7.1/parlai/zoo/hallucination/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      740 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/bart_fid_dpr.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      741 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/bart_fid_rag.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      749 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/bart_fid_rag_dpr_poly.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      745 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/bart_rag_dpr_poly.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      745 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/bart_rag_sequence.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      742 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/bart_rag_token.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      744 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/bart_rag_turn_do.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      745 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/bart_rag_turn_dtt.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      740 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/dropout_poly.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      892 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/multiset_dpr.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      791 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/wiki_index_compressed.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      778 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/wiki_index_exact.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1079 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/wiki_passages.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      769 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/hallucination/wow_passages.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.164186 parlai-1.7.1/parlai/zoo/image_chat/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/image_chat/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      553 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/image_chat/transresnet_multimodal.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.172131 parlai-1.7.1/parlai/zoo/light/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      580 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light/biranker_dialogue.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.228692 parlai-1.7.1/parlai/zoo/light_whoami/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      522 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/automated_expanded_attention_1024.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      514 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/expanded_and_multiobjective_1024.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      427 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/multiobjective.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      541 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/profile_expanded_attention_1024.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      530 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/profile_expanded_attention_128.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      394 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/rpa_reranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      452 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/rpa_reranker_auto_expanded_attention.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      402 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/rpa_ul_1024.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      400 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/rpa_ul_128.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      404 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/test_rpa_reranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      416 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/vanilla_1024.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      414 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/vanilla_128.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      738 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/light_whoami/whoami_download.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.235704 parlai-1.7.1/parlai/zoo/md_gender/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/md_gender/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      615 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/md_gender/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)   172674 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/model_list.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.261104 parlai-1.7.1/parlai/zoo/msc/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/msc/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      716 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/msc/blender3B_1024.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      727 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/msc/dialog_summarizer.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      709 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/msc/msc3B_1024.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      715 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/msc/summsc_fidrag3B.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      708 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/msc/summsc_rag3B.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.265519 parlai-1.7.1/parlai/zoo/multimodal_blenderbot/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/multimodal_blenderbot/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.274219 parlai-1.7.1/parlai/zoo/personality_captions/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/personality_captions/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      540 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/personality_captions/transresnet.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.315204 parlai-1.7.1/parlai/zoo/pretrained_transformers/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/pretrained_transformers/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      241 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/pretrained_transformers/bi_model_huge_reddit.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      241 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/pretrained_transformers/bi_model_huge_wikito.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      758 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/pretrained_transformers/build.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      241 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/pretrained_transformers/cross_model_huge_reddit.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      241 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/pretrained_transformers/cross_model_huge_wikito.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      241 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/pretrained_transformers/model_bi.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      241 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/pretrained_transformers/model_poly.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      241 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/pretrained_transformers/poly_model_huge_reddit.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      241 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/pretrained_transformers/poly_model_huge_wikito.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.323583 parlai-1.7.1/parlai/zoo/saferdialogues/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      220 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/saferdialogues/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      617 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/saferdialogues/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.340617 parlai-1.7.1/parlai/zoo/sea/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/sea/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      741 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/sea/bart_base.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      800 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/sea/bart_fid_sqse.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      766 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/sea/bart_sq_gen.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.396336 parlai-1.7.1/parlai/zoo/seeker/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      449 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/r2c2_base_3B.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      453 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/r2c2_base_400M.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      413 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/r2c2_blenderbot_3B.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      417 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/r2c2_blenderbot_400M.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      399 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/seeker_dialogue_3B.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      403 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/seeker_dialogue_400M.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      704 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/seeker_download.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      461 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/seeker_lm_dialogue_3B.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      438 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/seeker_lm_large.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      438 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/seeker_lm_med.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      429 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/seeker/seeker_lm_xl.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.402764 parlai-1.7.1/parlai/zoo/sensitive_topics_classifier/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/sensitive_topics_classifier/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      985 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/sensitive_topics_classifier/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.419357 parlai-1.7.1/parlai/zoo/style_gen/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/style_gen/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      811 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/style_gen/c75_labeled_dialogue_generator.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      778 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/style_gen/curr_only_classifier.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      782 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/style_gen/prev_curr_classifier.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.431534 parlai-1.7.1/parlai/zoo/tod/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/tod/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      873 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/tod/tod_base_no_api.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      892 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/tod/tod_base_yes_api.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.439584 parlai-1.7.1/parlai/zoo/tutorial_transformer_generator/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/tutorial_transformer_generator/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      923 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/tutorial_transformer_generator/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.447351 parlai-1.7.1/parlai/zoo/unittest/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/unittest/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      932 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/unittest/build.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.455724 parlai-1.7.1/parlai/zoo/wikipedia_full/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/wikipedia_full/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      545 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/wikipedia_full/tfidf_retriever.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.472153 parlai-1.7.1/parlai/zoo/wizard_of_wikipedia/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/wizard_of_wikipedia/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      527 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/wizard_of_wikipedia/end2end_generator.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      551 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/wizard_of_wikipedia/full_dialogue_retrieval_model.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      844 2022-08-23 20:50:22.000000 parlai-1.7.1/parlai/zoo/wizard_of_wikipedia/knowledge_retriever.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:32.975329 parlai-1.7.1/parlai.egg-info/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10106 2022-09-16 16:27:32.000000 parlai-1.7.1/parlai.egg-info/PKG-INFO
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    43177 2022-09-16 16:27:32.000000 parlai-1.7.1/parlai.egg-info/SOURCES.txt
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        1 2022-09-16 16:27:32.000000 parlai-1.7.1/parlai.egg-info/dependency_links.txt
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      109 2022-09-16 16:27:32.000000 parlai-1.7.1/parlai.egg-info/entry_points.txt
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      784 2022-09-16 16:27:32.000000 parlai-1.7.1/parlai.egg-info/requires.txt
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)       46 2022-09-16 16:27:32.000000 parlai-1.7.1/parlai.egg-info/top_level.txt
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.476069 parlai-1.7.1/projects/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      293 2022-08-23 20:50:22.000000 parlai-1.7.1/projects/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.484098 parlai-1.7.1/projects/anti_scaling/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/projects/anti_scaling/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    42981 2022-08-23 20:50:22.000000 parlai-1.7.1/projects/anti_scaling/distillation.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.493322 parlai-1.7.1/projects/anti_scaling/scripts/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/projects/anti_scaling/scripts/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1553 2022-08-23 20:50:22.000000 parlai-1.7.1/projects/anti_scaling/scripts/remove_projection_matrices.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.505427 parlai-1.7.1/projects/bb3/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/projects/bb3/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.533904 parlai-1.7.1/projects/bb3/agents/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:22.000000 parlai-1.7.1/projects/bb3/agents/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7736 2022-08-23 20:50:22.000000 parlai-1.7.1/projects/bb3/agents/module.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    30449 2022-08-23 20:50:22.000000 parlai-1.7.1/projects/bb3/agents/opt_api_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    35384 2022-09-16 16:17:54.000000 parlai-1.7.1/projects/bb3/agents/opt_bb3_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    57399 2022-09-16 16:17:54.000000 parlai-1.7.1/projects/bb3/agents/r2c2_bb3_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3874 2022-08-23 20:50:22.000000 parlai-1.7.1/projects/bb3/agents/search_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    22543 2022-09-16 16:17:54.000000 parlai-1.7.1/projects/bb3/agents/utils.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1490 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/constants.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    35982 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/prompts.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.588671 parlai-1.7.1/projects/bb3/tasks/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9769 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/module_level_tasks.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    69824 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/mutators.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3490 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/opt_decision_tasks.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11104 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/opt_dialogue_tasks.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7576 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/opt_knowledge_tasks.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1089 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/opt_memory_generation_tasks.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1113 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/opt_search_generation_tasks.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5685 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/r2c2_decision_tasks.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    14232 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/r2c2_dialogue_tasks.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8149 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/r2c2_knowledge_tasks.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      882 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/r2c2_memory_generation_tasks.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1100 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/bb3/tasks/r2c2_search_generation_tasks.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.592656 parlai-1.7.1/projects/blenderbot2/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/blenderbot2/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.608990 parlai-1.7.1/projects/blenderbot2/agents/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/blenderbot2/agents/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    34689 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/blenderbot2/agents/blenderbot2.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    35431 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/blenderbot2/agents/modules.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    14214 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/blenderbot2/agents/sub_modules.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.617432 parlai-1.7.1/projects/dialogue_unlikelihood/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/dialogue_unlikelihood/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    20340 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/dialogue_unlikelihood/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.626255 parlai-1.7.1/projects/image_chat/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      293 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/image_chat/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    16194 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/image_chat/interactive.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.638534 parlai-1.7.1/projects/image_chat/transresnet_multimodal/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/image_chat/transresnet_multimodal/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    19412 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/image_chat/transresnet_multimodal/modules.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    15704 2022-08-23 20:50:23.000000 parlai-1.7.1/projects/image_chat/transresnet_multimodal/transresnet_multimodal.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.646574 parlai-1.7.1/projects/multimodal_blenderbot/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:24.000000 parlai-1.7.1/projects/multimodal_blenderbot/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      485 2022-08-23 20:50:24.000000 parlai-1.7.1/projects/multimodal_blenderbot/agents.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.654597 parlai-1.7.1/projects/personality_captions/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      293 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/personality_captions/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    14003 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/personality_captions/interactive.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.667806 parlai-1.7.1/projects/personality_captions/transresnet/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/personality_captions/transresnet/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    20165 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/personality_captions/transresnet/modules.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    18285 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/personality_captions/transresnet/transresnet.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.680509 parlai-1.7.1/projects/safety_bench/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.697914 parlai-1.7.1/projects/safety_bench/model_wrappers/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/model_wrappers/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1091 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/model_wrappers/example_wrapper.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3384 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/model_wrappers/gpt_wrappers.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4901 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/model_wrappers/parlai_model_zoo_wrappers.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6505 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/prepare_integration_tests.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7164 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/run_unit_tests.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.711296 parlai-1.7.1/projects/safety_bench/unit_tests/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/unit_tests/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6036 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/unit_tests/generate_offensive_language_test.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5765 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/unit_tests/response_to_offensive_language_test.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.733844 parlai-1.7.1/projects/safety_bench/utils/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/utils/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      527 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/utils/colors.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5121 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/utils/perspective_api.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7593 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/utils/safety_testing.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1439 2022-08-23 20:50:25.000000 parlai-1.7.1/projects/safety_bench/utils/wrapper_loading.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.742252 parlai-1.7.1/projects/seeker/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.770159 parlai-1.7.1/projects/seeker/agents/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/agents/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    10436 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/agents/gpt2_seeker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    20080 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/agents/gpt2_seeker_modules.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4657 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/agents/modular_agent.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    32807 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/agents/seeker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9945 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/agents/seeker_modules.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.779481 parlai-1.7.1/projects/seeker/scripts/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/scripts/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    12206 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/scripts/generate_lm_data.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.810447 parlai-1.7.1/projects/seeker/tasks/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/tasks/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5958 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/tasks/dialogue.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11924 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/tasks/knowledge.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    16717 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/tasks/lm.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    17745 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/tasks/mutators.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6334 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/tasks/search_decision.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1026 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/tasks/search_query.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8603 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/seeker/utils.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.828935 parlai-1.7.1/projects/style_gen/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/style_gen/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8283 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/style_gen/classifier.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     8613 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/style_gen/modules.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1028 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/style_gen/style_gen.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.834220 parlai-1.7.1/projects/tod_simulator/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/tod_simulator/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.871481 parlai-1.7.1/projects/tod_simulator/scripts/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/tod_simulator/scripts/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6399 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/tod_simulator/scripts/cleanup_conversation.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1768 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/tod_simulator/scripts/do_get_passing_only_on_dir.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     7545 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/tod_simulator/scripts/get_al_samples_for_gsgd.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     4417 2022-08-23 20:50:26.000000 parlai-1.7.1/projects/tod_simulator/scripts/get_api_data.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2438 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/tod_simulator/scripts/get_interdistinct_on_conversations.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6078 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/tod_simulator/scripts/get_passing_only.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     6565 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/tod_simulator/scripts/get_quick_eval_stats.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    23195 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/tod_simulator/scripts/tod_distributed_uber_script.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.876344 parlai-1.7.1/projects/tod_simulator/tod_world_configs/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/tod_simulator/tod_world_configs/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.884484 parlai-1.7.1/projects/tod_simulator/world_metrics/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/tod_simulator/world_metrics/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    14697 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/tod_simulator/world_metrics/extended_world_metrics.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.888497 parlai-1.7.1/projects/wizard_of_wikipedia/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      293 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/__init__.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.905461 parlai-1.7.1/projects/wizard_of_wikipedia/generator/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)        0 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/generator/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    11912 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/generator/agents.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5292 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/generator/modules.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1262 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/generator/train_end2end.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.913730 parlai-1.7.1/projects/wizard_of_wikipedia/knowledge_retriever/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/knowledge_retriever/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13411 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/knowledge_retriever/knowledge_retriever.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.925823 parlai-1.7.1/projects/wizard_of_wikipedia/scripts/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/scripts/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1742 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/scripts/eval_retrieval_model.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1091 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/scripts/interactive_retrieval_model.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.938151 parlai-1.7.1/projects/wizard_of_wikipedia/wizard_transformer_ranker/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      198 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/wizard_transformer_ranker/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     3200 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/wizard_transformer_ranker/wizard_dict.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5619 2022-08-23 20:50:27.000000 parlai-1.7.1/projects/wizard_of_wikipedia/wizard_transformer_ranker/wizard_transformer_ranker.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      190 2022-08-23 20:50:27.000000 parlai-1.7.1/pyproject.toml
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)       38 2022-09-16 16:27:37.980351 parlai-1.7.1/setup.cfg
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     1660 2022-09-16 16:20:54.000000 parlai-1.7.1/setup.py
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:32.929891 parlai-1.7.1/tests/
-drwxrwxr-x   0 kshuster (1185200140) kshuster (1185200140)        0 2022-09-16 16:27:37.972668 parlai-1.7.1/tests/tod/
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)      199 2022-08-23 20:50:28.000000 parlai-1.7.1/tests/tod/__init__.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)    13552 2022-08-23 20:50:28.000000 parlai-1.7.1/tests/tod/test_tod_agents_and_teachers.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     2430 2022-08-23 20:50:28.000000 parlai-1.7.1/tests/tod/test_tod_teacher_metrics.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9206 2022-08-23 20:50:28.000000 parlai-1.7.1/tests/tod/test_tod_world_and_script.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9485 2022-08-23 20:50:28.000000 parlai-1.7.1/tests/tod/test_tod_world_metrics.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     9839 2022-08-23 20:50:28.000000 parlai-1.7.1/tests/tod/test_tod_world_metrics_in_script.py
--rw-rw-r--   0 kshuster (1185200140) kshuster (1185200140)     5227 2022-08-23 20:50:28.000000 parlai-1.7.1/tests/tod/test_tod_world_script_metrics.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.206426 parlai-1.7.2/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1086 2023-06-06 17:44:18.000000 parlai-1.7.2/LICENSE
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10832 2023-06-06 20:17:51.204239 parlai-1.7.2/PKG-INFO
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11681 2023-06-06 17:44:18.000000 parlai-1.7.2/README.md
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.094428 parlai-1.7.2/example_parlai_internal/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2734 2023-06-06 17:44:18.000000 parlai-1.7.2/example_parlai_internal/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:18.000000 parlai-1.7.2/example_parlai_internal/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.105853 parlai-1.7.2/parlai/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      749 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      222 2023-06-06 18:50:59.000000 parlai-1.7.2/parlai/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      547 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/__main__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.138380 parlai-1.7.2/parlai/agents/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1385 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.151197 parlai-1.7.2/parlai/agents/alice/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      555 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/alice/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/alice/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2114 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/alice/alice.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.172376 parlai-1.7.2/parlai/agents/bart/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      847 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bart/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bart/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6036 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bart/bart.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    18448 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bart/convert_fairseq_to_parlai.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2824 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bart/modules.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.184821 parlai-1.7.2/parlai/agents/bert_classifier/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      799 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_classifier/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_classifier/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8642 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_classifier/bert_classifier.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.217861 parlai-1.7.2/parlai/agents/bert_ranker/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1814 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_ranker/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_ranker/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2599 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_ranker/bert_dictionary.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      840 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_ranker/bert_ranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10030 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_ranker/bi_encoder_ranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5336 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_ranker/both_encoder_ranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3421 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_ranker/cross_encoder_ranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7284 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/bert_ranker/helpers.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.238753 parlai-1.7.2/parlai/agents/examples/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      535 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/examples/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/examples/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7495 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/examples/seq2seq.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3572 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/examples/tra.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6891 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/examples/transformer_variant.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.251921 parlai-1.7.2/parlai/agents/fid/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      702 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/fid/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/fid/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    18942 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/fid/fid.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.264810 parlai-1.7.2/parlai/agents/fixed_response/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      353 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/fixed_response/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/fixed_response/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1320 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/fixed_response/fixed_response.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.281214 parlai-1.7.2/parlai/agents/hred/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      876 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hred/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hred/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6521 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hred/hred.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9697 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hred/modules.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.311805 parlai-1.7.2/parlai/agents/hugging_face/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3704 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hugging_face/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hugging_face/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4067 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hugging_face/dialogpt.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8263 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hugging_face/dict.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    12801 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hugging_face/gpt2.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      960 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hugging_face/hugging_face.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13721 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/hugging_face/t5.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.328202 parlai-1.7.2/parlai/agents/image_seq2seq/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      801 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/image_seq2seq/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/image_seq2seq/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8317 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/image_seq2seq/image_seq2seq.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    15611 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/image_seq2seq/modules.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.340765 parlai-1.7.2/parlai/agents/ir_baseline/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      675 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/ir_baseline/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/ir_baseline/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9673 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/ir_baseline/ir_baseline.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.353575 parlai-1.7.2/parlai/agents/local_human/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      365 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/local_human/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/local_human/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3011 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/local_human/local_human.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.370809 parlai-1.7.2/parlai/agents/memnn/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      298 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/memnn/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/memnn/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8089 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/memnn/memnn.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7626 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/memnn/modules.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.424751 parlai-1.7.2/parlai/agents/rag/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13633 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    12531 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/args.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6130 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/conversion_utils.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10212 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/dpr.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    15598 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/indexers.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    48820 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/model_types.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    21182 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/modules.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3456 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/polyfaiss.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    34716 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/rag.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5245 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/retrieve_api.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    50690 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/retrievers.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.438811 parlai-1.7.2/parlai/agents/rag/scripts/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/scripts/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7678 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/scripts/generate_dense_embeddings.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4832 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/rag/scripts/index_dense_embeddings.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.451731 parlai-1.7.2/parlai/agents/random_candidate/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      531 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/random_candidate/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/random_candidate/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2698 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/random_candidate/random_candidate.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.464861 parlai-1.7.2/parlai/agents/repeat_label/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      284 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/repeat_label/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/repeat_label/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3041 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/repeat_label/repeat_label.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.477841 parlai-1.7.2/parlai/agents/repeat_query/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      224 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/repeat_query/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/repeat_query/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1328 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/repeat_query/repeat_query.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.499346 parlai-1.7.2/parlai/agents/reranker/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3364 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/reranker/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/reranker/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      849 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/reranker/classifier_gpt2_reranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3899 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/reranker/classifier_reranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    22618 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/reranker/reranker.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.512402 parlai-1.7.2/parlai/agents/retriever_reader/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      438 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/retriever_reader/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/retriever_reader/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3905 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/retriever_reader/retriever_reader.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.526220 parlai-1.7.2/parlai/agents/safe_local_human/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      461 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/safe_local_human/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/safe_local_human/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4597 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/safe_local_human/safe_local_human.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.545353 parlai-1.7.2/parlai/agents/seq2seq/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      827 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/seq2seq/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/seq2seq/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    24820 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/seq2seq/modules.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9302 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/seq2seq/seq2seq.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.563744 parlai-1.7.2/parlai/agents/starspace/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      494 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/starspace/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/starspace/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2571 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/starspace/modules.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    20522 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/starspace/starspace.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.592671 parlai-1.7.2/parlai/agents/test_agents/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)       44 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/test_agents/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/test_agents/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3451 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/test_agents/counter.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      807 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/test_agents/null.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4375 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/test_agents/test_agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      971 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/test_agents/transformer_generator_prefix.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1387 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/test_agents/unigram.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.624816 parlai-1.7.2/parlai/agents/tfidf_retriever/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      902 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6267 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/build_tfidf.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2100 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/doc_db.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3573 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/tfidf_doc_ranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9999 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/tfidf_retriever.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.646003 parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/
+-rwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)      718 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/__init__.py
+-rwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)     3970 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/regexp_tokenizer.py
+-rwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)     1630 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/simple_tokenizer.py
+-rwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)     2103 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/spacy_tokenizer.py
+-rwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)     2129 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/tokenizer.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4505 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/tfidf_retriever/utils.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.697852 parlai-1.7.2/parlai/agents/transformer/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1956 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5244 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/biencoder.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      343 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/classifier.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3755 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/crossencoder.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3329 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/decoder.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4429 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/dropout_poly.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      345 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/generator.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7810 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/image_polyencoder.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.747621 parlai-1.7.2/parlai/agents/transformer/modules/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      973 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10039 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/attention.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      248 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/constants.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    27590 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/decoder.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14521 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/encoder.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1712 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/ffn.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1802 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/functions.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4674 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/generator.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6176 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/mem_net.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4897 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/modular.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1560 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/modules/wrappers.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    22684 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/polyencoder.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      335 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/ranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    15643 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/transformer/transformer.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.761313 parlai-1.7.2/parlai/agents/unigram/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      250 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/unigram/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/unigram/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3913 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/agents/unigram/unigram.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.769788 parlai-1.7.2/parlai/chat_service/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5461 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.792532 parlai-1.7.2/parlai/chat_service/core/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/core/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4946 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/core/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    30802 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/core/chat_service_manager.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.797758 parlai-1.7.2/parlai/chat_service/core/server/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/core/server/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5922 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/core/socket.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7095 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/core/world_runner.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.801995 parlai-1.7.2/parlai/chat_service/services/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.826519 parlai-1.7.2/parlai/chat_service/services/browser_chat/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      844 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/browser_chat/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/browser_chat/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      320 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/browser_chat/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      464 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/browser_chat/browser_manager.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5420 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/browser_chat/client.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1408 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/browser_chat/run.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.854044 parlai-1.7.2/parlai/chat_service/services/messenger/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      489 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/messenger/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5685 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/messenger/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11419 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/messenger/message_sender.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11193 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/messenger/messenger_manager.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1109 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/messenger/run.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1262 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/messenger/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.883542 parlai-1.7.2/parlai/chat_service/services/terminal_chat/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      743 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/terminal_chat/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/terminal_chat/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      321 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/terminal_chat/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3646 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/terminal_chat/client.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1418 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/terminal_chat/run.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      458 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/terminal_chat/terminal_manager.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.903918 parlai-1.7.2/parlai/chat_service/services/websocket/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/websocket/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2424 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/websocket/agents.py
+-rwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)     1110 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/websocket/run.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2318 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/websocket/sockets.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10414 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/services/websocket/websocket_manager.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.908709 parlai-1.7.2/parlai/chat_service/tasks/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/tasks/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.917663 parlai-1.7.2/parlai/chat_service/tasks/chatbot/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/tasks/chatbot/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4333 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/tasks/chatbot/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.926176 parlai-1.7.2/parlai/chat_service/tasks/overworld_demo/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/tasks/overworld_demo/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8536 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/tasks/overworld_demo/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.935089 parlai-1.7.2/parlai/chat_service/tasks/qa_data_collection/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/tasks/qa_data_collection/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3338 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/tasks/qa_data_collection/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.965495 parlai-1.7.2/parlai/chat_service/utils/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/utils/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2449 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/utils/config.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3869 2023-06-06 17:44:18.000000 parlai-1.7.2/parlai/chat_service/utils/image.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1066 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/chat_service/utils/logging.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6342 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/chat_service/utils/misc.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10239 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/chat_service/utils/server.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2763 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/chat_service/utils/timeout.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.969918 parlai-1.7.2/parlai/clib/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/clib/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.983207 parlai-1.7.2/parlai/clib/cuda/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/clib/cuda/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2000 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/clib/cuda/ngram_repeat_block_cuda.cpp
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4118 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/clib/cuda/ngram_repeat_block_cuda_kernel.cu
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.086413 parlai-1.7.2/parlai/core/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3346 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      411 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    18269 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    24798 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/build_data.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    29950 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/dict.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      292 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/exceptions.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9312 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/image_featurizers.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14111 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/loader.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14471 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/logs.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1883 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/message.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    35793 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/metrics.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8263 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/mutators.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6204 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/opt.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    49959 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/params.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10294 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/script.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    99556 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/teachers.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.122276 parlai-1.7.2/parlai/core/tod/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5479 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/tod/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/tod/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4994 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/tod/teacher_metrics.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    32366 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/tod/tod_agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8951 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/tod/tod_core.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.131557 parlai-1.7.2/parlai/core/tod/tod_test_utils/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/tod/tod_test_utils/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6573 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/tod/tod_test_utils/test_agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13188 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/tod/tod_world.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4584 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/tod/world_metrics.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6448 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/tod/world_metrics_handlers.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    91762 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/torch_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    26840 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/torch_classifier_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    77741 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/torch_generator_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3581 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/torch_image_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    43701 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/torch_ranker_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    48703 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/core/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.140479 parlai-1.7.2/parlai/crowdsourcing/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4804 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.144680 parlai-1.7.2/parlai/crowdsourcing/tasks/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.198307 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13640 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1103 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/acute_eval_agent_state.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6689 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/acute_eval_blueprint.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2890 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/acute_eval_builder.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    17630 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/acute_eval_runner.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    31320 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/analysis.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4189 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/dump_task_to_acute_format.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3265 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/fast_acute_blueprint.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    21588 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/fast_eval.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2314 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/run.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7419 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/util.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.211198 parlai-1.7.2/parlai/crowdsourcing/tasks/chat_demo/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1153 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/chat_demo/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/chat_demo/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2474 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/chat_demo/run.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.228866 parlai-1.7.2/parlai/crowdsourcing/tasks/dialcrowd/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8304 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/dialcrowd/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/dialcrowd/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3861 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/dialcrowd/dialcrowd_blueprint.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.233712 parlai-1.7.2/parlai/crowdsourcing/tasks/dialcrowd/images/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/dialcrowd/images/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1350 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/dialcrowd/run.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.280001 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6629 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.289350 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/analysis/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/analysis/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    18886 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/analysis/compile_results.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4940 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/bot_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      362 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/constants.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2559 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/impl.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    24120 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/model_chat_blueprint.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1349 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/run.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.298301 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/scripts/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/scripts/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2901 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/scripts/save_image_contexts.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    19639 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/utils.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    27409 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/worlds.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5659 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/worlds_image_chat.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.320552 parlai-1.7.2/parlai/crowdsourcing/tasks/multi_model_chat/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      840 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/multi_model_chat/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/multi_model_chat/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11970 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/multi_model_chat/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13709 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/multi_model_chat/compile_results.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13554 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/multi_model_chat/multiparty_worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.350918 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6438 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.359433 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/analysis/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/analysis/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    24077 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/analysis/compile_results.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1840 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/bot_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2036 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/impl.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7337 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/per_turn_eval_blueprint.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1529 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/run.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    22952 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.381583 parlai-1.7.2/parlai/crowdsourcing/tasks/qa_data_collection/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1801 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/qa_data_collection/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:19.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/qa_data_collection/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2699 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/qa_data_collection/run.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      779 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/qa_data_collection/util.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2355 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/qa_data_collection/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.398893 parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2590 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.407858 parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/analysis/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/analysis/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    24682 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/analysis/compile_results.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1505 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/run.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    17918 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/turn_annotations_blueprint.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.445303 parlai-1.7.2/parlai/crowdsourcing/utils/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3846 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/utils/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/utils/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5080 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/utils/acceptability.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8802 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/utils/analysis.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1217 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/utils/frontend.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4024 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/utils/mturk.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    17594 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/utils/tests.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3648 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/crowdsourcing/utils/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.485679 parlai-1.7.2/parlai/mutators/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/mutators/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1001 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/mutators/context_shuffle.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1842 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/mutators/episode_reverse.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1836 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/mutators/episode_shuffle.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      935 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/mutators/flatten.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5493 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/mutators/flip_labels.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1518 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/mutators/last_turn.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1172 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/mutators/word_reverse.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1167 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/mutators/word_shuffle.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.499449 parlai-1.7.2/parlai/nn/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/nn/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      547 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/nn/checkpoint.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    17643 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/nn/lr_scheduler.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.508682 parlai-1.7.2/parlai/ops/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/ops/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2603 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/ops/ngram_repeat_block.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.522613 parlai-1.7.2/parlai/opt_presets/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      800 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/opt_presets/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/opt_presets/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2133 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/opt_presets/docs.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.679955 parlai-1.7.2/parlai/scripts/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3237 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/build_candidates.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5014 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/build_dict.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3049 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/compare_opts.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      954 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/convert_data_to_json_format.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3245 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/convert_data_to_parlai_format.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10549 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/convo_render.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5963 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/data_stats.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4517 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/detect_offensive_language.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3923 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/display_data.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2968 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/display_model.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1776 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/distributed_eval.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      972 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/distributed_tod_world_script.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1782 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/distributed_train.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9884 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/eval_model.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9590 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/eval_wordstat.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2038 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/extract_image_feature.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1360 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/flask.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    60325 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/generate_model_card.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3911 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/interactive.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10378 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/interactive_web.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2994 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/multiprocessing_eval.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3465 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/multiprocessing_train.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10248 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/party.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2758 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/profile_interactive.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2526 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/profile_train.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2667 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/safe_interactive.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5642 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/self_chat.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    17304 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/tod_world_script.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3714 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/token_stats.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4315 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/torchscript.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    39307 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/train_model.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2427 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/vacuum.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5106 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/scripts/verify_data.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.698915 parlai-1.7.2/parlai/tasks/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      826 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.716966 parlai-1.7.2/parlai/tasks/airdialogue/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/airdialogue/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3384 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/airdialogue/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1105 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/airdialogue/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      406 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/airdialogue/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.730741 parlai-1.7.2/parlai/tasks/amazon_qa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/amazon_qa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3690 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/amazon_qa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10704 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/amazon_qa/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.749624 parlai-1.7.2/parlai/tasks/anli/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/anli/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5829 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/anli/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1183 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/anli/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      326 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/anli/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.771858 parlai-1.7.2/parlai/tasks/aqua/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      208 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/aqua/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/aqua/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6809 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/aqua/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1241 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/aqua/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      312 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/aqua/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.785875 parlai-1.7.2/parlai/tasks/asdiv/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/asdiv/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2991 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/asdiv/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1370 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/asdiv/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.810115 parlai-1.7.2/parlai/tasks/babi/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      713 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/babi/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/babi/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3541 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/babi/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1158 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/babi/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      448 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/babi/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.838239 parlai-1.7.2/parlai/tasks/blended_skill_talk/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4473 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/blended_skill_talk/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/blended_skill_talk/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    23214 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/blended_skill_talk/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7608 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/blended_skill_talk/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      431 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/blended_skill_talk/test.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7028 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/blended_skill_talk/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.857107 parlai-1.7.2/parlai/tasks/booktest/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      232 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/booktest/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/booktest/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1090 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/booktest/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1172 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/booktest/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.880661 parlai-1.7.2/parlai/tasks/bot_adversarial_dialogue/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1269 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/bot_adversarial_dialogue/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/bot_adversarial_dialogue/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11317 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/bot_adversarial_dialogue/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3597 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/bot_adversarial_dialogue/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      987 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/bot_adversarial_dialogue/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.898672 parlai-1.7.2/parlai/tasks/c3/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/c3/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      624 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/c3/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1509 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/c3/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      369 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/c3/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.920969 parlai-1.7.2/parlai/tasks/casino/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1531 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/casino/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/casino/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13981 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/casino/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1722 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/casino/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      328 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/casino/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.943408 parlai-1.7.2/parlai/tasks/cbt/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      248 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cbt/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cbt/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1786 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cbt/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1150 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cbt/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      325 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cbt/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.958320 parlai-1.7.2/parlai/tasks/ccpe/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/ccpe/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5177 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/ccpe/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1211 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/ccpe/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.976486 parlai-1.7.2/parlai/tasks/clevr/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      285 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/clevr/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/clevr/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2236 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/clevr/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1167 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/clevr/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:46.995272 parlai-1.7.2/parlai/tasks/cmu_dog/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cmu_dog/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13286 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cmu_dog/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5770 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cmu_dog/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      329 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cmu_dog/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.012313 parlai-1.7.2/parlai/tasks/cnn_dm/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      258 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cnn_dm/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cnn_dm/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2986 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cnn_dm/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4296 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cnn_dm/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.039789 parlai-1.7.2/parlai/tasks/coco_caption/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      207 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/coco_caption/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/coco_caption/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13934 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/coco_caption/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2469 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/coco_caption/build_2014.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2106 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/coco_caption/build_2015.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2805 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/coco_caption/build_2017.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.053818 parlai-1.7.2/parlai/tasks/commonsenseqa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/commonsenseqa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2744 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/commonsenseqa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1269 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/commonsenseqa/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.081443 parlai-1.7.2/parlai/tasks/convai2/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      228 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai2/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai2/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7372 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai2/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1188 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai2/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      628 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai2/test.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4008 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai2/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.099763 parlai-1.7.2/parlai/tasks/convai2_wild_evaluation/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      297 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai2_wild_evaluation/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai2_wild_evaluation/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      764 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai2_wild_evaluation/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2522 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai2_wild_evaluation/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.117731 parlai-1.7.2/parlai/tasks/convai_chitchat/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      240 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai_chitchat/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      222 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai_chitchat/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3276 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai_chitchat/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1352 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/convai_chitchat/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.136811 parlai-1.7.2/parlai/tasks/copa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      450 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/copa/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/copa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2081 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/copa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1131 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/copa/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.155498 parlai-1.7.2/parlai/tasks/coqa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      468 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/coqa/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/coqa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      854 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/coqa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2939 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/coqa/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.177872 parlai-1.7.2/parlai/tasks/cornell_movie/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      227 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cornell_movie/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cornell_movie/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2448 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cornell_movie/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1222 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cornell_movie/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      412 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/cornell_movie/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.205131 parlai-1.7.2/parlai/tasks/dailydialog/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      372 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dailydialog/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dailydialog/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4169 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dailydialog/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1186 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dailydialog/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3123 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dailydialog/parse.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      412 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dailydialog/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.228032 parlai-1.7.2/parlai/tasks/dbll_babi/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      633 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dbll_babi/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dbll_babi/__init__.py
+-rwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)     2100 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dbll_babi/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1148 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dbll_babi/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      331 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dbll_babi/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.251316 parlai-1.7.2/parlai/tasks/dbll_movie/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      446 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dbll_movie/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dbll_movie/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2339 2023-06-06 17:44:20.000000 parlai-1.7.2/parlai/tasks/dbll_movie/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      756 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dbll_movie/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      399 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dbll_movie/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.274617 parlai-1.7.2/parlai/tasks/dealnodeal/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      315 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dealnodeal/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dealnodeal/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7383 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dealnodeal/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1217 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dealnodeal/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      332 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dealnodeal/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.287354 parlai-1.7.2/parlai/tasks/decanlp/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      536 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/decanlp/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/decanlp/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2011 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/decanlp/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.305044 parlai-1.7.2/parlai/tasks/decode/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/decode/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3029 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/decode/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1255 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/decode/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      328 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/decode/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.328877 parlai-1.7.2/parlai/tasks/dialog_babi/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      190 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialog_babi/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialog_babi/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2222 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialog_babi/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1182 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialog_babi/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      333 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialog_babi/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.352231 parlai-1.7.2/parlai/tasks/dialog_babi_plus/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      534 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialog_babi_plus/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialog_babi_plus/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1641 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialog_babi_plus/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1094 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialog_babi_plus/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      411 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialog_babi_plus/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.370937 parlai-1.7.2/parlai/tasks/dialogue_nli/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_nli/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4378 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_nli/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1256 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_nli/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      334 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_nli/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.393420 parlai-1.7.2/parlai/tasks/dialogue_qe/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      250 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_qe/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      222 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_qe/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2654 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_qe/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1395 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_qe/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      319 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_qe/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.412113 parlai-1.7.2/parlai/tasks/dialogue_safety/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_safety/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13726 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_safety/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3059 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_safety/base_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1377 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dialogue_safety/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.430450 parlai-1.7.2/parlai/tasks/dream/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dream/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2512 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dream/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1506 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dream/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      385 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dream/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.448481 parlai-1.7.2/parlai/tasks/dstc7/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dstc7/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4895 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dstc7/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1107 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dstc7/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      327 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/dstc7/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.466877 parlai-1.7.2/parlai/tasks/eli5/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6243 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2635 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4358 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.499679 parlai-1.7.2/parlai/tasks/eli5/data_creation/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/data_creation/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9191 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/data_creation/data_utils.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    21150 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/data_creation/download_reddit_qalist.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13468 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/data_creation/download_support_docs.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2215 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/data_creation/finalize_qda.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3441 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/data_creation/merge_support_docs.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5700 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/data_creation/select_sentences_tfidf.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.504451 parlai-1.7.2/parlai/tasks/eli5/data_creation/slurm_scripts/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eli5/data_creation/slurm_scripts/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.531945 parlai-1.7.2/parlai/tasks/empathetic_dialogues/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      818 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/empathetic_dialogues/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/empathetic_dialogues/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6462 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/empathetic_dialogues/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1216 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/empathetic_dialogues/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      342 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/empathetic_dialogues/test.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      367 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/empathetic_dialogues/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.545501 parlai-1.7.2/parlai/tasks/entailment_bank/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/entailment_bank/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5743 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/entailment_bank/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1294 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/entailment_bank/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.559633 parlai-1.7.2/parlai/tasks/eqasc/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eqasc/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3101 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eqasc/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1976 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/eqasc/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.588325 parlai-1.7.2/parlai/tasks/fits/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fits/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    27863 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fits/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1639 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fits/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      631 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fits/constants.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11361 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fits/mutators.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      585 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fits/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.606733 parlai-1.7.2/parlai/tasks/flickr30k/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      297 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/flickr30k/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/flickr30k/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6178 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/flickr30k/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1175 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/flickr30k/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.626099 parlai-1.7.2/parlai/tasks/friends/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/friends/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11265 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/friends/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3241 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/friends/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      844 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/friends/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.640022 parlai-1.7.2/parlai/tasks/fromfile/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      322 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fromfile/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fromfile/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5082 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fromfile/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.658677 parlai-1.7.2/parlai/tasks/funpedia/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/funpedia/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5122 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/funpedia/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1203 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/funpedia/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      695 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/funpedia/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.677025 parlai-1.7.2/parlai/tasks/fvqa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      455 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fvqa/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fvqa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5895 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fvqa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1129 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/fvqa/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.699877 parlai-1.7.2/parlai/tasks/genderation_bias/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2315 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/genderation_bias/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/genderation_bias/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10633 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/genderation_bias/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1461 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/genderation_bias/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4481 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/genderation_bias/utils.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.718775 parlai-1.7.2/parlai/tasks/glue/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      346 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/glue/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/glue/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4224 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/glue/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      893 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/glue/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.742095 parlai-1.7.2/parlai/tasks/google_sgd/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      207 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/google_sgd/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/google_sgd/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    12932 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/google_sgd/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1651 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/google_sgd/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      509 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/google_sgd/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.765142 parlai-1.7.2/parlai/tasks/google_sgd_simulation_splits/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      422 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/google_sgd_simulation_splits/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/google_sgd_simulation_splits/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6141 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/google_sgd_simulation_splits/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4950 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/google_sgd_simulation_splits/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      745 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/google_sgd_simulation_splits/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.788024 parlai-1.7.2/parlai/tasks/holl_e/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      867 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/holl_e/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/holl_e/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5553 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/holl_e/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1435 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/holl_e/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      384 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/holl_e/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.810409 parlai-1.7.2/parlai/tasks/hotpotqa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      447 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/hotpotqa/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/hotpotqa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1331 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/hotpotqa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3280 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/hotpotqa/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      474 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/hotpotqa/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.824188 parlai-1.7.2/parlai/tasks/huggingface/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      112 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/huggingface/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/huggingface/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4686 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/huggingface/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.833630 parlai-1.7.2/parlai/tasks/igc/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/igc/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11014 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/igc/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.857206 parlai-1.7.2/parlai/tasks/image_chat/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      753 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/image_chat/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/image_chat/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14335 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/image_chat/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1382 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/image_chat/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      781 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/image_chat/download_data.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.879875 parlai-1.7.2/parlai/tasks/insuranceqa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      259 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/insuranceqa/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/insuranceqa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1293 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/insuranceqa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8456 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/insuranceqa/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      455 2023-06-06 17:44:21.000000 parlai-1.7.2/parlai/tasks/insuranceqa/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.893265 parlai-1.7.2/parlai/tasks/integration_tests/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      160 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/integration_tests/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/integration_tests/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    16616 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/integration_tests/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.912059 parlai-1.7.2/parlai/tasks/interactive/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      117 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/interactive/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/interactive/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      346 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/interactive/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2993 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/interactive/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.935072 parlai-1.7.2/parlai/tasks/iwslt14/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      217 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/iwslt14/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/iwslt14/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1657 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/iwslt14/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1164 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/iwslt14/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      329 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/iwslt14/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.962895 parlai-1.7.2/parlai/tasks/jericho_world/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1542 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/jericho_world/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/jericho_world/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    21968 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/jericho_world/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1468 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/jericho_world/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1150 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/jericho_world/constants.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      706 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/jericho_world/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.976498 parlai-1.7.2/parlai/tasks/jsonfile/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      375 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/jsonfile/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/jsonfile/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2286 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/jsonfile/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:47.996052 parlai-1.7.2/parlai/tasks/lccc/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/lccc/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1445 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/lccc/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2104 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/lccc/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      312 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/lccc/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.028424 parlai-1.7.2/parlai/tasks/light_dialog/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      269 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10120 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2835 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13835 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog/builder.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      320 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog/test.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4531 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.056805 parlai-1.7.2/parlai/tasks/light_dialog_wild/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      332 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog_wild/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog_wild/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    17210 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog_wild/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3576 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog_wild/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    28587 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog_wild/builder.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      325 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_dialog_wild/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.075447 parlai-1.7.2/parlai/tasks/light_genderation_bias/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      257 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_genderation_bias/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_genderation_bias/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    12975 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_genderation_bias/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1183 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_genderation_bias/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.098869 parlai-1.7.2/parlai/tasks/light_multiparty/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      235 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_multiparty/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_multiparty/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    23562 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_multiparty/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1146 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_multiparty/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      842 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/light_multiparty/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.113061 parlai-1.7.2/parlai/tasks/math_dataset/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/math_dataset/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9478 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/math_dataset/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1326 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/math_dataset/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.135982 parlai-1.7.2/parlai/tasks/mctest/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      263 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mctest/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mctest/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      971 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mctest/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3391 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mctest/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      328 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mctest/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.200879 parlai-1.7.2/parlai/tasks/md_gender/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1717 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1170 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10426 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/convai2.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4296 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/funpedia.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5835 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/image_chat.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7525 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/light.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3524 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/new_data.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      449 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/opensubtitles.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8635 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/utils.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9828 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/wikipedia.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4487 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/wizard.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5048 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/worlds.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8921 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/md_gender/yelp.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.219579 parlai-1.7.2/parlai/tasks/metalwoz/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/metalwoz/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4462 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/metalwoz/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1527 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/metalwoz/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      410 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/metalwoz/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.242886 parlai-1.7.2/parlai/tasks/mnist_qa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      170 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mnist_qa/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mnist_qa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2285 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mnist_qa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1160 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mnist_qa/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      330 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mnist_qa/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.260573 parlai-1.7.2/parlai/tasks/moviedialog/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1034 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/moviedialog/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/moviedialog/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3239 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/moviedialog/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2270 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/moviedialog/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.279764 parlai-1.7.2/parlai/tasks/ms_marco/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      280 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/ms_marco/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/ms_marco/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1817 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/ms_marco/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4321 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/ms_marco/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.307215 parlai-1.7.2/parlai/tasks/msc/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/msc/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    30947 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/msc/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1342 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/msc/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2312 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/msc/constants.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1088 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/msc/mutators.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      619 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/msc/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.325091 parlai-1.7.2/parlai/tasks/msr_e2e/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/msr_e2e/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9993 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/msr_e2e/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1772 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/msr_e2e/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      421 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/msr_e2e/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.343449 parlai-1.7.2/parlai/tasks/mturkwikimovies/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      254 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mturkwikimovies/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mturkwikimovies/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      999 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mturkwikimovies/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1354 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mturkwikimovies/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.361818 parlai-1.7.2/parlai/tasks/multidogo/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multidogo/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6005 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multidogo/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    12446 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multidogo/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      479 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multidogo/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.385430 parlai-1.7.2/parlai/tasks/multinli/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      423 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multinli/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multinli/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5682 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multinli/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1127 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multinli/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      316 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multinli/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.403057 parlai-1.7.2/parlai/tasks/multiwoz_v20/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v20/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4210 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v20/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1065 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v20/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      402 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v20/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.421326 parlai-1.7.2/parlai/tasks/multiwoz_v21/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v21/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4210 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v21/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1069 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v21/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      402 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v21/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.449594 parlai-1.7.2/parlai/tasks/multiwoz_v22/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      328 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v22/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v22/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    23467 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v22/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7958 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v22/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2198 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v22/build_sha_check_script.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      517 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/multiwoz_v22/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.467751 parlai-1.7.2/parlai/tasks/mutualfriends/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      262 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mutualfriends/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mutualfriends/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3287 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mutualfriends/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1235 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mutualfriends/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.484932 parlai-1.7.2/parlai/tasks/mwsc/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      222 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mwsc/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mwsc/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1458 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mwsc/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3331 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/mwsc/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.503761 parlai-1.7.2/parlai/tasks/narrative_qa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      415 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/narrative_qa/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/narrative_qa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4471 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/narrative_qa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5668 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/narrative_qa/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.532177 parlai-1.7.2/parlai/tasks/natural_questions/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      269 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/natural_questions/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/natural_questions/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14049 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/natural_questions/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4281 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/natural_questions/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2178 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/natural_questions/build_open.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      487 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/natural_questions/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.545949 parlai-1.7.2/parlai/tasks/natural_questions/utils/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      165 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/natural_questions/utils/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/natural_questions/utils/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5999 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/natural_questions/utils/text_utils.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.555686 parlai-1.7.2/parlai/tasks/nli/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/nli/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2123 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/nli/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.574074 parlai-1.7.2/parlai/tasks/nlvr/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      286 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/nlvr/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/nlvr/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1880 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/nlvr/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1142 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/nlvr/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.592363 parlai-1.7.2/parlai/tasks/onecommon/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      387 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/onecommon/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/onecommon/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8582 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/onecommon/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1156 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/onecommon/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.614874 parlai-1.7.2/parlai/tasks/opensubtitles/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      342 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/opensubtitles/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/opensubtitles/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5991 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/opensubtitles/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/opensubtitles/build_2009.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11397 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/opensubtitles/build_2018.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.638491 parlai-1.7.2/parlai/tasks/personachat/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      251 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/personachat/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/personachat/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2629 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/personachat/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1149 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/personachat/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1141 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/personachat/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.662624 parlai-1.7.2/parlai/tasks/personality_captions/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      485 2023-06-06 17:44:22.000000 parlai-1.7.2/parlai/tasks/personality_captions/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/personality_captions/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9285 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/personality_captions/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1310 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/personality_captions/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2368 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/personality_captions/download_images.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.680226 parlai-1.7.2/parlai/tasks/personalized_dialog/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      613 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/personalized_dialog/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/personalized_dialog/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3758 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/personalized_dialog/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1232 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/personalized_dialog/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.694309 parlai-1.7.2/parlai/tasks/proof_writer/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/proof_writer/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13395 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/proof_writer/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1369 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/proof_writer/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.712957 parlai-1.7.2/parlai/tasks/prosocial_dialog/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/prosocial_dialog/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4388 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/prosocial_dialog/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1236 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/prosocial_dialog/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      572 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/prosocial_dialog/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.731161 parlai-1.7.2/parlai/tasks/qacnn/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      210 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qacnn/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qacnn/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      685 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qacnn/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2282 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qacnn/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.749330 parlai-1.7.2/parlai/tasks/qadailymail/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      237 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qadailymail/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qadailymail/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      691 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qadailymail/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2263 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qadailymail/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.768019 parlai-1.7.2/parlai/tasks/qangaroo/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      261 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qangaroo/README.md
+-rwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qangaroo/__init__.py
+-rwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)     3121 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qangaroo/agents.py
+-rwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)     1181 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qangaroo/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.784924 parlai-1.7.2/parlai/tasks/qasrl/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      250 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qasrl/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qasrl/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2721 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qasrl/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1635 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qasrl/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.802919 parlai-1.7.2/parlai/tasks/qazre/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      269 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qazre/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qazre/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1781 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qazre/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1192 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/qazre/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.825143 parlai-1.7.2/parlai/tasks/quac/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      740 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/quac/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/quac/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      854 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/quac/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3553 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/quac/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      312 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/quac/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.847536 parlai-1.7.2/parlai/tasks/reasoning/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reasoning/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2851 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reasoning/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    20126 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reasoning/base.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4558 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reasoning/question_answer.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.861063 parlai-1.7.2/parlai/tasks/reasoning/reason_types/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reasoning/reason_types/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1132 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reasoning/reason_types/free_form.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    37128 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reasoning/reason_types/step_by_step.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)       38 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reasoning/requirements.txt
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.880279 parlai-1.7.2/parlai/tasks/redial/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/redial/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4401 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/redial/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1014 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/redial/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      386 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/redial/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.899165 parlai-1.7.2/parlai/tasks/reframe_thoughts/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reframe_thoughts/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1644 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reframe_thoughts/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1278 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reframe_thoughts/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      338 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/reframe_thoughts/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.921880 parlai-1.7.2/parlai/tasks/saferdialogues/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1036 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/saferdialogues/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/saferdialogues/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3213 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/saferdialogues/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1298 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/saferdialogues/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      437 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/saferdialogues/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.941009 parlai-1.7.2/parlai/tasks/safety_mix/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/safety_mix/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3941 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/safety_mix/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    15347 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/safety_mix/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      506 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/safety_mix/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.963764 parlai-1.7.2/parlai/tasks/scan/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      424 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/scan/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/scan/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      684 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/scan/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2213 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/scan/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      326 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/scan/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.978121 parlai-1.7.2/parlai/tasks/self_chat/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/self_chat/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      460 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/self_chat/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6981 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/self_chat/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:48.996049 parlai-1.7.2/parlai/tasks/sensitive_topics_evaluation/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      303 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/sensitive_topics_evaluation/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/sensitive_topics_evaluation/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1387 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/sensitive_topics_evaluation/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1256 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/sensitive_topics_evaluation/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.018339 parlai-1.7.2/parlai/tasks/simplequestions/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      210 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/simplequestions/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/simplequestions/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      715 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/simplequestions/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1198 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/simplequestions/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      337 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/simplequestions/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.040726 parlai-1.7.2/parlai/tasks/snli/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      512 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/snli/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/snli/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2514 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/snli/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1116 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/snli/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      312 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/snli/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.062725 parlai-1.7.2/parlai/tasks/spolin/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      915 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/spolin/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/spolin/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2301 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/spolin/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1695 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/spolin/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      362 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/spolin/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.085093 parlai-1.7.2/parlai/tasks/squad/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      205 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/squad/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/squad/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14423 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/squad/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2204 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/squad/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      691 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/squad/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.109331 parlai-1.7.2/parlai/tasks/squad2/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      213 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/squad2/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/squad2/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    15503 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/squad2/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1436 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/squad2/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      730 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/squad2/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.132206 parlai-1.7.2/parlai/tasks/sst/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      386 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/sst/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/sst/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2118 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/sst/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1830 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/sst/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      375 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/sst/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.155392 parlai-1.7.2/parlai/tasks/style_gen/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1666 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/style_gen/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/style_gen/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5933 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/style_gen/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2485 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/style_gen/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      658 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/style_gen/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.173509 parlai-1.7.2/parlai/tasks/superglue/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      400 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/superglue/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/superglue/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2133 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/superglue/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      525 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/superglue/test.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    64268 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/task_list.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.196640 parlai-1.7.2/parlai/tasks/taskmaster/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    19615 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1625 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      773 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster/test.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5584 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster/tm_utils.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.220539 parlai-1.7.2/parlai/tasks/taskmaster2/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      179 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster2/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster2/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7886 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster2/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4014 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster2/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      416 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster2/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.239221 parlai-1.7.2/parlai/tasks/taskmaster3/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster3/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7046 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster3/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5232 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster3/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      429 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskmaster3/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.257054 parlai-1.7.2/parlai/tasks/taskntalk/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      244 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskntalk/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskntalk/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3737 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskntalk/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4163 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/taskntalk/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1795 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/tasks.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.271017 parlai-1.7.2/parlai/tasks/tod_json/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      496 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/tod_json/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/tod_json/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9036 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/tod_json/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.289420 parlai-1.7.2/parlai/tasks/triviaqa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/triviaqa/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/triviaqa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6284 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/triviaqa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3822 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/triviaqa/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.312688 parlai-1.7.2/parlai/tasks/twitter/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      233 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/twitter/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/twitter/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      695 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/twitter/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3851 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/twitter/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      329 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/twitter/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.335968 parlai-1.7.2/parlai/tasks/ubuntu/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      265 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/ubuntu/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/ubuntu/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3898 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/ubuntu/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1163 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/ubuntu/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      405 2023-06-06 17:44:23.000000 parlai-1.7.2/parlai/tasks/ubuntu/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.353539 parlai-1.7.2/parlai/tasks/visdial/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      213 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/visdial/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/visdial/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3332 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/visdial/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2812 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/visdial/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.371112 parlai-1.7.2/parlai/tasks/vqa_v1/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      186 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/vqa_v1/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/vqa_v1/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    17758 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/vqa_v1/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2109 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/vqa_v1/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.389717 parlai-1.7.2/parlai/tasks/vqa_v2/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      191 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/vqa_v2/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/vqa_v2/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5937 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/vqa_v2/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2135 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/vqa_v2/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.407815 parlai-1.7.2/parlai/tasks/webquestions/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      200 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/webquestions/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/webquestions/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      692 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/webquestions/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2414 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/webquestions/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.430322 parlai-1.7.2/parlai/tasks/wikimovies/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      237 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikimovies/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikimovies/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1895 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikimovies/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1178 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikimovies/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      332 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikimovies/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.448707 parlai-1.7.2/parlai/tasks/wikipedia/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      379 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikipedia/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikipedia/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6906 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikipedia/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1295 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikipedia/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.472129 parlai-1.7.2/parlai/tasks/wikiqa/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      251 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikiqa/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikiqa/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      979 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikiqa/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2789 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikiqa/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      328 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikiqa/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.494014 parlai-1.7.2/parlai/tasks/wikisql/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      284 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikisql/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikisql/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3495 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikisql/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1403 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikisql/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      392 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wikisql/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.526388 parlai-1.7.2/parlai/tasks/wizard_of_internet/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      620 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_internet/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_internet/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    24894 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_internet/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1212 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_internet/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2368 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_internet/constants.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9597 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_internet/mutators.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      954 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_internet/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.558560 parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      917 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    45682 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1091 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5943 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/mutators.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1253 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/test.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8657 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/worlds.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.581071 parlai-1.7.2/parlai/tasks/wmt/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      127 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wmt/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wmt/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      842 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wmt/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3419 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wmt/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      376 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wmt/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.603988 parlai-1.7.2/parlai/tasks/woz/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      362 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/woz/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/woz/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1915 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/woz/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1735 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/woz/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      374 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/woz/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.617587 parlai-1.7.2/parlai/tasks/wrapper/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      166 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wrapper/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wrapper/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6305 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/wrapper/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.635759 parlai-1.7.2/parlai/tasks/xpersona/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/xpersona/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1435 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/xpersona/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8152 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/xpersona/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      785 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/tasks/xpersona/test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.658732 parlai-1.7.2/parlai/torchscript/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1172 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/torchscript/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/torchscript/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2242 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/torchscript/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    21156 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/torchscript/modules.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.667970 parlai-1.7.2/parlai/torchscript/scripts/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/torchscript/scripts/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1350 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/torchscript/scripts/test_exported_model.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    22843 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/torchscript/tokenizer.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.756234 parlai-1.7.2/parlai/utils/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    31618 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/bpe.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10369 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/conversations.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6033 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/curated_response.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6447 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/data.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11398 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/distributed.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3423 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/flake8.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    31338 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/fp16.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7824 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/fsdp.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      901 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/io.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4916 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/logging.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    23309 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/misc.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1714 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/pickle.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8816 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/safety.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5006 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/strings.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14483 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/testing.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    22580 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/torch.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      944 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/typing.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5957 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/utils/world_logging.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.769721 parlai-1.7.2/parlai/zoo/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      430 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.780169 parlai-1.7.2/parlai/zoo/bart/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bart/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2295 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bart/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.808302 parlai-1.7.2/parlai/zoo/bb3/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11098 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bb3/MODEL_LICENSE.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bb3/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      678 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bb3/bb3_3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    15352 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bb3/data_card.md
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.812744 parlai-1.7.2/parlai/zoo/bb3/images/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bb3/images/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    31919 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bb3/model_card.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      690 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bb3/persona_summarizer.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.821984 parlai-1.7.2/parlai/zoo/bert/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bert/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1222 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bert/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.853669 parlai-1.7.2/parlai/zoo/blended_skill_talk/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blended_skill_talk/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      677 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blended_skill_talk/bst_single_task.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      672 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blended_skill_talk/convai2_single_task.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      679 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blended_skill_talk/ed_single_task.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      718 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blended_skill_talk/multi_task.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      763 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blended_skill_talk/multi_task_bst_tuned.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      683 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blended_skill_talk/wizard_single_task.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.907560 parlai-1.7.2/parlai/zoo/blender/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      539 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/blender_1Bdistill.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      421 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/blender_3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      543 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/blender_400Mdistill.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      421 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/blender_90M.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      421 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/blender_9B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2251 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/blender_ascii.txt
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      882 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      436 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/dict_3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      439 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/dict_90M.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      425 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/reddit_3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      425 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blender/reddit_9B.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.934451 parlai-1.7.2/parlai/zoo/blenderbot2/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blenderbot2/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      724 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blenderbot2/blenderbot2_3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      728 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blenderbot2/blenderbot2_400M.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      739 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blenderbot2/memory_decoder.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11895 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blenderbot2/model_card.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      741 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/blenderbot2/query_generator.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.947094 parlai-1.7.2/parlai/zoo/bot_adversarial_dialogue/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bot_adversarial_dialogue/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      801 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bot_adversarial_dialogue/multi_turn.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      803 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/bot_adversarial_dialogue/multi_turn_v0.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.968501 parlai-1.7.2/parlai/zoo/dialogue_bias/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_bias/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      752 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_bias/gender__ctrl_gen_tokens.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      689 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_bias/gender__name_scrambling.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      724 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_bias/gender__unlikelihood_sequence_level.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      718 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_bias/gender_ethnicity__name_scrambling.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:49.982472 parlai-1.7.2/parlai/zoo/dialogue_safety/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_safety/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      559 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_safety/multi_turn.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      581 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_safety/single_turn.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.046973 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      719 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      511 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_convai2_ctxt.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      541 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_convai2_ctxt_and_label.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      511 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_convai2_label.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      463 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_eli5_ctxt.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      532 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_eli5_ctxt_and_label.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      477 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_eli5_label.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      478 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_wiki_ctxt.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      547 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_wiki_ctxt_and_label.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      492 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_wiki_label.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      465 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/vocab_alpha1e0.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      465 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/vocab_alpha1e1.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      465 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/vocab_alpha1e2.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      465 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/vocab_alpha1e3.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.112853 parlai-1.7.2/parlai/zoo/dodecadialogue/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      318 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/all_tasks_mt.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1209 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      316 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/convai2_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      322 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/cornell_movie_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      321 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/daily_dialog_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      313 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/eli5_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      329 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/empathetic_dialogues_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      312 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/igc_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      319 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/image_chat_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      321 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/light_dialog_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      315 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/reddit_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      316 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/twitter_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      315 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/ubuntu_ft.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      328 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/dodecadialogue/wizard_of_wikipedia_ft.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.121967 parlai-1.7.2/parlai/zoo/fasttext_cc_vectors/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fasttext_cc_vectors/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      618 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fasttext_cc_vectors/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.131600 parlai-1.7.2/parlai/zoo/fasttext_vectors/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fasttext_vectors/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      574 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fasttext_vectors/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.163571 parlai-1.7.2/parlai/zoo/fits/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fits/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      744 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fits/bart_sq_gen.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      734 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fits/bb2_module_supervision.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      731 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fits/director_bb2_module.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      723 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fits/director_seeker_module.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      723 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fits/response_satisfaction.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      723 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/fits/seeker_module_supervision.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.172856 parlai-1.7.2/parlai/zoo/glove_vectors/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/glove_vectors/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      493 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/glove_vectors/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.240138 parlai-1.7.2/parlai/zoo/hallucination/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      740 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/bart_fid_dpr.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      741 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/bart_fid_rag.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      749 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/bart_fid_rag_dpr_poly.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      745 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/bart_rag_dpr_poly.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      745 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/bart_rag_sequence.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      742 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/bart_rag_token.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      744 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/bart_rag_turn_do.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      745 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/bart_rag_turn_dtt.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      740 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/dropout_poly.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      892 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/multiset_dpr.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      791 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/wiki_index_compressed.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      778 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/wiki_index_exact.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1079 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/wiki_passages.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      769 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/hallucination/wow_passages.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.249309 parlai-1.7.2/parlai/zoo/image_chat/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/image_chat/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      553 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/image_chat/transresnet_multimodal.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.258315 parlai-1.7.2/parlai/zoo/light/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/light/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      580 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/light/biranker_dialogue.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.321594 parlai-1.7.2/parlai/zoo/light_whoami/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/light_whoami/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      522 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/light_whoami/automated_expanded_attention_1024.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      514 2023-06-06 17:44:24.000000 parlai-1.7.2/parlai/zoo/light_whoami/expanded_and_multiobjective_1024.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      427 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/multiobjective.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      541 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/profile_expanded_attention_1024.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      530 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/profile_expanded_attention_128.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      394 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/rpa_reranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      452 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/rpa_reranker_auto_expanded_attention.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      402 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/rpa_ul_1024.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      400 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/rpa_ul_128.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      404 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/test_rpa_reranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      416 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/vanilla_1024.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      414 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/vanilla_128.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      738 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/light_whoami/whoami_download.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.329742 parlai-1.7.2/parlai/zoo/md_gender/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/md_gender/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      615 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/md_gender/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)   176160 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/model_list.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.355717 parlai-1.7.2/parlai/zoo/msc/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/msc/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      716 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/msc/blender3B_1024.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      727 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/msc/dialog_summarizer.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      709 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/msc/msc3B_1024.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      715 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/msc/summsc_fidrag3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      708 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/msc/summsc_rag3B.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.378032 parlai-1.7.2/parlai/zoo/multilight/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/multilight/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      400 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/multilight/speaker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      681 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/multilight/utils.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      449 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/multilight/utterance_3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      451 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/multilight/utterance_400m.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.387147 parlai-1.7.2/parlai/zoo/multimodal_blenderbot/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6657 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/multimodal_blenderbot/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/multimodal_blenderbot/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.396219 parlai-1.7.2/parlai/zoo/personality_captions/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/personality_captions/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      540 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/personality_captions/transresnet.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.446260 parlai-1.7.2/parlai/zoo/pretrained_transformers/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5267 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      241 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/bi_model_huge_reddit.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      241 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/bi_model_huge_wikito.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      758 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/build.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      241 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/cross_model_huge_reddit.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      241 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/cross_model_huge_wikito.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      241 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/model_bi.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      241 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/model_poly.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      241 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/poly_model_huge_reddit.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      241 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/pretrained_transformers/poly_model_huge_wikito.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.455660 parlai-1.7.2/parlai/zoo/saferdialogues/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      220 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/saferdialogues/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      617 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/saferdialogues/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.473213 parlai-1.7.2/parlai/zoo/sea/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/sea/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      741 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/sea/bart_base.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      800 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/sea/bart_fid_sqse.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      766 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/sea/bart_sq_gen.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.528674 parlai-1.7.2/parlai/zoo/seeker/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8047 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/model_card.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      449 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/r2c2_base_3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      453 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/r2c2_base_400M.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      413 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/r2c2_blenderbot_3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      417 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/r2c2_blenderbot_400M.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      399 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/seeker_dialogue_3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      403 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/seeker_dialogue_400M.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      704 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/seeker_download.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      461 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/seeker_lm_dialogue_3B.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      438 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/seeker_lm_large.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      438 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/seeker_lm_med.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      429 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/seeker/seeker_lm_xl.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.536561 parlai-1.7.2/parlai/zoo/sensitive_topics_classifier/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/sensitive_topics_classifier/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      985 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/sensitive_topics_classifier/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.554311 parlai-1.7.2/parlai/zoo/style_gen/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/style_gen/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      811 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/style_gen/c75_labeled_dialogue_generator.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      778 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/style_gen/curr_only_classifier.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      782 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/style_gen/prev_curr_classifier.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.566804 parlai-1.7.2/parlai/zoo/tod/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/tod/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      873 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/tod/tod_base_no_api.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      892 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/tod/tod_base_yes_api.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.575350 parlai-1.7.2/parlai/zoo/tutorial_transformer_generator/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/tutorial_transformer_generator/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      923 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/tutorial_transformer_generator/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.584475 parlai-1.7.2/parlai/zoo/unittest/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/unittest/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      932 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/unittest/build.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.593262 parlai-1.7.2/parlai/zoo/wikipedia_full/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/wikipedia_full/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      545 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/wikipedia_full/tfidf_retriever.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.610833 parlai-1.7.2/parlai/zoo/wizard_of_wikipedia/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/wizard_of_wikipedia/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      527 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/wizard_of_wikipedia/end2end_generator.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      551 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/wizard_of_wikipedia/full_dialogue_retrieval_model.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      844 2023-06-06 17:44:25.000000 parlai-1.7.2/parlai/zoo/wizard_of_wikipedia/knowledge_retriever.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.130616 parlai-1.7.2/parlai.egg-info/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10832 2023-06-06 20:17:43.000000 parlai-1.7.2/parlai.egg-info/PKG-INFO
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    50983 2023-06-06 20:17:44.000000 parlai-1.7.2/parlai.egg-info/SOURCES.txt
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        1 2023-06-06 20:17:43.000000 parlai-1.7.2/parlai.egg-info/dependency_links.txt
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      108 2023-06-06 20:17:43.000000 parlai-1.7.2/parlai.egg-info/entry_points.txt
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      809 2023-06-06 20:17:43.000000 parlai-1.7.2/parlai.egg-info/requires.txt
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)       46 2023-06-06 20:17:43.000000 parlai-1.7.2/parlai.egg-info/top_level.txt
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.619893 parlai-1.7.2/projects/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11752 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      293 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.631837 parlai-1.7.2/projects/anti_scaling/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3973 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/anti_scaling/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/anti_scaling/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    42981 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/anti_scaling/distillation.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.640763 parlai-1.7.2/projects/anti_scaling/scripts/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/anti_scaling/scripts/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1553 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/anti_scaling/scripts/remove_projection_matrices.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.658146 parlai-1.7.2/projects/bb3/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13251 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.695813 parlai-1.7.2/projects/bb3/agents/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13678 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/agents/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/agents/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8141 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/agents/module.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    31935 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/agents/opt_api_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    36878 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/agents/opt_bb3_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    57947 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/agents/r2c2_bb3_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3874 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/agents/search_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    22847 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/agents/utils.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1490 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/constants.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    36060 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/prompts.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.754078 parlai-1.7.2/projects/bb3/tasks/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      251 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13725 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/module_level_tasks.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    69824 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/mutators.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3490 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/opt_decision_tasks.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11104 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/opt_dialogue_tasks.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7576 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/opt_knowledge_tasks.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1089 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/opt_memory_generation_tasks.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1113 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/opt_search_generation_tasks.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5685 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/r2c2_decision_tasks.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14232 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/r2c2_dialogue_tasks.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8149 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/r2c2_knowledge_tasks.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      882 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/r2c2_memory_generation_tasks.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1100 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/bb3/tasks/r2c2_search_generation_tasks.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.762810 parlai-1.7.2/projects/blenderbot2/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6518 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/blenderbot2/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/blenderbot2/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.784993 parlai-1.7.2/projects/blenderbot2/agents/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6842 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/blenderbot2/agents/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/blenderbot2/agents/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    34689 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/blenderbot2/agents/blenderbot2.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    35431 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/blenderbot2/agents/modules.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14214 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/blenderbot2/agents/sub_modules.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.798286 parlai-1.7.2/projects/dialogue_unlikelihood/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1776 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/dialogue_unlikelihood/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/dialogue_unlikelihood/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    20340 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/dialogue_unlikelihood/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.811769 parlai-1.7.2/projects/image_chat/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3855 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/image_chat/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      293 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/image_chat/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    16634 2023-06-06 17:44:25.000000 parlai-1.7.2/projects/image_chat/interactive.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.824483 parlai-1.7.2/projects/image_chat/transresnet_multimodal/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/image_chat/transresnet_multimodal/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    19412 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/image_chat/transresnet_multimodal/modules.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    15704 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/image_chat/transresnet_multimodal/transresnet_multimodal.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.837219 parlai-1.7.2/projects/multimodal_blenderbot/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2093 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/multimodal_blenderbot/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/multimodal_blenderbot/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      485 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/multimodal_blenderbot/agents.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.850545 parlai-1.7.2/projects/personality_captions/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4305 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/personality_captions/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      293 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/personality_captions/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14003 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/personality_captions/interactive.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.863968 parlai-1.7.2/projects/personality_captions/transresnet/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/personality_captions/transresnet/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    20165 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/personality_captions/transresnet/modules.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    18285 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/personality_captions/transresnet/transresnet.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.881983 parlai-1.7.2/projects/safety_bench/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3908 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.899421 parlai-1.7.2/projects/safety_bench/model_wrappers/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/model_wrappers/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1091 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/model_wrappers/example_wrapper.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3384 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/model_wrappers/gpt_wrappers.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4901 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/model_wrappers/parlai_model_zoo_wrappers.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6505 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/prepare_integration_tests.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7164 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/run_unit_tests.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.912529 parlai-1.7.2/projects/safety_bench/unit_tests/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/unit_tests/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6036 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/unit_tests/generate_offensive_language_test.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5765 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/unit_tests/response_to_offensive_language_test.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.934457 parlai-1.7.2/projects/safety_bench/utils/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/utils/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      527 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/utils/colors.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5121 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/utils/perspective_api.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7593 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/utils/safety_testing.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1439 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/safety_bench/utils/wrapper_loading.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.947221 parlai-1.7.2/projects/seeker/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13991 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.977098 parlai-1.7.2/projects/seeker/agents/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/agents/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10436 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/agents/gpt2_seeker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    20080 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/agents/gpt2_seeker_modules.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4657 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/agents/modular_agent.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    32807 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/agents/seeker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9945 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/agents/seeker_modules.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:50.986904 parlai-1.7.2/projects/seeker/scripts/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/scripts/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    12206 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/scripts/generate_lm_data.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.021197 parlai-1.7.2/projects/seeker/tasks/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/tasks/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5958 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/tasks/dialogue.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11924 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/tasks/knowledge.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    16717 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/tasks/lm.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    17745 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/tasks/mutators.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6334 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/tasks/search_decision.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1026 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/tasks/search_query.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8603 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/seeker/utils.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.043576 parlai-1.7.2/projects/style_gen/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1735 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/style_gen/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/style_gen/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8283 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/style_gen/classifier.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     8613 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/style_gen/modules.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1028 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/style_gen/style_gen.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.052615 parlai-1.7.2/projects/tod_simulator/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    10405 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.091362 parlai-1.7.2/projects/tod_simulator/scripts/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/scripts/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6399 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/scripts/cleanup_conversation.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1768 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/scripts/do_get_passing_only_on_dir.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7545 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/scripts/get_al_samples_for_gsgd.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     4417 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/scripts/get_api_data.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2438 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/scripts/get_interdistinct_on_conversations.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6078 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/scripts/get_passing_only.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     6565 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/scripts/get_quick_eval_stats.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    23195 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/scripts/tod_distributed_uber_script.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.096125 parlai-1.7.2/projects/tod_simulator/tod_world_configs/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/tod_world_configs/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.104972 parlai-1.7.2/projects/tod_simulator/world_metrics/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/world_metrics/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    14697 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/tod_simulator/world_metrics/extended_world_metrics.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.114979 parlai-1.7.2/projects/wizard_of_wikipedia/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     7260 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/README.md
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      293 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/__init__.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.132203 parlai-1.7.2/projects/wizard_of_wikipedia/generator/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/generator/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    11912 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/generator/agents.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5292 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/generator/modules.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1262 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/generator/train_end2end.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.141387 parlai-1.7.2/projects/wizard_of_wikipedia/knowledge_retriever/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/knowledge_retriever/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13411 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/knowledge_retriever/knowledge_retriever.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.155341 parlai-1.7.2/projects/wizard_of_wikipedia/scripts/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/scripts/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1742 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/scripts/eval_retrieval_model.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1091 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/scripts/interactive_retrieval_model.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.167920 parlai-1.7.2/projects/wizard_of_wikipedia/wizard_transformer_ranker/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      198 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/wizard_transformer_ranker/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     3200 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/wizard_transformer_ranker/wizard_dict.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5619 2023-06-06 17:44:26.000000 parlai-1.7.2/projects/wizard_of_wikipedia/wizard_transformer_ranker/wizard_transformer_ranker.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      190 2023-06-06 17:44:26.000000 parlai-1.7.2/pyproject.toml
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)       38 2023-06-06 20:17:51.207475 parlai-1.7.2/setup.cfg
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     1660 2023-06-06 18:50:59.000000 parlai-1.7.2/setup.py
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:45.070664 parlai-1.7.2/tests/
+drwxrwxr-x   0 komeili  (1185200755) komeili  (1185200755)        0 2023-06-06 20:17:51.198109 parlai-1.7.2/tests/tod/
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)      199 2023-06-06 17:44:27.000000 parlai-1.7.2/tests/tod/__init__.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)    13552 2023-06-06 17:44:27.000000 parlai-1.7.2/tests/tod/test_tod_agents_and_teachers.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     2430 2023-06-06 17:44:27.000000 parlai-1.7.2/tests/tod/test_tod_teacher_metrics.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9206 2023-06-06 17:44:27.000000 parlai-1.7.2/tests/tod/test_tod_world_and_script.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9485 2023-06-06 17:44:27.000000 parlai-1.7.2/tests/tod/test_tod_world_metrics.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     9839 2023-06-06 17:44:27.000000 parlai-1.7.2/tests/tod/test_tod_world_metrics_in_script.py
+-rw-rw-r--   0 komeili  (1185200755) komeili  (1185200755)     5227 2023-06-06 17:44:27.000000 parlai-1.7.2/tests/tod/test_tod_world_script_metrics.py
```

### Comparing `parlai-1.7.1/LICENSE` & `parlai-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/PKG-INFO` & `parlai-1.7.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: parlai
-Version: 1.7.1
+Version: 1.7.2
 Summary: Unified platform for dialogue research.
 Home-page: http://parl.ai/
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 -----------
 
 [ParlAI](http://parl.ai) (pronounced “par-lay”) is a python framework for
 sharing, training and testing dialogue models, from open-domain chitchat, to
@@ -44,40 +42,62 @@
 
 ## Interactive Tutorial
 
 For those who want to start with ParlAI now, you can try our [Colab Tutorial](https://colab.research.google.com/drive/1bRMvN0lGXaTF5fuTidgvlAl-Lb41F7AD#scrollTo=KtVz5dCUmFkN).
 
 ## Installing ParlAI
 
-ParlAI currently requires Python3.8+ and [Pytorch](https://pytorch.org) 1.6 or higher.
-Dependencies of the core modules are listed in [`requirements.txt`](https://github.com/facebookresearch/ParlAI/blob/main/requirements.txt). Some
-models included (in [`parlai/agents`](https://github.com/facebookresearch/ParlAI/tree/main/parlai/agents)) have additional requirements.
-We *strongly* recommend you install ParlAI in a [venv](https://docs.python.org/3/library/venv.html) or [conda](https://www.anaconda.com/) environment.
+### Operating System
 
-We do not support Windows at this time, but many users [report success on Windows using Python 3.8](https://github.com/facebookresearch/ParlAI/issues/3989) and issues with Python 3.9. We are happy to accept patches that improve Windows support.
+ParlAI should work as inteded under Linux or macOS. We do not support Windows at this time, but many users [report success on Windows using Python 3.8](https://github.com/facebookresearch/ParlAI/issues/3989) and issues with Python 3.9. We are happy to accept patches that improve Windows support.
 
-**Standard Installation**
+### Python Interpreter
+
+ParlAI currently requires Python3.8+.
+
+### Requirements
+
+ParlAI supports [Pytorch](https://pytorch.org) 1.6 or higher.
+All requirements of the core modules are listed in [`requirements.txt`](https://github.com/facebookresearch/ParlAI/blob/main/requirements.txt). However, some models included (in [`parlai/agents`](https://github.com/facebookresearch/ParlAI/tree/main/parlai/agents)) have additional requirements.
+
+## Virtual Environment
+
+We *strongly* recommend you install ParlAI in a virtual environment using [venv](https://docs.python.org/3/library/venv.html) or [conda](https://www.anaconda.com/).
+
+### End User Installation
 
 If you want to use ParlAI without modifications, you can install it with:
 
 ```bash
-pip install parlai
+cd /path/to/your/parlai-app
+python3.8 -m venv venv
+venv/bin/pip install --upgrade pip setuptools wheel
+venv/bin/pip install parlai
 ```
 
-**Development Installation**
+### Developer Installation
 
 Many users will want to modify some parts of ParlAI. To set up a development
 environment, run the following commands to clone the repository and install
 ParlAI:
 
 ```bash
 git clone https://github.com/facebookresearch/ParlAI.git ~/ParlAI
-cd ~/ParlAI; python setup.py develop
+cd ~/ParlAI
+python3.8 -m venv venv
+venv/bin/pip install --upgrade pip setuptools wheel
+venv/bin/python setup.py develop
 ```
 
+> **Note**
+> Sometimes the install from source maynot work due to dependencies (specially in PyTorch related packaged).
+> In that case try building a fresh conda environment and running the similar to the following:
+> `conda install pytorch==2.0.0 torchvision torchaudio torchtext pytorch-cuda=11.8 -c pytorch -c nvidia`.
+> Check torch setup documentation for your CUDA and OS versions.
+
 All needed data will be downloaded to `~/ParlAI/data`. If you need to clear out
 the space used by these files, you can safely delete these directories and any
 files needed will be downloaded again.
 
 ## Documentation
 
  - [Quick Start](https://parl.ai/docs/tutorial_quick.html)
@@ -163,9 +183,7 @@
   journal={arXiv preprint arXiv:{1705.06476}},
   year={2017}
 }
 ```
 
 ## License
 ParlAI is MIT licensed. See the **[LICENSE](https://github.com/facebookresearch/ParlAI/blob/main/LICENSE)** file for details.
-
-
```

### Comparing `parlai-1.7.1/README.md` & `parlai-1.7.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     <a href="https://img.shields.io/github/contributors/facebookresearch/ParlAI">
     <img src="https://img.shields.io/github/contributors/facebookresearch/ParlAI"/>
   </a>
     <a href="https://twitter.com/parlai_parley">
     <img src="https://img.shields.io/twitter/follow/parlai_parley?label=Twitter&style=social" alt="Twitter" />
   </a>
  </p>
- 
+
 -------------------------------------------------------------------------------------------------------------------------------------------------------
 
 [ParlAI](http://parl.ai) (pronounced “par-lay”) is a python framework for
 sharing, training and testing dialogue models, from open-domain chitchat, to
 task-oriented dialogue, to visual question answering.
 
 Its goal is to provide researchers:
@@ -54,40 +54,62 @@
 
 ## Interactive Tutorial
 
 For those who want to start with ParlAI now, you can try our [Colab Tutorial](https://colab.research.google.com/drive/1bRMvN0lGXaTF5fuTidgvlAl-Lb41F7AD#scrollTo=KtVz5dCUmFkN).
 
 ## Installing ParlAI
 
-ParlAI currently requires Python3.8+ and [Pytorch](https://pytorch.org) 1.6 or higher.
-Dependencies of the core modules are listed in [`requirements.txt`](https://github.com/facebookresearch/ParlAI/blob/main/requirements.txt). Some
-models included (in [`parlai/agents`](https://github.com/facebookresearch/ParlAI/tree/main/parlai/agents)) have additional requirements.
-We *strongly* recommend you install ParlAI in a [venv](https://docs.python.org/3/library/venv.html) or [conda](https://www.anaconda.com/) environment.
+### Operating System
+
+ParlAI should work as inteded under Linux or macOS. We do not support Windows at this time, but many users [report success on Windows using Python 3.8](https://github.com/facebookresearch/ParlAI/issues/3989) and issues with Python 3.9. We are happy to accept patches that improve Windows support.
+
+### Python Interpreter
+
+ParlAI currently requires Python3.8+.
 
-We do not support Windows at this time, but many users [report success on Windows using Python 3.8](https://github.com/facebookresearch/ParlAI/issues/3989) and issues with Python 3.9. We are happy to accept patches that improve Windows support.
+### Requirements
 
-**Standard Installation**
+ParlAI supports [Pytorch](https://pytorch.org) 1.6 or higher.
+All requirements of the core modules are listed in [`requirements.txt`](https://github.com/facebookresearch/ParlAI/blob/main/requirements.txt). However, some models included (in [`parlai/agents`](https://github.com/facebookresearch/ParlAI/tree/main/parlai/agents)) have additional requirements.
+
+## Virtual Environment
+
+We *strongly* recommend you install ParlAI in a virtual environment using [venv](https://docs.python.org/3/library/venv.html) or [conda](https://www.anaconda.com/).
+
+### End User Installation
 
 If you want to use ParlAI without modifications, you can install it with:
 
 ```bash
-pip install parlai
+cd /path/to/your/parlai-app
+python3.8 -m venv venv
+venv/bin/pip install --upgrade pip setuptools wheel
+venv/bin/pip install parlai
 ```
 
-**Development Installation**
+### Developer Installation
 
 Many users will want to modify some parts of ParlAI. To set up a development
 environment, run the following commands to clone the repository and install
 ParlAI:
 
 ```bash
 git clone https://github.com/facebookresearch/ParlAI.git ~/ParlAI
-cd ~/ParlAI; python setup.py develop
+cd ~/ParlAI
+python3.8 -m venv venv
+venv/bin/pip install --upgrade pip setuptools wheel
+venv/bin/python setup.py develop
 ```
 
+> **Note**
+> Sometimes the install from source maynot work due to dependencies (specially in PyTorch related packaged).
+> In that case try building a fresh conda environment and running the similar to the following:
+> `conda install pytorch==2.0.0 torchvision torchaudio torchtext pytorch-cuda=11.8 -c pytorch -c nvidia`.
+> Check torch setup documentation for your CUDA and OS versions.
+
 All needed data will be downloaded to `~/ParlAI/data`. If you need to clear out
 the space used by these files, you can safely delete these directories and any
 files needed will be downloaded again.
 
 ## Documentation
 
  - [Quick Start](https://parl.ai/docs/tutorial_quick.html)
```

#### html2text {}

```diff
@@ -40,34 +40,44 @@
 check out [NEWS.md](https://github.com/facebookresearch/ParlAI/blob/main/
 NEWS.md).
  [https://raw.githubusercontent.com/facebookresearch/ParlAI/main/docs/source/
                         _static/img/parlai_example.png]
 ## Interactive Tutorial For those who want to start with ParlAI now, you can
 try our [Colab Tutorial](https://colab.research.google.com/drive/
 1bRMvN0lGXaTF5fuTidgvlAl-Lb41F7AD#scrollTo=KtVz5dCUmFkN). ## Installing ParlAI
-ParlAI currently requires Python3.8+ and [Pytorch](https://pytorch.org) 1.6 or
-higher. Dependencies of the core modules are listed in [`requirements.txt`]
-(https://github.com/facebookresearch/ParlAI/blob/main/requirements.txt). Some
+### Operating System ParlAI should work as inteded under Linux or macOS. We do
+not support Windows at this time, but many users [report success on Windows
+using Python 3.8](https://github.com/facebookresearch/ParlAI/issues/3989) and
+issues with Python 3.9. We are happy to accept patches that improve Windows
+support. ### Python Interpreter ParlAI currently requires Python3.8+. ###
+Requirements ParlAI supports [Pytorch](https://pytorch.org) 1.6 or higher. All
+requirements of the core modules are listed in [`requirements.txt`](https://
+github.com/facebookresearch/ParlAI/blob/main/requirements.txt). However, some
 models included (in [`parlai/agents`](https://github.com/facebookresearch/
-ParlAI/tree/main/parlai/agents)) have additional requirements. We *strongly*
-recommend you install ParlAI in a [venv](https://docs.python.org/3/library/
-venv.html) or [conda](https://www.anaconda.com/) environment. We do not support
-Windows at this time, but many users [report success on Windows using Python
-3.8](https://github.com/facebookresearch/ParlAI/issues/3989) and issues with
-Python 3.9. We are happy to accept patches that improve Windows support.
-**Standard Installation** If you want to use ParlAI without modifications, you
-can install it with: ```bash pip install parlai ``` **Development
-Installation** Many users will want to modify some parts of ParlAI. To set up a
-development environment, run the following commands to clone the repository and
-install ParlAI: ```bash git clone https://github.com/facebookresearch/
-ParlAI.git ~/ParlAI cd ~/ParlAI; python setup.py develop ``` All needed data
-will be downloaded to `~/ParlAI/data`. If you need to clear out the space used
-by these files, you can safely delete these directories and any files needed
-will be downloaded again. ## Documentation - [Quick Start](https://parl.ai/
-docs/tutorial_quick.html) - [Basics: world, agents, teachers, action and
+ParlAI/tree/main/parlai/agents)) have additional requirements. ## Virtual
+Environment We *strongly* recommend you install ParlAI in a virtual environment
+using [venv](https://docs.python.org/3/library/venv.html) or [conda](https://
+www.anaconda.com/). ### End User Installation If you want to use ParlAI without
+modifications, you can install it with: ```bash cd /path/to/your/parlai-app
+python3.8 -m venv venv venv/bin/pip install --upgrade pip setuptools wheel
+venv/bin/pip install parlai ``` ### Developer Installation Many users will want
+to modify some parts of ParlAI. To set up a development environment, run the
+following commands to clone the repository and install ParlAI: ```bash git
+clone https://github.com/facebookresearch/ParlAI.git ~/ParlAI cd ~/ParlAI
+python3.8 -m venv venv venv/bin/pip install --upgrade pip setuptools wheel
+venv/bin/python setup.py develop ``` > **Note** > Sometimes the install from
+source maynot work due to dependencies (specially in PyTorch related packaged).
+> In that case try building a fresh conda environment and running the similar
+to the following: > `conda install pytorch==2.0.0 torchvision torchaudio
+torchtext pytorch-cuda=11.8 -c pytorch -c nvidia`. > Check torch setup
+documentation for your CUDA and OS versions. All needed data will be downloaded
+to `~/ParlAI/data`. If you need to clear out the space used by these files, you
+can safely delete these directories and any files needed will be downloaded
+again. ## Documentation - [Quick Start](https://parl.ai/docs/
+tutorial_quick.html) - [Basics: world, agents, teachers, action and
 observations](https://parl.ai/docs/tutorial_basic.html) - [Creating a new
 dataset/task](http://parl.ai/docs/tutorial_task.html) - [List of available
 tasks/datasets](https://parl.ai/docs/tasks.html) - [Creating a seq2seq agent]
 (https://parl.ai/docs/tutorial_torch_generator_agent.html) - [List of available
 agents](https://parl.ai/docs/agents_list.html) - [Model zoo (list pretrained
 models)](https://parl.ai/docs/zoo.html) - [Running crowdsourcing tasks](http://
 parl.ai/docs/tutorial_crowdsourcing.html) - [Plug into Facebook Messenger]
```

### Comparing `parlai-1.7.1/parlai/__main__.py` & `parlai-1.7.2/parlai/__main__.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/alice/alice.py` & `parlai-1.7.2/parlai/agents/alice/alice.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/bart/bart.py` & `parlai-1.7.2/parlai/agents/bart/bart.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/bart/convert_fairseq_to_parlai.py` & `parlai-1.7.2/parlai/agents/bart/convert_fairseq_to_parlai.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/bart/modules.py` & `parlai-1.7.2/parlai/agents/bart/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/bert_classifier/bert_classifier.py` & `parlai-1.7.2/parlai/agents/bert_classifier/bert_classifier.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/bert_ranker/bert_dictionary.py` & `parlai-1.7.2/parlai/agents/bert_ranker/bert_dictionary.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/bert_ranker/bert_ranker.py` & `parlai-1.7.2/parlai/agents/bert_ranker/bert_ranker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/bert_ranker/bi_encoder_ranker.py` & `parlai-1.7.2/parlai/agents/bert_ranker/bi_encoder_ranker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/bert_ranker/both_encoder_ranker.py` & `parlai-1.7.2/parlai/agents/bert_ranker/both_encoder_ranker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/bert_ranker/cross_encoder_ranker.py` & `parlai-1.7.2/parlai/agents/bert_ranker/cross_encoder_ranker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/bert_ranker/helpers.py` & `parlai-1.7.2/parlai/agents/bert_ranker/helpers.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/examples/seq2seq.py` & `parlai-1.7.2/parlai/agents/examples/seq2seq.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/examples/tra.py` & `parlai-1.7.2/parlai/agents/examples/tra.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/examples/transformer_variant.py` & `parlai-1.7.2/parlai/agents/examples/transformer_variant.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/fid/fid.py` & `parlai-1.7.2/parlai/agents/fid/fid.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/fixed_response/fixed_response.py` & `parlai-1.7.2/parlai/agents/fixed_response/fixed_response.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/hred/hred.py` & `parlai-1.7.2/parlai/agents/hred/hred.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/hred/modules.py` & `parlai-1.7.2/parlai/agents/hred/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/hugging_face/dialogpt.py` & `parlai-1.7.2/parlai/agents/hugging_face/dialogpt.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/hugging_face/dict.py` & `parlai-1.7.2/parlai/agents/hugging_face/dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,20 @@
     from transformers import GPT2Tokenizer, T5TokenizerFast
 except ImportError:
     raise ImportError(
         "Need to install Hugging Face transformers repository. "
         "Try `pip install transformers`."
     )
 
-SPECIAL_TOKENS = {"bos_token": "<bos>", "eos_token": "<eos>", "pad_token": "<pad>"}
+SPECIAL_TOKENS = {
+    "bos_token": "<bos>",
+    "eos_token": "<eos>",
+    "pad_token": "<pad>",
+    "unk_token": "<unk>",
+}
 
 NO_OP = "x"
 
 
 class HuggingFaceDictionaryAgent(DictionaryAgent, ABC):
     """
     Use Hugging Face tokenizers.
@@ -178,35 +183,40 @@
     def _define_special_tokens(self, opt):
         if opt["add_special_tokens"]:
             # Add additional start/end/pad tokens
             self.hf_tokenizer.add_special_tokens(SPECIAL_TOKENS)
             self.start_token = SPECIAL_TOKENS["bos_token"]
             self.end_token = SPECIAL_TOKENS["eos_token"]
             self.null_token = SPECIAL_TOKENS["pad_token"]
+            self.unk_token = SPECIAL_TOKENS["unk_token"]
         else:
             # Only special token is end of text
             self.start_token = NO_OP  # hack, we cut off the start token
             self.end_token = "<|endoftext|>"
             self.null_token = "<|endoftext|>"
+            self.unk_token = "<|endoftext|>"
 
     def override_special_tokens(self, opt):
         # define special tokens
         self._define_special_tokens(opt)
         # now override
         self.start_idx = self.hf_tokenizer.convert_tokens_to_ids([self.start_token])[0]
         self.end_idx = self.hf_tokenizer.convert_tokens_to_ids([self.end_token])[0]
         self.null_idx = self.hf_tokenizer.convert_tokens_to_ids([self.null_token])[0]
+        self.unk_idx = self.hf_tokenizer.convert_tokens_to_ids([self.unk_token])[0]
         # set tok2ind for special tokens
         self.tok2ind[self.end_token] = self.end_idx
         self.tok2ind[self.start_token] = self.start_idx
         self.tok2ind[self.null_token] = self.null_idx
+        self.tok2ind[self.unk_token] = self.unk_idx
         # set ind2tok for special tokens
         self.ind2tok[self.end_idx] = self.end_token
         self.ind2tok[self.start_idx] = self.start_token
         self.ind2tok[self.null_idx] = self.null_token
+        self.ind2tok[self.unk_idx] = self.unk_token
 
 
 class DialoGPTDictionaryAgent(Gpt2DictionaryAgent):
     def get_tokenizer(self, opt):
         """
         Instantiate tokenizer.
         """
```

### Comparing `parlai-1.7.1/parlai/agents/hugging_face/gpt2.py` & `parlai-1.7.2/parlai/agents/hugging_face/gpt2.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/hugging_face/hugging_face.py` & `parlai-1.7.2/parlai/agents/hugging_face/hugging_face.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/hugging_face/t5.py` & `parlai-1.7.2/parlai/agents/hugging_face/t5.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,31 +23,43 @@
 from parlai.agents.hugging_face.hugging_face import HF_VERSION
 from parlai.agents.hugging_face.dict import T5DictionaryAgent
 
 from parlai.core.opt import Opt
 from parlai.core.params import ParlaiParser
 from parlai.core.torch_agent import Batch, TorchAgent
 from parlai.core.torch_generator_agent import TorchGeneratorAgent, TorchGeneratorModel
-from parlai.utils.fsdp import is_fsdp
+from parlai.utils.fsdp import is_fsdp, delay_halving
 
 
 def check_hf_version(v: Tuple[int, int]) -> bool:
     """
     Check that HF version is greater than 4.3.
     """
     main, sub = v
     return main > 4 or (main == 4 and sub >= 3)
 
 
 def build_t5(opt: Opt) -> T5ForConditionalGeneration:
     if not check_hf_version(HF_VERSION):
         raise RuntimeError('Must use transformers package >= 4.3 to use t5')
-    return T5ForConditionalGeneration.from_pretrained(
-        opt['t5_model_arch'], dropout_rate=opt['t5_dropout']
+    torch_dtype = (
+        torch.float16 if (opt['fp16'] and not delay_halving(opt)) else torch.float32
     )
+    try:
+        return T5ForConditionalGeneration.from_pretrained(
+            opt['t5_model_arch'],
+            dropout_rate=opt['t5_dropout'],
+            torch_dtype=torch_dtype,
+        )
+    except TypeError:
+        # it's not clear when HF added the `torch_dtype` option, but it is not
+        # available in 4.3.3, which is the earliest we support.
+        return T5ForConditionalGeneration.from_pretrained(
+            opt['t5_model_arch'], dropout_rate=opt['t5_dropout']
+        )
 
 
 def set_device(func):
     """
     Decorator for setting device.
 
     HF's model parallel uses `torch.cuda.set_device`, which does not vibe well with
@@ -82,15 +94,26 @@
     ) -> ParlaiParser:
         super().add_cmdline_args(parser, partial_opt=partial_opt)
         group = parser.add_argument_group('T5 Args')
         group.add_argument(
             '--t5-model-arch',
             type=str,
             default='t5-base',
-            choices=["t5-small", "t5-base", "t5-large", "t5-3b", "t5-11b"],
+            choices=[
+                "t5-small",
+                "t5-base",
+                "t5-large",
+                "t5-3b",
+                "t5-11b",
+                "google/flan-t5-small",
+                "google/flan-t5-base",
+                "google/flan-t5-large",
+                "google/flan-t5-xl",
+                "google/flan-t5-xxl",
+            ],
         )
         group.add_argument(
             '--t5-model-parallel',
             type='bool',
             default=False,
             help='use HF model parallel',
         )
@@ -171,27 +194,27 @@
         method = self.opt.get('inference', 'greedy')
 
         generation_params = {
             'input_ids': batch.text_vec,
             'max_length': max_ts,
             'min_length': self.beam_min_length,
             'do_sample': self.opt['inference'] in ['topk', 'topp'],
-            'early_stopping': None,
+            'early_stopping': 'never',
             'num_beams': beam_size,
             'temperature': self.temperature,
             'top_k': self.opt['topk'] if method in ['topk', 'delayedbeam'] else None,
             'top_p': self.opt['topp'] if method == 'nucleus' else None,
             'repetition_penalty': None,
             'bad_words_ids': bad_words_ids if bad_words_ids else None,
             'bos_token_id': self.START_IDX,
             'pad_token_id': self.NULL_IDX,
             'eos_token_id': self.END_IDX,
             'length_penalty': self.opt['beam_length_penalty'],
             'no_repeat_ngram_size': self.beam_block_ngram,
-            'num_return_sequences': None,
+            'num_return_sequences': 1,
             'attention_mask': batch.text_vec != self.NULL_IDX,
             'decoder_start_token_id': self.NULL_IDX,
         }
 
         if self.opt['t5_generation_config']:
             config = TASK_CONFIGS[self.opt['t5_generation_config']]
             config.pop('prefix', None)
@@ -344,15 +367,15 @@
     @set_device
     def output(self, tensor):
         """
         Compute output logits.
         """
         # Taken directly from HuggingFace
         # Rescale output before projecting on vocab
-        # See https://github.com/tensorflow/mesh/blob/fa19d69eafc9a482aff0b59ddd96b025c0cb207d/mesh_tensorflow/transformer/transformer.py#L586
+        # See https://github.com/tensorflow/mesh/blob/fa19d69/mesh_tensorflow/transformer/transformer.py#L586
         tensor = tensor * (self.t5.model_dim**-0.5)
         lm_logits = self.t5.lm_head(tensor)
         return lm_logits
 
 
 ###########################################################################
 # Task-specific generation configs for T5.                                #
```

### Comparing `parlai-1.7.1/parlai/agents/image_seq2seq/image_seq2seq.py` & `parlai-1.7.2/parlai/agents/image_seq2seq/image_seq2seq.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/image_seq2seq/modules.py` & `parlai-1.7.2/parlai/agents/image_seq2seq/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/ir_baseline/ir_baseline.py` & `parlai-1.7.2/parlai/agents/ir_baseline/ir_baseline.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/local_human/local_human.py` & `parlai-1.7.2/parlai/agents/local_human/local_human.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/memnn/memnn.py` & `parlai-1.7.2/parlai/agents/memnn/memnn.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/memnn/modules.py` & `parlai-1.7.2/parlai/agents/memnn/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/args.py` & `parlai-1.7.2/parlai/agents/rag/args.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/conversion_utils.py` & `parlai-1.7.2/parlai/agents/rag/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/dpr.py` & `parlai-1.7.2/parlai/agents/rag/dpr.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/indexers.py` & `parlai-1.7.2/parlai/agents/rag/indexers.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/model_types.py` & `parlai-1.7.2/parlai/agents/rag/model_types.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/modules.py` & `parlai-1.7.2/parlai/agents/rag/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/polyfaiss.py` & `parlai-1.7.2/parlai/agents/rag/polyfaiss.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/rag.py` & `parlai-1.7.2/parlai/agents/rag/rag.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/retrieve_api.py` & `parlai-1.7.2/parlai/agents/rag/retrieve_api.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/retrievers.py` & `parlai-1.7.2/parlai/agents/rag/retrievers.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/scripts/generate_dense_embeddings.py` & `parlai-1.7.2/parlai/agents/rag/scripts/generate_dense_embeddings.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/rag/scripts/index_dense_embeddings.py` & `parlai-1.7.2/parlai/agents/rag/scripts/index_dense_embeddings.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/random_candidate/random_candidate.py` & `parlai-1.7.2/parlai/agents/random_candidate/random_candidate.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/repeat_label/repeat_label.py` & `parlai-1.7.2/parlai/agents/repeat_label/repeat_label.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/repeat_query/repeat_query.py` & `parlai-1.7.2/parlai/agents/repeat_query/repeat_query.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/reranker/classifier_gpt2_reranker.py` & `parlai-1.7.2/parlai/agents/reranker/classifier_gpt2_reranker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/reranker/classifier_reranker.py` & `parlai-1.7.2/parlai/agents/reranker/classifier_reranker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/reranker/reranker.py` & `parlai-1.7.2/parlai/agents/reranker/reranker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/retriever_reader/retriever_reader.py` & `parlai-1.7.2/parlai/agents/retriever_reader/retriever_reader.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/safe_local_human/safe_local_human.py` & `parlai-1.7.2/parlai/agents/safe_local_human/safe_local_human.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/seq2seq/modules.py` & `parlai-1.7.2/parlai/agents/seq2seq/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/seq2seq/seq2seq.py` & `parlai-1.7.2/parlai/agents/seq2seq/seq2seq.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/starspace/modules.py` & `parlai-1.7.2/parlai/agents/starspace/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,24 @@
     def __init__(self, opt, num_features, dict):
         super().__init__()
         self.lt = nn.Embedding(
             num_features,
             opt['embeddingsize'],
             0,
             sparse=True,
-            max_norm=opt['embeddingnorm'],
         )
         if not opt['tfidf']:
             dict = None
         self.encoder = Encoder(self.lt, dict)
         if not opt['share_embeddings']:
             self.lt2 = nn.Embedding(
                 num_features,
                 opt['embeddingsize'],
                 0,
                 sparse=True,
-                max_norm=opt['embeddingnorm'],
             )
             self.encoder2 = Encoder(self.lt2, dict)
         else:
             self.encoder2 = self.encoder
         self.opt = opt
         self.lin = nn.Linear(opt['embeddingsize'], opt['embeddingsize'], bias=False)
         self.lins = 0
```

### Comparing `parlai-1.7.1/parlai/agents/starspace/starspace.py` & `parlai-1.7.2/parlai/agents/starspace/starspace.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/test_agents/counter.py` & `parlai-1.7.2/parlai/agents/test_agents/counter.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/test_agents/null.py` & `parlai-1.7.2/parlai/agents/test_agents/null.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/test_agents/test_agents.py` & `parlai-1.7.2/parlai/agents/test_agents/test_agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/test_agents/transformer_generator_prefix.py` & `parlai-1.7.2/parlai/agents/test_agents/transformer_generator_prefix.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/test_agents/unigram.py` & `parlai-1.7.2/parlai/agents/test_agents/unigram.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/tfidf_retriever/build_tfidf.py` & `parlai-1.7.2/parlai/agents/tfidf_retriever/build_tfidf.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/tfidf_retriever/doc_db.py` & `parlai-1.7.2/parlai/agents/tfidf_retriever/doc_db.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/tfidf_retriever/tfidf_doc_ranker.py` & `parlai-1.7.2/parlai/agents/tfidf_retriever/tfidf_doc_ranker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/tfidf_retriever/tfidf_retriever.py` & `parlai-1.7.2/parlai/agents/tfidf_retriever/tfidf_retriever.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/__init__.py` & `parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/regexp_tokenizer.py` & `parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/regexp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/simple_tokenizer.py` & `parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/spacy_tokenizer.py` & `parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/tfidf_retriever/tokenizers/tokenizer.py` & `parlai-1.7.2/parlai/agents/tfidf_retriever/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/tfidf_retriever/utils.py` & `parlai-1.7.2/parlai/agents/tfidf_retriever/utils.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/biencoder.py` & `parlai-1.7.2/parlai/agents/transformer/biencoder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/crossencoder.py` & `parlai-1.7.2/parlai/agents/transformer/crossencoder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/decoder.py` & `parlai-1.7.2/parlai/agents/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/dropout_poly.py` & `parlai-1.7.2/parlai/agents/transformer/dropout_poly.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/image_polyencoder.py` & `parlai-1.7.2/parlai/agents/transformer/image_polyencoder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/modules/__init__.py` & `parlai-1.7.2/parlai/agents/transformer/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/modules/attention.py` & `parlai-1.7.2/parlai/agents/transformer/modules/attention.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/modules/decoder.py` & `parlai-1.7.2/parlai/agents/transformer/modules/decoder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/modules/encoder.py` & `parlai-1.7.2/parlai/agents/transformer/modules/encoder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/modules/ffn.py` & `parlai-1.7.2/parlai/agents/transformer/modules/ffn.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/modules/functions.py` & `parlai-1.7.2/parlai/agents/transformer/modules/functions.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/modules/generator.py` & `parlai-1.7.2/parlai/agents/transformer/modules/generator.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/modules/mem_net.py` & `parlai-1.7.2/parlai/agents/transformer/modules/mem_net.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/modules/modular.py` & `parlai-1.7.2/parlai/agents/transformer/modules/modular.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/modules/wrappers.py` & `parlai-1.7.2/parlai/agents/transformer/modules/wrappers.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/polyencoder.py` & `parlai-1.7.2/parlai/agents/transformer/polyencoder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/transformer/transformer.py` & `parlai-1.7.2/parlai/agents/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/agents/unigram/unigram.py` & `parlai-1.7.2/parlai/agents/unigram/unigram.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/core/agents.py` & `parlai-1.7.2/parlai/chat_service/core/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/core/chat_service_manager.py` & `parlai-1.7.2/parlai/chat_service/core/chat_service_manager.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/core/socket.py` & `parlai-1.7.2/parlai/chat_service/core/socket.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/core/world_runner.py` & `parlai-1.7.2/parlai/chat_service/core/world_runner.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/browser_chat/client.py` & `parlai-1.7.2/parlai/chat_service/services/browser_chat/client.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/browser_chat/run.py` & `parlai-1.7.2/parlai/chat_service/services/browser_chat/run.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/messenger/agents.py` & `parlai-1.7.2/parlai/chat_service/services/messenger/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/messenger/message_sender.py` & `parlai-1.7.2/parlai/chat_service/services/messenger/message_sender.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/messenger/messenger_manager.py` & `parlai-1.7.2/parlai/chat_service/services/messenger/messenger_manager.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/messenger/run.py` & `parlai-1.7.2/parlai/chat_service/services/messenger/run.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/messenger/worlds.py` & `parlai-1.7.2/parlai/chat_service/services/messenger/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/terminal_chat/client.py` & `parlai-1.7.2/parlai/chat_service/services/terminal_chat/client.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/terminal_chat/run.py` & `parlai-1.7.2/parlai/chat_service/services/terminal_chat/run.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/websocket/agents.py` & `parlai-1.7.2/parlai/chat_service/services/websocket/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/websocket/run.py` & `parlai-1.7.2/parlai/chat_service/services/websocket/run.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/websocket/sockets.py` & `parlai-1.7.2/parlai/chat_service/services/websocket/sockets.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/services/websocket/websocket_manager.py` & `parlai-1.7.2/parlai/chat_service/services/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/tasks/chatbot/worlds.py` & `parlai-1.7.2/parlai/chat_service/tasks/chatbot/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/tasks/overworld_demo/worlds.py` & `parlai-1.7.2/parlai/chat_service/tasks/overworld_demo/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/tasks/qa_data_collection/worlds.py` & `parlai-1.7.2/parlai/chat_service/tasks/qa_data_collection/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/utils/config.py` & `parlai-1.7.2/parlai/chat_service/utils/config.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/utils/image.py` & `parlai-1.7.2/parlai/chat_service/utils/image.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/utils/logging.py` & `parlai-1.7.2/parlai/chat_service/utils/logging.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/utils/misc.py` & `parlai-1.7.2/parlai/chat_service/utils/misc.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/utils/server.py` & `parlai-1.7.2/parlai/chat_service/utils/server.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/chat_service/utils/timeout.py` & `parlai-1.7.2/parlai/chat_service/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/agents.py` & `parlai-1.7.2/parlai/core/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/build_data.py` & `parlai-1.7.2/parlai/core/build_data.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/dict.py` & `parlai-1.7.2/parlai/core/dict.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/image_featurizers.py` & `parlai-1.7.2/parlai/core/image_featurizers.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/loader.py` & `parlai-1.7.2/parlai/core/loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 Functions for loading modules for agents, tasks and teachers, worlds, and scripts.
 
 These functions are largely for converting strings specified in opts (like for --task)
 to the appropriate module.
 """
 
-from typing import Callable, Dict, Type
+from typing import Callable, Dict, Type, Tuple
 import importlib
 
 from collections import namedtuple
 
 script_registration = namedtuple('script_registration', ('klass', 'hidden', 'aliases'))
 
 
@@ -78,14 +78,56 @@
         TEACHER_REGISTRY[name] = cls_
         return cls_
 
     return _inner
 
 
 ##############################################################
+### PATH RESOLVER
+##############################################################
+# For use to register related packages. Keys entered below
+# will have a mapping from the repo key (such as 'internal:')
+# to info about that related package: the module root (to where
+# tasks, agents, and projects are contained), and the source.
+REGISTERED_REPOS = {
+    # To switch to local repo, useful for non-public projects
+    # (make a directory called 'parlai_internal' with your private agents)
+    # this will follow the same paths but look in parlai_internal instead
+    'internal:': {
+        'repo': 'parlai_internal',
+        'source': 'Check internal ParlAI documentation for access',
+    },
+    'fb:': {
+        'repo': 'parlai_fb',
+        'source': 'Check internal ParlAI documentation for access',
+    },
+    'light:': {
+        'repo': 'light.modeling',
+        'source': 'https://github.com/facebookresearch/LIGHT',
+    },
+    # Do you have a repo with ParlAI tasks? Add it below!
+}
+
+
+def assert_get_source_repo(asset_path: str) -> Tuple[str, str]:
+    for key, repo_info in REGISTERED_REPOS.items():
+        if asset_path.startswith(key):
+            repo = repo_info['repo']
+            try:
+                importlib.import_module(repo)
+            except ImportError:
+                source = repo_info['source']
+                raise Exception(
+                    f"Error importing library for {key}, try to install from source: {source}"
+                )
+            return repo, asset_path[len(key) :]
+    return 'parlai', asset_path
+
+
+##############################################################
 ### AGENT LOADER
 ##############################################################
 def _name_to_agent_class(name: str):
     """
     Convert agent name to class.
 
     This adds "Agent" to the end of the name and uppercases the first letter
@@ -135,24 +177,15 @@
     :return:
         module of agent
     """
     global AGENT_REGISTRY
     if agent_path in AGENT_REGISTRY:
         return AGENT_REGISTRY[agent_path]
 
-    repo = 'parlai'
-    if agent_path.startswith('internal:'):
-        # To switch to local repo, useful for non-public projects
-        # (make a directory called 'parlai_internal' with your private agents)
-        # this will follow the same paths but look in parlai_internal instead
-        repo = 'parlai_internal'
-        agent_path = agent_path[9:]
-    elif agent_path.startswith('fb:'):
-        repo = 'parlai_fb'
-        agent_path = agent_path[3:]
+    repo, agent_path = assert_get_source_repo(agent_path)
 
     if agent_path.startswith('projects:'):
         # e.g. -m projects:personachat:kvmemnn
         path_list = agent_path.split(':')
         if len(path_list) != 3:
             raise RuntimeError(
                 'projects paths should follow pattern '
@@ -198,24 +231,16 @@
     """
     Returns the task path list and repository containing the task as specified by
     `--task`.
 
     :param taskname: path to task class (specified in format detailed below)
     """
     task = taskname.strip()
-    repo = 'parlai'
-    if task.startswith('internal:'):
-        # To switch to local repo, useful for non-public projects
-        # (make a directory called 'parlai_internal' with your private agents)
-        repo = 'parlai_internal'
-        task = task[9:]
-    elif task.startswith('fb:'):
-        repo = 'parlai_fb'
-        task = task[3:]
 
+    repo, task = assert_get_source_repo(task)
     task_path_list = task.split(':')
 
     return task_path_list, repo
 
 
 def load_task_module(taskname: str):
     """
```

### Comparing `parlai-1.7.1/parlai/core/logs.py` & `parlai-1.7.2/parlai/scripts/eval_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,278 +1,318 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Facebook, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-"""
-Log metrics to tensorboard.
 
-This file provides interface to log any metrics in tensorboard, could be
-extended to any other tool like visdom.
+"""
+Basic example which iterates through the tasks specified and evaluates the given model
+on them.
 
-.. code-block: none
+## Examples
 
-   tensorboard --logdir <PARLAI_DATA/tensorboard> --port 8888.
+```shell
+parlai eval_model --task "babi:Task1k:2" -m "repeat_label"
+parlai eval_model --task convai2 --model-file "/path/to/model_file"
+```
 """
 
-import datetime
-import json
-import numbers
-import os
-import pathlib
-import re
-from typing import Optional
-
-import parlai.utils.logging as logging
-from parlai.core.metrics import Metric, dict_report, get_metric_display_data
+from parlai.core.params import ParlaiParser, print_announcements
+from parlai.core.agents import create_agent
+from parlai.core.logs import TensorboardLogger
+from parlai.core.metrics import (
+    aggregate_named_reports,
+    aggregate_unnamed_reports,
+    Metric,
+)
 from parlai.core.opt import Opt
-from parlai.core.params import ParlaiParser
+from parlai.core.worlds import create_task
+from parlai.utils.misc import TimeLogger, nice_report
+from parlai.utils.world_logging import WorldLogger
+from parlai.core.script import ParlaiScript, register_script
 from parlai.utils.io import PathManager
+import parlai.utils.logging as logging
 
-_TB_SUMMARY_INVALID_TAG_CHARACTERS = re.compile(r'[^-/\w\.]')
-
-
-class TensorboardLogger(object):
-    """
-    Log objects to tensorboard.
-    """
+import json
+import os
+import random
 
-    @classmethod
-    def add_cmdline_args(
-        cls, parser: ParlaiParser, partial_opt: Optional[Opt] = None
-    ) -> ParlaiParser:
-        """
-        Add tensorboard CLI args.
-        """
-        logger = parser.add_argument_group('Tensorboard Arguments')
-        logger.add_argument(
-            '-tblog',
-            '--tensorboard-log',
-            type='bool',
-            default=False,
-            help="Tensorboard logging of metrics",
-            hidden=False,
-        )
-        logger.add_argument(
-            '-tblogdir',
-            '--tensorboard-logdir',
-            type=str,
-            default=None,
-            help="Tensorboard logging directory, defaults to model_file.tensorboard",
-            hidden=False,
+from parlai.utils.distributed import (
+    is_primary_worker,
+    all_gather_list,
+    is_distributed,
+    get_rank,
+)
+
+# the index to access classifier agent's output in the world
+CLASSIFIER_AGENT = 1
+
+
+def setup_args(parser=None):
+    if parser is None:
+        parser = ParlaiParser(True, True, 'Evaluate a model')
+    # Get command line arguments
+    parser.add_argument(
+        '-rf',
+        '--report-filename',
+        type=str,
+        default='',
+        help='Saves a json file of the evaluation report either as an '
+        'extension to the model-file (if begins with a ".") or a whole '
+        'file path. Set to the empty string to not save at all.',
+    )
+    parser.add_argument(
+        '--world-logs',
+        type=str,
+        default='',
+        help='Saves a jsonl file of the world logs.'
+        'Set to the empty string to not save at all.',
+    )
+    parser.add_argument(
+        '--save-format',
+        type=str,
+        default='conversations',
+        choices=['conversations', 'parlai'],
+    )
+    parser.add_argument(
+        '--area-under-curve-digits',
+        '-auc',
+        type=int,
+        default=-1,
+        help='a positive number indicates to calculate the area under the '
+        'roc curve and it also determines how many decimal digits of the '
+        'predictions to keep (higher numbers->more precise); also used '
+        'to determine whether or not to calculate the AUC metric',
+    )
+    parser.add_argument(
+        '--area-under-curve-class',
+        '-auclass',
+        type=str,
+        default=None,
+        nargs='*',
+        help='the name(s) of the class to calculate the auc for',
+    )
+    parser.add_argument('-ne', '--num-examples', type=int, default=-1)
+    parser.add_argument('-d', '--display-examples', type='bool', default=False)
+    parser.add_argument('-ltim', '--log-every-n-secs', type=float, default=10)
+    parser.add_argument(
+        '-mcs',
+        '--metrics',
+        type=str,
+        default='default',
+        help='list of metrics to show/compute, e.g. all, default,'
+        'or give a list split by , like '
+        'ppl,f1,accuracy,hits@1,rouge,bleu'
+        'the rouge metrics will be computed as rouge-1, rouge-2 and rouge-l',
+    )
+    parser.add_argument(
+        '-micro',
+        '--aggregate-micro',
+        type='bool',
+        default=False,
+        help='Report micro-averaged metrics instead of macro averaged metrics.',
+        recommended=False,
+    )
+    WorldLogger.add_cmdline_args(parser, partial_opt=None)
+    TensorboardLogger.add_cmdline_args(parser, partial_opt=None)
+    parser.set_params(datatype='valid')
+    return parser
+
+
+def _save_eval_stats(opt, report):
+    if not is_primary_worker:
+        return
+    report_fname = opt['report_filename']
+    if report_fname == '':
+        return
+    if report_fname.startswith('.'):
+        report_fname = opt['model_file'] + report_fname
+
+    json_serializable_report = report
+    for k, v in report.items():
+        if isinstance(v, Metric):
+            v = v.value()
+        json_serializable_report[k] = v
+
+    # Save report
+    with PathManager.open(report_fname, 'w') as f:
+        logging.info(f'Saving model report to {report_fname}')
+        json.dump({'opt': opt, 'report': json_serializable_report}, f, indent=4)
+        f.write("\n")  # for jq
+
+
+def get_task_world_logs(task, world_logs, is_multitask=False):
+    if not is_multitask:
+        return world_logs
+    else:
+        base_outfile, extension = os.path.splitext(world_logs)
+        return f'{base_outfile}_{task}{extension}'
+
+
+def prepare_tb_logger(opt):
+    if opt['tensorboard_log'] and is_primary_worker():
+        tb_logger = TensorboardLogger(opt)
+    else:
+        tb_logger = None
+
+    if 'train' in opt['datatype']:
+        setting = 'train'
+    elif 'valid' in opt['datatype']:
+        setting = 'valid'
+    else:
+        setting = 'test'
+    return tb_logger, setting
+
+
+def get_n_parleys(opt):
+    trainstats_suffix = '.trainstats'
+    if opt.get('model_file') and PathManager.exists(
+        opt['model_file'] + trainstats_suffix
+    ):
+        with PathManager.open(opt['model_file'] + trainstats_suffix) as ts:
+            obj = json.load(ts)
+            parleys = obj.get('parleys', 0)
+    else:
+        parleys = 0
+    return parleys
+
+
+def _eval_single_world(opt, agent, task):
+    logging.info(f'Evaluating task {task} using datatype {opt.get("datatype")}.')
+    # set up world logger
+    task_opt = opt.copy()  # copy opt since we're editing the task
+    task_opt['task'] = task
+    # add task suffix in case of multi-tasking
+    if opt['world_logs']:
+        task_opt['world_logs'] = get_task_world_logs(
+            task, task_opt['world_logs'], is_multitask=len(opt['task'].split(',')) > 1
         )
-        return parser
 
-    def __init__(self, opt: Opt):
-        try:
-            # tensorboard is a very expensive thing to import. Wait until the
-            # last second to import it.
-            from tensorboardX import SummaryWriter
-        except ImportError:
-            raise ImportError('Please run `pip install tensorboard tensorboardX`.')
+    world_logger = WorldLogger(task_opt) if task_opt['world_logs'] else None
+
+    world = create_task(task_opt, agent)  # create worlds for tasks
 
-        if opt['tensorboard_logdir'] is not None:
-            tbpath = opt['tensorboard_logdir']
+    # set up logging
+    log_every_n_secs = opt.get('log_every_n_secs', -1)
+    if log_every_n_secs <= 0:
+        log_every_n_secs = float('inf')
+    log_time = TimeLogger()
+
+    # max number of examples to evaluate
+    max_cnt = opt['num_examples'] if opt['num_examples'] > 0 else float('inf')
+    cnt = 0
+    total_cnt = world.num_examples()
+
+    if is_distributed():
+        logging.warning('Progress bar is approximate in distributed mode.')
+
+    while not world.epoch_done() and cnt < max_cnt:
+        cnt += opt.get('batchsize', 1)
+        world.parley()
+        if world_logger is not None:
+            world_logger.log(world)
+        if opt['display_examples']:
+            # display examples
+            print(world.display() + '\n~~')
+        if log_time.time() > log_every_n_secs:
+            report = world.report()
+            text, report = log_time.log(
+                report.get('exs', 0), min(max_cnt, total_cnt), report
+            )
+            logging.info(text)
+
+    if world_logger is not None:
+        # dump world acts to file
+        world_logger.reset()  # add final acts to logs
+        if is_distributed():
+            rank = get_rank()
+            base_outfile, extension = os.path.splitext(task_opt['world_logs'])
+            outfile = base_outfile + f'_{rank}' + extension
         else:
-            tbpath = opt['model_file'] + '.tensorboard'
+            outfile = task_opt['world_logs']
+        world_logger.write(outfile, world, file_format=opt['save_format'])
 
-        logging.debug(f'Saving tensorboard logs to: {tbpath}')
-        if not PathManager.exists(tbpath):
-            PathManager.mkdirs(tbpath)
-        self.writer = SummaryWriter(tbpath, comment=json.dumps(opt))
-
-    def log_metrics(self, setting, step, report):
-        """
-        Log all metrics to tensorboard.
-
-        :param setting:
-            One of train/valid/test. Will be used as the title for the graph.
-        :param step:
-            Number of parleys
-        :param report:
-            The report to log
-        """
-        for k, v in report.items():
-            v = v.value() if isinstance(v, Metric) else v
-            if not isinstance(v, numbers.Number):
-                logging.error(f'k {k} v {v} is not a number')
-                continue
-            display = get_metric_display_data(metric=k)
-            # Remove invalid characters for TensborboardX Summary beforehand
-            # so that the logs aren't cluttered with warnings.
-            tag = _TB_SUMMARY_INVALID_TAG_CHARACTERS.sub('_', f'{k}/{setting}')
-            try:
-                self.writer.add_scalar(
-                    tag,
-                    v,
-                    global_step=step,
-                    display_name=f"{display.title}",
-                    summary_description=display.description,
-                )
-            except TypeError:
-                # internal tensorboard doesn't support custom display titles etc
-                self.writer.add_scalar(tag, v, global_step=step)
+    report = aggregate_unnamed_reports(all_gather_list(world.report()))
 
-    def flush(self):
-        self.writer.flush()
+    if isinstance(world.agents, list) and len(world.agents) > 1:
+        classifier_agent = world.agents[CLASSIFIER_AGENT]
+        if hasattr(classifier_agent, 'calc_auc') and classifier_agent.calc_auc:
+            for class_indices, curr_auc in zip(
+                classifier_agent.auc_class_indices, classifier_agent.aucs
+            ):
+                report[f'AUC_{classifier_agent.class_list[class_indices]}'] = curr_auc
+            classifier_agent.reset_auc()
+            # for safety measures
+            agent.reset_auc()
+    world.reset()
+    return report
 
 
-class WandbLogger(object):
-    """
-    Log objects to Weights and Biases.
+def eval_model(opt):
     """
+    Evaluates a model.
 
-    @classmethod
-    def add_cmdline_args(
-        cls, parser: ParlaiParser, partial_opt: Optional[Opt] = None
-    ) -> ParlaiParser:
-        """
-        Add WandB CLI args.
-        """
-        logger = parser.add_argument_group('WandB Arguments')
-        logger.add_argument(
-            '-wblog',
-            '--wandb-log',
-            type='bool',
-            default=False,
-            help="Enable W&B logging of metrics",
-        )
-        logger.add_argument(
-            '--wandb-name',
-            type=str,
-            default=None,
-            help='W&B run name. If not set, WandB will randomly generate a name.',
-            hidden=True,
+    :param opt: tells the evaluation function how to run
+    :return: the final result of calling report()
+    """
+    random.seed(42)
+    if 'train' in opt['datatype'] and 'evalmode' not in opt['datatype']:
+        raise ValueError(
+            'You should use --datatype train:evalmode if you want to evaluate on '
+            'the training set.'
         )
 
-        logger.add_argument(
-            '--wandb-project',
-            type=str,
-            default=None,
-            help='W&B project name. Defaults to timestamp. Usually the name of the sweep.',
-            hidden=False,
-        )
-        logger.add_argument(
-            '--wandb-entity',
-            type=str,
-            default=None,
-            help='W&B entity name.',
-            hidden=False,
-        )
+    # load model and possibly print opt
+    agent = create_agent(opt, requireModelExists=True)
+    agent.opt.log()
+
+    tb_logger, setting = prepare_tb_logger(opt)
+
+    if tb_logger:
+        n_parleys = get_n_parleys(opt)
+
+    tasks = opt['task'].split(',')
+    reports = []
+    for task in tasks:
+        task_report = _eval_single_world(opt, agent, task)
+        reports.append(task_report)
+        logging.report(f"Report for {task}:\n{nice_report(task_report)}")
+
+    report = aggregate_named_reports(
+        dict(zip(tasks, reports)), micro_average=opt.get('aggregate_micro', False)
+    )
+
+    # print announcements and report
+    print_announcements(opt)
+    logging.info(
+        f'Finished evaluating tasks {tasks} using datatype {opt.get("datatype")}'
+    )
+
+    print(nice_report(report))
+    _save_eval_stats(opt, report)
+    if tb_logger:
+        tb_logger.log_metrics(setting, n_parleys, report)
+        tb_logger.flush()
+    return report
 
-        logger.add_argument(
-            '--wandb-log-model',
-            type=bool,
-            default=False,
-            help='Enable logging of model artifacts to weight and biases',
-            hidden=False,
-        )
-        return logger
 
-    def __init__(self, opt: Opt, model=None):
-        try:
-            # wand is a very expensive thing to import. Wait until the
-            # last second to import it.
-            import wandb
-
-        except ImportError:
-            raise ImportError('Please run `pip install wandb`.')
-
-        name = opt.get('wandb_name')
-        project = opt.get('wandb_project') or datetime.datetime.now().strftime(
-            '%Y-%m-%d-%H-%M'
-        )
+class Evaluator:
+    def __init__(self, opt: Opt):
+        self.opt = opt
 
-        self.run = wandb.init(
-            name=name,
-            project=project,
-            dir=os.path.dirname(opt['model_file']),
-            notes=f"{opt['model_file']}",
-            entity=opt.get('wandb_entity'),
-            reinit=True,  # in case of preemption
-            resume=True,  # requeued runs should be treated as single run
-        )
-        # suppress wandb's output
-        logging.getLogger("wandb").setLevel(logging.ERROR)
+    def eval_model(self):
+        return eval_model(self.opt)
+
+
+@register_script('eval_model', aliases=['em', 'eval'])
+class EvalModel(ParlaiScript):
+    @classmethod
+    def setup_args(cls):
+        return setup_args()
 
-        if not self.run.resumed:
-            task_arg = opt.get("task", None)
-            if task_arg:
-                if (
-                    len(task_arg.split(",")) == 1
-                ):  # It gets confusing to parse these args for multitask teachers, so don't.
-                    maybe_task_opts = task_arg.split(":")
-                    for task_opt in maybe_task_opts:
-                        if len(task_opt.split("=")) == 2:
-                            k, v = task_opt.split("=")
-                            setattr(self.run.config, k, v)
-
-            for key, value in opt.items():
-                if key not in self.run.config:  # set by task logic
-                    if value is None or isinstance(value, (str, numbers.Number, tuple)):
-                        setattr(self.run.config, key, value)
-
-        self.model_file = opt.get('model_file', None)
-        if model is not None:
-            self.run.watch(model)
-
-    def log_metrics(self, setting, step, report):
-        """
-        Log all metrics to W&B.
-
-        :param setting:
-            One of train/valid/test. Will be used as the title for the graph.
-        :param step:
-            Number of parleys
-        :param report:
-            The report to log
-        """
-        report = dict_report(report)
-        report = {
-            f'{k}/{setting}': v
-            for k, v in report.items()
-            if isinstance(v, numbers.Number)
-        }
-        report['custom_step'] = step
-        self.run.log(report)
-
-    def log_final(self, setting, report):
-        report = dict_report(report)
-        report = {
-            f'{k}/{setting}': v
-            for k, v in report.items()
-            if isinstance(v, numbers.Number)
-        }
-        for key, value in report.items():
-            self.run.summary[key] = value
-
-    def log_model(self, model_file=None):
-        if self.model_file is not None:
-            if not model_file:
-                model_file = self.model_file
-            model_file = pathlib.Path(model_file)
-            if model_file.exists():
-                self.run.log_artifact(
-                    str(model_file),
-                    name=f"{self.run.name}-{model_file.name}",
-                    type="model",
-                )
-            vocab_file = model_file.with_suffix('.dict')
-            if vocab_file.exists():
-                self.run.log_artifact(
-                    str(vocab_file),
-                    name=f"{self.run.name}-{vocab_file.name}",
-                    type="vocab",
-                )
-            stats_file = model_file.with_suffix('.trainstats')
-            if stats_file.exists():
-                self.run.log_artifact(
-                    str(stats_file),
-                    name=f"{self.run.name}-{stats_file.name}",
-                    type="stats",
-                )
+    def run(self):
+        self.evaluator = Evaluator(self.opt)
+        return self.evaluator.eval_model()
 
-    def finish(self):
-        self.run.finish()
 
-    def flush(self):
-        pass
+if __name__ == '__main__':
+    EvalModel.main()
```

### Comparing `parlai-1.7.1/parlai/core/message.py` & `parlai-1.7.2/parlai/core/message.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/metrics.py` & `parlai-1.7.2/parlai/core/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Counter as TCounter,
     Dict,
     List,
     NamedTuple,
     Optional,
     Set,
     Tuple,
+    Type,
     Union,
 )
 
 import torch
 
 from parlai.core.message import Message
 from parlai.utils.misc import warn_once
@@ -268,28 +269,48 @@
         return int(cls.as_number(obj))
 
     @classmethod
     def many(cls, *objs: List[TVector]) -> List[Metric]:
         """
         Construct many of a Metric from the base parts.
 
-        Useful if you separately compute numerators and denomenators, etc.
+        Useful if you separately compute numerators and denominators, etc.
         """
         lengths = [len(o) for o in objs]
         objs = list(objs)  # convert from tuple for inplace modification
         for i, o in enumerate(objs):
             if isinstance(o, torch.Tensor):
                 # if the tensor is on GPU, make sure we transfer the whole thing
                 # at once, instead of one-element-at-a-time during our list
                 # comprehension
                 objs[i] = o.tolist()
         if len(set(lengths)) != 1:
             raise IndexError(f'Uneven {cls.__name__} constructions: {lengths}')
         return [cls(*items) for items in zip(*objs)]
 
+    @classmethod
+    def from_mask(
+        cls, metric_per_token: torch.Tensor, mask: torch.Tensor
+    ) -> List[Metric]:
+        """
+        From token-level metrics, returns an aggregate MyMetric per example in the
+        batch.
+
+        :param metric_per_token:
+            a (batchsize x num_tokens) Tensor
+        :param mask:
+            a (batchsize x num_tokens) Tensor to mask out tokens that should *not* be considered in the aggregate metric calculation.
+        :return:
+            a (batchsize) Tensor
+        """
+        tokens_per_ex = mask.long().sum(dim=-1)
+        metric_per_ex = (metric_per_token * mask).sum(dim=-1)
+        metrics = cls.many(metric_per_ex, tokens_per_ex)
+        return metrics
+
 
 class FixedMetric(Metric):
     """
     Fixed metrics are verified to be the same when combined, or throw an error.
 
     FixedMetric is used for things like total_train_updates, which should not be
     combined across different multitasks or different workers.
@@ -1073,14 +1094,16 @@
 
         self._consume_user_metrics(observation)
 
     def _consume_user_metrics(self, observation):
         # User-reported metrics
         if 'metrics' in observation:
             for uk, v in observation['metrics'].items():
+                if v is None:
+                    continue
                 if uk in ALL_METRICS:
                     # don't let the user override our metrics
                     uk = f'USER_{uk}'
                 assert isinstance(uk, str), f'{type(uk)} is not a str'
                 if not isinstance(v, Metric):
                     warn_once(f'Metric {uk} is assumed to be averaged per example.')
                     v = AverageMetric(v)
```

### Comparing `parlai-1.7.1/parlai/core/mutators.py` & `parlai-1.7.2/parlai/core/mutators.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/opt.py` & `parlai-1.7.2/parlai/core/opt.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/params.py` & `parlai-1.7.2/parlai/core/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -770,19 +770,19 @@
         """
         grp = self.add_argument_group('Distributed Training')
         grp.add_argument(
             '--distributed-world-size', type=int, help='Number of workers.'
         )
         grp.add_argument(
             '--ddp-backend',
-            # TODO: add in zero3. https://github.com/facebookresearch/ParlAI/issues/3753
-            choices=['ddp', 'zero2'],
+            choices=['ddp', 'zero2', 'zero3'],
             default='ddp',
             help=(
                 'Distributed backend. Zero2 can be faster but is more experimental. '
+                'Zero3 significantly reduces memory pressure. '
                 'DDP is the most tested.'
             ),
         )
         return grp
 
     def add_model_args(self):
         """
```

### Comparing `parlai-1.7.1/parlai/core/script.py` & `parlai-1.7.2/parlai/core/script.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/teachers.py` & `parlai-1.7.2/parlai/core/teachers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1726,16 +1726,20 @@
                     for example, example_begins in self._return_episode_examples(eps):
                         yield example, example_begins
 
     def _get_ep_from_turns(self, xturns, yturns):
         eps = []
         for xturn, yturn in zip(xturns, yturns):
             turn = {}
-            turn['text'] = xturn.get('text').strip()
-            turn['labels'] = [yturn.get('text').strip()]
+            turn['text'] = xturn.get('text')
+            turn['labels'] = [yturn.get('text')]
+
+            turn['x_turn'] = dict(xturn)
+            turn['y_turn'] = dict(yturn)
+
             eps.append(turn)
         return eps
 
 
 class AbstractImageTeacher(FixedDialogTeacher):
     """
     Abstract class to allow easier creation of image + dialogue tasks.
@@ -1833,16 +1837,16 @@
         if not isinstance(a, str):
             raise argparse.ArgumentTypeError(
                 '%s must be a string representing image model name' % a
             )
         available_model_names = self.get_available_image_mode_names()
         if a not in available_model_names:
             raise argparse.ArgumentTypeError(
-                '\"%s\" unknown image model name. Choose from: %s. Currently suggested resnet is resnet152 and resnext is resnext101_32x48d_wsl.'
-                % (a, available_model_names)
+                f'"{a}" unknown image model name. Choose from: {available_model_names}.'
+                'Currently suggested resnet is resnet152 and resnext is resnext101_32x48d_wsl.'
             )
         return a
 
     @classmethod
     def add_cmdline_args(
         cls, parser: ParlaiParser, partial_opt: Optional[Opt] = None
     ) -> ParlaiParser:
```

### Comparing `parlai-1.7.1/parlai/core/tod/teacher_metrics.py` & `parlai-1.7.2/parlai/core/tod/teacher_metrics.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/tod/tod_agents.py` & `parlai-1.7.2/parlai/core/tod/tod_agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/tod/tod_core.py` & `parlai-1.7.2/parlai/core/tod/tod_core.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/tod/tod_test_utils/test_agents.py` & `parlai-1.7.2/parlai/core/tod/tod_test_utils/test_agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/tod/tod_world.py` & `parlai-1.7.2/parlai/core/tod/tod_world.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/tod/world_metrics.py` & `parlai-1.7.2/parlai/core/tod/world_metrics.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/tod/world_metrics_handlers.py` & `parlai-1.7.2/parlai/core/tod/world_metrics_handlers.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/torch_agent.py` & `parlai-1.7.2/parlai/core/torch_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,21 @@
 from parlai.core.agents import Agent
 from parlai.core.dict import DictionaryAgent, TokenizationMode
 from parlai.nn.lr_scheduler import ParlAILRScheduler
 from parlai.core.message import Message
 from parlai.utils.distributed import is_distributed
 from parlai.utils.misc import AttrDict, warn_once
 from parlai.utils.io import PathManager
-from parlai.utils.fsdp import should_sync_gradnorm, is_fsdp, DEFAULT_DDP_BACKEND
+from parlai.utils.fsdp import (
+    should_sync_gradnorm,
+    is_fsdp,
+    DEFAULT_DDP_BACKEND,
+    FSDP_AVAILABLE,
+    get_state_dict,
+)
 from parlai.utils.fp16 import (
     SafeFP16Optimizer,
     MemoryEfficientFP16Optimizer,
     MemoryEfficientFP16Adam,
     Adafactor,
 )
 from parlai.core.metrics import (
@@ -1977,16 +1983,19 @@
         Override this method for more specific saving.
         """
         states = {}
         if hasattr(self, 'model'):  # save model params
             if hasattr(self.model, 'module') and not is_fsdp(self.model):
                 # did we wrap in a DistributedDataParallel or DataParallel
                 states['model'] = self.model.module.state_dict()
+            elif is_fsdp(self.model) and FSDP_AVAILABLE:
+                # FSDP Model; use fancy saving
+                states['model'] = get_state_dict(self.model)
             else:
-                # regular model or FSDP
+                # regular model
                 states['model'] = self.model.state_dict()
 
         if hasattr(self, 'optimizer'):
             # save optimizer params
             states['optimizer'] = self.optimizer.state_dict()
             states['optimizer_type'] = self.opt['optimizer']
```

### Comparing `parlai-1.7.1/parlai/core/torch_classifier_agent.py` & `parlai-1.7.2/parlai/core/torch_classifier_agent.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/torch_generator_agent.py` & `parlai-1.7.2/parlai/core/torch_generator_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -428,28 +428,47 @@
             choices={
                 'beam',
                 'greedy',
                 'topk',
                 'nucleus',
                 'delayedbeam',
                 'delayednucleusbeam',
+                'factual_nucleus',
             },
             default='greedy',
             help='Generation algorithm',
         )
         agent.add_argument(
             '--topk', type=int, default=10, help='K used in Top K sampling'
         )
         agent.add_argument(
             '--topp', type=float, default=0.9, help='p used in nucleus sampling'
         )
         agent.add_argument(
             '--beam-delay', type=int, default=30, help='used in delayedbeam search'
         )
         agent.add_argument(
+            '--lambda-decay',
+            type=float,
+            default=0.9,
+            help='decay factor in factual nucleus sampling',
+        )
+        agent.add_argument(
+            '--omega-bound',
+            type=float,
+            default=0.3,
+            help='lower bound in factual nucleus sampling',
+        )
+        agent.add_argument(
+            '--p-reset',
+            type='bool',
+            default=True,
+            help='Whether to reset p value in factual nucleus at full stops',
+        )
+        agent.add_argument(
             '--beam-block-list-filename',
             type=str,
             default=None,
             help='Load a text file of hard blocks for beam search to never say.',
         )
         agent.add_argument(
             '--temperature',
@@ -465,14 +484,20 @@
         )
         parser.add_argument(
             '--gpu-beam-blocking',
             type='bool',
             help='Set to use CUDA kernel for beam search ngram blocking',
             default=False,
         )
+        parser.add_argument(
+            '--verbose-topk',
+            type=int,
+            help='Return the topk logits in the act message, if verbose mode is set.',
+            default=-1,
+        )
 
         super().add_cmdline_args(parser, partial_opt=partial_opt)
         return agent
 
     def __init__(self, opt: Opt, shared=None):
         init_model, is_finetune = self._get_init_model(opt, shared)
         super().__init__(opt, shared)
@@ -493,16 +518,18 @@
         if shared:
             # set up shared properties
             states = shared.get('states', {})
             self.beam_block_list = shared.get('beam_block_list')
         else:
             # this is not a shared instance of this class, so do full init
             self.criterion = self.build_criterion()
+
+            self.model = self.build_model()
             with fsdp_utils.maybe_fsdp_wrap(opt):
-                self.model = fsdp_utils.fsdp_wrap(self.build_model())
+                self.model = fsdp_utils.fsdp_wrap(self.model)
                 if self.fp16 and not fsdp_utils.delay_halving(opt):
                     self.model = self.model.half()
 
             # load the block_list for beam search
             self.beam_block_list = self._load_beam_block_list()
 
             if self.model is None or self.criterion is None:
@@ -692,50 +719,61 @@
         >>> model.encoder(*_encoder_input(batch))
 
         This is intentionally overridable so that richer models can pass the
         additional inputs directly to the encoder.
         """
         return self._model_input(batch)
 
+    def record_per_token_metrics(self, batch, loss_per_token):
+        """
+        Override this method for custom loss values that require loss_per_token.
+        """
+        pass
+
     def compute_loss(self, batch, return_output=False):
         """
         Compute and return the loss for the given batch.
 
         Easily overridable for customized loss functions.
 
         If return_output is True, the full output from the call to self.model()
         is also returned, via a (loss, model_output) pair.
         """
         if batch.label_vec is None:
             raise ValueError('Cannot compute loss without a label.')
         model_output = self.model(*self._model_input(batch), ys=batch.label_vec)
         scores, preds, *_ = model_output
         score_view = scores.reshape(-1, scores.size(-1))
-        loss = self.criterion(score_view, batch.label_vec.view(-1))
-        loss = loss.view(scores.shape[:-1]).sum(dim=1)
-        # save loss to metrics
+        loss_flattened = self.criterion(score_view, batch.label_vec.view(-1))
+        loss_per_token = loss_flattened.view(scores.shape[:-1])
         notnull = batch.label_vec.ne(self.NULL_IDX)
-        target_tokens = notnull.long().sum(dim=-1)
-        correct = ((batch.label_vec == preds) * notnull).sum(dim=-1)
 
+        # save loss to metrics
         # cross entropy loss
-        self.record_local_metric('loss', AverageMetric.many(loss, target_tokens))
+        self.record_local_metric(
+            'loss', AverageMetric.from_mask(loss_per_token, notnull)
+        )
         # perplexity
-        self.record_local_metric('ppl', PPLMetric.many(loss, target_tokens))
+        self.record_local_metric('ppl', PPLMetric.from_mask(loss_per_token, notnull))
         # token-wise accuracy
         self.record_local_metric(
-            'token_acc', AverageMetric.many(correct, target_tokens)
+            'token_acc', AverageMetric.from_mask(batch.label_vec == preds, notnull)
         )
         # utterance-wise exact match
+        num_target_tokens = notnull.long().sum(dim=-1)
+        num_tokens_correct = ((batch.label_vec == preds) * notnull).sum(dim=-1)
         self.record_local_metric(
-            'token_em', AverageMetric.many(correct == target_tokens)
+            'token_em', AverageMetric.many(num_tokens_correct == num_target_tokens)
         )
+        self.record_per_token_metrics(batch, loss_per_token)
+
         # actually do backwards loss
+        loss = loss_per_token.sum(dim=1)
         loss = loss.sum()
-        loss /= target_tokens.sum()  # average loss per token
+        loss /= num_target_tokens.sum()  # average loss per token
         if return_output:
             return (loss, model_output)
         else:
             return loss
 
     def train_step(self, batch):
         """
@@ -877,23 +915,35 @@
         if batch.text_vec is not None:
             bsz = batch.text_vec.size(0)
         else:
             bsz = len(batch.image)
         self.model.eval()
         cand_scores = None
         token_losses = None
+        logits = None
+        logit_inds = None
         text_token_info = None
 
         if batch.label_vec is not None:
             # calculate loss on targets with teacher forcing
             loss, model_output = self.compute_loss(batch, return_output=True)
             if self.show_token_details:
                 token_losses = self._construct_label_token_losses(
                     batch.label_vec, model_output
                 )
+                logits = model_output[0]
+                k = self.opt['verbose_topk']
+                if k != -1:
+                    tk = torch.topk(logits, k, dim=2)
+                    logits = tk.values
+                    logit_inds = tk.indices
+                    if isinstance(logit_inds, torch.Tensor):
+                        logit_inds = logit_inds.cpu().numpy().tolist()
+                if isinstance(logits, torch.Tensor):
+                    logits = logits.cpu().numpy().tolist()
 
         beam_preds_scores = None
         preds = None
         if self.skip_generation:
             warn_once("--skip-generation true produces limited metrics")
         else:
             maxlen = self.label_truncate or 256
@@ -941,15 +991,20 @@
             for beam_text_token_info in beam_texts_token_info:
                 text_token_info.append(beam_text_token_info[0])
 
         if text and self.compute_tokenized_bleu:
             # compute additional bleu scores
             self._compute_fairseq_bleu(batch, preds)
         retval = Output(
-            text, cand_choices, token_losses=token_losses, cand_scores=cand_scores
+            text,
+            cand_choices,
+            token_losses=token_losses,
+            cand_scores=cand_scores,
+            logits=logits,
+            logit_inds=logit_inds,
         )
 
         if not self.skip_generation:
             retval.beam_texts = beam_texts
             retval.beam_texts_token_info = beam_texts_token_info
             retval.text_token_info = text_token_info
         return retval
@@ -1043,14 +1098,33 @@
                 padding_token=self.NULL_IDX,
                 bos_token=self.START_IDX,
                 eos_token=self.END_IDX,
                 device=device,
                 verbose=verbose,
                 gpu_beam_blocking=self.opt.get('gpu_beam_blocking', False),
             )
+        elif method == 'factual_nucleus':
+            return FactualNucleusSampling(
+                self.opt['topp'],
+                self.opt['lambda_decay'],
+                self.opt['omega_bound'],
+                self.opt['p_reset'],
+                beam_size,
+                min_length=self.beam_min_length,
+                block_ngram=self.beam_block_ngram,
+                context_block_ngram=self.beam_context_block_ngram,
+                length_penalty=self.opt.get('beam_length_penalty', 0.65),
+                padding_token=self.NULL_IDX,
+                bos_token=self.START_IDX,
+                eos_token=self.END_IDX,
+                device=device,
+                verbose=verbose,
+                gpu_beam_blocking=self.opt.get('gpu_beam_blocking', False),
+                dict=self.dict,
+            )
         else:
             raise ValueError(f"Can't use inference method {method}")
 
     def _get_batch_context(self, batch):
         """
         Version of TGA._get_context() that operates on full batches for speed.
         """
@@ -1333,14 +1407,15 @@
         bos_token=1,
         eos_token=2,
         min_length=3,
         device='cpu',
         length_penalty=0.65,
         verbose=False,
         gpu_beam_blocking=False,
+        dict=None,
     ):
         """
         Instantiate Beam object.
 
         :param beam_size:
             number of hypothesis in the beam
         :param block_ngram:
@@ -1353,14 +1428,16 @@
             beginning of sentence token ID
         :param eos_token:
             end of sentence token ID
         :param min_length:
             minimum length of the predicted sequence
         :param device:
             What device to use for computations
+        :param dict:
+            dictionary, if necessary
         """
         self.beam_size = beam_size
         self.length_penalty = length_penalty
         self.block_ngram = block_ngram
         self.min_length = min_length
         self.eos = eos_token
         self.bos = bos_token
@@ -1389,19 +1466,18 @@
                 self.token_details.append([{"token_logprob": 0.0, "token_rank": 0}])
 
         # keeps tuples (score, time_step, hyp_id)
         self.finished = []
         self.eos_top = False
         self.eos_top_ts = None
         self.n_best_counter = 0
-        self.gpu_beam_blocking = gpu_beam_blocking
+        self.gpu_beam_blocking = gpu_beam_blocking and torch.cuda.is_available()
         self.partial_hyps = torch.tensor([[self.bos] for i in range(beam_size)])
         if self.gpu_beam_blocking:
             self.partial_hyps = self.partial_hyps.cuda()
-        if torch.cuda.is_available():
             self.no_repeat_ngram_op = NGramRepeatBlock()
 
     def set_context(self: TSType, context: torch.LongTensor) -> TSType:
         """
         Set the internal context representation and return self.
 
         :param context:
@@ -1436,15 +1512,15 @@
 
     def set_block_list(self: TSType, block_list: Optional[SearchBlocklist]) -> TSType:
         self.block_list = block_list
         return self
 
     def get_output_from_current_step(self):
         """
-        Get the outputput at the current step.
+        Get the output at the current step.
         """
         return self.outputs[-1]
 
     def get_backtrack_from_current_step(self):
         """
         Get the backtrack at the current step.
         """
@@ -1592,15 +1668,15 @@
         # might need to change later
         if self.partial_hyps.get_device() == -1:
             hyp_device = 'cpu'
         else:
             hyp_device = self.partial_hyps.get_device()
         self.partial_hyps = torch.cat(
             (
-                self.partial_hyps[path_selection.hypothesis_ids.long()],
+                self.partial_hyps[path_selection.hypothesis_ids.long().to(hyp_device)],
                 path_selection.token_ids.view(path_selection.token_ids.shape[0], -1).to(
                     hyp_device
                 ),
             ),
             1,
         )
 
@@ -1950,28 +2026,44 @@
     See https://arxiv.org/abs/1904.09751 for details.
     """
 
     def __init__(self, p, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.p = p
 
+    def update_p(self, tokens: torch.Tensor):
+        pass
+
+    def get_mask(self, sorted_probs: torch.Tensor) -> torch.Tensor:
+        """
+        Get probability mask.
+
+        :param sorted_probs:
+            sorted probabilities
+
+        :return mask:
+            mask out tokens below the p value when sampling.
+        """
+        return (sorted_probs.cumsum(dim=-1) - sorted_probs) >= self.p
+
     def select_paths(self, logprobs, prior_scores, current_length) -> _PathSelection:
         # Unlike the other treesearch methods, we have to switch to linspace
         # for the probabilities in order to compute the CDF.
         probs = torch.softmax(logprobs, dim=-1)
         sprobs, sinds = probs.sort(dim=-1, descending=True)
         # The subtraction here is to get the exclusive prefix sum,
         # to guarantee the first element is not masked
-        mask = (sprobs.cumsum(dim=-1) - sprobs) >= self.p
+        mask = self.get_mask(sprobs)
         trunc_sprobs = sprobs.detach().clone()
         trunc_sprobs[mask] = 0
         trunc_sprobs.div_(trunc_sprobs.sum(dim=-1).unsqueeze(1))
         choices = torch.multinomial(trunc_sprobs, 1)[:, 0]
         hyp_ids = torch.arange(logprobs.size(0)).to(logprobs.device)
         tok_ids = sinds[hyp_ids, choices]
+        self.update_p(tok_ids)
         # Convert back to logspace.
         scores = trunc_sprobs[hyp_ids, choices].log()
         best_scores = prior_scores.expand_as(scores) + scores
 
         token_details: Optional[List[_PathSelectionTokenDetails]] = None
         if self.verbose:
             tok_logprobs = sprobs[hyp_ids, choices].log().view(-1).cpu().numpy()
@@ -1985,7 +2077,57 @@
 
         return _PathSelection(
             hypothesis_ids=hyp_ids,
             token_ids=tok_ids,
             scores=best_scores,
             token_details=token_details,
         )
+
+
+class FactualNucleusSampling(NucleusSampling):
+    """
+    Factual Nucleus Sampling.
+
+    See https://arxiv.org/pdf/2206.04624.pdf for more information
+    """
+
+    def __init__(
+        self, p, lambda_decay, omega_bound, p_reset, beam_size, *args, **kwargs
+    ):
+        super().__init__(p, beam_size, *args, **kwargs)
+        assert 'dict' in kwargs
+        buffer = torch.zeros(beam_size)
+        self.p = buffer.clone().fill_(p).unsqueeze(1)
+        self.init_p = self.p.clone()
+        self.lambda_decay = lambda_decay
+        self.omega_bound = torch.tensor(omega_bound)
+        self.toks_since_reset = buffer.clone()
+        self.full_stop_list = torch.tensor(
+            [kwargs['dict'].txt2vec(w) for w in ['.', '?', '!']]
+        )
+        self.p_reset = p_reset
+
+    def update_p(self, tokens: torch.Tensor):
+        """
+        Updates sampling P value according to tokens generated.
+
+        When tokens are *not* punctuation, p is decayed by lambda_decay factor.
+
+        Otherwise, we reset the p value.
+
+        :param tokens:
+            sampled tokens.
+        """
+        for i, t in enumerate(tokens):
+            if self.full_stop_list.to(tokens.device).eq(t).sum() > 0:
+                self.toks_since_reset[i] = 0
+            else:
+                self.toks_since_reset[i] += 1
+            decay_factor = max(0, self.toks_since_reset[i] - 1)
+            self.p[i] = torch.max(
+                self.omega_bound, self.init_p[i] * (self.lambda_decay ** (decay_factor))
+            )
+
+    def get_mask(self, sorted_probs: torch.Tensor) -> torch.Tensor:
+        return (sorted_probs.cumsum(dim=-1) - sorted_probs) >= self.p.expand(
+            sorted_probs.size()
+        ).to(sorted_probs.device)
```

### Comparing `parlai-1.7.1/parlai/core/torch_image_agent.py` & `parlai-1.7.2/parlai/core/torch_image_agent.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/torch_ranker_agent.py` & `parlai-1.7.2/parlai/core/torch_ranker_agent.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/core/worlds.py` & `parlai-1.7.2/parlai/core/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/acute_eval_agent_state.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/acute_eval_agent_state.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/acute_eval_blueprint.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/acute_eval_blueprint.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/acute_eval_builder.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/acute_eval_builder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/acute_eval_runner.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/acute_eval_runner.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/analysis.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/analysis.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/dump_task_to_acute_format.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/dump_task_to_acute_format.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/fast_acute_blueprint.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/fast_acute_blueprint.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/fast_eval.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/fast_eval.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/run.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/run.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/acute_eval/util.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/acute_eval/util.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/chat_demo/run.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/chat_demo/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import os
 from dataclasses import dataclass, field
 
 import hydra
-from omegaconf import DictConfig
+from omegaconf import DictConfig, MISSING
 
 # From the Mephisto repo
 from examples.parlai_chat_task_demo.parlai_test_script import (
     TestScriptConfig,
     TASK_DIRECTORY,
 )
 from mephisto.operations.hydra_config import register_script_config
```

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/dialcrowd/dialcrowd_blueprint.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/dialcrowd/dialcrowd_blueprint.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import json
 import logging
 import os
 from dataclasses import dataclass, field
-from typing import Any, Dict, TYPE_CHECKING
+from typing import Any, Dict, List, Union, TYPE_CHECKING
 
 from mephisto.operations.registry import register_mephisto_abstraction
 from mephisto.abstractions.blueprint import SharedTaskState
 from mephisto.abstractions.blueprints.static_react_task.static_react_blueprint import (
     StaticReactBlueprint,
     StaticReactBlueprintArgs,
 )
@@ -49,14 +49,16 @@
     This Blueprint has a subtasks number option to combine multiple conversations into
     "sub-HITs".
 
     It also has options for the onboarding data answers and the annotation bucket
     definitions.
     """
 
+    _initialization_data_dicts: Union[List[List[Dict[str, Any]]], List[Dict[str, Any]]]
+
     ArgsClass = DialCrowdStaticBlueprintArgs
     BLUEPRINT_TYPE = STATIC_BLUEPRINT_TYPE
 
     def __init__(
         self, task_run: "TaskRun", args: "DictConfig", shared_state: "SharedTaskState"
     ):
         super().__init__(task_run, args=args, shared_state=shared_state)
@@ -73,15 +75,15 @@
         grouped_data = []
         logging.info(
             f'Raw data length: {len(self.raw_data)}. self.subtasks_per_unit: {self.subtasks_per_unit}'
         )
         for i in range(0, len(self._initialization_data_dicts), self.subtasks_per_unit):
             chunk = self._initialization_data_dicts[i : i + self.subtasks_per_unit]
             grouped_data.append(chunk)
-        self._initialization_data_dicts = grouped_data
+        self._initialization_data_dicts = grouped_data  # type: ignore
         # Last group may have less unless an exact multiple
         logging.info(
             f'Grouped data into {len(self._initialization_data_dicts)} tasks with {self.subtasks_per_unit} subtasks each.'
         )
 
     def get_frontend_args(self) -> Dict[str, Any]:
         """
```

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/dialcrowd/run.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/dialcrowd/run.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/analysis/compile_results.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/analysis/compile_results.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/bot_agent.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/bot_agent.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/impl.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 from omegaconf import DictConfig, OmegaConf
 
 from parlai.crowdsourcing.utils.mturk import soft_block_mturk_workers
 from parlai.crowdsourcing.tasks.model_chat.model_chat_blueprint import (
     SharedModelChatTaskState,
 )
 
+import parlai.crowdsourcing.tasks.pairwise_per_turn_eval.worlds as world_module
 
-def run_task(cfg: DictConfig, task_directory: str, world_module=None):
+
+def run_task(cfg: DictConfig, task_directory: str):
     """
     Run task, given configuration.
     """
 
     frontend_source_dir = os.path.join(task_directory, "webapp")
     frontend_build_dir = os.path.join(frontend_source_dir, "build")
+
     _ = frontend_build_dir  # Unused at the moment
 
     db, cfg = load_db_and_process_config(cfg)
     print(f'\nHydra config:\n{OmegaConf.to_yaml(cfg)}')
 
     random.seed(42)
```

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/model_chat_blueprint.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/model_chat_blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,17 +151,19 @@
     override_opt: Dict[str, Any] = field(
         default_factory=dict,
         metadata={
             "help": "Additional args to pass to initialize the context generator "
             "in order to override the parlai parser defaults."
         },
     )
-    emoji_picker: bool = field(
-        default=False,
-        metadata={"help": "Show emoji picker."},
+    allowed_worker_qualification: Optional[str] = field(
+        default=None,
+        metadata={
+            "help": "The qualification name for the workers that are exclusively allowed to do the HITs from this task."
+        },
     )
 
 
 class BaseModelChatBlueprint(ParlAIChatBlueprint, ABC):
     """
     This Blueprint uses somewhat specialized arguments for turn annotations, manages
     their validation, and also has specialized data storage for the result format.
@@ -199,17 +201,19 @@
 
         if args.blueprint.get("chat_data_folder") == '':
             raise ValueError('Must provide a valid chat data folder')
         assert '~' not in args.blueprint.chat_data_folder, (
             f'"~" can\'t currently be parsed in the chat data folder path '
             f'{args.blueprint.chat_data_folder}'
         )
-        # Currently Hydra overrides the tilde key at lower levels as described here: https://hydra.cc/docs/next/advanced/override_grammar/basic/#grammar
-        # Thus the TILDE key cannot be used in replacement for $HOME variable
-        # Some hacky solution can probably be achieved but won't be good code so for now this assert is written as a placeholder
+        # Currently Hydra overrides the tilde key at lower levels as described here:
+        # https://hydra.cc/docs/next/advanced/override_grammar/basic/#grammar
+        # Thus the TILDE key cannot be used in replacement for $HOME variable.
+        # Some hacky solution can probably be achieved but won't be good code so for now
+        # this assert is written as a placeholder
 
         if args.blueprint.get("annotations_config_path", "") != "":
             full_path = os.path.expanduser(args.blueprint.annotations_config_path)
             assert os.path.exists(
                 full_path
             ), f"Target annotation config path {full_path} doesn't exist"
 
@@ -295,15 +299,14 @@
             "annotation_question": self.args.blueprint.annotation_question,
             "annotation_buckets": annotation_buckets,
             "onboarding_data": getattr(self, 'onboard_task_data', None),
             "left_pane_text": self.left_pane_text,
             "frame_height": 650,
             "final_rating_question": self.args.blueprint.final_rating_question,
             "block_mobile": True,
-            "emoji_picker": self.args.blueprint.emoji_picker,
         }
 
 
 @dataclass
 class ModelChatBlueprintArgs(BaseModelChatBlueprintArgs):
     _blueprint_type: str = BLUEPRINT_TYPE
     _group: str = field(
```

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/run.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/run.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/scripts/save_image_contexts.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/scripts/save_image_contexts.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/utils.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/utils.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/worlds.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/model_chat/worlds_image_chat.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/worlds_image_chat.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/analysis/compile_results.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/analysis/compile_results.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/bot_agent.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/bot_agent.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/impl.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/model_chat/impl.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,34 +3,33 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import os
 import random
 
+from omegaconf import DictConfig, OmegaConf
 from mephisto.operations.operator import Operator
 from mephisto.tools.scripts import load_db_and_process_config
-from omegaconf import DictConfig, OmegaConf
+from mephisto.data_model.qualification import QUAL_EXISTS
+from mephisto.utils.qualifications import make_qualification_dict
 
 from parlai.crowdsourcing.utils.mturk import soft_block_mturk_workers
 from parlai.crowdsourcing.tasks.model_chat.model_chat_blueprint import (
     SharedModelChatTaskState,
 )
 
-import parlai.crowdsourcing.tasks.pairwise_per_turn_eval.worlds as world_module
 
-
-def run_task(cfg: DictConfig, task_directory: str):
+def run_task(cfg: DictConfig, task_directory: str, world_module=None):
     """
     Run task, given configuration.
     """
 
     frontend_source_dir = os.path.join(task_directory, "webapp")
     frontend_build_dir = os.path.join(frontend_source_dir, "build")
-
     _ = frontend_build_dir  # Unused at the moment
 
     db, cfg = load_db_and_process_config(cfg)
     print(f'\nHydra config:\n{OmegaConf.to_yaml(cfg)}')
 
     random.seed(42)
 
@@ -45,15 +44,25 @@
 
     soft_block_qual_name = cfg.mephisto.blueprint.get(
         'block_qualification', f'{task_name}_block'
     )
     # Default to a task-specific name to avoid soft-block collisions
     soft_block_mturk_workers(cfg=cfg, db=db, soft_block_qual_name=soft_block_qual_name)
 
-    # Init
-    shared_state = SharedModelChatTaskState(world_module=world_module)
+    # TODO: this maybe moved to the parent class: SharedModelChatTaskState
+    if cfg.mephisto.blueprint.allowed_worker_qualification is not None:
+        use_qualifications = [
+            make_qualification_dict(
+                cfg.mephisto.blueprint.allowed_worker_qualification, QUAL_EXISTS, None
+            ),
+        ]
+        shared_state = SharedModelChatTaskState(
+            world_module=world_module, qualifications=use_qualifications
+        )
+    else:
+        shared_state = SharedModelChatTaskState(world_module=world_module)
 
     operator = Operator(db)
     operator.validate_and_run_config(run_config=cfg.mephisto, shared_state=shared_state)
     operator.wait_for_runs_then_shutdown(
         skip_input=True, log_rate=cfg.monitoring_log_rate
     )
```

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/per_turn_eval_blueprint.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/per_turn_eval_blueprint.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/run.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/run.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/worlds.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/pairwise_per_turn_eval/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/qa_data_collection/run.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/qa_data_collection/run.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/qa_data_collection/util.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/qa_data_collection/util.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/qa_data_collection/worlds.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/qa_data_collection/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/turn_annotations_static/analysis/compile_results.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/analysis/compile_results.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/turn_annotations_static/run.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/run.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/tasks/turn_annotations_static/turn_annotations_blueprint.py` & `parlai-1.7.2/parlai/crowdsourcing/tasks/turn_annotations_static/turn_annotations_blueprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import json
 import logging
 import math
 import os
 import random
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, TYPE_CHECKING
+from typing import Any, Dict, List, Optional, Union, TYPE_CHECKING
 
 import numpy as np
 from mephisto.operations.registry import register_mephisto_abstraction
 from mephisto.abstractions.blueprint import SharedTaskState
 from mephisto.abstractions.blueprints.static_react_task.static_react_blueprint import (
     StaticReactBlueprint,
     StaticReactBlueprintArgs,
@@ -53,15 +53,17 @@
     )
     subtasks_per_unit: int = field(
         default=-1, metadata={"help": "Number of subtasks/comparisons to do per unit"}
     )
     annotation_indices_jsonl: Optional[str] = field(
         default=None,
         metadata={
-            "help": "Specify which utterance indices to annotate per conversation in a JSONL file. Must be same length as conversations data-jsonl file. See example file in task_config/annotation_indices_example.jsonl"
+            "help": "Specify which utterance indices to annotate per conversation in a JSONL file. "
+            "Must be same length as conversations data-jsonl file. "
+            "See example file in task_config/annotation_indices_example.jsonl"
         },
     )
     annotation_last_only: Optional[bool] = field(
         default=False,
         metadata={
             "help": "If you only want to annotate the last utterance of each conversation. Cannot be used with annotation_indices_jsonl."
         },
@@ -83,16 +85,16 @@
         metadata={
             "help": "Path to data and answers for onboarding task in JSON format"
         },
     )
     annotations_config_path: str = field(
         default="",
         metadata={
-            "help": "As per Turn Annotations task, path to annotation buckets which will be checkboxes in the frontend for worker to annotate an utterance. Set to "
-            " to disable checkboxes."
+            "help": "As per Turn Annotations task, path to annotation buckets which will be checkboxes in"
+            " the frontend for worker to annotate an utterance. Set to disable checkboxes."
         },
     )
     response_field: bool = field(
         default=False,
         metadata={
             "help": "If we want a freeform textbox input for the crowdworker to respond to the message."
         },
@@ -109,14 +111,16 @@
     This Blueprint has a subtasks number option to combine multiple conversations into
     "sub-HITs".
 
     It also has options for the onboarding data answers and the annotation bucket
     definitions.
     """
 
+    _initialization_data_dicts: Union[List[List[Dict[str, Any]]], List[Dict[str, Any]]]
+
     ArgsClass = TurnAnnotationsStaticBlueprintArgs
     BLUEPRINT_TYPE = STATIC_BLUEPRINT_TYPE
 
     def __init__(
         self, task_run: "TaskRun", args: "DictConfig", shared_state: "SharedTaskState"
     ):
         super().__init__(task_run, args=args, shared_state=shared_state)
@@ -148,15 +152,16 @@
                 line = f.readline()
                 while line:
                     conversation_indices = json.loads(line)
                     self.annotation_indices.append(conversation_indices)
                     line = f.readline()
             if len(self.annotation_indices) != len(self.raw_data):
                 raise Exception(
-                    f'Cannot specify a different length of annotation indices ({len(self.annotation_indices)}) than conversations ({len(self.raw_data)}).'
+                    f'Cannot specify a different length of annotation indices '
+                    f'({len(self.annotation_indices)}) than conversations ({len(self.raw_data)}).'
                 )
             # TODO: should check that utterances specified are all bot
             # utterances (agent_idx == 1)
 
         if self.conversation_count:
             self.raw_data = self.raw_data[: self.conversation_count]
             if self.annotation_indices:
@@ -173,15 +178,15 @@
         grouped_data = []
         logging.info(
             f'Raw data length: {len(self.raw_data)}. self.subtasks_per_unit: {self.subtasks_per_unit}'
         )
         for i in range(0, len(self._initialization_data_dicts), self.subtasks_per_unit):
             chunk = self._initialization_data_dicts[i : i + self.subtasks_per_unit]
             grouped_data.append(chunk)
-        self._initialization_data_dicts = grouped_data
+        self._initialization_data_dicts = grouped_data  # type: ignore
         # Last group may have less unless an exact multiple
         logging.info(
             f'Grouped data into {len(self._initialization_data_dicts)} tasks with {self.subtasks_per_unit} subtasks each.'
         )
 
     def get_frontend_args(self) -> Dict[str, Any]:
         """
@@ -233,15 +238,17 @@
             if annotation_indices:
                 total_annotation_count += len(annotation_indices[conv_idx])
                 # We only want to show the conversation up to the last
                 # utterance we need annotations on, b/c otherwise may confuse
                 # or bias the turkers
                 if len(annotation_indices[conv_idx]) > 1:
                     logging.info(
-                        f'Splitting {len(annotation_indices[conv_idx])} separate problematic utterance annotations in the same conversation into two separate conversations for this task. This avoids biasing the turkers with utterances that may come after one of the annotations.'
+                        f'Splitting {len(annotation_indices[conv_idx])} separate problematic utterance '
+                        'annotations in the same conversation into two separate conversations for this task. '
+                        'This avoids biasing the turkers with utterances that may come after one of the annotations.'
                     )
                 for a in annotation_indices[conv_idx]:
                     processed_dialog = self._process_conversation(d, [a])
                     output.append(processed_dialog)
             elif self.annotation_last_only:
                 # Annotate only the last utterance
                 last_idx = len(d['dialog']) * 2 - 1
@@ -255,15 +262,17 @@
                 total_annotation_count += len(d['dialog']) / 2
                 processed_dialog = self._process_conversation(
                     d, annotation_indices=None
                 )
                 output.append(processed_dialog)
 
         print(
-            f'process_data: Processed {len(data_dicts)} total conversations into {len(output)} conversations in the full data with {total_annotation_count} total turn annotations. (Does not account for units per assignment value - i.e. multiple annotations.)'
+            f'process_data: Processed {len(data_dicts)} total conversations into {len(output)} '
+            f'conversations in the full data with {total_annotation_count} total turn annotations. '
+            f'(Does not account for units per assignment value - i.e. multiple annotations.)'
         )
 
         np.random.shuffle(output)
         return output
 
     def _process_conversation(self, d, annotation_indices: Optional[List[int]] = None):
         """
@@ -322,28 +331,34 @@
                     }
                 )
                 adjusted_turn_idx += 1
         if max_turn_to_show is not None and adjusted_turn_idx < max_turn_to_show:
             raise Exception(
                 f'Conversation had {adjusted_turn_idx} but max_turn_to_show was {max_turn_to_show}'
             )
-        assert any(
-            nd['do_annotate'] for nd in new_dialogue
-        ), f'Have to annotate at least one index in the conversation! But new_dialogue was: {new_dialogue}, raw dialogue was: {d["dialog"]}, annotation_indices was: {annotation_indices}, length of dialogue was {len(new_dialogue)}, adjusted_turn_idx was: {adjusted_turn_idx}, max_turn_to_show: {max_turn_to_show}'
+        assert any(nd['do_annotate'] for nd in new_dialogue), (
+            f'Have to annotate at least one index in the conversation! But new_dialogue was: {new_dialogue},'
+            f' raw dialogue was: {d["dialog"]}, annotation_indices was: {annotation_indices}, '
+            f'length of dialogue was {len(new_dialogue)}, adjusted_turn_idx was: {adjusted_turn_idx}, '
+            f'max_turn_to_show: {max_turn_to_show}'
+        )
 
         return new_dialogue
 
 
 @dataclass
 class TurnAnnotationsStaticInFlightQABlueprintArgs(TurnAnnotationsStaticBlueprintArgs):
     _blueprint_type: str = STATIC_IN_FLIGHT_QA_BLUEPRINT_TYPE
     _group: str = field(
         default="TurnAnnotationsStaticInFlightQABlueprint",
         metadata={
-            'help': """This task mixes in a live onboarding as the last subtask (in addition to an onboarding at the start), and actually increases the number of subtasks per unit by 1."""
+            'help': (
+                "This task mixes in a live onboarding as the last subtask (in addition to an onboarding at the start),"
+                " and actually increases the number of subtasks per unit by 1."
+            )
         },
     )
     onboarding_in_flight_data: str = field(
         default=os.path.join(get_task_path(), 'task_config/onboarding_in_flight.jsonl'),
         metadata={
             "help": "Path to data and answers for onboarding task in JSON-L format (one JSON object per line per onboarding)"
         },
@@ -380,15 +395,15 @@
         )
 
         # Re-chunk the data to add a quality control convo as the last subtask
         # No shuffling of the data for reproducibility's sake
         # (quality control will always be last subtask)
         # TODO: I don't think we need to re-chunk this actually; just iterate
         # over the data and add the quality control task
-        all_data = []
+        all_data: List[Any] = []
         for grp in self._initialization_data_dicts:
             all_data.extend(grp)
 
         grouped_data = []
         number_of_tasks = math.floor(len(all_data) / self.subtasks_per_unit)
         for i in range(0, number_of_tasks):
             data_index = i * self.subtasks_per_unit
@@ -397,9 +412,10 @@
             chunk.append(self.quality_control_convos[qc_convo_idx])
             grouped_data.append(chunk)
 
         self._initialization_data_dicts = grouped_data
         self.subtasks_per_unit = len(chunk)
 
         print(
-            f'{self.__class__.__name__}: Grouped data into {len(self._initialization_data_dicts)} tasks with {self.subtasks_per_unit} subtasks each (added in-flight qualification task).'
+            f'{self.__class__.__name__}: Grouped data into {len(self._initialization_data_dicts)}'
+            f'tasks with {self.subtasks_per_unit} subtasks each (added in-flight qualification task).'
         )
```

### Comparing `parlai-1.7.1/parlai/crowdsourcing/utils/acceptability.py` & `parlai-1.7.2/parlai/crowdsourcing/utils/acceptability.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/utils/analysis.py` & `parlai-1.7.2/parlai/crowdsourcing/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/utils/frontend.py` & `parlai-1.7.2/parlai/crowdsourcing/utils/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     frontend_build_dir = os.path.join(frontend_source_dir, "build")
     return_dir = os.getcwd()
 
     # Build the task
     os.chdir(frontend_source_dir)
     if os.path.exists(frontend_build_dir):
         shutil.rmtree(frontend_build_dir)
-    packages_installed = subprocess.call(["npm", "install"])
+    packages_installed = subprocess.call(["npm", "install", "--force"])
     if packages_installed != 0:
         raise Exception(
             "please make sure npm is installed, otherwise view "
             "the above error for more info."
         )
     webpack_complete = subprocess.call(["npm", "run", "dev"])
     if webpack_complete != 0:
```

### Comparing `parlai-1.7.1/parlai/crowdsourcing/utils/mturk.py` & `parlai-1.7.2/parlai/crowdsourcing/utils/mturk.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/crowdsourcing/utils/tests.py` & `parlai-1.7.2/parlai/crowdsourcing/utils/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 import tempfile
 import time
 import unittest
 from typing import Any, Dict, List, Optional, Sequence, Union
 
 import numpy as np
 import torch
+from parlai.utils import logging
 from hydra.experimental import compose, initialize
 from mephisto.abstractions.blueprint import SharedTaskState
 from mephisto.abstractions.databases.local_database import LocalMephistoDB
+from mephisto.data_model.task_run import TaskRunArgs
 from mephisto.operations.operator import Operator
 from mephisto.tools.scripts import augment_config_from_db
+from mephisto.utils.metrics import InaccessiblePrometheusServer
 from pytest_regressions.data_regression import DataRegressionFixture
 
 
 class AbstractCrowdsourcingTest:
     """
     Abstract class for end-to-end tests of Mephisto-based crowdsourcing tasks.
 
@@ -49,16 +52,19 @@
     def _teardown(self):
         """
         To be run after a test.
 
         Should be called in a pytest setup/teardown fixture.
         """
 
-        if self.operator is not None:
-            self.operator.force_shutdown()
+        try:
+            if self.operator is not None:
+                self.operator.force_shutdown()
+        except InaccessiblePrometheusServer as e:
+            logging.warning(f'InaccessiblePrometheusServer: {e}')
 
         if self.server is not None:
             self.server.shutdown_mock()
 
     def _set_up_config(
         self,
         task_directory: str,
@@ -98,14 +104,17 @@
             )
 
         self.data_dir = tempfile.mkdtemp()
         self.database_path = os.path.join(self.data_dir, "mephisto.db")
         self.db = LocalMephistoDB(self.database_path)
         self.config = augment_config_from_db(self.config, self.db)
         self.config.mephisto.architect.should_run_server = True
+        self.config.mephisto.task = TaskRunArgs(
+            **self.config.mephisto.task, no_submission_patience=1
+        )
 
     def _set_up_server(self, shared_state: Optional[SharedTaskState] = None):
         """
         Set up the operator and server.
         """
         self.operator = Operator(self.db)
         self.operator.launch_task_run(self.config.mephisto, shared_state=shared_state)
```

### Comparing `parlai-1.7.1/parlai/crowdsourcing/utils/worlds.py` & `parlai-1.7.2/parlai/crowdsourcing/utils/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/mutators/context_shuffle.py` & `parlai-1.7.2/parlai/mutators/context_shuffle.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/mutators/episode_reverse.py` & `parlai-1.7.2/parlai/mutators/episode_reverse.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/mutators/episode_shuffle.py` & `parlai-1.7.2/parlai/mutators/episode_shuffle.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/mutators/flatten.py` & `parlai-1.7.2/parlai/mutators/flatten.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/mutators/flip_labels.py` & `parlai-1.7.2/parlai/mutators/flip_labels.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/mutators/last_turn.py` & `parlai-1.7.2/parlai/mutators/last_turn.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/mutators/word_reverse.py` & `parlai-1.7.2/parlai/mutators/word_reverse.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/mutators/word_shuffle.py` & `parlai-1.7.2/parlai/mutators/word_shuffle.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/nn/checkpoint.py` & `parlai-1.7.2/parlai/nn/checkpoint.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/nn/lr_scheduler.py` & `parlai-1.7.2/parlai/nn/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/ops/ngram_repeat_block.py` & `parlai-1.7.2/parlai/ops/ngram_repeat_block.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,42 +12,40 @@
 import parlai.utils.logging as logging
 import torch
 from torch import nn
 
 import os
 from torch.utils.cpp_extension import load
 
-current = os.getcwd()
-abspath = os.path.abspath(__file__)
-dname = os.path.dirname(abspath)
-os.chdir(dname)
-
-
-try:
-    ngram_repeat_block_cuda = load(
-        name='ngram_repeat_block_cuda',
-        sources=[
-            '../clib/cuda/ngram_repeat_block_cuda.cpp',
-            '../clib/cuda/ngram_repeat_block_cuda_kernel.cu',
-        ],
-    )
-except Exception as e:
-    logging.warning(f"Unable to load ngram blocking on GPU: {e}")
-    ngram_repeat_block_cuda = None
-
-os.chdir(current)
-
 
 class NGramRepeatBlock(nn.Module):
     """
     Wrapper class for calling ngram_repeat_block cuda extension.
     """
 
     def __init__(self):
         super(NGramRepeatBlock, self).__init__()
+        current = os.getcwd()
+        abspath = os.path.abspath(__file__)
+        dname = os.path.dirname(abspath)
+        os.chdir(dname)
+
+        try:
+            self.ngram_repeat_block_cuda = load(
+                name='ngram_repeat_block_cuda',
+                sources=[
+                    '../clib/cuda/ngram_repeat_block_cuda.cpp',
+                    '../clib/cuda/ngram_repeat_block_cuda_kernel.cu',
+                ],
+            )
+        except Exception as e:
+            logging.warning(f"Unable to load ngram blocking on GPU: {e}")
+            self.ngram_repeat_block_cuda = None
+
+        os.chdir(current)
 
     def forward(
         self,
         hypothesis,
         context,
         lprobs,
         bsz,
@@ -71,15 +69,15 @@
         if not if_context_blocking:
             context = torch.Tensor([0]).long()
         assert hypothesis.size(0) == bsz * beam_size
         assert lprobs.size(0) == bsz * beam_size
         hypothesis = hypothesis.contiguous()
         context = context.contiguous()
         lprobs = lprobs.contiguous()
-        return ngram_repeat_block_cuda.forward(
+        return self.ngram_repeat_block_cuda.forward(
             hypothesis,
             context,
             lprobs,
             bsz,
             step,
             beam_size,
             no_repeat_ngram_size,
```

### Comparing `parlai-1.7.1/parlai/opt_presets/docs.py` & `parlai-1.7.2/parlai/opt_presets/docs.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/build_candidates.py` & `parlai-1.7.2/parlai/scripts/build_candidates.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/build_dict.py` & `parlai-1.7.2/parlai/scripts/build_dict.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/compare_opts.py` & `parlai-1.7.2/parlai/scripts/compare_opts.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/convert_data_to_json_format.py` & `parlai-1.7.2/parlai/scripts/convert_data_to_json_format.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/convert_data_to_parlai_format.py` & `parlai-1.7.2/parlai/scripts/convert_data_to_parlai_format.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/convo_render.py` & `parlai-1.7.2/parlai/scripts/convo_render.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/data_stats.py` & `parlai-1.7.2/parlai/scripts/data_stats.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/detect_offensive_language.py` & `parlai-1.7.2/parlai/scripts/detect_offensive_language.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/display_data.py` & `parlai-1.7.2/parlai/scripts/display_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,19 +47,26 @@
 
 def simple_display(opt, world, turn):
     if opt['batchsize'] > 1:
         raise RuntimeError('Simple view only support batchsize=1')
     act = world.get_acts()[0]
     if turn == 0:
         text = "- - - NEW EPISODE: " + act.get('id', "[no agent id]") + " - - -"
-        print(colorize(text, 'highlight'))
+        print(
+            colorize(
+                text.encode('utf-16', 'surrogatepass').decode('utf-16'), 'highlight'
+            )
+        )
     text = act.get('text', '[no text field]')
-    print(colorize(text, 'text'))
+    print(colorize(text.encode('utf-16', 'surrogatepass').decode('utf-16'), 'text'))
     labels = act.get('labels', act.get('eval_labels', ['[no labels field]']))
-    labels = '|'.join(labels)
+    if len(labels) == 1 and labels[0] is None:
+        labels = str(labels)
+    else:
+        labels = '|'.join(labels)
     print('   ' + colorize(labels, 'labels'))
 
 
 def display_data(opt):
     # force ordered data to prevent repeats
     if 'ordered' not in opt['datatype'] and 'train' in opt['datatype']:
         opt['datatype'] = f"{opt['datatype']}:ordered"
@@ -74,15 +81,18 @@
     turn = 0
     for _ in range(opt['num_examples']):
         world.parley()
 
         # NOTE: If you want to look at the data from here rather than calling
         # world.display() you could access world.acts[0] directly, see simple_display above.
         if opt.get('verbose', False) or opt.get('display_add_fields', ''):
-            print(world.display() + '\n~~')
+            print(
+                world.display().encode('utf-16', 'surrogatepass').decode('utf-16')
+                + '\n~~'
+            )
         else:
             simple_display(opt, world, turn)
             turn += 1
             if world.get_acts()[0]['episode_done']:
                 turn = 0
 
         if world.epoch_done():
```

### Comparing `parlai-1.7.1/parlai/scripts/display_model.py` & `parlai-1.7.2/parlai/scripts/display_model.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/distributed_eval.py` & `parlai-1.7.2/parlai/scripts/distributed_eval.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 #SBATCH --ntasks-per-node=8
 #SBATCH --mem=64G
 #SBATCH --cpus-per-task=10
 srun python -u -m parlai.scripts.distributed_eval \
   -m seq2seq -t convai2 --dict-file /path/to/dict-file
 ```
 """
-
-import parlai.scripts.eval_model as eval_model
 from parlai.core.script import ParlaiScript
+import parlai.scripts.eval_model as eval_model
 import parlai.utils.distributed as distributed_utils
+import parlai.utils.fsdp as fsdp_utils
 
 
 def setup_args():
     parser = eval_model.setup_args()
     parser.add_distributed_training_args()
     parser.add_argument('--port', type=int, default=61337, help='TCP port number')
     return parser
@@ -47,12 +47,14 @@
 class DistributedEval(ParlaiScript):
     @classmethod
     def setup_args(cls):
         return setup_args()
 
     def run(self):
         with distributed_utils.slurm_distributed_context(self.opt) as opt:
-            return eval_model.eval_model(opt)
+            self.evaluator = fsdp_utils.JoinableEvaluator(opt)
+            with fsdp_utils.fsdp_join(self.evaluator):
+                return self.evaluator.eval_model()
 
 
 if __name__ == '__main__':
     DistributedEval.main()
```

### Comparing `parlai-1.7.1/parlai/scripts/distributed_tod_world_script.py` & `parlai-1.7.2/parlai/scripts/distributed_tod_world_script.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/distributed_train.py` & `parlai-1.7.2/parlai/scripts/distributed_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
   -m seq2seq -t convai2 --dict-file /path/to/dict-file
 ```
 """
 
 import parlai.scripts.train_model as single_train
 from parlai.core.script import ParlaiScript
 import parlai.utils.distributed as distributed_utils
+import parlai.utils.fsdp as fsdp_utils
 
 
 def setup_args():
     parser = single_train.setup_args()
     parser.add_distributed_training_args()
     parser.add_argument('--port', type=int, default=61337, help='TCP port number')
     return parser
@@ -47,13 +48,14 @@
 class DistributedTrain(ParlaiScript):
     @classmethod
     def setup_args(cls):
         return setup_args()
 
     def run(self):
         with distributed_utils.slurm_distributed_context(self.opt) as opt:
-            self.train_loop = single_train.TrainLoop(opt)
-            return self.train_loop.train()
+            self.train_loop = fsdp_utils.JoinableTrainLoop(opt)
+            with fsdp_utils.fsdp_join(self.train_loop):
+                return self.train_loop.train()
 
 
 if __name__ == '__main__':
     DistributedTrain.main()
```

### Comparing `parlai-1.7.1/parlai/scripts/eval_model.py` & `parlai-1.7.2/parlai/tasks/genderation_bias/agents.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,305 +1,320 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Facebook, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-
 """
-Basic example which iterates through the tasks specified and evaluates the given model
-on them.
+Generates a controllable_gen version of a ParlAI task, i.e., for tasks with multi-turn
+dialogues (episodes), this will generate a task with single example episodes, in which
+we append to the context a special classification token.
+
+In order to use this teacher, specify the task flag as follows:
+`--task genderation_bias:controllable_task:<ORIGINAL TASK NAME>`.
 
-## Examples
+As an example, try running:
 
-```shell
-parlai eval_model --task "babi:Task1k:2" -m "repeat_label"
-parlai eval_model --task convai2 --model-file "/path/to/model_file"
-```
+`parlai display_data -t genderation_bias:controllable_task:convai2`
 """
 
-from parlai.core.params import ParlaiParser, print_announcements
-from parlai.core.agents import create_agent
-from parlai.core.logs import TensorboardLogger
-from parlai.core.metrics import (
-    aggregate_named_reports,
-    aggregate_unnamed_reports,
-    Metric,
-)
-from parlai.core.worlds import create_task
-from parlai.utils.misc import TimeLogger, nice_report
-from parlai.utils.world_logging import WorldLogger
-from parlai.core.script import ParlaiScript, register_script
+from parlai.core.params import ParlaiParser
+from parlai.core.message import Message
+from parlai.core.opt import Opt
+from parlai.core.teachers import FixedDialogTeacher
 from parlai.utils.io import PathManager
 import parlai.utils.logging as logging
+from parlai.utils.typing import TShared
+
+from parlai.tasks.genderation_bias.build import build
+from parlai.tasks.genderation_bias.utils import (
+    flatten_and_classify,
+    get_original_task_module,
+)
 
+from copy import deepcopy
+import datetime
+import glob
 import json
 import os
-import random
-
-from parlai.utils.distributed import (
-    is_primary_worker,
-    all_gather_list,
-    is_distributed,
-    get_rank,
-)
+from tqdm import tqdm
+from typing import List, Optional, Tuple
 
-# the index to access classifier agent's output in the world
-CLASSIFIER_AGENT = 1
 
+class ControllableTaskTeacher(FixedDialogTeacher):
+    """
+    Generates a controllable_gen version of a ParlAI task, i.e., for tasks with multi-
+    turn dialogues (episodes), this will generate a task with single example episodes,
+    in which we append to the context a special classification token.
+    """
 
-def setup_args(parser=None):
-    if parser is None:
-        parser = ParlaiParser(True, True, 'Evaluate a model')
-    # Get command line arguments
-    parser.add_argument(
-        '-rf',
-        '--report-filename',
-        type=str,
-        default='',
-        help='Saves a json file of the evaluation report either as an '
-        'extension to the model-file (if begins with a ".") or a whole '
-        'file path. Set to the empty string to not save at all.',
-    )
-    parser.add_argument(
-        '--world-logs',
-        type=str,
-        default='',
-        help='Saves a jsonl file of the world logs.'
-        'Set to the empty string to not save at all.',
-    )
-    parser.add_argument(
-        '--save-format',
-        type=str,
-        default='conversations',
-        choices=['conversations', 'parlai'],
-    )
-    parser.add_argument(
-        '--area-under-curve-digits',
-        '-auc',
-        type=int,
-        default=-1,
-        help='a positive number indicates to calculate the area under the roc curve and it also determines how many decimal digits of the predictions to keep (higher numbers->more precise); also used to determine whether or not to calculate the AUC metric',
-    )
-    parser.add_argument(
-        '--area-under-curve-class',
-        '-auclass',
-        type=str,
-        default=None,
-        nargs='*',
-        help='the name(s) of the class to calculate the auc for',
-    )
-    parser.add_argument('-ne', '--num-examples', type=int, default=-1)
-    parser.add_argument('-d', '--display-examples', type='bool', default=False)
-    parser.add_argument('-ltim', '--log-every-n-secs', type=float, default=10)
-    parser.add_argument(
-        '-mcs',
-        '--metrics',
-        type=str,
-        default='default',
-        help='list of metrics to show/compute, e.g. all, default,'
-        'or give a list split by , like '
-        'ppl,f1,accuracy,hits@1,rouge,bleu'
-        'the rouge metrics will be computed as rouge-1, rouge-2 and rouge-l',
-    )
-    parser.add_argument(
-        '-micro',
-        '--aggregate-micro',
-        type='bool',
-        default=False,
-        help='Report micro-averaged metrics instead of macro averaged metrics.',
-        recommended=False,
-    )
-    WorldLogger.add_cmdline_args(parser, partial_opt=None)
-    TensorboardLogger.add_cmdline_args(parser, partial_opt=None)
-    parser.set_params(datatype='valid')
-    return parser
-
-
-def _save_eval_stats(opt, report):
-    if not is_primary_worker:
-        return
-    report_fname = opt['report_filename']
-    if report_fname == '':
-        return
-    if report_fname.startswith('.'):
-        report_fname = opt['model_file'] + report_fname
-
-    json_serializable_report = report
-    for k, v in report.items():
-        if isinstance(v, Metric):
-            v = v.value()
-        json_serializable_report[k] = v
-
-    # Save report
-    with PathManager.open(report_fname, 'w') as f:
-        logging.info(f'Saving model report to {report_fname}')
-        json.dump({'opt': opt, 'report': json_serializable_report}, f, indent=4)
-        f.write("\n")  # for jq
-
-
-def get_task_world_logs(task, world_logs, is_multitask=False):
-    if not is_multitask:
-        return world_logs
-    else:
-        base_outfile, extension = os.path.splitext(world_logs)
-        return f'{base_outfile}_{task}{extension}'
-
-
-def prepare_tb_logger(opt):
-    if opt['tensorboard_log'] and is_primary_worker():
-        tb_logger = TensorboardLogger(opt)
-    else:
-        tb_logger = None
-
-    if 'train' in opt['datatype']:
-        setting = 'train'
-    elif 'valid' in opt['datatype']:
-        setting = 'valid'
-    else:
-        setting = 'test'
-    return tb_logger, setting
-
-
-def get_n_parleys(opt):
-    trainstats_suffix = '.trainstats'
-    if opt.get('model_file') and PathManager.exists(
-        opt['model_file'] + trainstats_suffix
-    ):
-        with PathManager.open(opt['model_file'] + trainstats_suffix) as ts:
-            obj = json.load(ts)
-            parleys = obj.get('parleys', 0)
-    else:
-        parleys = 0
-    return parleys
-
-
-def _eval_single_world(opt, agent, task):
-    logging.info(f'Evaluating task {task} using datatype {opt.get("datatype")}.')
-    # set up world logger
-    task_opt = opt.copy()  # copy opt since we're editing the task
-    task_opt['task'] = task
-    # add task suffix in case of multi-tasking
-    if opt['world_logs']:
-        task_opt['world_logs'] = get_task_world_logs(
-            task, task_opt['world_logs'], is_multitask=len(opt['task'].split(',')) > 1
+    @classmethod
+    def add_cmdline_args(
+        cls, parser: ParlaiParser, partial_opt: Optional[Opt] = None
+    ) -> ParlaiParser:
+        super().add_cmdline_args(parser, partial_opt)
+        flattened = parser.add_argument_group('ControllableTaskTeacher Flattening Args')
+        flattened.add_argument(
+            '--flatten-include-labels',
+            type='bool',
+            default=True,
+            help='Include labels in the history when flattening an episode',
         )
+        flattened.add_argument(
+            '--flatten-delimiter',
+            type=str,
+            default='\n',
+            help='How to join the dialogue history from previous turns.',
+        )
+        flattened.add_argument(
+            '--flatten-max-context-length',
+            type=int,
+            default=-1,
+            help='Maximum number of utterances to include per episode. '
+            'Default -1 keeps all.',
+        )
+        agent = parser.add_argument_group('ControllableTaskTeacher Args')
+        agent.add_argument(
+            '--invalidate-cache',
+            type='bool',
+            default=False,
+            help='Set this to True to rebuild the data (may want to do this if '
+            'original data has changed or you want to rebuild with new options)',
+        )
+        agent.add_argument(
+            '--max-examples',
+            type=int,
+            default=-1,
+            help='If greater than zero, will stop building after a certain num of exs',
+        )
+        agent.add_argument(
+            '--fixed-control',
+            type=str,
+            default='',
+            help='Always append this fixed control string, good for deploy time.',
+        )
+        # Add the arguments for the task teacher
+        opt = parser.parse_and_process_known_args()[0]
+        tasks = get_original_task_module(opt, multi_possible=True)
+        for task in tasks:
+            if hasattr(task, 'add_cmdline_args'):
+                task.add_cmdline_args(parser, partial_opt=partial_opt)
+        return parser
+
+    def __init__(self, opt: Opt, shared: TShared = None):
+        assert opt['flatten_delimiter'] == opt.get(
+            'delimiter', '\n'
+        ), '--flatten-delimiter and --delimiter are set differently, please inspect and set to the same to avoid unexpected results'
+        self.opt = opt
 
-    world_logger = WorldLogger(task_opt) if task_opt['world_logs'] else None
-
-    world = create_task(task_opt, agent)  # create worlds for tasks
+        if shared and 'data' in shared:
+            self.data = shared['data']
+        else:
+            self.word_lists = self.build_wordlists(opt)
+            self.data = self._setup_data(opt)
 
-    # set up logging
-    log_every_n_secs = opt.get('log_every_n_secs', -1)
-    if log_every_n_secs <= 0:
-        log_every_n_secs = float('inf')
-    log_time = TimeLogger()
-
-    # max number of examples to evaluate
-    max_cnt = opt['num_examples'] if opt['num_examples'] > 0 else float('inf')
-    cnt = 0
-    total_cnt = world.num_examples()
-
-    if is_distributed():
-        logging.warning('Progress bar is approximate in distributed mode.')
-
-    while not world.epoch_done() and cnt < max_cnt:
-        cnt += opt.get('batchsize', 1)
-        world.parley()
-        if world_logger is not None:
-            world_logger.log(world)
-        if opt['display_examples']:
-            # display examples
-            print(world.display() + '\n~~')
-        if log_time.time() > log_every_n_secs:
-            report = world.report()
-            text, report = log_time.log(
-                report.get('exs', 0), min(max_cnt, total_cnt), report
-            )
-            logging.info(text)
+        super().__init__(opt, shared)
+        self.reset()
 
-    if world_logger is not None:
-        # dump world acts to file
-        world_logger.reset()  # add final acts to logs
-        if is_distributed():
-            rank = get_rank()
-            base_outfile, extension = os.path.splitext(task_opt['world_logs'])
-            outfile = base_outfile + f'_{rank}' + extension
-        else:
-            outfile = task_opt['world_logs']
-        world_logger.write(outfile, world, file_format=opt['save_format'])
+    def num_episodes(self) -> int:
+        return len(self.data)
 
-    report = aggregate_unnamed_reports(all_gather_list(world.report()))
+    def num_examples(self) -> int:
+        return len(self.data)
+
+    def _get_save_path(self, datapath: str, date: str) -> str:
+        """
+        Return save path for the controllable gen data.
+
+        :param datapath:
+            path to ParlAI Data
+        :param date:
+            current date
+
+        :return path:
+            return path to save
+        """
+        return os.path.join(
+            datapath,
+            f"{self.original_task_name.replace(':', '_')}_flattened_controllable_gen_{date}",
+        )
 
-    if isinstance(world.agents, list) and len(world.agents) > 1:
-        classifier_agent = world.agents[CLASSIFIER_AGENT]
-        if hasattr(classifier_agent, 'calc_auc') and classifier_agent.calc_auc:
-            for class_indices, curr_auc in zip(
-                classifier_agent.auc_class_indices, classifier_agent.aucs
-            ):
-                report[f'AUC_{classifier_agent.class_list[class_indices]}'] = curr_auc
-            classifier_agent.reset_auc()
-            # for safety measures
-            agent.reset_auc()
-    world.reset()
-    return report
+    @classmethod
+    def build_wordlists(cls, opt: Opt) -> Tuple[List[str], List[str]]:
+        """
+        Load list of explicitly gendered words.
+
+        Words taken from <https://github.com/uclanlp/gn_glove/blob/main/wordlist/>.
+
+        Examples include brother, girl, actress, husbands, etc.
+        """
+        build(opt['datapath'])
+        folder = os.path.join(opt['datapath'], 'genderation_bias')
+        male_words = os.path.join(folder, 'male_word_file.txt')
+        female_words = os.path.join(folder, 'female_word_file.txt')
+
+        with open(male_words, 'r') as f:
+            male = f.read().splitlines()
+
+        with open(female_words, 'r') as f:
+            female = f.read().splitlines()
+
+        return male, female
+
+    def _setup_data(self, opt: Opt) -> List[List[Message]]:
+        """
+        Flatten and classify the normal task data.
+
+        Save/load where applicable.
+
+        :param opt:
+            options dict.
+        """
+        # create save directory, if it does not already exist
+        self.original_task_name = ':'.join(opt['task'].split(':')[2:])
+        self.save_dir = self._get_save_path(
+            opt['datapath'], str(datetime.datetime.today())
+        )
+        os.makedirs(self.save_dir, exist_ok=True)
 
+        fname = f"{opt['datatype'].split(':')[0]}.json"
+        self.save_path = os.path.join(self.save_dir, fname)
 
-def eval_model(opt):
-    """
-    Evaluates a model.
+        data = self.load_data(opt, fname)
+        if data is not None:
+            # successfully load data
+            return data
+
+        # build the original teacher
+        original_task_module = get_original_task_module(opt)
+        teacher_opt = deepcopy(opt)
+        teacher_opt['task'] = self.original_task_name
+        teacher = original_task_module(teacher_opt)
+
+        total_exs = teacher.num_examples()
+        if self.opt['max_examples'] > 0:
+            total_exs = min(self.opt['max_examples'], total_exs)
 
-    :param opt: tells the evaluation function how to run
-    :return: the final result of calling report()
-    """
-    random.seed(42)
-    if 'train' in opt['datatype'] and 'evalmode' not in opt['datatype']:
-        raise ValueError(
-            'You should use --datatype train:evalmode if you want to evaluate on '
-            'the training set.'
+        progress_bar = tqdm(
+            total=total_exs, unit='ex', unit_scale=True, desc='Building flattened data'
         )
 
-    # load model and possibly print opt
-    agent = create_agent(opt, requireModelExists=True)
-    agent.opt.log()
-
-    tb_logger, setting = prepare_tb_logger(opt)
-
-    if tb_logger:
-        n_parleys = get_n_parleys(opt)
-
-    tasks = opt['task'].split(',')
-    reports = []
-    for task in tasks:
-        task_report = _eval_single_world(opt, agent, task)
-        reports.append(task_report)
-        logging.report(f"Report for {task}:\n{nice_report(task_report)}")
-
-    report = aggregate_named_reports(
-        dict(zip(tasks, reports)), micro_average=opt.get('aggregate_micro', False)
-    )
-
-    # print announcements and report
-    print_announcements(opt)
-    logging.info(
-        f'Finished evaluating tasks {tasks} using datatype {opt.get("datatype")}'
-    )
-
-    print(nice_report(report))
-    _save_eval_stats(opt, report)
-    if tb_logger:
-        tb_logger.log_metrics(setting, n_parleys, report)
-        tb_logger.flush()
-    return report
+        all_episodes = []
+        num_exs = 0
+        while num_exs < total_exs:
+            current_episode = []
+            episode_done = False
+
+            while not episode_done:
+                action = Message(teacher.act())
+                current_episode.append(action)
+                episode_done = action.get('episode_done', False)
+                num_exs += 1
+
+            # flatten the episode into 1-example episodes with context
+            flattened_ep = flatten_and_classify(
+                current_episode,
+                opt['flatten_max_context_length'],
+                include_labels=opt['flatten_include_labels'],
+                delimiter=opt['flatten_delimiter'],
+                word_lists=self.word_lists,
+            )
+            all_episodes += flattened_ep
 
+            progress_bar.update(len(flattened_ep))
 
-@register_script('eval_model', aliases=['em', 'eval'])
-class EvalModel(ParlaiScript):
-    @classmethod
-    def setup_args(cls):
-        return setup_args()
+        # save data for future use
+        self.save_data(all_episodes)
 
-    def run(self):
-        return eval_model(self.opt)
+        return all_episodes
+
+    def load_data(self, opt: Opt, filename: str) -> Optional[List[List[Message]]]:
+        """
+        Attempt to load pre-build data.
+
+        Checks for the most recently build data via the date string.
+
+        :param opt:
+            options dict
+        :param filename:
+            name of (potentially) saved data
+
+        :return episodes:
+            return list of episodes, if available
+        """
+        # first check for the most recent date
+        save_dir = self._get_save_path(opt['datapath'], '*')
+        all_dates = []
+        for fname in glob.glob(os.path.join(save_dir, filename)):
+            date = os.path.split(fname)[0].split('_')[-1]
+            all_dates.append(date)
+
+        if len(all_dates) > 0:
+            most_recent = os.path.join(
+                self._get_save_path(opt['datapath'], sorted(all_dates)[-1]), filename
+            )
+        else:
+            # data has not been built yet
+            return None
+
+        if opt['invalidate_cache']:
+            # invalidate the cache and remove the existing data
+            logging.warning(
+                f' [ WARNING: invalidating cache at {self.save_path} and rebuilding the data. ]'
+            )
+            if self.save_path == most_recent:
+                os.remove(self.save_path)
+            return None
+
+        # Loading from most recent date
+        self.save_path = most_recent
+        logging.info(f' [ Data already exists. Loading from: {self.save_path} ]')
+        with PathManager.open(self.save_path, 'rb') as f:
+            data = json.load(f)
+
+        return data
+
+    def save_data(self, data: List[List[Message]]):
+        """
+        Save the data via dumping to a json file.
+
+        :param data:
+            list of episodes
+        """
+        try:
+            json_data = json.dumps(data)
+            with PathManager.open(self.save_path, 'w') as f:
+                f.write(json_data)
+            logging.info(f'[ Data successfully saved to path: {self.save_path} ]')
+        except Exception:
+            logging.warning('Data is not json serializable; not saving')
+
+    def get(self, episode_idx: int, entry_idx: int = 0) -> Message:
+        """
+        Return a flattened example.
+
+        If using a fixed control, put that in instead of what was originally in the text.
+
+        :param episode_idx:
+            index of ep in data
+        :param entry_idx:
+            index of ex in ep
+
+        :return ex:
+            return an example
+        """
+        ex = Message(self.data[episode_idx])
+
+        if self.opt['fixed_control'] != '':
+            old_text = ' '.join(ex['text'].split(' ')[:-1])
+            text = f"{old_text} {self.opt['fixed_control']}"
+            ex.force_set('text', text)
+
+        return ex
+
+    def share(self):
+        shared = super().share()
+        shared['data'] = self.data
+        return shared
 
 
-if __name__ == '__main__':
-    EvalModel.main()
+class DefaultTeacher(ControllableTaskTeacher):
+    pass
```

### Comparing `parlai-1.7.1/parlai/scripts/eval_wordstat.py` & `parlai-1.7.2/parlai/scripts/eval_wordstat.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/extract_image_feature.py` & `parlai-1.7.2/parlai/scripts/extract_image_feature.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/flask.py` & `parlai-1.7.2/parlai/scripts/flask.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/generate_model_card.py` & `parlai-1.7.2/parlai/scripts/generate_model_card.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/interactive.py` & `parlai-1.7.2/parlai/scripts/interactive.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/interactive_web.py` & `parlai-1.7.2/parlai/scripts/interactive_web.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/multiprocessing_eval.py` & `parlai-1.7.2/parlai/scripts/multiprocessing_eval.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 parlai multiprocessing_eval --model-file "zoo:tutorial_transformer_generator/model" --batchsize 16 --task convai2
 ```
 """
 
 import torch
 import os
 import signal
-import parlai.utils.distributed as distributed_utils
 import parlai.scripts.eval_model as eval_model
+import parlai.utils.distributed as distributed_utils
+import parlai.utils.fsdp as fsdp_utils
 from parlai.core.script import ParlaiScript, register_script
 
 
 def multiprocess_eval(
     rank, opt, port=61337, rank_offset=0, gpu=None, hostname='localhost'
 ):
     """
@@ -39,15 +40,17 @@
     Invoked by launch_and_eval, not instantiated directly.
     """
     init_method = f'tcp://{hostname}:{port}'
     with distributed_utils.distributed_context(
         rank, opt, rank_offset, gpu, init_method=init_method
     ) as opt:
         opt['multiprocessing'] = True
-        return eval_model.eval_model(opt)
+        evaluator = fsdp_utils.JoinableEvaluator(opt)
+        with fsdp_utils.fsdp_join(evaluator):
+            return evaluator.eval_model()
 
 
 def launch_and_eval(opt, port):
     """
     Perform a fork() to many processes.
     """
     # Launch multiple subprocesses
```

### Comparing `parlai-1.7.1/parlai/scripts/multiprocessing_train.py` & `parlai-1.7.2/parlai/scripts/multiprocessing_train.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,28 +25,31 @@
 
 import torch
 import os
 import signal
 import traceback
 import parlai.scripts.train_model as single_train
 import parlai.utils.distributed as distributed_utils
+import parlai.utils.fsdp as fsdp_utils
 from parlai.core.script import ParlaiScript, register_script
 
 
 def multiprocess_train(
     rank, opt, port=61337, rank_offset=0, gpu=None, hostname='localhost'
 ):
     init_method = f"tcp://{hostname}:{port}"
     with distributed_utils.distributed_context(
         rank, opt, rank_offset, gpu, init_method=init_method
     ) as opt:
         # Run the actual training
         opt['multiprocessing'] = True
+        loop = fsdp_utils.JoinableTrainLoop(opt)
         try:
-            return single_train.TrainLoop(opt).train()
+            with fsdp_utils.fsdp_join(loop):
+                return loop.train()
         except Exception:
             import parlai.utils.logging as logging
 
             logging.critical(traceback.format_exc())
             logging.critical(
                 f"Got the above exception on worker {rank + rank_offset}. "
                 "This may cause hangs requiring manual killing of processes."
```

### Comparing `parlai-1.7.1/parlai/scripts/party.py` & `parlai-1.7.2/parlai/scripts/party.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/profile_interactive.py` & `parlai-1.7.2/parlai/scripts/profile_interactive.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/profile_train.py` & `parlai-1.7.2/parlai/scripts/profile_train.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/safe_interactive.py` & `parlai-1.7.2/parlai/scripts/safe_interactive.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/self_chat.py` & `parlai-1.7.2/parlai/scripts/self_chat.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/tod_world_script.py` & `parlai-1.7.2/parlai/scripts/tod_world_script.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/token_stats.py` & `parlai-1.7.2/parlai/scripts/token_stats.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/torchscript.py` & `parlai-1.7.2/parlai/scripts/torchscript.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/train_model.py` & `parlai-1.7.2/parlai/scripts/train_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from typing import Tuple
 
 import numpy as np
 
 import parlai.utils.logging as logging
 from parlai.core.agents import create_agent, create_agent_from_shared
 from parlai.core.exceptions import StopTrainException
-from parlai.core.logs import TensorboardLogger, WandbLogger
+from parlai.core.logs import TensorboardLogger, WandbLogger, ClearMLLogger
 from parlai.core.metrics import Metric
 from parlai.core.metrics import (
     aggregate_named_reports,
     aggregate_unnamed_reports,
     dict_report,
 )
 from parlai.core.opt import Opt
@@ -277,14 +277,15 @@
         default='conversations',
         choices=['conversations', 'parlai'],
     )
     train.add_argument('--seed', type=int, default=None)
     WorldLogger.add_cmdline_args(parser, partial_opt=None)
     TensorboardLogger.add_cmdline_args(parser, partial_opt=None)
     WandbLogger.add_cmdline_args(parser, partial_opt=None)
+    ClearMLLogger.add_cmdline_args(parser, partial_opt=None)
     parser = setup_dict_args(parser)
     return parser
 
 
 def set_seed(seed):
     random.seed(seed)
     torch.manual_seed(seed)
@@ -468,14 +469,16 @@
                             f.close()
 
         if opt['tensorboard_log'] and is_primary_worker():
             self.tb_logger = TensorboardLogger(opt)
         if opt['wandb_log'] and is_primary_worker():
             model = self.agent.model if hasattr(self.agent, 'model') else None
             self.wb_logger = WandbLogger(opt, model)
+        if opt['clearml_log'] and is_primary_worker():
+            self.clearml_logger = ClearMLLogger(opt)
 
     def save_model(self, suffix=None):
         """
         Save the model to disk, possibly with a suffix.
         """
         if not self.opt.get('model_file'):
             # nothing to save to, just exit
@@ -563,14 +566,19 @@
             self.tb_logger.log_metrics('valid', self.parleys, valid_report)
             # flush on a validation
             self.tb_logger.flush()
         if opt['wandb_log'] and is_primary_worker():
             valid_report['total_exs'] = self._total_exs
             self.wb_logger.log_metrics('valid', self.parleys, valid_report)
 
+        if opt['clearml_log'] and is_primary_worker():
+            valid_report['total_exs'] = self._total_exs
+            self.clearml_logger.log_metrics('valid', self.parleys, valid_report)
+            self.clearml_logger.flush()
+
         # send valid metrics to agent if the agent wants them
         if hasattr(self.agent, 'receive_metrics'):
             self.agent.receive_metrics(valid_report)
 
         # check which metric to look at
         new_valid = valid_report[opt['validation_metric']]
 
@@ -625,15 +633,17 @@
             opt['validation_patience'] > 0
             and self.impatience >= opt['validation_patience']
         ):
             logging.info('ran out of patience! stopping training.')
             return True
         return False
 
-    def _run_single_eval(self, opt, valid_world, max_exs, datatype, is_multitask, task):
+    def _run_single_eval(
+        self, opt, valid_world, max_exs, datatype, is_multitask, task, index
+    ):
 
         # run evaluation on a single world
         valid_world.reset()
 
         world_logger = None
         task_opt = opt.copy()
         # set up world logger for the "test" fold
@@ -648,14 +658,18 @@
         while not valid_world.epoch_done() and cnt < max_cnt:
             valid_world.parley()
             if world_logger is not None:
                 world_logger.log(valid_world)
             if cnt == 0 and opt['display_examples']:
                 print(valid_world.display() + '\n~~')
                 print(valid_world.report())
+                if opt['clearml_log'] and is_primary_worker():
+                    self.clearml_logger.log_debug_samples(
+                        datatype, valid_world.display(), index=index
+                    )
             cnt = valid_world.report().get('exs') or 0
 
         if world_logger is not None:
             # dump world acts to file
             world_logger.reset()  # add final acts to logs
             if is_distributed():
                 rank = get_rank()
@@ -703,15 +717,15 @@
         is_multitask = len(valid_worlds) > 1
         for index, v_world in enumerate(valid_worlds):
             if opt.get('evaltask'):
                 task = opt['evaltask'].split(',')[index]
             else:
                 task = opt['task'].split(',')[index]
             task_report = self._run_single_eval(
-                opt, v_world, max_exs_per_worker, datatype, is_multitask, task
+                opt, v_world, max_exs_per_worker, datatype, is_multitask, task, index
             )
             reports.append(task_report)
 
         tasks = [world.getID() for world in valid_worlds]
         named_reports = dict(zip(tasks, reports))
         report = aggregate_named_reports(
             named_reports, micro_average=self.opt.get('aggregate_micro', False)
@@ -753,14 +767,16 @@
             final_datatype,
             final_max_exs,
             write_log=True,
             extra_log_suffix="_extra",
         )
         if opt['wandb_log'] and is_primary_worker():
             self.wb_logger.log_final(final_datatype, final_valid_report)
+        if opt['clearml_log'] and is_primary_worker():
+            self.clearml_logger.log_final(final_datatype, final_valid_report)
 
         return final_valid_report
 
     def _sync_metrics(self, metrics):
         """
         Sync training metrics across workers.
 
@@ -894,14 +910,16 @@
         self.log_time.reset()
         self._last_log_steps = 0
 
         if opt['tensorboard_log'] and is_primary_worker():
             self.tb_logger.log_metrics('train', self.parleys, train_report)
         if opt['wandb_log'] and is_primary_worker():
             self.wb_logger.log_metrics('train', self.parleys, train_report)
+        if opt['clearml_log'] and is_primary_worker():
+            self.clearml_logger.log_metrics('train', self.parleys, train_report)
 
         return train_report
 
     def train_steps(self):
         """
         Core training loop.
 
@@ -1022,14 +1040,17 @@
             test_worlds, opt, 'test', max_exs, write_log=True
         )
 
         if opt['wandb_log'] and is_primary_worker():
             self.wb_logger.log_final('valid', self.final_valid_report)
             self.wb_logger.log_final('test', self.final_test_report)
             self.wb_logger.finish()
+        if opt['clearml_log'] and is_primary_worker():
+            self.clearml_logger.log_final('Validation Report', self.final_valid_report)
+            self.clearml_logger.log_final('Test Report', self.final_test_report)
 
         if valid_worlds:
             for valid_world in valid_worlds:
                 valid_world.shutdown()
         if test_worlds:
             for test_world in test_worlds:
                 test_world.shutdown()
@@ -1038,14 +1059,18 @@
 
         if opt['final_extra_opt'] != '':
             self.final_extra_valid_report = self._run_final_extra_eval(opt)
 
         if opt['wandb_log'] and is_primary_worker():
             self.wb_logger.finish()
 
+        if opt['clearml_log'] and is_primary_worker():
+            self.clearml_logger.upload_artifact('dictionary', opt['dict_file'])
+            self.clearml_logger.close()
+
         self._save_train_stats()
 
         return self.final_valid_report, self.final_test_report
 
 
 @register_script('train_model', aliases=['tm', 'train'])
 class TrainModel(ParlaiScript):
```

### Comparing `parlai-1.7.1/parlai/scripts/vacuum.py` & `parlai-1.7.2/parlai/scripts/vacuum.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/scripts/verify_data.py` & `parlai-1.7.2/parlai/scripts/verify_data.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/airdialogue/agents.py` & `parlai-1.7.2/parlai/tasks/airdialogue/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/airdialogue/build.py` & `parlai-1.7.2/parlai/tasks/airdialogue/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/amazon_qa/agents.py` & `parlai-1.7.2/parlai/tasks/amazon_qa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/amazon_qa/build.py` & `parlai-1.7.2/parlai/tasks/amazon_qa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/anli/agents.py` & `parlai-1.7.2/parlai/tasks/anli/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/anli/build.py` & `parlai-1.7.2/parlai/tasks/anli/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/aqua/agents.py` & `parlai-1.7.2/parlai/tasks/mwsc/agents.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,49 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Facebook, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
+#
+# Download and build the data if it does not exist.
 
 from parlai.core.teachers import DialogTeacher
 from parlai.utils.io import PathManager
 from .build import build
-
 import os
-import copy
 import json
 
 
-AQUA = 'AQuA'
-AQUA_QUESTION_KEY = 'question'
-AQUA_ANSWER_KEY = 'correct'
-AQUA_OPTIONS_KEY = 'options'
-AQUA_RATIONALE_KEY = 'rationale'
-RATIONALE_QUESTION_TEXT = 'Can you provide a rationale for your answer?'
-
-
-def _path(opt):
-    build(opt)
-
-    dt = opt['datatype'].split(':')[0]
-
-    if dt == 'train':
-        prefix = 'train'
-    # Using matched set as valid and mismatched set as test
-    elif dt == 'valid':
-        prefix = 'dev'
-    elif dt == 'test':
-        prefix = 'test'
-    else:
-        raise RuntimeError('Not valid datatype.')
-
-    data_path = os.path.join(opt['datapath'], AQUA, AQUA, prefix + '.tok.json')
-
-    return data_path
-
-
-def setup_data(path):
-    print('loading: ' + path)
+class MWSCTeacher(DialogTeacher):
+    def __init__(self, opt, shared=None):
+        # store datatype
+        self.dt = opt['datatype'].split(':')[0]
 
-    with PathManager.open(path, 'r') as data_file:
-        for line in data_file:
-            question = json.loads(line)
-            question_text = question[AQUA_QUESTION_KEY]
-            answer = ord(question[AQUA_ANSWER_KEY]) - ord('A')
-            labels = question[AQUA_OPTIONS_KEY]
-            answer = [labels[answer]]
-            yield (question_text, answer, None, labels), True
+        # store identifier for the teacher in the dialog
+        self.id = 'mwsc'
 
-            # Ask for a rationale now
-            rationale = [question[AQUA_RATIONALE_KEY]]
-            yield (RATIONALE_QUESTION_TEXT, rationale, None, rationale), False
+        build(opt)
+        self.datapath = os.path.join(opt['datapath'], 'MWSC')
+        opt['datafile'] = self._path(opt)
 
+        super().__init__(opt, shared)
 
-class DefaultTeacher(DialogTeacher):
-    def __init__(self, opt, shared=None):
-        opt = copy.deepcopy(opt)
-        data_path = _path(opt)
-        opt['datafile'] = data_path
-        self.id = 'AQuA'
+    def _path(self, opt):
+        build(opt)
+        dt = opt['datatype'].split(':')[0]
+        return os.path.join(self.datapath, dt + '.json')
+
+    def setup_data(self, input_path):
+        print('loading: ' + input_path)
+        new_episode = True
+
+        with PathManager.open(input_path) as file:
+            for l in file:
+                schema_line = json.loads(l.strip())
+                answer = schema_line.get('answer')
+                question = schema_line.get('question')
+                context = schema_line.get('context')
+                yield (context + '\n' + question, [answer], None, None), new_episode
 
-        super().__init__(opt, shared)
 
-    def setup_data(self, path):
-        return setup_data(path)
+class DefaultTeacher(MWSCTeacher):
+    pass
```

### Comparing `parlai-1.7.1/parlai/tasks/aqua/build.py` & `parlai-1.7.2/parlai/tasks/aqua/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/babi/agents.py` & `parlai-1.7.2/parlai/tasks/babi/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/babi/build.py` & `parlai-1.7.2/parlai/tasks/babi/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/blended_skill_talk/agents.py` & `parlai-1.7.2/parlai/tasks/blended_skill_talk/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/blended_skill_talk/build.py` & `parlai-1.7.2/parlai/tasks/blended_skill_talk/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/blended_skill_talk/worlds.py` & `parlai-1.7.2/parlai/tasks/blended_skill_talk/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/booktest/agents.py` & `parlai-1.7.2/parlai/tasks/booktest/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/booktest/build.py` & `parlai-1.7.2/parlai/tasks/booktest/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/bot_adversarial_dialogue/agents.py` & `parlai-1.7.2/parlai/tasks/bot_adversarial_dialogue/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/bot_adversarial_dialogue/build.py` & `parlai-1.7.2/parlai/tasks/bot_adversarial_dialogue/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/bot_adversarial_dialogue/test.py` & `parlai-1.7.2/parlai/tasks/bot_adversarial_dialogue/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/c3/agents.py` & `parlai-1.7.2/parlai/tasks/c3/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/c3/build.py` & `parlai-1.7.2/parlai/tasks/c3/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/casino/agents.py` & `parlai-1.7.2/parlai/tasks/casino/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/casino/build.py` & `parlai-1.7.2/parlai/tasks/casino/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/cbt/agents.py` & `parlai-1.7.2/parlai/tasks/cbt/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/cbt/build.py` & `parlai-1.7.2/parlai/tasks/cbt/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/ccpe/agents.py` & `parlai-1.7.2/parlai/tasks/ccpe/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/ccpe/build.py` & `parlai-1.7.2/parlai/tasks/ccpe/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/clevr/agents.py` & `parlai-1.7.2/parlai/tasks/clevr/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/clevr/build.py` & `parlai-1.7.2/parlai/tasks/clevr/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/cmu_dog/agents.py` & `parlai-1.7.2/parlai/tasks/cmu_dog/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/cmu_dog/build.py` & `parlai-1.7.2/parlai/tasks/cmu_dog/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/cnn_dm/agents.py` & `parlai-1.7.2/parlai/tasks/cnn_dm/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/cnn_dm/build.py` & `parlai-1.7.2/parlai/tasks/cnn_dm/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/coco_caption/agents.py` & `parlai-1.7.2/parlai/tasks/coco_caption/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/coco_caption/build_2014.py` & `parlai-1.7.2/parlai/tasks/coco_caption/build_2014.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/coco_caption/build_2015.py` & `parlai-1.7.2/parlai/tasks/coco_caption/build_2015.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/coco_caption/build_2017.py` & `parlai-1.7.2/parlai/tasks/coco_caption/build_2017.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/commonsenseqa/agents.py` & `parlai-1.7.2/parlai/tasks/commonsenseqa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/commonsenseqa/build.py` & `parlai-1.7.2/parlai/tasks/commonsenseqa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/convai2/agents.py` & `parlai-1.7.2/parlai/tasks/convai2/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/convai2/build.py` & `parlai-1.7.2/parlai/tasks/convai2/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/convai2/test.py` & `parlai-1.7.2/parlai/tasks/convai2/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/convai2/worlds.py` & `parlai-1.7.2/parlai/tasks/convai2/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/convai2_wild_evaluation/agents.py` & `parlai-1.7.2/parlai/tasks/convai2_wild_evaluation/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/convai2_wild_evaluation/build.py` & `parlai-1.7.2/parlai/tasks/convai2_wild_evaluation/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/convai_chitchat/agents.py` & `parlai-1.7.2/parlai/tasks/convai_chitchat/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/convai_chitchat/build.py` & `parlai-1.7.2/parlai/tasks/convai_chitchat/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/copa/agents.py` & `parlai-1.7.2/parlai/tasks/copa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/copa/build.py` & `parlai-1.7.2/parlai/tasks/copa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/coqa/agents.py` & `parlai-1.7.2/parlai/tasks/coqa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/coqa/build.py` & `parlai-1.7.2/parlai/tasks/coqa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/cornell_movie/agents.py` & `parlai-1.7.2/parlai/tasks/cornell_movie/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/cornell_movie/build.py` & `parlai-1.7.2/parlai/tasks/cornell_movie/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dailydialog/agents.py` & `parlai-1.7.2/parlai/tasks/dailydialog/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dailydialog/build.py` & `parlai-1.7.2/parlai/tasks/dailydialog/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dailydialog/parse.py` & `parlai-1.7.2/parlai/tasks/dailydialog/parse.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dbll_babi/agents.py` & `parlai-1.7.2/parlai/tasks/dbll_babi/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dbll_babi/build.py` & `parlai-1.7.2/parlai/tasks/dbll_babi/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dbll_movie/agents.py` & `parlai-1.7.2/parlai/tasks/dbll_movie/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dbll_movie/build.py` & `parlai-1.7.2/parlai/tasks/dbll_movie/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dealnodeal/agents.py` & `parlai-1.7.2/parlai/tasks/dealnodeal/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dealnodeal/build.py` & `parlai-1.7.2/parlai/tasks/dealnodeal/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/decanlp/agents.py` & `parlai-1.7.2/parlai/tasks/decanlp/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/decode/agents.py` & `parlai-1.7.2/parlai/tasks/decode/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/decode/build.py` & `parlai-1.7.2/parlai/tasks/decode/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialog_babi/agents.py` & `parlai-1.7.2/parlai/tasks/dialog_babi/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialog_babi/build.py` & `parlai-1.7.2/parlai/tasks/dialog_babi/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialog_babi_plus/agents.py` & `parlai-1.7.2/parlai/tasks/dialog_babi_plus/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialog_babi_plus/build.py` & `parlai-1.7.2/parlai/tasks/dialog_babi_plus/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialogue_nli/agents.py` & `parlai-1.7.2/parlai/tasks/dialogue_nli/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialogue_nli/build.py` & `parlai-1.7.2/parlai/tasks/dialogue_nli/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialogue_qe/agents.py` & `parlai-1.7.2/parlai/tasks/dialogue_qe/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialogue_qe/build.py` & `parlai-1.7.2/parlai/tasks/dialogue_qe/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialogue_safety/agents.py` & `parlai-1.7.2/parlai/tasks/dialogue_safety/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialogue_safety/base_agent.py` & `parlai-1.7.2/parlai/tasks/dialogue_safety/base_agent.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dialogue_safety/build.py` & `parlai-1.7.2/parlai/tasks/dialogue_safety/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dream/agents.py` & `parlai-1.7.2/parlai/tasks/dream/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dream/build.py` & `parlai-1.7.2/parlai/tasks/dream/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dstc7/agents.py` & `parlai-1.7.2/parlai/tasks/dstc7/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/dstc7/build.py` & `parlai-1.7.2/parlai/tasks/dstc7/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/eli5/agents.py` & `parlai-1.7.2/parlai/tasks/eli5/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/eli5/build.py` & `parlai-1.7.2/parlai/tasks/eli5/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/eli5/data_creation/data_utils.py` & `parlai-1.7.2/parlai/tasks/eli5/data_creation/data_utils.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/eli5/data_creation/download_reddit_qalist.py` & `parlai-1.7.2/parlai/tasks/eli5/data_creation/download_reddit_qalist.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/eli5/data_creation/download_support_docs.py` & `parlai-1.7.2/parlai/tasks/eli5/data_creation/download_support_docs.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/eli5/data_creation/finalize_qda.py` & `parlai-1.7.2/parlai/tasks/eli5/data_creation/finalize_qda.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/eli5/data_creation/merge_support_docs.py` & `parlai-1.7.2/parlai/tasks/eli5/data_creation/merge_support_docs.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/eli5/data_creation/select_sentences_tfidf.py` & `parlai-1.7.2/parlai/tasks/eli5/data_creation/select_sentences_tfidf.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/empathetic_dialogues/agents.py` & `parlai-1.7.2/parlai/tasks/empathetic_dialogues/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/empathetic_dialogues/build.py` & `parlai-1.7.2/parlai/tasks/empathetic_dialogues/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/fits/agents.py` & `parlai-1.7.2/parlai/tasks/fits/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/fits/build.py` & `parlai-1.7.2/parlai/tasks/fits/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/fits/constants.py` & `parlai-1.7.2/parlai/tasks/fits/constants.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/fits/mutators.py` & `parlai-1.7.2/parlai/tasks/fits/mutators.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/fits/test.py` & `parlai-1.7.2/parlai/tasks/fits/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/flickr30k/agents.py` & `parlai-1.7.2/parlai/tasks/flickr30k/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/flickr30k/build.py` & `parlai-1.7.2/parlai/tasks/flickr30k/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/friends/agents.py` & `parlai-1.7.2/parlai/tasks/friends/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/friends/build.py` & `parlai-1.7.2/parlai/tasks/friends/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/friends/test.py` & `parlai-1.7.2/parlai/tasks/friends/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/fromfile/agents.py` & `parlai-1.7.2/parlai/tasks/fromfile/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/funpedia/agents.py` & `parlai-1.7.2/parlai/tasks/funpedia/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/funpedia/build.py` & `parlai-1.7.2/parlai/tasks/funpedia/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/funpedia/test.py` & `parlai-1.7.2/parlai/tasks/funpedia/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/fvqa/agents.py` & `parlai-1.7.2/parlai/tasks/fvqa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/fvqa/build.py` & `parlai-1.7.2/parlai/tasks/fvqa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/genderation_bias/build.py` & `parlai-1.7.2/parlai/tasks/genderation_bias/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/genderation_bias/utils.py` & `parlai-1.7.2/parlai/tasks/genderation_bias/utils.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/glue/agents.py` & `parlai-1.7.2/parlai/tasks/glue/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/glue/test.py` & `parlai-1.7.2/parlai/tasks/glue/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/google_sgd/agents.py` & `parlai-1.7.2/parlai/tasks/google_sgd/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/google_sgd/build.py` & `parlai-1.7.2/parlai/tasks/google_sgd/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/google_sgd_simulation_splits/agents.py` & `parlai-1.7.2/parlai/tasks/google_sgd_simulation_splits/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/google_sgd_simulation_splits/build.py` & `parlai-1.7.2/parlai/tasks/google_sgd_simulation_splits/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/google_sgd_simulation_splits/test.py` & `parlai-1.7.2/parlai/tasks/google_sgd_simulation_splits/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/holl_e/agents.py` & `parlai-1.7.2/parlai/tasks/holl_e/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/holl_e/build.py` & `parlai-1.7.2/parlai/tasks/holl_e/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/hotpotqa/agents.py` & `parlai-1.7.2/parlai/tasks/hotpotqa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/hotpotqa/build.py` & `parlai-1.7.2/parlai/tasks/hotpotqa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/huggingface/agents.py` & `parlai-1.7.2/parlai/tasks/huggingface/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/igc/agents.py` & `parlai-1.7.2/parlai/tasks/igc/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/image_chat/agents.py` & `parlai-1.7.2/parlai/tasks/image_chat/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/image_chat/build.py` & `parlai-1.7.2/parlai/tasks/image_chat/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/image_chat/download_data.py` & `parlai-1.7.2/parlai/tasks/image_chat/download_data.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/insuranceqa/agents.py` & `parlai-1.7.2/parlai/tasks/insuranceqa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/insuranceqa/build.py` & `parlai-1.7.2/parlai/tasks/insuranceqa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/integration_tests/agents.py` & `parlai-1.7.2/parlai/tasks/integration_tests/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/interactive/worlds.py` & `parlai-1.7.2/parlai/tasks/interactive/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/iwslt14/agents.py` & `parlai-1.7.2/parlai/tasks/iwslt14/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/iwslt14/build.py` & `parlai-1.7.2/parlai/tasks/iwslt14/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/jericho_world/agents.py` & `parlai-1.7.2/parlai/tasks/jericho_world/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/jericho_world/build.py` & `parlai-1.7.2/parlai/tasks/jericho_world/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/jericho_world/constants.py` & `parlai-1.7.2/parlai/tasks/jericho_world/constants.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/jericho_world/test.py` & `parlai-1.7.2/parlai/tasks/jericho_world/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/jsonfile/agents.py` & `parlai-1.7.2/parlai/tasks/jsonfile/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/lccc/agents.py` & `parlai-1.7.2/parlai/tasks/lccc/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/lccc/build.py` & `parlai-1.7.2/parlai/tasks/lccc/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/light_dialog/agents.py` & `parlai-1.7.2/parlai/tasks/light_dialog/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/light_dialog/build.py` & `parlai-1.7.2/parlai/tasks/light_dialog/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/light_dialog/builder.py` & `parlai-1.7.2/parlai/tasks/light_dialog/builder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/light_dialog/worlds.py` & `parlai-1.7.2/parlai/tasks/light_dialog/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/light_dialog_wild/agents.py` & `parlai-1.7.2/parlai/tasks/light_dialog_wild/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/light_dialog_wild/build.py` & `parlai-1.7.2/parlai/tasks/light_dialog_wild/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/light_dialog_wild/builder.py` & `parlai-1.7.2/parlai/tasks/light_dialog_wild/builder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/light_genderation_bias/agents.py` & `parlai-1.7.2/parlai/tasks/light_genderation_bias/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/light_genderation_bias/build.py` & `parlai-1.7.2/parlai/tasks/light_genderation_bias/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/mctest/agents.py` & `parlai-1.7.2/parlai/tasks/mctest/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/mctest/build.py` & `parlai-1.7.2/parlai/tasks/mctest/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/agents.py` & `parlai-1.7.2/parlai/tasks/md_gender/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/build.py` & `parlai-1.7.2/parlai/tasks/md_gender/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/convai2.py` & `parlai-1.7.2/parlai/tasks/md_gender/convai2.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/funpedia.py` & `parlai-1.7.2/parlai/tasks/md_gender/funpedia.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/image_chat.py` & `parlai-1.7.2/parlai/tasks/md_gender/image_chat.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/light.py` & `parlai-1.7.2/parlai/tasks/md_gender/light.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/new_data.py` & `parlai-1.7.2/parlai/tasks/md_gender/new_data.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/utils.py` & `parlai-1.7.2/parlai/tasks/md_gender/utils.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/wikipedia.py` & `parlai-1.7.2/parlai/tasks/md_gender/wikipedia.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/wizard.py` & `parlai-1.7.2/parlai/tasks/md_gender/wizard.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/worlds.py` & `parlai-1.7.2/parlai/tasks/md_gender/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/md_gender/yelp.py` & `parlai-1.7.2/parlai/tasks/md_gender/yelp.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/metalwoz/agents.py` & `parlai-1.7.2/parlai/tasks/metalwoz/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/metalwoz/build.py` & `parlai-1.7.2/parlai/tasks/metalwoz/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/mnist_qa/agents.py` & `parlai-1.7.2/parlai/tasks/mnist_qa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/mnist_qa/build.py` & `parlai-1.7.2/parlai/tasks/mnist_qa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/moviedialog/agents.py` & `parlai-1.7.2/parlai/tasks/moviedialog/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/moviedialog/build.py` & `parlai-1.7.2/parlai/tasks/moviedialog/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/ms_marco/agents.py` & `parlai-1.7.2/parlai/tasks/ms_marco/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/ms_marco/build.py` & `parlai-1.7.2/parlai/tasks/ms_marco/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/msc/agents.py` & `parlai-1.7.2/parlai/tasks/msc/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/msc/build.py` & `parlai-1.7.2/parlai/tasks/msc/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/msc/constants.py` & `parlai-1.7.2/parlai/tasks/msc/constants.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/msc/mutators.py` & `parlai-1.7.2/parlai/tasks/msc/mutators.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/msc/test.py` & `parlai-1.7.2/parlai/tasks/msc/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/msr_e2e/agents.py` & `parlai-1.7.2/parlai/tasks/msr_e2e/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/msr_e2e/build.py` & `parlai-1.7.2/parlai/tasks/msr_e2e/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/mturkwikimovies/agents.py` & `parlai-1.7.2/parlai/tasks/mturkwikimovies/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/mturkwikimovies/build.py` & `parlai-1.7.2/parlai/tasks/mturkwikimovies/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multidogo/agents.py` & `parlai-1.7.2/parlai/tasks/multidogo/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multidogo/build.py` & `parlai-1.7.2/parlai/tasks/multidogo/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multinli/agents.py` & `parlai-1.7.2/parlai/tasks/multinli/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multinli/build.py` & `parlai-1.7.2/parlai/tasks/multinli/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multiwoz_v20/agents.py` & `parlai-1.7.2/parlai/tasks/multiwoz_v20/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multiwoz_v20/build.py` & `parlai-1.7.2/parlai/tasks/multiwoz_v20/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multiwoz_v21/agents.py` & `parlai-1.7.2/parlai/tasks/multiwoz_v21/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multiwoz_v21/build.py` & `parlai-1.7.2/parlai/tasks/multiwoz_v21/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multiwoz_v22/agents.py` & `parlai-1.7.2/parlai/tasks/multiwoz_v22/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multiwoz_v22/build.py` & `parlai-1.7.2/parlai/tasks/multiwoz_v22/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multiwoz_v22/build_sha_check_script.py` & `parlai-1.7.2/parlai/tasks/multiwoz_v22/build_sha_check_script.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/multiwoz_v22/test.py` & `parlai-1.7.2/parlai/tasks/multiwoz_v22/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/mutualfriends/agents.py` & `parlai-1.7.2/parlai/tasks/mutualfriends/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/mutualfriends/build.py` & `parlai-1.7.2/parlai/tasks/mutualfriends/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/mwsc/agents.py` & `parlai-1.7.2/parlai/tasks/woz/agents.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,43 +7,69 @@
 # Download and build the data if it does not exist.
 
 from parlai.core.teachers import DialogTeacher
 from parlai.utils.io import PathManager
 from .build import build
 import os
 import json
+import copy
 
+FILE_START = 'woz_'
+FILE_END = '_en.json'
 
-class MWSCTeacher(DialogTeacher):
+
+def _path(opt):
+    build(opt)
+
+    dt = opt['datatype'].split(':')[0]
+
+    if dt == 'train':
+        suffix = 'train'
+    # Using matched set as valid and mismatched set as test
+    elif dt == 'valid':
+        suffix = 'validate'
+    elif dt == 'test':
+        suffix = 'test'
+    else:
+        raise RuntimeError('Not valid datatype.')
+
+    data_path = os.path.join(opt['datapath'], 'WoZ', FILE_START + suffix + FILE_END)
+    return data_path
+
+
+class WoZTeacher(DialogTeacher):
     def __init__(self, opt, shared=None):
+
+        opt = copy.deepcopy(opt)
+        data_path = _path(opt)
+
+        opt['datafile'] = data_path
+
         # store datatype
         self.dt = opt['datatype'].split(':')[0]
 
         # store identifier for the teacher in the dialog
-        self.id = 'mwsc'
+        self.id = 'woz'
 
         build(opt)
-        self.datapath = os.path.join(opt['datapath'], 'MWSC')
-        opt['datafile'] = self._path(opt)
 
         super().__init__(opt, shared)
 
-    def _path(self, opt):
-        build(opt)
-        dt = opt['datatype'].split(':')[0]
-        return os.path.join(self.datapath, dt + '.json')
-
     def setup_data(self, input_path):
         print('loading: ' + input_path)
+
         new_episode = True
 
         with PathManager.open(input_path) as file:
-            for l in file:
-                schema_line = json.loads(l.strip())
-                answer = schema_line.get('answer')
-                question = schema_line.get('question')
-                context = schema_line.get('context')
-                yield (context + '\n' + question, [answer], None, None), new_episode
+            data = json.load(file)
+
+        for dialogue in data:
+            for line in dialogue['dialogue']:
+                answer = [':'.join(turn_label) for turn_label in line['turn_label']]
+                question = "What is the change in the dialogue state?"
+                context = line['transcript']
+                if answer:
+                    yield (context + '\n' + question, answer, None, None), new_episode
 
 
-class DefaultTeacher(MWSCTeacher):
+class DefaultTeacher(WoZTeacher):
     pass
```

### Comparing `parlai-1.7.1/parlai/tasks/mwsc/build.py` & `parlai-1.7.2/parlai/tasks/mwsc/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/narrative_qa/agents.py` & `parlai-1.7.2/parlai/tasks/narrative_qa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/narrative_qa/build.py` & `parlai-1.7.2/parlai/tasks/narrative_qa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/natural_questions/agents.py` & `parlai-1.7.2/parlai/tasks/natural_questions/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/natural_questions/build.py` & `parlai-1.7.2/parlai/tasks/natural_questions/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/natural_questions/build_open.py` & `parlai-1.7.2/parlai/tasks/natural_questions/build_open.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/natural_questions/utils/text_utils.py` & `parlai-1.7.2/parlai/tasks/natural_questions/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/nli/agents.py` & `parlai-1.7.2/parlai/tasks/nli/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/nlvr/agents.py` & `parlai-1.7.2/parlai/tasks/nlvr/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/nlvr/build.py` & `parlai-1.7.2/parlai/tasks/nlvr/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/onecommon/agents.py` & `parlai-1.7.2/parlai/tasks/onecommon/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/onecommon/build.py` & `parlai-1.7.2/parlai/tasks/onecommon/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/opensubtitles/agents.py` & `parlai-1.7.2/parlai/tasks/opensubtitles/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/opensubtitles/build_2009.py` & `parlai-1.7.2/parlai/tasks/opensubtitles/build_2009.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/opensubtitles/build_2018.py` & `parlai-1.7.2/parlai/tasks/opensubtitles/build_2018.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/personachat/agents.py` & `parlai-1.7.2/parlai/tasks/personachat/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/personachat/build.py` & `parlai-1.7.2/parlai/tasks/personachat/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/personachat/test.py` & `parlai-1.7.2/parlai/tasks/personachat/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/personality_captions/agents.py` & `parlai-1.7.2/parlai/tasks/personality_captions/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/personality_captions/build.py` & `parlai-1.7.2/parlai/tasks/personality_captions/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/personality_captions/download_images.py` & `parlai-1.7.2/parlai/tasks/personality_captions/download_images.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/personalized_dialog/agents.py` & `parlai-1.7.2/parlai/tasks/personalized_dialog/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/personalized_dialog/build.py` & `parlai-1.7.2/parlai/tasks/personalized_dialog/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/qacnn/agents.py` & `parlai-1.7.2/parlai/tasks/qacnn/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/qacnn/build.py` & `parlai-1.7.2/parlai/tasks/qacnn/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/qadailymail/agents.py` & `parlai-1.7.2/parlai/tasks/qadailymail/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/qadailymail/build.py` & `parlai-1.7.2/parlai/tasks/qadailymail/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/qangaroo/agents.py` & `parlai-1.7.2/parlai/tasks/qangaroo/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/qangaroo/build.py` & `parlai-1.7.2/parlai/tasks/qangaroo/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/qasrl/agents.py` & `parlai-1.7.2/parlai/tasks/qasrl/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/qasrl/build.py` & `parlai-1.7.2/parlai/tasks/qasrl/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/qazre/agents.py` & `parlai-1.7.2/parlai/tasks/qazre/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/qazre/build.py` & `parlai-1.7.2/parlai/tasks/qazre/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/quac/agents.py` & `parlai-1.7.2/parlai/tasks/quac/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/quac/build.py` & `parlai-1.7.2/parlai/tasks/quac/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/redial/agents.py` & `parlai-1.7.2/parlai/tasks/redial/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/redial/build.py` & `parlai-1.7.2/parlai/tasks/redial/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/saferdialogues/agents.py` & `parlai-1.7.2/parlai/tasks/saferdialogues/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/saferdialogues/build.py` & `parlai-1.7.2/parlai/tasks/saferdialogues/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/safety_mix/agents.py` & `parlai-1.7.2/parlai/tasks/safety_mix/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/safety_mix/build.py` & `parlai-1.7.2/parlai/tasks/safety_mix/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/scan/agents.py` & `parlai-1.7.2/parlai/tasks/scan/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/scan/build.py` & `parlai-1.7.2/parlai/tasks/scan/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/self_chat/worlds.py` & `parlai-1.7.2/parlai/tasks/self_chat/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/sensitive_topics_evaluation/agents.py` & `parlai-1.7.2/parlai/tasks/sensitive_topics_evaluation/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/sensitive_topics_evaluation/build.py` & `parlai-1.7.2/parlai/tasks/sensitive_topics_evaluation/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/simplequestions/agents.py` & `parlai-1.7.2/parlai/tasks/simplequestions/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/simplequestions/build.py` & `parlai-1.7.2/parlai/tasks/simplequestions/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/snli/agents.py` & `parlai-1.7.2/parlai/tasks/snli/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/snli/build.py` & `parlai-1.7.2/parlai/tasks/snli/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/spolin/agents.py` & `parlai-1.7.2/parlai/tasks/spolin/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/spolin/build.py` & `parlai-1.7.2/parlai/tasks/spolin/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/squad/agents.py` & `parlai-1.7.2/parlai/tasks/squad/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/squad/build.py` & `parlai-1.7.2/parlai/tasks/squad/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/squad/test.py` & `parlai-1.7.2/parlai/tasks/squad/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/squad2/agents.py` & `parlai-1.7.2/parlai/tasks/squad2/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/squad2/build.py` & `parlai-1.7.2/parlai/tasks/squad2/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/squad2/test.py` & `parlai-1.7.2/parlai/tasks/squad2/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/sst/agents.py` & `parlai-1.7.2/parlai/tasks/sst/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/sst/build.py` & `parlai-1.7.2/parlai/tasks/sst/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/style_gen/agents.py` & `parlai-1.7.2/parlai/tasks/style_gen/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/style_gen/build.py` & `parlai-1.7.2/parlai/tasks/style_gen/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/style_gen/test.py` & `parlai-1.7.2/parlai/tasks/style_gen/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/superglue/agents.py` & `parlai-1.7.2/parlai/tasks/superglue/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/superglue/test.py` & `parlai-1.7.2/parlai/tasks/superglue/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/task_list.py` & `parlai-1.7.2/parlai/tasks/task_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -486,18 +486,18 @@
         "display_name": "Natural Questions",
         "task": "natural_questions",
         "tags": ["QA"],
         "description": (
             "An open domain question answering dataset. "
             "Each example contains real questions that people searched "
             "for in Google and the content of the a Wikipedia article that "
-            "was amongst the top 5 search resutls for that query, "
+            "was amongst the top 5 search results for that query, "
             "and its annotations. The annotations have the options of a long "
             "answer that is seleced from span of major content entities in "
-            "the Wikipedia article (e.g., paragraphs, tables), a short answer"
+            "the Wikipedia article (e.g., paragraphs, tables), a short answer "
             "that is selected from one or more short span of words in the "
             "article, or 'yes/no'. The existence of any of these answer "
             "formats depends on whether the main question can be answered, "
             "given the article; if not they are left empty."
         ),
         "links": {
             "paper": "https://research.google/pubs/pub47761/",
@@ -538,14 +538,26 @@
         "description": (
             "Simulated dataset of restaurant booking focused on personalization "
             "based on user profiles."
         ),
         "links": {"arXiv": "https://arxiv.org/abs/1706.07503"},
     },
     {
+        "id": "prosocial_dialog",
+        "display_name": "Prosocial Dialog",
+        "task": "prosocial_dialog",
+        "tags": [],
+        "description": (
+            "Prosocial Dialog dataset of 58K dialogues between a speaker showing "
+            "potentially unsafe behavior and a speaker giving constructive feedback "
+            "for more socially acceptable behavior."
+        ),
+        "links": {"arXiv": "https://arxiv.org/abs/2205.12688"},
+    },
+    {
         "id": "QACNN",
         "display_name": "QA CNN",
         "task": "qacnn",
         "tags": ["Cloze"],
         "description": (
             "Cloze dataset based on a missing (anonymized) entity phrase from a "
             "CNN article"
@@ -586,14 +598,26 @@
         "display_name": "Simple Questions",
         "task": "simplequestions",
         "tags": ["QA"],
         "description": ("Open-domain QA dataset based on Freebase triples."),
         "links": {"arXiv": "https://arxiv.org/abs/1506.02075"},
     },
     {
+        "id": "ReframeUnhelpfulThoughts",
+        "display_name": "Reframe Unhelpful Thoughts",
+        "task": "reframe_thoughts",
+        "tags": [],
+        "description": (
+            "Dataset of about 10k examples of thoughts containing unhelpful "
+            "thought patterns conditioned on a given persona, accompanied by about "
+            "27k positive reframes."
+        ),
+        "links": {},
+    },
+    {
         "id": "SNLI",
         "display_name": "The Stanford Natural Language Inference (SNLI) Corpus",
         "task": "snli",
         "tags": ["Entailment"],
         "description": (
             "The SNLI corpus (version 1.0) is a collection of 570k "
             "human-written English sentence pairs manually labeled for balanced "
@@ -667,15 +691,15 @@
         "display_name": "Ubuntu",
         "task": "ubuntu",
         "tags": ["ChitChat", "Dodeca"],
         "description": (
             "Dialogs between an Ubuntu user and an expert trying to fix issue, "
             "we use the V2 version, which cleaned the data to some extent. "
         ),
-        "links": {"arXiv": "https://arxiv.org/abs/1506.08909."},
+        "links": {"arXiv": "https://arxiv.org/abs/1506.08909"},
     },
     {
         "id": "WebQuestions",
         "display_name": "Web Questions",
         "task": "webquestions",
         "tags": ["QA"],
         "description": ("Open-domain QA dataset from Web queries."),
@@ -1439,15 +1463,17 @@
     },
     {
         "id": "TaskMaster3",
         "display_name": "TicketTalk (Taskmaster3)",
         "task": "taskmaster3",
         "tags": ["Goal"],
         "description": (
-            "Taskmaster3 is a dataset of movie ticket dialogues collected in a self-chat manner. To induce conversational variety, crowd workers were asked to generate conversations given dozens of different instructions of different level of specificity, some purposefully including conversational  errors."
+            "Taskmaster3 is a dataset of movie ticket dialogues collected in a self-chat manner. To induce conversational"
+            + "variety, crowd workers were asked to generate conversations given dozens of different instructions of"
+            + "different level of specificity, some purposefully including conversational  errors."
         ),
     },
     {
         "id": "GenderationBiasControlTask",
         "display_name": "GenderationBiasControlTask",
         "task": "genderation_bias:controllable_task",
         "tags": [],
@@ -1536,15 +1562,16 @@
     },
     {
         "id": "CaSiNo",
         "display_name": "CaSiNo (CampSite Negotiation Dialogues)",
         "task": "casino",
         "tags": ["Negotiation"],
         "description": (
-            "A dataset of 1030 negotiation dialogues. Two participants take the role of campsite neighbors and negotiate for Food, Water, and Firewood packages, based on their individual preferences and requirements."
+            "A dataset of 1030 negotiation dialogues. Two participants take the role of campsite neighbors and negotiate for"
+            + "Food, Water, and Firewood packages, based on their individual preferences and requirements."
         ),
         "links": {
             "paper": "https://aclanthology.org/2021.naacl-main.254.pdf",
             "website": "https://github.com/kushalchawla/CaSiNo",
         },
     },
     {
@@ -1584,21 +1611,102 @@
         },
     },
     {
         "id": "SPOLIN",
         "display_name": "SPOLIN",
         "task": "spolin",
         "tags": ["all", "engaging", "improv", "open-ended", "common ground"],
-        "description": "Conversation pairs from the SPOLIN dataset. The pairs abide by the Yes-and principle of improvisational theatre (improv).",
+        "description": "Conversation pairs from the SPOLIN dataset. The pairs abide by the Yes-and principle of"
+        + "improvisational theatre (improv).",
         "links": {
             "arXiv": "https://arxiv.org/abs/2004.09544",
             "website": "https://justin-cho.com/spolin",
         },
     },
     {
         "id": "Feedback for Interactive Talk & Search",
         "display_name": "FITS",
         "task": "fits",
         "tags": ["all", "engaging", "improve", "open-ended"],
-        "description": "A human-model dialogue dataset consist of 14k dialogues where human speakers give feedbacks on bot responses. ",
+        "description": "A human-model dialogue dataset consist of 14k dialogues where human speakers give feedbacks on bot responses.",
+    },
+    {
+        "id": "EntailmentBank",
+        "display_name": "EntailmentBank",
+        "task": "entailment_bank",
+        "tags": ["Entailment", "Reasoning"],
+        "links": {
+            "paper": "https://aclanthology.org/2021.emnlp-main.585.pdf",
+            "website": "https://allenai.org/data/entailmentbank",
+        },
+        "description": (
+            "2k multi-step entailment trees, explaining the answers to ARC science questions."
+        ),
+    },
+    {
+        "id": "ASDIV",
+        "display_name": "ASDIV",
+        "task": "asdiv",
+        "tags": ["Math", "Reasoning"],
+        "links": {
+            "paper": "https://aclanthology.org/2020.acl-main.92.pdf",
+            "website": "https://github.com/chaochun/nlu-asdiv-dataset",
+        },
+        "description": (
+            "A diverse corpus for evaluating and developing English math Wword problem solvers."
+        ),
+    },
+    {
+        "id": "MathDataset",
+        "display_name": "MathDataset",
+        "task": "math_dataset",
+        "tags": ["Math", "Reasoning"],
+        "links": {
+            "paper": "https://arxiv.org/pdf/2103.03874.pdf",
+            "website": "https://github.com/hendrycks/math/",
+        },
+        "description": ("12,500 challenging competition mathematics problems."),
+    },
+    {
+        "id": "EQASC",
+        "display_name": "EQASC",
+        "task": "eqasc",
+        "tags": ["QA", "Reasoning"],
+        "links": {
+            "paper": "https://aclanthology.org/2020.emnlp-main.10.pdf",
+            "website": "https://github.com/harsh19/Reasoning-Chains-MultihopQA",
+        },
+        "description": ("Reasoning chains for multihop question-answering set QASC."),
+    },
+    {
+        "id": "ReasoningFramework",
+        "display_name": "Reasoning Framework",
+        "task": "reasoning",
+        "tags": ["Reasoning"],
+        "description": ("Reasoning teacher framework."),
+    },
+    {
+        "id": "ProofWriter",
+        "display_name": "ProofWriter",
+        "task": "proof_writer",
+        "tags": ["Reasoning"],
+        "links": {
+            "paper": "https://aclanthology.org/2021.findings-acl.317.pdf",
+            "website": "https://allenai.org/data/proofwriter",
+        },
+        "description": (
+            "A synthentically dataset of initial clauses and rules, with questions about statements that these initial"
+            + "clauses and rules imply."
+        ),
+    },
+    {
+        "id": "MultiLIGHT",
+        "display_name": "Multi-party LIGHT",
+        "task": "light_multiparty",
+        "tags": ["All", "ChitChat"],
+        "links": {
+            "paper": "https://arxiv.org/pdf/2304.13835.pdf",
+            "website": "http://parl.ai/projects/light_multiparty",
+        },
+        "description": "Multi-party async conversation between 3 role-playing characters.",
     },
 ]
```

### Comparing `parlai-1.7.1/parlai/tasks/taskmaster/agents.py` & `parlai-1.7.2/parlai/tasks/taskmaster/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/taskmaster/build.py` & `parlai-1.7.2/parlai/tasks/taskmaster/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/taskmaster/test.py` & `parlai-1.7.2/parlai/tasks/taskmaster/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/taskmaster/tm_utils.py` & `parlai-1.7.2/parlai/tasks/taskmaster/tm_utils.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/taskmaster2/agents.py` & `parlai-1.7.2/parlai/tasks/taskmaster2/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/taskmaster2/build.py` & `parlai-1.7.2/parlai/tasks/taskmaster2/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/taskmaster3/agents.py` & `parlai-1.7.2/parlai/tasks/taskmaster3/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/taskmaster3/build.py` & `parlai-1.7.2/parlai/tasks/taskmaster3/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/taskntalk/agents.py` & `parlai-1.7.2/parlai/tasks/taskntalk/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/taskntalk/build.py` & `parlai-1.7.2/parlai/tasks/taskntalk/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/tasks.py` & `parlai-1.7.2/parlai/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/tod_json/agents.py` & `parlai-1.7.2/parlai/tasks/tod_json/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/triviaqa/agents.py` & `parlai-1.7.2/parlai/tasks/triviaqa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/triviaqa/build.py` & `parlai-1.7.2/parlai/tasks/triviaqa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/twitter/agents.py` & `parlai-1.7.2/parlai/tasks/twitter/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/twitter/build.py` & `parlai-1.7.2/parlai/tasks/twitter/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/ubuntu/agents.py` & `parlai-1.7.2/parlai/tasks/ubuntu/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/ubuntu/build.py` & `parlai-1.7.2/parlai/tasks/ubuntu/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/visdial/agents.py` & `parlai-1.7.2/parlai/tasks/visdial/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/visdial/build.py` & `parlai-1.7.2/parlai/tasks/visdial/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/vqa_v1/agents.py` & `parlai-1.7.2/parlai/tasks/vqa_v1/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/vqa_v1/build.py` & `parlai-1.7.2/parlai/tasks/vqa_v1/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/vqa_v2/agents.py` & `parlai-1.7.2/parlai/tasks/vqa_v2/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/vqa_v2/build.py` & `parlai-1.7.2/parlai/tasks/vqa_v2/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/webquestions/agents.py` & `parlai-1.7.2/parlai/tasks/webquestions/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/webquestions/build.py` & `parlai-1.7.2/parlai/tasks/webquestions/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wikimovies/agents.py` & `parlai-1.7.2/parlai/tasks/wikimovies/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wikimovies/build.py` & `parlai-1.7.2/parlai/tasks/wikimovies/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wikipedia/agents.py` & `parlai-1.7.2/parlai/tasks/wikipedia/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wikipedia/build.py` & `parlai-1.7.2/parlai/tasks/wikipedia/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wikiqa/agents.py` & `parlai-1.7.2/parlai/tasks/wikiqa/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wikiqa/build.py` & `parlai-1.7.2/parlai/tasks/wikiqa/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wikisql/agents.py` & `parlai-1.7.2/parlai/tasks/wikisql/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wikisql/build.py` & `parlai-1.7.2/parlai/tasks/wikisql/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wizard_of_internet/agents.py` & `parlai-1.7.2/parlai/tasks/wizard_of_internet/agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     during a full dialogue. Teachers that are drived from this class are
     responsible for slicing data and selecting the actions that they need.
     NOTE: Do NOT use this directly, use its children.
     """
 
     def __init__(self, opt: Opt, shared=None):
         opt = deepcopy(opt)
-        self.datatype = get_dtype(opt)
+        self.datatype = opt.get('datatype', 'train')
         opt['datafile'] = _path(opt)
         self.include_persona = opt.get('include_persona', CONST.INCLUDE_PERSONA_DEFAULT)
         self.skip_empty_text = opt.get(
             'skip_empty_text', CONST.SKIP_ON_EMPTY_TEXT_DEFAULT
         )
         self.text_flatten_delimeter = opt.get('delimiter', '\n')
         self.docs_delim = opt.get('docs_delimiter', '\n')
```

### Comparing `parlai-1.7.1/parlai/tasks/wizard_of_internet/build.py` & `parlai-1.7.2/parlai/tasks/wizard_of_internet/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wizard_of_internet/constants.py` & `parlai-1.7.2/parlai/tasks/wizard_of_internet/constants.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wizard_of_internet/mutators.py` & `parlai-1.7.2/parlai/tasks/wizard_of_internet/mutators.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wizard_of_internet/test.py` & `parlai-1.7.2/parlai/tasks/wizard_of_internet/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/agents.py` & `parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/build.py` & `parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/mutators.py` & `parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/mutators.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/test.py` & `parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wizard_of_wikipedia/worlds.py` & `parlai-1.7.2/parlai/tasks/wizard_of_wikipedia/worlds.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wmt/agents.py` & `parlai-1.7.2/parlai/tasks/wmt/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wmt/build.py` & `parlai-1.7.2/parlai/tasks/wmt/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/woz/build.py` & `parlai-1.7.2/parlai/tasks/woz/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/wrapper/agents.py` & `parlai-1.7.2/parlai/tasks/wrapper/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/xpersona/agents.py` & `parlai-1.7.2/parlai/tasks/xpersona/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/xpersona/build.py` & `parlai-1.7.2/parlai/tasks/xpersona/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/tasks/xpersona/test.py` & `parlai-1.7.2/parlai/tasks/xpersona/test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/torchscript/agents.py` & `parlai-1.7.2/parlai/torchscript/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/torchscript/modules.py` & `parlai-1.7.2/parlai/torchscript/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/torchscript/scripts/test_exported_model.py` & `parlai-1.7.2/parlai/torchscript/scripts/test_exported_model.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/torchscript/tokenizer.py` & `parlai-1.7.2/parlai/torchscript/tokenizer.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/bpe.py` & `parlai-1.7.2/parlai/utils/bpe.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/conversations.py` & `parlai-1.7.2/parlai/utils/conversations.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/curated_response.py` & `parlai-1.7.2/parlai/utils/curated_response.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/data.py` & `parlai-1.7.2/parlai/utils/data.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/distributed.py` & `parlai-1.7.2/parlai/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/flake8.py` & `parlai-1.7.2/parlai/utils/flake8.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/fp16.py` & `parlai-1.7.2/parlai/utils/fp16.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/io.py` & `parlai-1.7.2/parlai/utils/io.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/logging.py` & `parlai-1.7.2/parlai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/misc.py` & `parlai-1.7.2/parlai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/pickle.py` & `parlai-1.7.2/parlai/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/safety.py` & `parlai-1.7.2/parlai/utils/safety.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/strings.py` & `parlai-1.7.2/parlai/utils/strings.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/testing.py` & `parlai-1.7.2/parlai/utils/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,30 @@
     import fairseq  # noqa: F401
 
     FAIRSEQ_AVAILABLE = True
 except ImportError:
     FAIRSEQ_AVAILABLE = False
 
 
+try:
+    import mephisto  # noqa: F401
+
+    MEPHISTO_AVAILABLE = True
+except ImportError:
+    MEPHISTO_AVAILABLE = False
+
+
+try:
+    import clearml  # noqa: F401
+
+    CLEARML__AVAILABLE = True
+except ImportError:
+    CLEARML__AVAILABLE = False
+
+
 def is_this_circleci():
     """
     Return if we are currently running in CircleCI.
     """
     return bool(os.environ.get('CIRCLECI'))
 
 
@@ -82,14 +98,24 @@
     else:
         from packaging import version
 
         skip = version.parse(torch.__version__) < version.parse('1.7.0')
     return unittest.skipIf(skip, reason)(testfn)
 
 
+def skipUnlessTorch113(testfn, reason='Test requires pytorch 1.13+'):
+    if not TORCH_AVAILABLE:
+        skip = True
+    else:
+        from packaging import version
+
+        skip = version.parse(torch.__version__) >= version.parse('1.13')
+    return unittest.skipIf(skip, reason)(testfn)
+
+
 def skipIfGPU(testfn, reason='Test is CPU-only'):
     """
     Decorate a test to skip if a GPU is available.
 
     Useful for disabling hogwild tests.
     """
     return unittest.skipIf(GPU_AVAILABLE, reason)(testfn)
@@ -126,14 +152,28 @@
 def skipUnlessFairseq(testfn, reason='fairseq not installed'):
     """
     Decorate a test to skip unless fairseq is installed.
     """
     return unittest.skipUnless(FAIRSEQ_AVAILABLE, reason)(testfn)
 
 
+def skipUnlessMephisto(testfn, reason='mephisto not installed'):
+    """
+    Decorate a test to skip unless mephisto is installed.
+    """
+    return unittest.skipUnless(MEPHISTO_AVAILABLE, reason)(testfn)
+
+
+def skipUnlessClearML(testfn, reason='clearml not installed'):
+    """
+    Decorate a test to skip unless clearml is installed.
+    """
+    return unittest.skipUnless(CLEARML__AVAILABLE, reason)(testfn)
+
+
 class retry(object):
     """
     Decorator for flaky tests. Test is run up to ntries times, retrying on failure.
 
     :param ntries:
         the number of tries to attempt
     :param log_retry:
```

### Comparing `parlai-1.7.1/parlai/utils/torch.py` & `parlai-1.7.2/parlai/utils/torch.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/typing.py` & `parlai-1.7.2/parlai/utils/typing.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/utils/world_logging.py` & `parlai-1.7.2/parlai/utils/world_logging.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/bart/build.py` & `parlai-1.7.2/parlai/zoo/bart/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/bb3/bb3_3B.py` & `parlai-1.7.2/parlai/zoo/bb3/bb3_3B.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/bb3/persona_summarizer.py` & `parlai-1.7.2/parlai/zoo/bb3/persona_summarizer.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/bert/build.py` & `parlai-1.7.2/parlai/zoo/bert/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blended_skill_talk/bst_single_task.py` & `parlai-1.7.2/parlai/zoo/blended_skill_talk/bst_single_task.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blended_skill_talk/convai2_single_task.py` & `parlai-1.7.2/parlai/zoo/blended_skill_talk/convai2_single_task.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blended_skill_talk/ed_single_task.py` & `parlai-1.7.2/parlai/zoo/blended_skill_talk/ed_single_task.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blended_skill_talk/multi_task.py` & `parlai-1.7.2/parlai/zoo/blended_skill_talk/multi_task.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blended_skill_talk/multi_task_bst_tuned.py` & `parlai-1.7.2/parlai/zoo/blended_skill_talk/multi_task_bst_tuned.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blended_skill_talk/wizard_single_task.py` & `parlai-1.7.2/parlai/zoo/blended_skill_talk/wizard_single_task.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blender/blender_1Bdistill.py` & `parlai-1.7.2/parlai/zoo/blender/blender_1Bdistill.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blender/blender_400Mdistill.py` & `parlai-1.7.2/parlai/zoo/blender/blender_400Mdistill.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blender/build.py` & `parlai-1.7.2/parlai/zoo/blender/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blenderbot2/blenderbot2_3B.py` & `parlai-1.7.2/parlai/zoo/blenderbot2/blenderbot2_3B.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blenderbot2/blenderbot2_400M.py` & `parlai-1.7.2/parlai/zoo/blenderbot2/blenderbot2_400M.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blenderbot2/memory_decoder.py` & `parlai-1.7.2/parlai/zoo/blenderbot2/memory_decoder.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/blenderbot2/query_generator.py` & `parlai-1.7.2/parlai/zoo/blenderbot2/query_generator.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/bot_adversarial_dialogue/multi_turn.py` & `parlai-1.7.2/parlai/zoo/bot_adversarial_dialogue/multi_turn.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/bot_adversarial_dialogue/multi_turn_v0.py` & `parlai-1.7.2/parlai/zoo/bot_adversarial_dialogue/multi_turn_v0.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dialogue_bias/gender__ctrl_gen_tokens.py` & `parlai-1.7.2/parlai/zoo/dialogue_bias/gender__ctrl_gen_tokens.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dialogue_bias/gender__name_scrambling.py` & `parlai-1.7.2/parlai/zoo/dialogue_bias/gender__name_scrambling.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dialogue_bias/gender__unlikelihood_sequence_level.py` & `parlai-1.7.2/parlai/zoo/dialogue_bias/gender__unlikelihood_sequence_level.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dialogue_bias/gender_ethnicity__name_scrambling.py` & `parlai-1.7.2/parlai/zoo/dialogue_bias/gender_ethnicity__name_scrambling.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dialogue_safety/multi_turn.py` & `parlai-1.7.2/parlai/zoo/dialogue_safety/multi_turn.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dialogue_safety/single_turn.py` & `parlai-1.7.2/parlai/zoo/dialogue_safety/single_turn.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/build.py` & `parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_convai2_ctxt_and_label.py` & `parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_convai2_ctxt_and_label.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_eli5_ctxt_and_label.py` & `parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_eli5_ctxt_and_label.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dialogue_unlikelihood/rep_wiki_ctxt_and_label.py` & `parlai-1.7.2/parlai/zoo/dialogue_unlikelihood/rep_wiki_ctxt_and_label.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/dodecadialogue/build.py` & `parlai-1.7.2/parlai/zoo/dodecadialogue/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/fasttext_cc_vectors/build.py` & `parlai-1.7.2/parlai/zoo/fasttext_cc_vectors/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/fasttext_vectors/build.py` & `parlai-1.7.2/parlai/zoo/fasttext_vectors/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/fits/bart_sq_gen.py` & `parlai-1.7.2/parlai/zoo/fits/bart_sq_gen.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/fits/bb2_module_supervision.py` & `parlai-1.7.2/parlai/zoo/fits/bb2_module_supervision.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/fits/director_bb2_module.py` & `parlai-1.7.2/parlai/zoo/fits/director_bb2_module.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/fits/director_seeker_module.py` & `parlai-1.7.2/parlai/zoo/fits/director_seeker_module.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/fits/response_satisfaction.py` & `parlai-1.7.2/parlai/zoo/fits/response_satisfaction.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/fits/seeker_module_supervision.py` & `parlai-1.7.2/parlai/zoo/fits/seeker_module_supervision.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/bart_fid_dpr.py` & `parlai-1.7.2/parlai/zoo/hallucination/bart_fid_dpr.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/bart_fid_rag.py` & `parlai-1.7.2/parlai/zoo/hallucination/bart_fid_rag.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/bart_fid_rag_dpr_poly.py` & `parlai-1.7.2/parlai/zoo/hallucination/bart_fid_rag_dpr_poly.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/bart_rag_dpr_poly.py` & `parlai-1.7.2/parlai/zoo/hallucination/bart_rag_dpr_poly.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/bart_rag_sequence.py` & `parlai-1.7.2/parlai/zoo/hallucination/bart_rag_sequence.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/bart_rag_token.py` & `parlai-1.7.2/parlai/zoo/hallucination/bart_rag_token.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/bart_rag_turn_do.py` & `parlai-1.7.2/parlai/zoo/hallucination/bart_rag_turn_do.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/bart_rag_turn_dtt.py` & `parlai-1.7.2/parlai/zoo/hallucination/bart_rag_turn_dtt.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/dropout_poly.py` & `parlai-1.7.2/parlai/zoo/hallucination/dropout_poly.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/multiset_dpr.py` & `parlai-1.7.2/parlai/zoo/hallucination/multiset_dpr.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/wiki_index_compressed.py` & `parlai-1.7.2/parlai/zoo/hallucination/wiki_index_compressed.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/wiki_index_exact.py` & `parlai-1.7.2/parlai/zoo/hallucination/wiki_index_exact.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/wiki_passages.py` & `parlai-1.7.2/parlai/zoo/hallucination/wiki_passages.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/hallucination/wow_passages.py` & `parlai-1.7.2/parlai/zoo/hallucination/wow_passages.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/image_chat/transresnet_multimodal.py` & `parlai-1.7.2/parlai/zoo/image_chat/transresnet_multimodal.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/light/biranker_dialogue.py` & `parlai-1.7.2/parlai/zoo/light/biranker_dialogue.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/light_whoami/automated_expanded_attention_1024.py` & `parlai-1.7.2/parlai/zoo/light_whoami/automated_expanded_attention_1024.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/light_whoami/expanded_and_multiobjective_1024.py` & `parlai-1.7.2/parlai/zoo/light_whoami/expanded_and_multiobjective_1024.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/light_whoami/profile_expanded_attention_1024.py` & `parlai-1.7.2/parlai/zoo/light_whoami/profile_expanded_attention_1024.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/light_whoami/profile_expanded_attention_128.py` & `parlai-1.7.2/parlai/zoo/light_whoami/profile_expanded_attention_128.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/light_whoami/whoami_download.py` & `parlai-1.7.2/parlai/zoo/light_whoami/whoami_download.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/md_gender/build.py` & `parlai-1.7.2/parlai/zoo/md_gender/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/model_list.py` & `parlai-1.7.2/parlai/zoo/model_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 
 # Copyright (c) Facebook, Inc. and its affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+# flake8: noqa
+
 """
 The Model Zoo.
 
 This file contains a list of all the models in the model zoo, the path to
 load them, agents & tasks associated (e.g. they were trained using) and a
 description. Using the path you should be able to download and use the model
 automatically, e.g.:
@@ -1420,16 +1422,23 @@
     {
         "title": "Style-controlled generation: current-utterance-only classifier",
         "id": "style_gen",
         "path": "zoo:style_gen/curr_only_classifier/model",
         "agent": "projects.style_gen.classifier:ClassifierAgent",
         "task": "style_gen:LabeledBlendedSkillTalk",
         "project": 'https://github.com/facebookresearch/ParlAI/tree/main/projects/style_gen',
-        "description": "Classifier trained on Image-Chat turns 2 and 3 to classify the personality of an example given that utterance as the sole context.",
-        "example": "parlai eval_model --task style_gen:CurrUttOnlyStyle --wrapper-task style_gen:LabeledBlendedSkillTalk --model-file zoo:style_gen/curr_only_classifier/model --model projects.style_gen.classifier:ClassifierAgent --classes-from-file image_chat_personalities_file",
+        "description": (
+            "Classifier trained on Image-Chat turns 2 and 3 to classify the personality"
+            " of an example given that utterance as the sole context."
+        ),
+        "example": """
+        parlai eval_model --task style_gen:CurrUttOnlyStyle --wrapper-task style_gen:LabeledBlendedSkillTalk \
+            --model-file zoo:style_gen/curr_only_classifier/model \
+            --model projects.style_gen.classifier:ClassifierAgent --classes-from-file image_chat_personalities_file
+        """,
         "result": """
 16:46:41 | Finished evaluating tasks ['style_gen:CurrUttOnlyStyle'] using datatype valid
     accuracy  bleu-4  <PER_CLASS_METRICS_SNIPPED>  clen  ctpb  ctps  ctrunc  ctrunclen  exps  exs    f1  gpu_mem  llen  loss    lr  ltpb  ltps  ltrunc  ltrunclen   tpb   tps  \
        .4311 .004642                              19.18 19.18 425.9       0          0  22.2 5651 .4363    .1586 5.633 2.658 5e-10 5.633 125.1       0          0 24.82 550.9
     weighted_f1
           .4319
 """,  # The accuracy is low here because the task was labeled using a different classifier, zoo:style_gen/prev_curr_classifier/model
@@ -3056,8 +3065,72 @@
             "parlai i -mf zoo:bb3/persona_summarizer/model --skip-generation false --inference beam --beam-size 3 --beam-block-ngram 3 --beam-min-length 10"
         ),
         "result": """
             Enter Your Message: I love my job as an AI researcher - I get to work on so many cool problems!
             [Bart]: I am an AI researcher. I love my job.
         """,
     },
+    {
+        "title": "Multi-party speaker prediction",
+        "id": "multilight",
+        "path": "zoo:multilight/speaker/model",
+        "agent": "bart",
+        "task": "light_multiparty:SpeakerPrediction",
+        "project": "https://parl.ai/projects/multilight",
+        "description": (
+            "Predicts the most plausible next speaker at any point during a three-player conversation in LIGHT."
+        ),
+        "example": (
+            """
+            parlai eval_model --model-file zoo:multilight/speaker/model --task light_multiparty:SpeakerPrediction \
+                --add-location-to-context true --add-personas-to-context true --include-speaker-in-label false
+            """
+        ),
+        "result": """
+            Report for light_multiparty:SpeakerPrediction:
+            clen  ctpb  ctps  ctrunc  ctrunclen  exps   exs  gpu_mem  llen  loss    lr  ltpb  ltps  ltrunc  ltrunclen  ppl  token_acc  token_em   tpb  tps
+            473.5 420.2  6130   .4140      54.44 14.59 11005    .1218 3.091 .3438 5e-10 3.091 45.09       0          0 1.41      .8462     .5256 423.3 6175
+            """,  # noqa: E501
+    },
+    {
+        "title": "Multi-party utterance only 3B",
+        "id": "multilight",
+        "path": "zoo:multilight/utterance_3B/model",
+        "agent": "bart",
+        "task": "light_multiparty",
+        "project": "https://parl.ai/projects/multilight",
+        "description": ("Utterance generation model for the multi-party LIGHT game."),
+        "example": (
+            """
+            parlai eval_model --model-file zoo:multilight/utterance_3B/model --task light_multiparty \
+                --add-location-to-context true --add-personas-to-context true --include-speaker-in-label false --add-speaker-to-context-end true
+            """
+        ),
+        "result": """
+            Report for light_multiparty:
+            clen  ctpb  ctps  ctrunc  ctrunclen  exps   exs  gpu_mem  llen  loss    lr  ltpb  ltps  ltrunc  ltrunclen   ppl  token_acc  token_em  tpb  tps
+            478.6 423.2  5603   .4249      56.58 13.24 11005    .7931 15.83 2.584 5e-07 15.83 209.6       0          0 13.25      .4308         0  439 5813
+            """,  # noqa: E501
+    },
+    {
+        "title": "Multi-party utterance only 400m",
+        "id": "multilight",
+        "path": "zoo:multilight/utterance_400m/model",
+        "agent": "bart",
+        "task": "light_multiparty",
+        "project": "https://parl.ai/projects/multilight",
+        "description": (
+            "Utterance generation model for the multi-party LIGHT game. This is the smaller version of the original 3B model presented in the paper."
+        ),
+        "example": (
+            """
+            parlai eval_model --model-file zoo:multilight/utterance_400m/model --task light_multiparty \
+                --add-location-to-context true --add-personas-to-context true --include-speaker-in-label false --add-speaker-to-context-end true
+            """
+        ),
+        "result": """
+            Report for light_multiparty:
+            clen  ctpb  ctps  ctrunc  ctrunclen  exps   exs  gpu_mem  llen  loss    lr  ltpb  ltps  ltrunc  ltrunclen   ppl  token_acc  token_em   tpb  tps
+            477.6 422.6  7264   .4222      56.16 17.19 11005    .1204 15.83 2.714 1e-06 15.83 272.1       0          0 15.08      .4140         0 438.4 7536
+            """,  # noqa: E501
+    },
 ]
```

### Comparing `parlai-1.7.1/parlai/zoo/msc/blender3B_1024.py` & `parlai-1.7.2/parlai/zoo/msc/blender3B_1024.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/msc/dialog_summarizer.py` & `parlai-1.7.2/parlai/zoo/msc/dialog_summarizer.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/msc/msc3B_1024.py` & `parlai-1.7.2/parlai/zoo/msc/msc3B_1024.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/msc/summsc_fidrag3B.py` & `parlai-1.7.2/parlai/zoo/msc/summsc_fidrag3B.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/msc/summsc_rag3B.py` & `parlai-1.7.2/parlai/zoo/msc/summsc_rag3B.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/personality_captions/transresnet.py` & `parlai-1.7.2/parlai/zoo/personality_captions/transresnet.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/pretrained_transformers/build.py` & `parlai-1.7.2/parlai/zoo/pretrained_transformers/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/saferdialogues/build.py` & `parlai-1.7.2/parlai/zoo/saferdialogues/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 from parlai.core.build_data import download_models
 
 
 def download(datapath):
     opt = {'datapath': datapath}
-    version = 'v0.1'
+    version = 'v0.2'
     fnames = [f'models_{version}.tar.gz']
     download_models(
         opt,
         fnames,
         model_folder='saferdialogues',
         version=version,
         use_model_type=False,
```

### Comparing `parlai-1.7.1/parlai/zoo/sea/bart_base.py` & `parlai-1.7.2/parlai/zoo/sea/bart_base.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/sea/bart_fid_sqse.py` & `parlai-1.7.2/parlai/zoo/sea/bart_fid_sqse.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/sea/bart_sq_gen.py` & `parlai-1.7.2/parlai/zoo/sea/bart_sq_gen.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/seeker/seeker_download.py` & `parlai-1.7.2/parlai/zoo/seeker/seeker_download.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/sensitive_topics_classifier/build.py` & `parlai-1.7.2/parlai/zoo/sensitive_topics_classifier/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/style_gen/c75_labeled_dialogue_generator.py` & `parlai-1.7.2/parlai/zoo/style_gen/c75_labeled_dialogue_generator.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/style_gen/curr_only_classifier.py` & `parlai-1.7.2/parlai/zoo/style_gen/curr_only_classifier.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/style_gen/prev_curr_classifier.py` & `parlai-1.7.2/parlai/zoo/style_gen/prev_curr_classifier.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/tod/tod_base_no_api.py` & `parlai-1.7.2/parlai/zoo/tod/tod_base_no_api.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/tod/tod_base_yes_api.py` & `parlai-1.7.2/parlai/zoo/tod/tod_base_yes_api.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/tutorial_transformer_generator/build.py` & `parlai-1.7.2/parlai/zoo/tutorial_transformer_generator/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/unittest/build.py` & `parlai-1.7.2/parlai/zoo/unittest/build.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/wikipedia_full/tfidf_retriever.py` & `parlai-1.7.2/parlai/zoo/wikipedia_full/tfidf_retriever.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/wizard_of_wikipedia/end2end_generator.py` & `parlai-1.7.2/parlai/zoo/wizard_of_wikipedia/end2end_generator.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/wizard_of_wikipedia/full_dialogue_retrieval_model.py` & `parlai-1.7.2/parlai/zoo/wizard_of_wikipedia/full_dialogue_retrieval_model.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai/zoo/wizard_of_wikipedia/knowledge_retriever.py` & `parlai-1.7.2/parlai/zoo/wizard_of_wikipedia/knowledge_retriever.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/parlai.egg-info/PKG-INFO` & `parlai-1.7.2/parlai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: parlai
-Version: 1.7.1
+Version: 1.7.2
 Summary: Unified platform for dialogue research.
 Home-page: http://parl.ai/
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 -----------
 
 [ParlAI](http://parl.ai) (pronounced “par-lay”) is a python framework for
 sharing, training and testing dialogue models, from open-domain chitchat, to
@@ -44,40 +42,62 @@
 
 ## Interactive Tutorial
 
 For those who want to start with ParlAI now, you can try our [Colab Tutorial](https://colab.research.google.com/drive/1bRMvN0lGXaTF5fuTidgvlAl-Lb41F7AD#scrollTo=KtVz5dCUmFkN).
 
 ## Installing ParlAI
 
-ParlAI currently requires Python3.8+ and [Pytorch](https://pytorch.org) 1.6 or higher.
-Dependencies of the core modules are listed in [`requirements.txt`](https://github.com/facebookresearch/ParlAI/blob/main/requirements.txt). Some
-models included (in [`parlai/agents`](https://github.com/facebookresearch/ParlAI/tree/main/parlai/agents)) have additional requirements.
-We *strongly* recommend you install ParlAI in a [venv](https://docs.python.org/3/library/venv.html) or [conda](https://www.anaconda.com/) environment.
+### Operating System
 
-We do not support Windows at this time, but many users [report success on Windows using Python 3.8](https://github.com/facebookresearch/ParlAI/issues/3989) and issues with Python 3.9. We are happy to accept patches that improve Windows support.
+ParlAI should work as inteded under Linux or macOS. We do not support Windows at this time, but many users [report success on Windows using Python 3.8](https://github.com/facebookresearch/ParlAI/issues/3989) and issues with Python 3.9. We are happy to accept patches that improve Windows support.
 
-**Standard Installation**
+### Python Interpreter
+
+ParlAI currently requires Python3.8+.
+
+### Requirements
+
+ParlAI supports [Pytorch](https://pytorch.org) 1.6 or higher.
+All requirements of the core modules are listed in [`requirements.txt`](https://github.com/facebookresearch/ParlAI/blob/main/requirements.txt). However, some models included (in [`parlai/agents`](https://github.com/facebookresearch/ParlAI/tree/main/parlai/agents)) have additional requirements.
+
+## Virtual Environment
+
+We *strongly* recommend you install ParlAI in a virtual environment using [venv](https://docs.python.org/3/library/venv.html) or [conda](https://www.anaconda.com/).
+
+### End User Installation
 
 If you want to use ParlAI without modifications, you can install it with:
 
 ```bash
-pip install parlai
+cd /path/to/your/parlai-app
+python3.8 -m venv venv
+venv/bin/pip install --upgrade pip setuptools wheel
+venv/bin/pip install parlai
 ```
 
-**Development Installation**
+### Developer Installation
 
 Many users will want to modify some parts of ParlAI. To set up a development
 environment, run the following commands to clone the repository and install
 ParlAI:
 
 ```bash
 git clone https://github.com/facebookresearch/ParlAI.git ~/ParlAI
-cd ~/ParlAI; python setup.py develop
+cd ~/ParlAI
+python3.8 -m venv venv
+venv/bin/pip install --upgrade pip setuptools wheel
+venv/bin/python setup.py develop
 ```
 
+> **Note**
+> Sometimes the install from source maynot work due to dependencies (specially in PyTorch related packaged).
+> In that case try building a fresh conda environment and running the similar to the following:
+> `conda install pytorch==2.0.0 torchvision torchaudio torchtext pytorch-cuda=11.8 -c pytorch -c nvidia`.
+> Check torch setup documentation for your CUDA and OS versions.
+
 All needed data will be downloaded to `~/ParlAI/data`. If you need to clear out
 the space used by these files, you can safely delete these directories and any
 files needed will be downloaded again.
 
 ## Documentation
 
  - [Quick Start](https://parl.ai/docs/tutorial_quick.html)
@@ -163,9 +183,7 @@
   journal={arXiv preprint arXiv:{1705.06476}},
   year={2017}
 }
 ```
 
 ## License
 ParlAI is MIT licensed. See the **[LICENSE](https://github.com/facebookresearch/ParlAI/blob/main/LICENSE)** file for details.
-
-
```

### Comparing `parlai-1.7.1/parlai.egg-info/SOURCES.txt` & `parlai-1.7.2/parlai.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,142 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+example_parlai_internal/README.md
 example_parlai_internal/__init__.py
+parlai/README.md
 parlai/__init__.py
 parlai/__main__.py
 parlai.egg-info/PKG-INFO
 parlai.egg-info/SOURCES.txt
 parlai.egg-info/dependency_links.txt
 parlai.egg-info/entry_points.txt
 parlai.egg-info/requires.txt
 parlai.egg-info/top_level.txt
+parlai/agents/README.md
 parlai/agents/__init__.py
+parlai/agents/alice/README.md
 parlai/agents/alice/__init__.py
 parlai/agents/alice/alice.py
+parlai/agents/bart/README.md
 parlai/agents/bart/__init__.py
 parlai/agents/bart/bart.py
 parlai/agents/bart/convert_fairseq_to_parlai.py
 parlai/agents/bart/modules.py
+parlai/agents/bert_classifier/README.md
 parlai/agents/bert_classifier/__init__.py
 parlai/agents/bert_classifier/bert_classifier.py
+parlai/agents/bert_ranker/README.md
 parlai/agents/bert_ranker/__init__.py
 parlai/agents/bert_ranker/bert_dictionary.py
 parlai/agents/bert_ranker/bert_ranker.py
 parlai/agents/bert_ranker/bi_encoder_ranker.py
 parlai/agents/bert_ranker/both_encoder_ranker.py
 parlai/agents/bert_ranker/cross_encoder_ranker.py
 parlai/agents/bert_ranker/helpers.py
+parlai/agents/examples/README.md
 parlai/agents/examples/__init__.py
 parlai/agents/examples/seq2seq.py
 parlai/agents/examples/tra.py
 parlai/agents/examples/transformer_variant.py
+parlai/agents/fid/README.md
 parlai/agents/fid/__init__.py
 parlai/agents/fid/fid.py
+parlai/agents/fixed_response/README.md
 parlai/agents/fixed_response/__init__.py
 parlai/agents/fixed_response/fixed_response.py
+parlai/agents/hred/README.md
 parlai/agents/hred/__init__.py
 parlai/agents/hred/hred.py
 parlai/agents/hred/modules.py
+parlai/agents/hugging_face/README.md
 parlai/agents/hugging_face/__init__.py
 parlai/agents/hugging_face/dialogpt.py
 parlai/agents/hugging_face/dict.py
 parlai/agents/hugging_face/gpt2.py
 parlai/agents/hugging_face/hugging_face.py
 parlai/agents/hugging_face/t5.py
+parlai/agents/image_seq2seq/README.md
 parlai/agents/image_seq2seq/__init__.py
 parlai/agents/image_seq2seq/image_seq2seq.py
 parlai/agents/image_seq2seq/modules.py
+parlai/agents/ir_baseline/README.md
 parlai/agents/ir_baseline/__init__.py
 parlai/agents/ir_baseline/ir_baseline.py
+parlai/agents/local_human/README.md
 parlai/agents/local_human/__init__.py
 parlai/agents/local_human/local_human.py
+parlai/agents/memnn/README.md
 parlai/agents/memnn/__init__.py
 parlai/agents/memnn/memnn.py
 parlai/agents/memnn/modules.py
+parlai/agents/rag/README.md
 parlai/agents/rag/__init__.py
 parlai/agents/rag/args.py
 parlai/agents/rag/conversion_utils.py
 parlai/agents/rag/dpr.py
 parlai/agents/rag/indexers.py
 parlai/agents/rag/model_types.py
 parlai/agents/rag/modules.py
 parlai/agents/rag/polyfaiss.py
 parlai/agents/rag/rag.py
 parlai/agents/rag/retrieve_api.py
 parlai/agents/rag/retrievers.py
 parlai/agents/rag/scripts/__init__.py
 parlai/agents/rag/scripts/generate_dense_embeddings.py
 parlai/agents/rag/scripts/index_dense_embeddings.py
+parlai/agents/random_candidate/README.md
 parlai/agents/random_candidate/__init__.py
 parlai/agents/random_candidate/random_candidate.py
+parlai/agents/repeat_label/README.md
 parlai/agents/repeat_label/__init__.py
 parlai/agents/repeat_label/repeat_label.py
+parlai/agents/repeat_query/README.md
 parlai/agents/repeat_query/__init__.py
 parlai/agents/repeat_query/repeat_query.py
+parlai/agents/reranker/README.md
 parlai/agents/reranker/__init__.py
 parlai/agents/reranker/classifier_gpt2_reranker.py
 parlai/agents/reranker/classifier_reranker.py
 parlai/agents/reranker/reranker.py
+parlai/agents/retriever_reader/README.md
 parlai/agents/retriever_reader/__init__.py
 parlai/agents/retriever_reader/retriever_reader.py
+parlai/agents/safe_local_human/README.md
 parlai/agents/safe_local_human/__init__.py
 parlai/agents/safe_local_human/safe_local_human.py
+parlai/agents/seq2seq/README.md
 parlai/agents/seq2seq/__init__.py
 parlai/agents/seq2seq/modules.py
 parlai/agents/seq2seq/seq2seq.py
+parlai/agents/starspace/README.md
 parlai/agents/starspace/__init__.py
 parlai/agents/starspace/modules.py
 parlai/agents/starspace/starspace.py
+parlai/agents/test_agents/README.md
 parlai/agents/test_agents/__init__.py
 parlai/agents/test_agents/counter.py
 parlai/agents/test_agents/null.py
 parlai/agents/test_agents/test_agents.py
 parlai/agents/test_agents/transformer_generator_prefix.py
 parlai/agents/test_agents/unigram.py
+parlai/agents/tfidf_retriever/README.md
 parlai/agents/tfidf_retriever/__init__.py
 parlai/agents/tfidf_retriever/build_tfidf.py
 parlai/agents/tfidf_retriever/doc_db.py
 parlai/agents/tfidf_retriever/tfidf_doc_ranker.py
 parlai/agents/tfidf_retriever/tfidf_retriever.py
 parlai/agents/tfidf_retriever/utils.py
 parlai/agents/tfidf_retriever/tokenizers/__init__.py
 parlai/agents/tfidf_retriever/tokenizers/regexp_tokenizer.py
 parlai/agents/tfidf_retriever/tokenizers/simple_tokenizer.py
 parlai/agents/tfidf_retriever/tokenizers/spacy_tokenizer.py
 parlai/agents/tfidf_retriever/tokenizers/tokenizer.py
+parlai/agents/transformer/README.md
 parlai/agents/transformer/__init__.py
 parlai/agents/transformer/biencoder.py
 parlai/agents/transformer/classifier.py
 parlai/agents/transformer/crossencoder.py
 parlai/agents/transformer/decoder.py
 parlai/agents/transformer/dropout_poly.py
 parlai/agents/transformer/generator.py
@@ -123,35 +151,39 @@
 parlai/agents/transformer/modules/encoder.py
 parlai/agents/transformer/modules/ffn.py
 parlai/agents/transformer/modules/functions.py
 parlai/agents/transformer/modules/generator.py
 parlai/agents/transformer/modules/mem_net.py
 parlai/agents/transformer/modules/modular.py
 parlai/agents/transformer/modules/wrappers.py
+parlai/agents/unigram/README.md
 parlai/agents/unigram/__init__.py
 parlai/agents/unigram/unigram.py
+parlai/chat_service/README.md
 parlai/chat_service/__init__.py
 parlai/chat_service/core/__init__.py
 parlai/chat_service/core/agents.py
 parlai/chat_service/core/chat_service_manager.py
 parlai/chat_service/core/socket.py
 parlai/chat_service/core/world_runner.py
 parlai/chat_service/core/server/__init__.py
 parlai/chat_service/services/__init__.py
+parlai/chat_service/services/browser_chat/README.md
 parlai/chat_service/services/browser_chat/__init__.py
 parlai/chat_service/services/browser_chat/agents.py
 parlai/chat_service/services/browser_chat/browser_manager.py
 parlai/chat_service/services/browser_chat/client.py
 parlai/chat_service/services/browser_chat/run.py
 parlai/chat_service/services/messenger/__init__.py
 parlai/chat_service/services/messenger/agents.py
 parlai/chat_service/services/messenger/message_sender.py
 parlai/chat_service/services/messenger/messenger_manager.py
 parlai/chat_service/services/messenger/run.py
 parlai/chat_service/services/messenger/worlds.py
+parlai/chat_service/services/terminal_chat/README.md
 parlai/chat_service/services/terminal_chat/__init__.py
 parlai/chat_service/services/terminal_chat/agents.py
 parlai/chat_service/services/terminal_chat/client.py
 parlai/chat_service/services/terminal_chat/run.py
 parlai/chat_service/services/terminal_chat/terminal_manager.py
 parlai/chat_service/services/websocket/__init__.py
 parlai/chat_service/services/websocket/agents.py
@@ -170,14 +202,17 @@
 parlai/chat_service/utils/image.py
 parlai/chat_service/utils/logging.py
 parlai/chat_service/utils/misc.py
 parlai/chat_service/utils/server.py
 parlai/chat_service/utils/timeout.py
 parlai/clib/__init__.py
 parlai/clib/cuda/__init__.py
+parlai/clib/cuda/ngram_repeat_block_cuda.cpp
+parlai/clib/cuda/ngram_repeat_block_cuda_kernel.cu
+parlai/core/README.md
 parlai/core/__init__.py
 parlai/core/agents.py
 parlai/core/build_data.py
 parlai/core/dict.py
 parlai/core/exceptions.py
 parlai/core/image_featurizers.py
 parlai/core/loader.py
@@ -191,72 +226,87 @@
 parlai/core/teachers.py
 parlai/core/torch_agent.py
 parlai/core/torch_classifier_agent.py
 parlai/core/torch_generator_agent.py
 parlai/core/torch_image_agent.py
 parlai/core/torch_ranker_agent.py
 parlai/core/worlds.py
+parlai/core/tod/README.md
 parlai/core/tod/__init__.py
 parlai/core/tod/teacher_metrics.py
 parlai/core/tod/tod_agents.py
 parlai/core/tod/tod_core.py
 parlai/core/tod/tod_world.py
 parlai/core/tod/world_metrics.py
 parlai/core/tod/world_metrics_handlers.py
 parlai/core/tod/tod_test_utils/__init__.py
 parlai/core/tod/tod_test_utils/test_agents.py
+parlai/crowdsourcing/README.md
 parlai/crowdsourcing/__init__.py
 parlai/crowdsourcing/tasks/__init__.py
+parlai/crowdsourcing/tasks/acute_eval/README.md
 parlai/crowdsourcing/tasks/acute_eval/__init__.py
 parlai/crowdsourcing/tasks/acute_eval/acute_eval_agent_state.py
 parlai/crowdsourcing/tasks/acute_eval/acute_eval_blueprint.py
 parlai/crowdsourcing/tasks/acute_eval/acute_eval_builder.py
 parlai/crowdsourcing/tasks/acute_eval/acute_eval_runner.py
 parlai/crowdsourcing/tasks/acute_eval/analysis.py
 parlai/crowdsourcing/tasks/acute_eval/dump_task_to_acute_format.py
 parlai/crowdsourcing/tasks/acute_eval/fast_acute_blueprint.py
 parlai/crowdsourcing/tasks/acute_eval/fast_eval.py
 parlai/crowdsourcing/tasks/acute_eval/run.py
 parlai/crowdsourcing/tasks/acute_eval/util.py
+parlai/crowdsourcing/tasks/chat_demo/README.md
 parlai/crowdsourcing/tasks/chat_demo/__init__.py
 parlai/crowdsourcing/tasks/chat_demo/run.py
+parlai/crowdsourcing/tasks/dialcrowd/README.md
 parlai/crowdsourcing/tasks/dialcrowd/__init__.py
 parlai/crowdsourcing/tasks/dialcrowd/dialcrowd_blueprint.py
 parlai/crowdsourcing/tasks/dialcrowd/run.py
 parlai/crowdsourcing/tasks/dialcrowd/images/__init__.py
+parlai/crowdsourcing/tasks/model_chat/README.md
 parlai/crowdsourcing/tasks/model_chat/__init__.py
 parlai/crowdsourcing/tasks/model_chat/bot_agent.py
 parlai/crowdsourcing/tasks/model_chat/constants.py
 parlai/crowdsourcing/tasks/model_chat/impl.py
 parlai/crowdsourcing/tasks/model_chat/model_chat_blueprint.py
 parlai/crowdsourcing/tasks/model_chat/run.py
 parlai/crowdsourcing/tasks/model_chat/utils.py
 parlai/crowdsourcing/tasks/model_chat/worlds.py
 parlai/crowdsourcing/tasks/model_chat/worlds_image_chat.py
 parlai/crowdsourcing/tasks/model_chat/analysis/__init__.py
 parlai/crowdsourcing/tasks/model_chat/analysis/compile_results.py
 parlai/crowdsourcing/tasks/model_chat/scripts/__init__.py
 parlai/crowdsourcing/tasks/model_chat/scripts/save_image_contexts.py
+parlai/crowdsourcing/tasks/multi_model_chat/README.md
+parlai/crowdsourcing/tasks/multi_model_chat/__init__.py
+parlai/crowdsourcing/tasks/multi_model_chat/agents.py
+parlai/crowdsourcing/tasks/multi_model_chat/compile_results.py
+parlai/crowdsourcing/tasks/multi_model_chat/multiparty_worlds.py
+parlai/crowdsourcing/tasks/pairwise_per_turn_eval/README.md
 parlai/crowdsourcing/tasks/pairwise_per_turn_eval/__init__.py
 parlai/crowdsourcing/tasks/pairwise_per_turn_eval/bot_agent.py
 parlai/crowdsourcing/tasks/pairwise_per_turn_eval/impl.py
 parlai/crowdsourcing/tasks/pairwise_per_turn_eval/per_turn_eval_blueprint.py
 parlai/crowdsourcing/tasks/pairwise_per_turn_eval/run.py
 parlai/crowdsourcing/tasks/pairwise_per_turn_eval/worlds.py
 parlai/crowdsourcing/tasks/pairwise_per_turn_eval/analysis/__init__.py
 parlai/crowdsourcing/tasks/pairwise_per_turn_eval/analysis/compile_results.py
+parlai/crowdsourcing/tasks/qa_data_collection/README.md
 parlai/crowdsourcing/tasks/qa_data_collection/__init__.py
 parlai/crowdsourcing/tasks/qa_data_collection/run.py
 parlai/crowdsourcing/tasks/qa_data_collection/util.py
 parlai/crowdsourcing/tasks/qa_data_collection/worlds.py
+parlai/crowdsourcing/tasks/turn_annotations_static/README.md
 parlai/crowdsourcing/tasks/turn_annotations_static/__init__.py
 parlai/crowdsourcing/tasks/turn_annotations_static/run.py
 parlai/crowdsourcing/tasks/turn_annotations_static/turn_annotations_blueprint.py
 parlai/crowdsourcing/tasks/turn_annotations_static/analysis/__init__.py
 parlai/crowdsourcing/tasks/turn_annotations_static/analysis/compile_results.py
+parlai/crowdsourcing/utils/README.md
 parlai/crowdsourcing/utils/__init__.py
 parlai/crowdsourcing/utils/acceptability.py
 parlai/crowdsourcing/utils/analysis.py
 parlai/crowdsourcing/utils/frontend.py
 parlai/crowdsourcing/utils/mturk.py
 parlai/crowdsourcing/utils/tests.py
 parlai/crowdsourcing/utils/worlds.py
@@ -270,14 +320,15 @@
 parlai/mutators/word_reverse.py
 parlai/mutators/word_shuffle.py
 parlai/nn/__init__.py
 parlai/nn/checkpoint.py
 parlai/nn/lr_scheduler.py
 parlai/ops/__init__.py
 parlai/ops/ngram_repeat_block.py
+parlai/opt_presets/README.md
 parlai/opt_presets/__init__.py
 parlai/opt_presets/docs.py
 parlai/scripts/__init__.py
 parlai/scripts/build_candidates.py
 parlai/scripts/build_dict.py
 parlai/scripts/compare_opts.py
 parlai/scripts/convert_data_to_json_format.py
@@ -306,137 +357,165 @@
 parlai/scripts/self_chat.py
 parlai/scripts/tod_world_script.py
 parlai/scripts/token_stats.py
 parlai/scripts/torchscript.py
 parlai/scripts/train_model.py
 parlai/scripts/vacuum.py
 parlai/scripts/verify_data.py
+parlai/tasks/README.md
 parlai/tasks/__init__.py
 parlai/tasks/task_list.py
 parlai/tasks/tasks.py
 parlai/tasks/airdialogue/__init__.py
 parlai/tasks/airdialogue/agents.py
 parlai/tasks/airdialogue/build.py
 parlai/tasks/airdialogue/test.py
 parlai/tasks/amazon_qa/__init__.py
 parlai/tasks/amazon_qa/agents.py
 parlai/tasks/amazon_qa/build.py
 parlai/tasks/anli/__init__.py
 parlai/tasks/anli/agents.py
 parlai/tasks/anli/build.py
 parlai/tasks/anli/test.py
+parlai/tasks/aqua/README.md
 parlai/tasks/aqua/__init__.py
 parlai/tasks/aqua/agents.py
 parlai/tasks/aqua/build.py
 parlai/tasks/aqua/test.py
+parlai/tasks/asdiv/__init__.py
+parlai/tasks/asdiv/agents.py
+parlai/tasks/asdiv/build.py
+parlai/tasks/babi/README.md
 parlai/tasks/babi/__init__.py
 parlai/tasks/babi/agents.py
 parlai/tasks/babi/build.py
 parlai/tasks/babi/test.py
+parlai/tasks/blended_skill_talk/README.md
 parlai/tasks/blended_skill_talk/__init__.py
 parlai/tasks/blended_skill_talk/agents.py
 parlai/tasks/blended_skill_talk/build.py
 parlai/tasks/blended_skill_talk/test.py
 parlai/tasks/blended_skill_talk/worlds.py
+parlai/tasks/booktest/README.md
 parlai/tasks/booktest/__init__.py
 parlai/tasks/booktest/agents.py
 parlai/tasks/booktest/build.py
+parlai/tasks/bot_adversarial_dialogue/README.md
 parlai/tasks/bot_adversarial_dialogue/__init__.py
 parlai/tasks/bot_adversarial_dialogue/agents.py
 parlai/tasks/bot_adversarial_dialogue/build.py
 parlai/tasks/bot_adversarial_dialogue/test.py
 parlai/tasks/c3/__init__.py
 parlai/tasks/c3/agents.py
 parlai/tasks/c3/build.py
 parlai/tasks/c3/test.py
+parlai/tasks/casino/README.md
 parlai/tasks/casino/__init__.py
 parlai/tasks/casino/agents.py
 parlai/tasks/casino/build.py
 parlai/tasks/casino/test.py
+parlai/tasks/cbt/README.md
 parlai/tasks/cbt/__init__.py
 parlai/tasks/cbt/agents.py
 parlai/tasks/cbt/build.py
 parlai/tasks/cbt/test.py
 parlai/tasks/ccpe/__init__.py
 parlai/tasks/ccpe/agents.py
 parlai/tasks/ccpe/build.py
+parlai/tasks/clevr/README.md
 parlai/tasks/clevr/__init__.py
 parlai/tasks/clevr/agents.py
 parlai/tasks/clevr/build.py
 parlai/tasks/cmu_dog/__init__.py
 parlai/tasks/cmu_dog/agents.py
 parlai/tasks/cmu_dog/build.py
 parlai/tasks/cmu_dog/test.py
+parlai/tasks/cnn_dm/README.md
 parlai/tasks/cnn_dm/__init__.py
 parlai/tasks/cnn_dm/agents.py
 parlai/tasks/cnn_dm/build.py
+parlai/tasks/coco_caption/README.md
 parlai/tasks/coco_caption/__init__.py
 parlai/tasks/coco_caption/agents.py
 parlai/tasks/coco_caption/build_2014.py
 parlai/tasks/coco_caption/build_2015.py
 parlai/tasks/coco_caption/build_2017.py
 parlai/tasks/commonsenseqa/__init__.py
 parlai/tasks/commonsenseqa/agents.py
 parlai/tasks/commonsenseqa/build.py
+parlai/tasks/convai2/README.md
 parlai/tasks/convai2/__init__.py
 parlai/tasks/convai2/agents.py
 parlai/tasks/convai2/build.py
 parlai/tasks/convai2/test.py
 parlai/tasks/convai2/worlds.py
+parlai/tasks/convai2_wild_evaluation/README.md
 parlai/tasks/convai2_wild_evaluation/__init__.py
 parlai/tasks/convai2_wild_evaluation/agents.py
 parlai/tasks/convai2_wild_evaluation/build.py
+parlai/tasks/convai_chitchat/README.md
 parlai/tasks/convai_chitchat/__init__.py
 parlai/tasks/convai_chitchat/agents.py
 parlai/tasks/convai_chitchat/build.py
+parlai/tasks/copa/README.md
 parlai/tasks/copa/__init__.py
 parlai/tasks/copa/agents.py
 parlai/tasks/copa/build.py
+parlai/tasks/coqa/README.md
 parlai/tasks/coqa/__init__.py
 parlai/tasks/coqa/agents.py
 parlai/tasks/coqa/build.py
+parlai/tasks/cornell_movie/README.md
 parlai/tasks/cornell_movie/__init__.py
 parlai/tasks/cornell_movie/agents.py
 parlai/tasks/cornell_movie/build.py
 parlai/tasks/cornell_movie/test.py
+parlai/tasks/dailydialog/README.md
 parlai/tasks/dailydialog/__init__.py
 parlai/tasks/dailydialog/agents.py
 parlai/tasks/dailydialog/build.py
 parlai/tasks/dailydialog/parse.py
 parlai/tasks/dailydialog/test.py
+parlai/tasks/dbll_babi/README.md
 parlai/tasks/dbll_babi/__init__.py
 parlai/tasks/dbll_babi/agents.py
 parlai/tasks/dbll_babi/build.py
 parlai/tasks/dbll_babi/test.py
+parlai/tasks/dbll_movie/README.md
 parlai/tasks/dbll_movie/__init__.py
 parlai/tasks/dbll_movie/agents.py
 parlai/tasks/dbll_movie/build.py
 parlai/tasks/dbll_movie/test.py
+parlai/tasks/dealnodeal/README.md
 parlai/tasks/dealnodeal/__init__.py
 parlai/tasks/dealnodeal/agents.py
 parlai/tasks/dealnodeal/build.py
 parlai/tasks/dealnodeal/test.py
+parlai/tasks/decanlp/README.md
 parlai/tasks/decanlp/__init__.py
 parlai/tasks/decanlp/agents.py
 parlai/tasks/decode/__init__.py
 parlai/tasks/decode/agents.py
 parlai/tasks/decode/build.py
 parlai/tasks/decode/test.py
+parlai/tasks/dialog_babi/README.md
 parlai/tasks/dialog_babi/__init__.py
 parlai/tasks/dialog_babi/agents.py
 parlai/tasks/dialog_babi/build.py
 parlai/tasks/dialog_babi/test.py
+parlai/tasks/dialog_babi_plus/README.md
 parlai/tasks/dialog_babi_plus/__init__.py
 parlai/tasks/dialog_babi_plus/agents.py
 parlai/tasks/dialog_babi_plus/build.py
 parlai/tasks/dialog_babi_plus/test.py
 parlai/tasks/dialogue_nli/__init__.py
 parlai/tasks/dialogue_nli/agents.py
 parlai/tasks/dialogue_nli/build.py
 parlai/tasks/dialogue_nli/test.py
+parlai/tasks/dialogue_qe/README.md
 parlai/tasks/dialogue_qe/__init__.py
 parlai/tasks/dialogue_qe/agents.py
 parlai/tasks/dialogue_qe/build.py
 parlai/tasks/dialogue_qe/test.py
 parlai/tasks/dialogue_safety/__init__.py
 parlai/tasks/dialogue_safety/agents.py
 parlai/tasks/dialogue_safety/base_agent.py
@@ -445,121 +524,158 @@
 parlai/tasks/dream/agents.py
 parlai/tasks/dream/build.py
 parlai/tasks/dream/test.py
 parlai/tasks/dstc7/__init__.py
 parlai/tasks/dstc7/agents.py
 parlai/tasks/dstc7/build.py
 parlai/tasks/dstc7/test.py
+parlai/tasks/eli5/README.md
 parlai/tasks/eli5/__init__.py
 parlai/tasks/eli5/agents.py
 parlai/tasks/eli5/build.py
 parlai/tasks/eli5/data_creation/__init__.py
 parlai/tasks/eli5/data_creation/data_utils.py
 parlai/tasks/eli5/data_creation/download_reddit_qalist.py
 parlai/tasks/eli5/data_creation/download_support_docs.py
 parlai/tasks/eli5/data_creation/finalize_qda.py
 parlai/tasks/eli5/data_creation/merge_support_docs.py
 parlai/tasks/eli5/data_creation/select_sentences_tfidf.py
 parlai/tasks/eli5/data_creation/slurm_scripts/__init__.py
+parlai/tasks/empathetic_dialogues/README.md
 parlai/tasks/empathetic_dialogues/__init__.py
 parlai/tasks/empathetic_dialogues/agents.py
 parlai/tasks/empathetic_dialogues/build.py
 parlai/tasks/empathetic_dialogues/test.py
 parlai/tasks/empathetic_dialogues/worlds.py
+parlai/tasks/entailment_bank/__init__.py
+parlai/tasks/entailment_bank/agents.py
+parlai/tasks/entailment_bank/build.py
+parlai/tasks/eqasc/__init__.py
+parlai/tasks/eqasc/agents.py
+parlai/tasks/eqasc/build.py
 parlai/tasks/fits/__init__.py
 parlai/tasks/fits/agents.py
 parlai/tasks/fits/build.py
 parlai/tasks/fits/constants.py
 parlai/tasks/fits/mutators.py
 parlai/tasks/fits/test.py
+parlai/tasks/flickr30k/README.md
 parlai/tasks/flickr30k/__init__.py
 parlai/tasks/flickr30k/agents.py
 parlai/tasks/flickr30k/build.py
 parlai/tasks/friends/__init__.py
 parlai/tasks/friends/agents.py
 parlai/tasks/friends/build.py
 parlai/tasks/friends/test.py
+parlai/tasks/fromfile/README.md
 parlai/tasks/fromfile/__init__.py
 parlai/tasks/fromfile/agents.py
 parlai/tasks/funpedia/__init__.py
 parlai/tasks/funpedia/agents.py
 parlai/tasks/funpedia/build.py
 parlai/tasks/funpedia/test.py
+parlai/tasks/fvqa/README.md
 parlai/tasks/fvqa/__init__.py
 parlai/tasks/fvqa/agents.py
 parlai/tasks/fvqa/build.py
+parlai/tasks/genderation_bias/README.md
 parlai/tasks/genderation_bias/__init__.py
 parlai/tasks/genderation_bias/agents.py
 parlai/tasks/genderation_bias/build.py
 parlai/tasks/genderation_bias/utils.py
+parlai/tasks/glue/README.md
 parlai/tasks/glue/__init__.py
 parlai/tasks/glue/agents.py
 parlai/tasks/glue/test.py
+parlai/tasks/google_sgd/README.md
 parlai/tasks/google_sgd/__init__.py
 parlai/tasks/google_sgd/agents.py
 parlai/tasks/google_sgd/build.py
 parlai/tasks/google_sgd/test.py
+parlai/tasks/google_sgd_simulation_splits/README.md
 parlai/tasks/google_sgd_simulation_splits/__init__.py
 parlai/tasks/google_sgd_simulation_splits/agents.py
 parlai/tasks/google_sgd_simulation_splits/build.py
 parlai/tasks/google_sgd_simulation_splits/test.py
+parlai/tasks/holl_e/README.md
 parlai/tasks/holl_e/__init__.py
 parlai/tasks/holl_e/agents.py
 parlai/tasks/holl_e/build.py
 parlai/tasks/holl_e/test.py
+parlai/tasks/hotpotqa/README.md
 parlai/tasks/hotpotqa/__init__.py
 parlai/tasks/hotpotqa/agents.py
 parlai/tasks/hotpotqa/build.py
 parlai/tasks/hotpotqa/test.py
+parlai/tasks/huggingface/README.md
 parlai/tasks/huggingface/__init__.py
 parlai/tasks/huggingface/agents.py
 parlai/tasks/igc/__init__.py
 parlai/tasks/igc/agents.py
+parlai/tasks/image_chat/README.md
 parlai/tasks/image_chat/__init__.py
 parlai/tasks/image_chat/agents.py
 parlai/tasks/image_chat/build.py
 parlai/tasks/image_chat/download_data.py
+parlai/tasks/insuranceqa/README.md
 parlai/tasks/insuranceqa/__init__.py
 parlai/tasks/insuranceqa/agents.py
 parlai/tasks/insuranceqa/build.py
 parlai/tasks/insuranceqa/test.py
+parlai/tasks/integration_tests/README.md
 parlai/tasks/integration_tests/__init__.py
 parlai/tasks/integration_tests/agents.py
+parlai/tasks/interactive/README.md
 parlai/tasks/interactive/__init__.py
 parlai/tasks/interactive/agents.py
 parlai/tasks/interactive/worlds.py
+parlai/tasks/iwslt14/README.md
 parlai/tasks/iwslt14/__init__.py
 parlai/tasks/iwslt14/agents.py
 parlai/tasks/iwslt14/build.py
 parlai/tasks/iwslt14/test.py
+parlai/tasks/jericho_world/README.md
 parlai/tasks/jericho_world/__init__.py
 parlai/tasks/jericho_world/agents.py
 parlai/tasks/jericho_world/build.py
 parlai/tasks/jericho_world/constants.py
 parlai/tasks/jericho_world/test.py
+parlai/tasks/jsonfile/README.md
 parlai/tasks/jsonfile/__init__.py
 parlai/tasks/jsonfile/agents.py
 parlai/tasks/lccc/__init__.py
 parlai/tasks/lccc/agents.py
 parlai/tasks/lccc/build.py
 parlai/tasks/lccc/test.py
+parlai/tasks/light_dialog/README.md
 parlai/tasks/light_dialog/__init__.py
 parlai/tasks/light_dialog/agents.py
 parlai/tasks/light_dialog/build.py
 parlai/tasks/light_dialog/builder.py
 parlai/tasks/light_dialog/test.py
 parlai/tasks/light_dialog/worlds.py
+parlai/tasks/light_dialog_wild/README.md
 parlai/tasks/light_dialog_wild/__init__.py
 parlai/tasks/light_dialog_wild/agents.py
 parlai/tasks/light_dialog_wild/build.py
 parlai/tasks/light_dialog_wild/builder.py
 parlai/tasks/light_dialog_wild/test.py
+parlai/tasks/light_genderation_bias/README.md
 parlai/tasks/light_genderation_bias/__init__.py
 parlai/tasks/light_genderation_bias/agents.py
 parlai/tasks/light_genderation_bias/build.py
+parlai/tasks/light_multiparty/README.md
+parlai/tasks/light_multiparty/__init__.py
+parlai/tasks/light_multiparty/agents.py
+parlai/tasks/light_multiparty/build.py
+parlai/tasks/light_multiparty/test.py
+parlai/tasks/math_dataset/__init__.py
+parlai/tasks/math_dataset/agents.py
+parlai/tasks/math_dataset/build.py
+parlai/tasks/mctest/README.md
 parlai/tasks/mctest/__init__.py
 parlai/tasks/mctest/agents.py
 parlai/tasks/mctest/build.py
 parlai/tasks/mctest/test.py
 parlai/tasks/md_gender/__init__.py
 parlai/tasks/md_gender/agents.py
 parlai/tasks/md_gender/build.py
@@ -574,251 +690,324 @@
 parlai/tasks/md_gender/wizard.py
 parlai/tasks/md_gender/worlds.py
 parlai/tasks/md_gender/yelp.py
 parlai/tasks/metalwoz/__init__.py
 parlai/tasks/metalwoz/agents.py
 parlai/tasks/metalwoz/build.py
 parlai/tasks/metalwoz/test.py
+parlai/tasks/mnist_qa/README.md
 parlai/tasks/mnist_qa/__init__.py
 parlai/tasks/mnist_qa/agents.py
 parlai/tasks/mnist_qa/build.py
 parlai/tasks/mnist_qa/test.py
+parlai/tasks/moviedialog/README.md
 parlai/tasks/moviedialog/__init__.py
 parlai/tasks/moviedialog/agents.py
 parlai/tasks/moviedialog/build.py
+parlai/tasks/ms_marco/README.md
 parlai/tasks/ms_marco/__init__.py
 parlai/tasks/ms_marco/agents.py
 parlai/tasks/ms_marco/build.py
 parlai/tasks/msc/__init__.py
 parlai/tasks/msc/agents.py
 parlai/tasks/msc/build.py
 parlai/tasks/msc/constants.py
 parlai/tasks/msc/mutators.py
 parlai/tasks/msc/test.py
 parlai/tasks/msr_e2e/__init__.py
 parlai/tasks/msr_e2e/agents.py
 parlai/tasks/msr_e2e/build.py
 parlai/tasks/msr_e2e/test.py
+parlai/tasks/mturkwikimovies/README.md
 parlai/tasks/mturkwikimovies/__init__.py
 parlai/tasks/mturkwikimovies/agents.py
 parlai/tasks/mturkwikimovies/build.py
 parlai/tasks/multidogo/__init__.py
 parlai/tasks/multidogo/agents.py
 parlai/tasks/multidogo/build.py
 parlai/tasks/multidogo/test.py
+parlai/tasks/multinli/README.md
 parlai/tasks/multinli/__init__.py
 parlai/tasks/multinli/agents.py
 parlai/tasks/multinli/build.py
 parlai/tasks/multinli/test.py
 parlai/tasks/multiwoz_v20/__init__.py
 parlai/tasks/multiwoz_v20/agents.py
 parlai/tasks/multiwoz_v20/build.py
 parlai/tasks/multiwoz_v20/test.py
 parlai/tasks/multiwoz_v21/__init__.py
 parlai/tasks/multiwoz_v21/agents.py
 parlai/tasks/multiwoz_v21/build.py
 parlai/tasks/multiwoz_v21/test.py
+parlai/tasks/multiwoz_v22/README.md
 parlai/tasks/multiwoz_v22/__init__.py
 parlai/tasks/multiwoz_v22/agents.py
 parlai/tasks/multiwoz_v22/build.py
 parlai/tasks/multiwoz_v22/build_sha_check_script.py
 parlai/tasks/multiwoz_v22/test.py
+parlai/tasks/mutualfriends/README.md
 parlai/tasks/mutualfriends/__init__.py
 parlai/tasks/mutualfriends/agents.py
 parlai/tasks/mutualfriends/build.py
+parlai/tasks/mwsc/README.md
 parlai/tasks/mwsc/__init__.py
 parlai/tasks/mwsc/agents.py
 parlai/tasks/mwsc/build.py
+parlai/tasks/narrative_qa/README.md
 parlai/tasks/narrative_qa/__init__.py
 parlai/tasks/narrative_qa/agents.py
 parlai/tasks/narrative_qa/build.py
+parlai/tasks/natural_questions/README.md
 parlai/tasks/natural_questions/__init__.py
 parlai/tasks/natural_questions/agents.py
 parlai/tasks/natural_questions/build.py
 parlai/tasks/natural_questions/build_open.py
 parlai/tasks/natural_questions/test.py
+parlai/tasks/natural_questions/utils/README.md
 parlai/tasks/natural_questions/utils/__init__.py
 parlai/tasks/natural_questions/utils/text_utils.py
 parlai/tasks/nli/__init__.py
 parlai/tasks/nli/agents.py
+parlai/tasks/nlvr/README.md
 parlai/tasks/nlvr/__init__.py
 parlai/tasks/nlvr/agents.py
 parlai/tasks/nlvr/build.py
+parlai/tasks/onecommon/README.md
 parlai/tasks/onecommon/__init__.py
 parlai/tasks/onecommon/agents.py
 parlai/tasks/onecommon/build.py
+parlai/tasks/opensubtitles/README.md
 parlai/tasks/opensubtitles/__init__.py
 parlai/tasks/opensubtitles/agents.py
 parlai/tasks/opensubtitles/build_2009.py
 parlai/tasks/opensubtitles/build_2018.py
+parlai/tasks/personachat/README.md
 parlai/tasks/personachat/__init__.py
 parlai/tasks/personachat/agents.py
 parlai/tasks/personachat/build.py
 parlai/tasks/personachat/test.py
+parlai/tasks/personality_captions/README.md
 parlai/tasks/personality_captions/__init__.py
 parlai/tasks/personality_captions/agents.py
 parlai/tasks/personality_captions/build.py
 parlai/tasks/personality_captions/download_images.py
+parlai/tasks/personalized_dialog/README.md
 parlai/tasks/personalized_dialog/__init__.py
 parlai/tasks/personalized_dialog/agents.py
 parlai/tasks/personalized_dialog/build.py
+parlai/tasks/proof_writer/__init__.py
+parlai/tasks/proof_writer/agents.py
+parlai/tasks/proof_writer/build.py
+parlai/tasks/prosocial_dialog/__init__.py
+parlai/tasks/prosocial_dialog/agents.py
+parlai/tasks/prosocial_dialog/build.py
+parlai/tasks/prosocial_dialog/test.py
+parlai/tasks/qacnn/README.md
 parlai/tasks/qacnn/__init__.py
 parlai/tasks/qacnn/agents.py
 parlai/tasks/qacnn/build.py
+parlai/tasks/qadailymail/README.md
 parlai/tasks/qadailymail/__init__.py
 parlai/tasks/qadailymail/agents.py
 parlai/tasks/qadailymail/build.py
+parlai/tasks/qangaroo/README.md
 parlai/tasks/qangaroo/__init__.py
 parlai/tasks/qangaroo/agents.py
 parlai/tasks/qangaroo/build.py
+parlai/tasks/qasrl/README.md
 parlai/tasks/qasrl/__init__.py
 parlai/tasks/qasrl/agents.py
 parlai/tasks/qasrl/build.py
+parlai/tasks/qazre/README.md
 parlai/tasks/qazre/__init__.py
 parlai/tasks/qazre/agents.py
 parlai/tasks/qazre/build.py
+parlai/tasks/quac/README.md
 parlai/tasks/quac/__init__.py
 parlai/tasks/quac/agents.py
 parlai/tasks/quac/build.py
 parlai/tasks/quac/test.py
+parlai/tasks/reasoning/__init__.py
+parlai/tasks/reasoning/agents.py
+parlai/tasks/reasoning/base.py
+parlai/tasks/reasoning/question_answer.py
+parlai/tasks/reasoning/requirements.txt
+parlai/tasks/reasoning/reason_types/__init__.py
+parlai/tasks/reasoning/reason_types/free_form.py
+parlai/tasks/reasoning/reason_types/step_by_step.py
 parlai/tasks/redial/__init__.py
 parlai/tasks/redial/agents.py
 parlai/tasks/redial/build.py
 parlai/tasks/redial/test.py
+parlai/tasks/reframe_thoughts/__init__.py
+parlai/tasks/reframe_thoughts/agents.py
+parlai/tasks/reframe_thoughts/build.py
+parlai/tasks/reframe_thoughts/test.py
+parlai/tasks/saferdialogues/README.md
 parlai/tasks/saferdialogues/__init__.py
 parlai/tasks/saferdialogues/agents.py
 parlai/tasks/saferdialogues/build.py
 parlai/tasks/saferdialogues/test.py
 parlai/tasks/safety_mix/__init__.py
 parlai/tasks/safety_mix/agents.py
 parlai/tasks/safety_mix/build.py
 parlai/tasks/safety_mix/test.py
+parlai/tasks/scan/README.md
 parlai/tasks/scan/__init__.py
 parlai/tasks/scan/agents.py
 parlai/tasks/scan/build.py
 parlai/tasks/scan/test.py
 parlai/tasks/self_chat/__init__.py
 parlai/tasks/self_chat/agents.py
 parlai/tasks/self_chat/worlds.py
+parlai/tasks/sensitive_topics_evaluation/README.md
 parlai/tasks/sensitive_topics_evaluation/__init__.py
 parlai/tasks/sensitive_topics_evaluation/agents.py
 parlai/tasks/sensitive_topics_evaluation/build.py
+parlai/tasks/simplequestions/README.md
 parlai/tasks/simplequestions/__init__.py
 parlai/tasks/simplequestions/agents.py
 parlai/tasks/simplequestions/build.py
 parlai/tasks/simplequestions/test.py
+parlai/tasks/snli/README.md
 parlai/tasks/snli/__init__.py
 parlai/tasks/snli/agents.py
 parlai/tasks/snli/build.py
 parlai/tasks/snli/test.py
+parlai/tasks/spolin/README.md
 parlai/tasks/spolin/__init__.py
 parlai/tasks/spolin/agents.py
 parlai/tasks/spolin/build.py
 parlai/tasks/spolin/test.py
+parlai/tasks/squad/README.md
 parlai/tasks/squad/__init__.py
 parlai/tasks/squad/agents.py
 parlai/tasks/squad/build.py
 parlai/tasks/squad/test.py
+parlai/tasks/squad2/README.md
 parlai/tasks/squad2/__init__.py
 parlai/tasks/squad2/agents.py
 parlai/tasks/squad2/build.py
 parlai/tasks/squad2/test.py
+parlai/tasks/sst/README.md
 parlai/tasks/sst/__init__.py
 parlai/tasks/sst/agents.py
 parlai/tasks/sst/build.py
 parlai/tasks/sst/test.py
+parlai/tasks/style_gen/README.md
 parlai/tasks/style_gen/__init__.py
 parlai/tasks/style_gen/agents.py
 parlai/tasks/style_gen/build.py
 parlai/tasks/style_gen/test.py
+parlai/tasks/superglue/README.md
 parlai/tasks/superglue/__init__.py
 parlai/tasks/superglue/agents.py
 parlai/tasks/superglue/test.py
 parlai/tasks/taskmaster/__init__.py
 parlai/tasks/taskmaster/agents.py
 parlai/tasks/taskmaster/build.py
 parlai/tasks/taskmaster/test.py
 parlai/tasks/taskmaster/tm_utils.py
+parlai/tasks/taskmaster2/README.md
 parlai/tasks/taskmaster2/__init__.py
 parlai/tasks/taskmaster2/agents.py
 parlai/tasks/taskmaster2/build.py
 parlai/tasks/taskmaster2/test.py
 parlai/tasks/taskmaster3/__init__.py
 parlai/tasks/taskmaster3/agents.py
 parlai/tasks/taskmaster3/build.py
 parlai/tasks/taskmaster3/test.py
+parlai/tasks/taskntalk/README.md
 parlai/tasks/taskntalk/__init__.py
 parlai/tasks/taskntalk/agents.py
 parlai/tasks/taskntalk/build.py
+parlai/tasks/tod_json/README.md
 parlai/tasks/tod_json/__init__.py
 parlai/tasks/tod_json/agents.py
+parlai/tasks/triviaqa/README.md
 parlai/tasks/triviaqa/__init__.py
 parlai/tasks/triviaqa/agents.py
 parlai/tasks/triviaqa/build.py
+parlai/tasks/twitter/README.md
 parlai/tasks/twitter/__init__.py
 parlai/tasks/twitter/agents.py
 parlai/tasks/twitter/build.py
 parlai/tasks/twitter/test.py
+parlai/tasks/ubuntu/README.md
 parlai/tasks/ubuntu/__init__.py
 parlai/tasks/ubuntu/agents.py
 parlai/tasks/ubuntu/build.py
 parlai/tasks/ubuntu/test.py
+parlai/tasks/visdial/README.md
 parlai/tasks/visdial/__init__.py
 parlai/tasks/visdial/agents.py
 parlai/tasks/visdial/build.py
+parlai/tasks/vqa_v1/README.md
 parlai/tasks/vqa_v1/__init__.py
 parlai/tasks/vqa_v1/agents.py
 parlai/tasks/vqa_v1/build.py
+parlai/tasks/vqa_v2/README.md
 parlai/tasks/vqa_v2/__init__.py
 parlai/tasks/vqa_v2/agents.py
 parlai/tasks/vqa_v2/build.py
+parlai/tasks/webquestions/README.md
 parlai/tasks/webquestions/__init__.py
 parlai/tasks/webquestions/agents.py
 parlai/tasks/webquestions/build.py
+parlai/tasks/wikimovies/README.md
 parlai/tasks/wikimovies/__init__.py
 parlai/tasks/wikimovies/agents.py
 parlai/tasks/wikimovies/build.py
 parlai/tasks/wikimovies/test.py
+parlai/tasks/wikipedia/README.md
 parlai/tasks/wikipedia/__init__.py
 parlai/tasks/wikipedia/agents.py
 parlai/tasks/wikipedia/build.py
+parlai/tasks/wikiqa/README.md
 parlai/tasks/wikiqa/__init__.py
 parlai/tasks/wikiqa/agents.py
 parlai/tasks/wikiqa/build.py
 parlai/tasks/wikiqa/test.py
+parlai/tasks/wikisql/README.md
 parlai/tasks/wikisql/__init__.py
 parlai/tasks/wikisql/agents.py
 parlai/tasks/wikisql/build.py
 parlai/tasks/wikisql/test.py
+parlai/tasks/wizard_of_internet/README.md
 parlai/tasks/wizard_of_internet/__init__.py
 parlai/tasks/wizard_of_internet/agents.py
 parlai/tasks/wizard_of_internet/build.py
 parlai/tasks/wizard_of_internet/constants.py
 parlai/tasks/wizard_of_internet/mutators.py
 parlai/tasks/wizard_of_internet/test.py
+parlai/tasks/wizard_of_wikipedia/README.md
 parlai/tasks/wizard_of_wikipedia/__init__.py
 parlai/tasks/wizard_of_wikipedia/agents.py
 parlai/tasks/wizard_of_wikipedia/build.py
 parlai/tasks/wizard_of_wikipedia/mutators.py
 parlai/tasks/wizard_of_wikipedia/test.py
 parlai/tasks/wizard_of_wikipedia/worlds.py
+parlai/tasks/wmt/README.md
 parlai/tasks/wmt/__init__.py
 parlai/tasks/wmt/agents.py
 parlai/tasks/wmt/build.py
 parlai/tasks/wmt/test.py
+parlai/tasks/woz/README.md
 parlai/tasks/woz/__init__.py
 parlai/tasks/woz/agents.py
 parlai/tasks/woz/build.py
 parlai/tasks/woz/test.py
+parlai/tasks/wrapper/README.md
 parlai/tasks/wrapper/__init__.py
 parlai/tasks/wrapper/agents.py
 parlai/tasks/xpersona/__init__.py
 parlai/tasks/xpersona/agents.py
 parlai/tasks/xpersona/build.py
 parlai/tasks/xpersona/test.py
+parlai/torchscript/README.md
 parlai/torchscript/__init__.py
 parlai/torchscript/agents.py
 parlai/torchscript/modules.py
 parlai/torchscript/tokenizer.py
 parlai/torchscript/scripts/__init__.py
 parlai/torchscript/scripts/test_exported_model.py
 parlai/utils/__init__.py
@@ -836,20 +1025,24 @@
 parlai/utils/pickle.py
 parlai/utils/safety.py
 parlai/utils/strings.py
 parlai/utils/testing.py
 parlai/utils/torch.py
 parlai/utils/typing.py
 parlai/utils/world_logging.py
+parlai/zoo/README.md
 parlai/zoo/__init__.py
 parlai/zoo/model_list.py
 parlai/zoo/bart/__init__.py
 parlai/zoo/bart/build.py
+parlai/zoo/bb3/MODEL_LICENSE.md
 parlai/zoo/bb3/__init__.py
 parlai/zoo/bb3/bb3_3B.py
+parlai/zoo/bb3/data_card.md
+parlai/zoo/bb3/model_card.md
 parlai/zoo/bb3/persona_summarizer.py
 parlai/zoo/bb3/images/__init__.py
 parlai/zoo/bert/__init__.py
 parlai/zoo/bert/build.py
 parlai/zoo/blended_skill_talk/__init__.py
 parlai/zoo/blended_skill_talk/bst_single_task.py
 parlai/zoo/blended_skill_talk/convai2_single_task.py
@@ -859,23 +1052,25 @@
 parlai/zoo/blended_skill_talk/wizard_single_task.py
 parlai/zoo/blender/__init__.py
 parlai/zoo/blender/blender_1Bdistill.py
 parlai/zoo/blender/blender_3B.py
 parlai/zoo/blender/blender_400Mdistill.py
 parlai/zoo/blender/blender_90M.py
 parlai/zoo/blender/blender_9B.py
+parlai/zoo/blender/blender_ascii.txt
 parlai/zoo/blender/build.py
 parlai/zoo/blender/dict_3B.py
 parlai/zoo/blender/dict_90M.py
 parlai/zoo/blender/reddit_3B.py
 parlai/zoo/blender/reddit_9B.py
 parlai/zoo/blenderbot2/__init__.py
 parlai/zoo/blenderbot2/blenderbot2_3B.py
 parlai/zoo/blenderbot2/blenderbot2_400M.py
 parlai/zoo/blenderbot2/memory_decoder.py
+parlai/zoo/blenderbot2/model_card.md
 parlai/zoo/blenderbot2/query_generator.py
 parlai/zoo/bot_adversarial_dialogue/__init__.py
 parlai/zoo/bot_adversarial_dialogue/multi_turn.py
 parlai/zoo/bot_adversarial_dialogue/multi_turn_v0.py
 parlai/zoo/dialogue_bias/__init__.py
 parlai/zoo/dialogue_bias/gender__ctrl_gen_tokens.py
 parlai/zoo/dialogue_bias/gender__name_scrambling.py
@@ -964,17 +1159,24 @@
 parlai/zoo/md_gender/build.py
 parlai/zoo/msc/__init__.py
 parlai/zoo/msc/blender3B_1024.py
 parlai/zoo/msc/dialog_summarizer.py
 parlai/zoo/msc/msc3B_1024.py
 parlai/zoo/msc/summsc_fidrag3B.py
 parlai/zoo/msc/summsc_rag3B.py
+parlai/zoo/multilight/__init__.py
+parlai/zoo/multilight/speaker.py
+parlai/zoo/multilight/utils.py
+parlai/zoo/multilight/utterance_3B.py
+parlai/zoo/multilight/utterance_400m.py
+parlai/zoo/multimodal_blenderbot/README.md
 parlai/zoo/multimodal_blenderbot/__init__.py
 parlai/zoo/personality_captions/__init__.py
 parlai/zoo/personality_captions/transresnet.py
+parlai/zoo/pretrained_transformers/README.md
 parlai/zoo/pretrained_transformers/__init__.py
 parlai/zoo/pretrained_transformers/bi_model_huge_reddit.py
 parlai/zoo/pretrained_transformers/bi_model_huge_wikito.py
 parlai/zoo/pretrained_transformers/build.py
 parlai/zoo/pretrained_transformers/cross_model_huge_reddit.py
 parlai/zoo/pretrained_transformers/cross_model_huge_wikito.py
 parlai/zoo/pretrained_transformers/model_bi.py
@@ -984,14 +1186,15 @@
 parlai/zoo/saferdialogues/__init__.py
 parlai/zoo/saferdialogues/build.py
 parlai/zoo/sea/__init__.py
 parlai/zoo/sea/bart_base.py
 parlai/zoo/sea/bart_fid_sqse.py
 parlai/zoo/sea/bart_sq_gen.py
 parlai/zoo/seeker/__init__.py
+parlai/zoo/seeker/model_card.md
 parlai/zoo/seeker/r2c2_base_3B.py
 parlai/zoo/seeker/r2c2_base_400M.py
 parlai/zoo/seeker/r2c2_blenderbot_3B.py
 parlai/zoo/seeker/r2c2_blenderbot_400M.py
 parlai/zoo/seeker/seeker_dialogue_3B.py
 parlai/zoo/seeker/seeker_dialogue_400M.py
 parlai/zoo/seeker/seeker_download.py
@@ -1014,22 +1217,26 @@
 parlai/zoo/unittest/build.py
 parlai/zoo/wikipedia_full/__init__.py
 parlai/zoo/wikipedia_full/tfidf_retriever.py
 parlai/zoo/wizard_of_wikipedia/__init__.py
 parlai/zoo/wizard_of_wikipedia/end2end_generator.py
 parlai/zoo/wizard_of_wikipedia/full_dialogue_retrieval_model.py
 parlai/zoo/wizard_of_wikipedia/knowledge_retriever.py
+projects/README.md
 projects/__init__.py
+projects/anti_scaling/README.md
 projects/anti_scaling/__init__.py
 projects/anti_scaling/distillation.py
 projects/anti_scaling/scripts/__init__.py
 projects/anti_scaling/scripts/remove_projection_matrices.py
+projects/bb3/README.md
 projects/bb3/__init__.py
 projects/bb3/constants.py
 projects/bb3/prompts.py
+projects/bb3/agents/README.md
 projects/bb3/agents/__init__.py
 projects/bb3/agents/module.py
 projects/bb3/agents/opt_api_agent.py
 projects/bb3/agents/opt_bb3_agent.py
 projects/bb3/agents/r2c2_bb3_agent.py
 projects/bb3/agents/search_agent.py
 projects/bb3/agents/utils.py
@@ -1042,33 +1249,40 @@
 projects/bb3/tasks/opt_memory_generation_tasks.py
 projects/bb3/tasks/opt_search_generation_tasks.py
 projects/bb3/tasks/r2c2_decision_tasks.py
 projects/bb3/tasks/r2c2_dialogue_tasks.py
 projects/bb3/tasks/r2c2_knowledge_tasks.py
 projects/bb3/tasks/r2c2_memory_generation_tasks.py
 projects/bb3/tasks/r2c2_search_generation_tasks.py
+projects/blenderbot2/README.md
 projects/blenderbot2/__init__.py
+projects/blenderbot2/agents/README.md
 projects/blenderbot2/agents/__init__.py
 projects/blenderbot2/agents/blenderbot2.py
 projects/blenderbot2/agents/modules.py
 projects/blenderbot2/agents/sub_modules.py
+projects/dialogue_unlikelihood/README.md
 projects/dialogue_unlikelihood/__init__.py
 projects/dialogue_unlikelihood/agents.py
+projects/image_chat/README.md
 projects/image_chat/__init__.py
 projects/image_chat/interactive.py
 projects/image_chat/transresnet_multimodal/__init__.py
 projects/image_chat/transresnet_multimodal/modules.py
 projects/image_chat/transresnet_multimodal/transresnet_multimodal.py
+projects/multimodal_blenderbot/README.md
 projects/multimodal_blenderbot/__init__.py
 projects/multimodal_blenderbot/agents.py
+projects/personality_captions/README.md
 projects/personality_captions/__init__.py
 projects/personality_captions/interactive.py
 projects/personality_captions/transresnet/__init__.py
 projects/personality_captions/transresnet/modules.py
 projects/personality_captions/transresnet/transresnet.py
+projects/safety_bench/README.md
 projects/safety_bench/__init__.py
 projects/safety_bench/prepare_integration_tests.py
 projects/safety_bench/run_unit_tests.py
 projects/safety_bench/model_wrappers/__init__.py
 projects/safety_bench/model_wrappers/example_wrapper.py
 projects/safety_bench/model_wrappers/gpt_wrappers.py
 projects/safety_bench/model_wrappers/parlai_model_zoo_wrappers.py
@@ -1076,14 +1290,15 @@
 projects/safety_bench/unit_tests/generate_offensive_language_test.py
 projects/safety_bench/unit_tests/response_to_offensive_language_test.py
 projects/safety_bench/utils/__init__.py
 projects/safety_bench/utils/colors.py
 projects/safety_bench/utils/perspective_api.py
 projects/safety_bench/utils/safety_testing.py
 projects/safety_bench/utils/wrapper_loading.py
+projects/seeker/README.md
 projects/seeker/__init__.py
 projects/seeker/utils.py
 projects/seeker/agents/__init__.py
 projects/seeker/agents/gpt2_seeker.py
 projects/seeker/agents/gpt2_seeker_modules.py
 projects/seeker/agents/modular_agent.py
 projects/seeker/agents/seeker.py
@@ -1093,31 +1308,34 @@
 projects/seeker/tasks/__init__.py
 projects/seeker/tasks/dialogue.py
 projects/seeker/tasks/knowledge.py
 projects/seeker/tasks/lm.py
 projects/seeker/tasks/mutators.py
 projects/seeker/tasks/search_decision.py
 projects/seeker/tasks/search_query.py
+projects/style_gen/README.md
 projects/style_gen/__init__.py
 projects/style_gen/classifier.py
 projects/style_gen/modules.py
 projects/style_gen/style_gen.py
+projects/tod_simulator/README.md
 projects/tod_simulator/__init__.py
 projects/tod_simulator/scripts/__init__.py
 projects/tod_simulator/scripts/cleanup_conversation.py
 projects/tod_simulator/scripts/do_get_passing_only_on_dir.py
 projects/tod_simulator/scripts/get_al_samples_for_gsgd.py
 projects/tod_simulator/scripts/get_api_data.py
 projects/tod_simulator/scripts/get_interdistinct_on_conversations.py
 projects/tod_simulator/scripts/get_passing_only.py
 projects/tod_simulator/scripts/get_quick_eval_stats.py
 projects/tod_simulator/scripts/tod_distributed_uber_script.py
 projects/tod_simulator/tod_world_configs/__init__.py
 projects/tod_simulator/world_metrics/__init__.py
 projects/tod_simulator/world_metrics/extended_world_metrics.py
+projects/wizard_of_wikipedia/README.md
 projects/wizard_of_wikipedia/__init__.py
 projects/wizard_of_wikipedia/generator/__init__.py
 projects/wizard_of_wikipedia/generator/agents.py
 projects/wizard_of_wikipedia/generator/modules.py
 projects/wizard_of_wikipedia/generator/train_end2end.py
 projects/wizard_of_wikipedia/knowledge_retriever/__init__.py
 projects/wizard_of_wikipedia/knowledge_retriever/knowledge_retriever.py
```

### Comparing `parlai-1.7.1/parlai.egg-info/requires.txt` & `parlai-1.7.2/parlai.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 coloredlogs
 datasets<2.2.2,>=1.4.1
 docutils<0.16,>=0.14
 emoji
 fairscale~=0.4.1
-docformatter
+docformatter~=1.4.0
 flake8-bugbear
 flake8
 fuzzywuzzy
 google-cloud-storage
-importlib-metadata<4.3
 iopath~=0.1.8
 gitdb2
 GitPython
 hydra-core>=1.1.0
 ipython
-torch>=1.4.0
+torch
+torchvision
 joblib
 nltk
 omegaconf>=2.1.1
 pandas
 pytest_regressions
 pytest
 pexpect
 Pillow
 py-gfm
 py-rouge
 pyyaml
 pyzmq
 regex>=2021.8.3
-myst-parser~=0.12.2
+myst-parser<1
 attrs~=20.2.0
 requests-mock
 requests<3,>=2.21.0
 scikit-learn
 scipy
 sh
 sphinx_rtd_theme
 sphinx-autodoc-typehints~=1.10.3
-Sphinx~=2.2.0
+Sphinx~=5.1.0
 subword-nmt
-tensorboardX
+tensorboardX<=2.5.0
 tokenizers>=0.8.0
 tomli>=2.0.0
-torchtext>=0.5.0
+torchtext
 tornado
 tqdm~=4.62.1
 typing-extensions
 Unidecode
-urllib3>=1.26.5
+urllib3<1.27,>=1.26.5
 websocket-client
 jsonlines
-numpy~=1.22
+numpy~=1.23.0
 markdown<=3.3.2
 jinja2
 ninja~=1.10.2.3
-protobuf~=3.20
+protobuf<=3.20.3,>=3.8.0
 contractions~=0.1.72
 fsspec~=2022.2.0
+google-api-core<=2.11.0
```

### Comparing `parlai-1.7.1/projects/anti_scaling/distillation.py` & `parlai-1.7.2/projects/anti_scaling/distillation.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/anti_scaling/scripts/remove_projection_matrices.py` & `parlai-1.7.2/projects/anti_scaling/scripts/remove_projection_matrices.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/agents/module.py` & `parlai-1.7.2/projects/bb3/agents/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,23 +23,25 @@
     SEARCH_KNOWLEDGE = 'skm'
     CONTEXTUAL_DIALOGUE = 'crm'
     MEMORY_DIALOGUE = 'mrm'
     SEARCH_DIALOGUE = 'srm'
     VANILLA_DIALOGUE = 'vrm'
     GROUNDED_DIALOGUE = 'grm'
     OPENING_DIALOGUE = 'orm'
+    BOT_DIALOGUE = 'brm'
 
     @staticmethod
     def dialogue_modules() -> List['Module']:
         return [
             Module.CONTEXTUAL_DIALOGUE,
             Module.MEMORY_DIALOGUE,
             Module.SEARCH_DIALOGUE,
             Module.VANILLA_DIALOGUE,
             Module.GROUNDED_DIALOGUE,
+            Module.BOT_DIALOGUE,
             Module.OPENING_DIALOGUE,
         ]
 
     @staticmethod
     def knowledge_modules() -> List['Module']:
         return [
             Module.CONTEXTUAL_KNOWLEDGE,
@@ -111,14 +113,15 @@
             'skm': 'search_knowledge',
             'crm': 'contextual_dialogue',
             'mrm': 'memory_dialogue',
             'srm': 'search_dialogue',
             'vrm': 'vanilla_dialogue',
             'grm': 'grounded_dialogue',
             'orm': 'opening_dialogue',
+            'brm': 'bot_dialogue',
         }
 
     ##############
     # R2C2 Func. #
     ##############
     def r2c2_prompt(self):
         """
@@ -134,14 +137,15 @@
             'skm': CONST.GENERATE_KNOWLEDGE,
             'mrm': '',
             'crm': '',
             'srm': '',
             'vrm': '',
             'grm': '',
             'orm': '',
+            'brm': '',
         }[self.value]
 
     def special_tokens(self):
         return {
             Module.CONTEXTUAL_KNOWLEDGE.message_name(): (
                 CONST.BEGIN_ENTITY,
                 CONST.END_ENTITY,
@@ -173,14 +177,15 @@
             'mkm': "A conversation between two persons. Person 2 recalls an interesting fact about Person 1 or Person 2.\n\n",
             'crm': "A conversation between two persons. Person 2 would like to continue talking about a previous topic in the conversation.\n\n",
             'mrm': "A conversation between two persons. Person 2 would like to chat about an interesting fact about Person 1 or Person 2.\n\n",
             'srm': "A conversation between two persons. Person 2 would like to tell Person 1 about something Person 2 found on the internet.\n\n",
             'vrm': "A conversation between two persons.\n\n",
             'grm': "A conversation between two persons. Person 2 responds in a given style.\n\n",
             'orm': "A conversation between two persons. Person 2 begins the conversation given information about Person 1.\n\n",
+            'brm': "A conversation between two persons.\n\n",
         }[self.value]
 
     def opt_final_prefix(self):
         """
         Final prefix to put after constructing context for OPT.
         """
         import projects.bb3.prompts as PROMPT
@@ -195,34 +200,41 @@
             'skm': PROMPT.SEARCH_KNOWLEDGE_PREFIX,
             'mrm': PROMPT.SELF_PREFIX,
             'crm': PROMPT.SELF_PREFIX,
             'srm': PROMPT.SELF_PREFIX,
             'vrm': PROMPT.SELF_PREFIX,
             'grm': PROMPT.SELF_PREFIX,
             'orm': PROMPT.OPENING_PREFIX,
+            'brm': PROMPT.SELF_PREFIX,
         }[self.value]
 
     def opt_shots(self) -> str:
         import projects.bb3.prompts as PROMPT
 
         return PROMPT.SHOTS[self]
 
     def opt_pre_context_tok(self):
         import projects.bb3.prompts as PROMPT
 
-        if self.is_knowledge() and self is not Module.CONTEXTUAL_KNOWLEDGE:
+        if (
+            (self.is_knowledge() and self is not Module.CONTEXTUAL_KNOWLEDGE)
+            or self is Module.GROUNDED_DIALOGUE
+            or self is Module.BOT_DIALOGUE
+        ):
             return PROMPT.PRE_CONTEXT_TOK
         return ''
 
     def opt_post_context_tok(self):
         import projects.bb3.prompts as PROMPT
 
         if self.is_dialogue() and self not in [
             Module.VANILLA_DIALOGUE,
             Module.OPENING_DIALOGUE,
+            Module.GROUNDED_DIALOGUE,
+            Module.BOT_DIALOGUE,
         ]:
             return PROMPT.POST_CONTEXT_TOK
         return ''
 
     def opt_dialogue_knowledge_prefix(self):
         return {
             'mrm': "Personal Fact: ",
```

### Comparing `parlai-1.7.1/projects/bb3/agents/opt_api_agent.py` & `parlai-1.7.2/projects/bb3/agents/opt_api_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,20 @@
         prompt: Optional[str] = None,
         opt: Optional[Opt] = None,
         dictionary: Optional[DictionaryAgent] = None,
     ):
         super().__init__(prompt)
         assert opt is not None
         self.add_speaker_prefixes = opt.get('add_speaker_prefixes', True)
+        self.SPEAKER_SELF = (
+            opt.get('self_prefix', self.SPEAKER_SELF) or self.SPEAKER_SELF
+        )
+        self.SPEAKER_OTHER = (
+            opt.get('partner_prefix', self.SPEAKER_OTHER) or self.SPEAKER_OTHER
+        )
         self.max_prompt_len = opt.get('max_prompt_len', PROMPT.MAX_PROMPT_LEN)
         self.module = Module(opt['module'])
         self.dictionary = dictionary
         self.memories_included = self.module is Module.MEMORY_DECISION and opt.get(
             'memory_decision_use_memories', False
         )
         self.one_turn_history = (
@@ -108,14 +114,18 @@
             if effective_shots == 0:
                 self.shots = ''
             elif effective_shots > 0:
                 self.shots = (
                     '\n\n'.join(self.shots.split('\n\n')[:effective_shots]) + '\n\n'
                 )
         self.final_prefix = f"{self.module.opt_final_prefix()}:"
+        if opt.get('final_prefix'):
+            self.final_prefix = f"{opt['final_prefix']}:"
+        if opt.get('final_prefix_space'):
+            self.final_prefix = f"{self.final_prefix} "
         self.pre_context_tok = self.module.opt_pre_context_tok()
         self.post_context_tok = self.module.opt_post_context_tok()
         self.style_string = (
             f"{PROMPT.STYLE_PREFIX}: {opt['insert_style']}"
             if opt.get('insert_style')
             else ''
         )
@@ -135,16 +145,16 @@
         assert text is not None
         lines = text.split("\n")
         assert len(lines) >= 1
         while lines and any(
             p in lines[0]
             for p in [
                 'your persona',
-                PROMPT.SELF_MEMORY_PREFIX,
-                PROMPT.PARTNER_MEMORY_PREFIX,
+                f"{self.SPEAKER_SELF}'s Persona",
+                f"{self.SPEAKER_OTHER}'s Persona",
             ]
         ):
             self.turns.append(lines.pop(0))
         end_of_context = len(self.turns)
         speakers = itertools.cycle([self.SPEAKER_OTHER, self.SPEAKER_SELF])
         for speaker, line in zip(speakers, lines[::-1]):
             if (
@@ -209,14 +219,33 @@
         parser.add_argument(
             '--prompt',
             choices=PROMPTS.keys(),
             default='none',
             help='Pre-made prompts. Use --raw-prompt to manually write one.',
         )
         parser.add_argument(
+            '--self-prefix',
+            default=PROMPT.SELF_PREFIX,
+            help="Prefix token indicating 'self' turn",
+        )
+        parser.add_argument(
+            '--partner-prefix',
+            default=PROMPT.PARTNER_PREFIX,
+            help="Prefix token indicating 'partner' turn",
+        )
+        parser.add_argument(
+            '--final-prefix', default=None, help="Specify to override the final prefix."
+        )
+        parser.add_argument(
+            '--final-prefix-space',
+            default=False,
+            type='bool',
+            help="Specify to include a space after the final prefix.",
+        )
+        parser.add_argument(
             '--raw-prompt', default=None, help='Use to manually specify a raw prompt.'
         )
         parser.add_argument(
             '--inference',
             default='greedy',
             choices=[
                 'nucleus',
@@ -289,14 +318,15 @@
         parser.add_argument(
             '--alpha-frequency-src',
             default=0.5,
             type=float,
             help='penalty applied to the logits for frequency of previous tokens in the context',
         )
         parser.add_argument('--temperature', default=1.0, type=float)
+        parser.add_argument('--stop-token', default="\n", type=str)
         parser.add_argument('--server', default=APIUtils.DEFAULT_SERVER, type=str)
         parser.add_argument(
             '--max-retry-api',
             default=-1,
             type=int,
             help='Number of times to retry on API request failures (< 0 for unlimited retry).',
         )
@@ -454,15 +484,15 @@
 
             gen_params = {
                 'best_of': self.opt['beam_size'],
                 'top_p': self.opt['topp'],
                 'temperature': self.opt['temperature'],
                 'min_tokens': self.opt['beam_min_length'],
                 'max_tokens': self.opt['beam_max_length'],
-                'stop': "\n",
+                'stop': self.opt['stop_token'],
                 'echo': False,
                 'lambda_decay': self.opt['lambda_decay'],
                 'omega_bound': self.opt['omega_bound'],
                 'alpha_presence': self.opt['alpha_presence'],
                 'alpha_frequency': self.opt['alpha_frequency'],
                 'alpha_presence_src': self.opt['alpha_presence_src'],
                 'alpha_frequency_src': self.opt['alpha_frequency_src'],
@@ -567,14 +597,20 @@
             '--generation-take-last-newline',
             type='bool',
             default=True,
             help='if a generation is returned with a newline character, set True to take last newline. '
             'set False to take first new line.',
         )
         parser.add_argument(
+            '--generation-allow-newline',
+            type='bool',
+            default=False,
+            help='if a generation is returned with a newline character, set True to return all generated tokens.',
+        )
+        parser.add_argument(
             '--memory-decision-use-memories',
             type='bool',
             default=False,
             help='If true, the memory decision module will have access to memories when making the decision',
         )
         parser.add_argument(
             '--exclude-knowledge-from-ctxt-penalty',
@@ -680,15 +716,15 @@
             alpha_src_penalty_end_idx=self._get_alpha_src_penalty_end_idx(observations),
         )
 
         for r in results:
             if not APIUtils.is_request_failed_response(r):
                 r['choices'][0]['text'] = r['choices'][0]['text'].strip("\n")
 
-        if any(
+        if not self.opt.get('generation_allow_newline') and any(
             '\n' in res['choices'][0]['text']
             for res in results
             if not APIUtils.is_request_failed_response(res)
         ):
             if self.opt.get('generation_take_last_newline', True):
                 logging.warning("Generation contains newline; taking last utterance")
             else:
```

### Comparing `parlai-1.7.1/projects/bb3/agents/opt_bb3_agent.py` & `parlai-1.7.2/projects/bb3/agents/opt_bb3_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 from projects.bb3.agents.module import Module
 from projects.bb3.agents.r2c2_bb3_agent import BlenderBot3Agent as R2C2Agent
 from projects.bb3.agents.opt_api_agent import BB3OPTAgent
 from projects.bb3.agents.search_agent import SearchAgent
 from projects.bb3.agents.utils import (
     Decision,
     APIUtils,
-    MemoryUtils,
     is_opener,
     DisplayUtils,
     set_failed_reply,
 )
 import projects.bb3.prompts as PROMPT
 
 
@@ -142,26 +141,62 @@
         group.add_argument('--debug-bb3', type='bool', default=False, dest='debug_bb3')
         group.add_argument(
             '--max-prompt-len',
             type=int,
             default=PROMPT.MAX_PROMPT_LEN,
             help='Longest sequence to send to API',
         )
+        group.add_argument(
+            '--self-prefix',
+            type=str,
+            default=PROMPT.SELF_PREFIX,
+            help='Token for prefixing self responses',
+        )
+        group.add_argument(
+            '--self-memory-prefix',
+            type=str,
+            default=PROMPT.SELF_MEMORY_PREFIX,
+            help='Token for prefixing self memories',
+        )
+        group.add_argument(
+            '--partner-prefix',
+            type=str,
+            default=PROMPT.PARTNER_PREFIX,
+            help='Token for prefixing self responses',
+        )
+        group.add_argument(
+            '--partner-memory-prefix',
+            type=str,
+            default=PROMPT.PARTNER_MEMORY_PREFIX,
+            help='Token for prefixing self memories',
+        )
         parser.add_argument(
             '--metaseq-max-retry-api',
             default=-1,
             type=int,
             help='Number of times to retry on API request failures (< 0 for unlimited retry).',
         )
         parser.add_argument('--metaseq-server-timeout', default=20.0, type=float)
         return parser
 
     def __init__(self, opt, shared=None):
         opt['model_file'] = 'zoo:'
         super().__init__(opt, shared)
+        self.self_prefix = opt.get('self_prefix', PROMPT.SELF_PREFIX)
+        self.partner_prefix = opt.get('partner_prefix', PROMPT.PARTNER_PREFIX)
+        self.self_memory_prefix = opt.get(
+            'self_memory_prefix', PROMPT.SELF_MEMORY_PREFIX
+        )
+        self.partner_memory_prefix = opt.get(
+            'partner_memory_prefix', PROMPT.PARTNER_MEMORY_PREFIX
+        )
+        self.memory_utils.self_prefix = self.self_prefix
+        self.memory_utils.partner_prefix = self.partner_prefix
+        self.memory_utils.self_memory_prefix = self.self_memory_prefix
+        self.memory_utils.partner_memory_prefix = self.partner_memory_prefix
         # Always init search agent
         if not shared:
             agent_opts = self.opts[Module.SEARCH_KNOWLEDGE]
             top_agent = self._init_top_agent(agent_opts)
             # two mappings; one for code access, one for debug access.
             self.agents[Module.SEARCH_KNOWLEDGE.agent_name()] = top_agent
             self.agents[Module.SEARCH_KNOWLEDGE] = top_agent
@@ -236,27 +271,27 @@
             return mdm observation with memories in the context.
         """
         self.agents[Module.MEMORY_DECISION].reset()
 
         original_text = ag_obs['text']
         self_memory_text, partner_memory_text = '', ''
         self_memories = [
-            m.replace(f"{PROMPT.SELF_MEMORY_PREFIX}: ", '')
+            m.replace(f"{self.self_memory_prefix}: ", '')
             for m in self.memories
-            if m.startswith(PROMPT.SELF_MEMORY_PREFIX)
+            if m.startswith(self.self_memory_prefix)
         ]
         if self_memories:
-            self_memory_text = f"{PROMPT.MEMORY_KNOWLEDGE_PREFIX}: {PROMPT.SELF_MEMORY_PREFIX}: {' '.join(self_memories)}\n"
+            self_memory_text = f"{PROMPT.MEMORY_KNOWLEDGE_PREFIX}: {self.self_memory_prefix}: {' '.join(self_memories)}\n"
         partner_memories = [
-            m.replace(f"{PROMPT.PARTNER_MEMORY_PREFIX}: ", '')
+            m.replace(f"{self.partner_memory_prefix}: ", '')
             for m in self.memories
-            if m.startswith(PROMPT.PARTNER_MEMORY_PREFIX)
+            if m.startswith(self.partner_memory_prefix)
         ]
         if partner_memories:
-            partner_memory_text = f"{PROMPT.MEMORY_KNOWLEDGE_PREFIX}: {PROMPT.PARTNER_MEMORY_PREFIX}: {' '.join(partner_memories)}\n"
+            partner_memory_text = f"{PROMPT.MEMORY_KNOWLEDGE_PREFIX}: {self.partner_memory_prefix}: {' '.join(partner_memories)}\n"
 
         new_text = f"{self_memory_text}{partner_memory_text}{original_text}"
         ag_obs.force_set('text', new_text)
         return ag_obs
 
     def get_orm_observation(
         self, observation: Message, opening_memories: Dict[str, int]
@@ -272,19 +307,21 @@
         :return observation:
             return the ORM observation
         """
         agent = self.agents[Module.OPENING_DIALOGUE]
         agent.reset()
         prefixed_memories = {}
         for mem, val in opening_memories.items():
-            mem = MemoryUtils.maybe_add_memory_prefix(mem, 'partner', self.MODEL_TYPE)
+            mem = self.memory_utils.maybe_add_memory_prefix(
+                mem, 'partner', self.MODEL_TYPE
+            )
             prefixed_memories[mem] = val
 
         new_obs = copy.deepcopy(observation)
-        memories_to_use = MemoryUtils.get_available_memories(
+        memories_to_use = self.memory_utils.get_available_memories(
             '',
             prefixed_memories,
             set(),
             dictionary=self.dictionary,
             **self._get_memory_heuristic_values(),
         )
         if not memories_to_use:
@@ -314,15 +351,17 @@
         opening_memories = None
         if memories:
             if isinstance(memories, dict):
                 opening_memories = {mem: int(turns) for mem, turns in memories.items()}
             elif isinstance(memories, list):
                 opening_memories = {}
                 for mem in memories:
-                    opening_memories = MemoryUtils.add_memory(mem, opening_memories)
+                    opening_memories = self.memory_utils.add_memory(
+                        mem, opening_memories
+                    )
 
         assert not opening_memories or isinstance(opening_memories, dict)
         return opening_memories
 
     def observe(self, observation: Message) -> Dict[Module, Message]:
         # handle passed memories as well
         observation = Message(observation)
@@ -481,22 +520,22 @@
         # re-assign memories
         for i, reply in enumerate(batch_reply_knowledge):
             if i in memory_indices:
                 text = reply[Module.MEMORY_KNOWLEDGE.message_name()].strip()
                 do_split = True
                 if any(
                     text.startswith(p)
-                    for p in [PROMPT.PARTNER_MEMORY_PREFIX, PROMPT.SELF_MEMORY_PREFIX]
+                    for p in [self.partner_memory_prefix, self.self_memory_prefix]
                 ):
                     # no need to split the memory to find it
                     do_split = False
                 true_memory = ''
                 for memory in available_memory[i]:
                     raw_mem = (
-                        MemoryUtils.split_prefix_memory(memory)[-1]
+                        self.memory_utils.split_prefix_memory(memory)[-1]
                         if do_split
                         else memory
                     )
                     if raw_mem == text:
                         true_memory = memory
                         break
                 if true_memory:
@@ -627,17 +666,16 @@
                     extra_knowledge.append(obs['prompt'].split('\n')[-2])
                 old_prompt = primary_obs[-1]['prompt'].split('\n')
                 primary_obs[-1].force_set(
                     'prompt',
                     '\n'.join(old_prompt[:-1] + extra_knowledge + old_prompt[-1:]),
                 )
                 combined_obs.append(primary_obs)
-            dialogue_replies = self.batch_agents[Module.SEARCH_DIALOGUE].batch_act(
-                [o[-1] for o in combined_obs]
-            )
+            batch_agent = self.batch_agents[self.combined_dialogue_module]
+            dialogue_replies = batch_agent.batch_act([o[-1] for o in combined_obs])
             dialogue_obs = combined_obs
         else:
             raise NotImplementedError('Both is not implemented')
 
         batch_reply_dialogue = [Message({}) for _ in range(len(observations))]
 
         # collate dialogue replies
@@ -702,20 +740,20 @@
         :param observations:
             raw observations
 
         :return batch_act:
             return batch act from the opening dialogue agent.
         """
         module = Module.OPENING_DIALOGUE
-        batch_act = [Message({'text': PROMPT.SELF_PREFIX})] * len(observations)
+        batch_act = [Message({'text': self.self_prefix})] * len(observations)
 
         def _failed_messages(replies):
             return any(
                 p in o['text']
-                for p in [PROMPT.SELF_PREFIX, PROMPT.PARTNER_PREFIX]
+                for p in [self.self_prefix, self.partner_prefix]
                 for o in replies
             )
 
         retries = 0
         opening_obs = [o[module] for o in observations]
         while _failed_messages(batch_act) and retries < 3:
             batch_act = self.batch_agents[Module.OPENING_DIALOGUE].batch_act(
@@ -734,18 +772,18 @@
                         if i in mem_indices
                     },
                 )
         if _failed_messages(batch_act):
             for reply in batch_act:
                 text = reply.pop('text')
                 for p in [
-                    PROMPT.SELF_MEMORY_PREFIX,
-                    PROMPT.PARTNER_MEMORY_PREFIX,
-                    PROMPT.SELF_PREFIX,
-                    PROMPT.PARTNER_PREFIX,
+                    self.self_memory_prefix,
+                    self.partner_memory_prefix,
+                    self.self_prefix,
+                    self.partner_prefix,
                 ]:
                     text = text.replace(f"{p}:", '').replace(p, '')
                 reply['text'] = text
 
         return batch_act
 
     def batch_act_simple(
```

### Comparing `parlai-1.7.1/projects/bb3/agents/r2c2_bb3_agent.py` & `parlai-1.7.2/projects/bb3/agents/r2c2_bb3_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,21 @@
             choices=['combined', 'separate', 'both'],
             default='combined',
             help='Specify the way in which the model uses knowledge.\n'
             'combined: condition on all knowledge simultaneously'
             'separate: condition on all knowledge separately, re-ranke later'
             'both: do both combined and separate and re-rank final beam',
         )
+        group.add_argument(
+            '--combined-dialogue-module',
+            type=str,
+            choices=[m.tag() for m in Module.dialogue_modules()],
+            default=Module.SEARCH_DIALOGUE.tag(),
+            help='Specify which agent module handles the final dialogue response',
+        )
         parser.add_argument(
             '--ignore-in-session-memories-mkm',
             type='bool',
             default=False,
             help='If true, we do not look at the in-session memories when '
             'generating from the MKM',
         )
@@ -466,14 +473,16 @@
         self.search_decision = Decision(opt['search_decision'])
         self.memory_decision = Decision(opt['memory_decision'])
         self.contextual_knowledge_decision = Decision(
             opt['contextual_knowledge_decision']
         )
         self.inject_query_string = opt.get('inject_query_string', '')
         self.knowledge_conditioning = opt['knowledge_conditioning']
+        self.combined_dialogue_module = Module(opt['combined_dialogue_module'])
+        self.memory_utils = MemoryUtils
 
         for m in Module:
             agent = self._init_shared_model(m)
             self.agents[m.agent_name()], self.agents[m] = agent, agent
             if m.is_dialogue():
                 self.clones[m.agent_name()], self.clones[m] = [agent], [agent]
 
@@ -702,15 +711,15 @@
         :param observations:
             incoming batch observations
 
         :return memories:
             return a list of memories for each batch item.
         """
         return [
-            MemoryUtils.get_available_memories(
+            self.memory_utils.get_available_memories(
                 o['raw']['text'],
                 o['raw']['memories'],
                 o['raw']['in_session_memories'],
                 self.dictionary,
                 **self._get_memory_heuristic_values(),
             )
             for o in observations
@@ -1012,15 +1021,15 @@
         full_text = [
             clean_text(
                 o[Module.CONTEXTUAL_KNOWLEDGE].get('full_text', o.get('text', ''))
             )
             for o in observations
         ]
         clones = self.clones[Module.SEARCH_DIALOGUE]
-        agent = self.agents[Module.SEARCH_DIALOGUE]
+        agent = self.agents[self.combined_dialogue_module]
         dialogue_agent_observations = []
         for i, (obs, knowledge_obs) in enumerate(
             zip(observations, batch_reply_knowledge)
         ):
             temp_history = '\n'
             srm_obs = copy.deepcopy(obs['raw'])
             for m in Module.knowledge_modules():
@@ -1256,21 +1265,21 @@
             )
             reply.force_set(
                 f'{Module.MEMORY_GENERATOR.message_name()}_partner',
                 mgm_partner.get('text', ''),
             )
             mems = copy.deepcopy(mems)
             for message, person in zip([mgm_self, mgm_partner], ['self', 'partner']):
-                if MemoryUtils.is_valid_memory(
+                if self.memory_utils.is_valid_memory(
                     mems,
                     message.get('text', ''),
-                    MemoryUtils.get_memory_prefix(person, self.MODEL_TYPE),
+                    self.memory_utils.get_memory_prefix(person, self.MODEL_TYPE),
                 ):
-                    mems = MemoryUtils.add_memory(
-                        MemoryUtils.add_memory_prefix(
+                    mems = self.memory_utils.add_memory(
+                        self.memory_utils.add_memory_prefix(
                             message['text'], person, self.MODEL_TYPE
                         ),
                         mems,
                     )
             reply.force_set('memories', mems)
             reply.force_set(
                 Module.SEARCH_KNOWLEDGE.message_name(),
@@ -1493,21 +1502,25 @@
         """
         # add new memories
         memory_key = Module.MEMORY_GENERATOR.message_name()
         for person in ['self', 'partner']:
             memory_candidate = self_message.get(f"{memory_key}_{person}")
             if not memory_candidate:
                 continue
-            if MemoryUtils.is_valid_memory(
+            if self.memory_utils.is_valid_memory(
                 self.memories,
                 memory_candidate,
-                MemoryUtils.get_memory_prefix(person, self.MODEL_TYPE),
+                self.memory_utils.get_memory_prefix(person, self.MODEL_TYPE),
             ):
-                memory_to_add = MemoryUtils.add_memory_prefix(
+                memory_to_add = self.memory_utils.add_memory_prefix(
                     memory_candidate, person, self.MODEL_TYPE
                 )
-                self.memories = MemoryUtils.add_memory(memory_to_add, self.memories)
+                self.memories = self.memory_utils.add_memory(
+                    memory_to_add, self.memories
+                )
                 self.in_session_memories.add(memory_to_add)
 
         # update mem usage
         used_memory = self_message.get(Module.MEMORY_KNOWLEDGE.message_name(), '')
-        self.memories = MemoryUtils.update_memory_usage(used_memory, self.memories)
+        self.memories = self.memory_utils.update_memory_usage(
+            used_memory, self.memories
+        )
```

### Comparing `parlai-1.7.1/projects/bb3/agents/search_agent.py` & `parlai-1.7.2/projects/bb3/agents/search_agent.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/agents/utils.py` & `parlai-1.7.2/projects/bb3/agents/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,69 +172,76 @@
 
 ################
 # Memory Utils #
 ################
 
 
 class MemoryUtils:
-    @staticmethod
-    def is_opt_ft_mem_format(memory_text: str) -> bool:
+    self_memory_prefix: str = PROMPT.SELF_MEMORY_PREFIX
+    partner_memory_prefix: str = PROMPT.PARTNER_MEMORY_PREFIX
+
+    self_prefix: str = PROMPT.SELF_PREFIX
+    partner_prefix: str = PROMPT.PARTNER_PREFIX
+
+    @classmethod
+    def is_opt_ft_mem_format(cls, memory_text: str) -> bool:
         return (
             ':' in memory_text
-            and memory_text.startswith(PROMPT.SELF_MEMORY_PREFIX)
-            or memory_text.startswith(PROMPT.PARTNER_MEMORY_PREFIX)
+            and memory_text.startswith(cls.self_memory_prefix)
+            or memory_text.startswith(cls.partner_memory_prefix)
         )
 
-    @staticmethod
-    def _is_r2c2_format(memory_text: str) -> bool:
+    @classmethod
+    def _is_r2c2_format(cls, memory_text: str) -> bool:
         return (
             ':' in memory_text
             and memory_text.startswith("your persona")
             or memory_text.startswith("partner's persona")
         )
 
-    @staticmethod
-    def _is_opt_prompt_format(memory_text: str) -> bool:
-        return memory_text.startswith(PROMPT.SELF_PREFIX) or memory_text.startswith(
-            PROMPT.PARTNER_PREFIX
+    @classmethod
+    def _is_opt_prompt_format(cls, memory_text: str) -> bool:
+        return memory_text.startswith(cls.self_prefix) or memory_text.startswith(
+            cls.partner_prefix
         )
 
-    @staticmethod
-    def validate_memory_format(memory_text: str):
+    @classmethod
+    def validate_memory_format(cls, memory_text: str):
         assert (
             MemoryUtils._is_r2c2_format(memory_text)
             or MemoryUtils._is_opt_prompt_format(memory_text)
             or MemoryUtils.is_opt_ft_mem_format(memory_text)
         ), f'Provided memory "{memory_text}" has invalid format for chatbot memory field.'
 
-    @staticmethod
-    def split_prefix_memory(memory_text: str) -> Tuple[str, str]:
+    @classmethod
+    def split_prefix_memory(cls, memory_text: str) -> Tuple[str, str]:
         MemoryUtils.validate_memory_format(memory_text)
         try:
             prfx, mem = memory_text.split(':', 1)
         except ValueError:
             # prompt agent sometimes says things like,
             # "Person 2 is"...
-            assert memory_text.startswith(PROMPT.SELF_PREFIX) or memory_text.startswith(
-                PROMPT.PARTNER_PREFIX
+            assert memory_text.startswith(cls.self_prefix) or memory_text.startswith(
+                cls.partner_prefix
             )
-            if memory_text.startswith(PROMPT.SELF_PREFIX):
+            if memory_text.startswith(cls.self_prefix):
                 prfx, mem = (
-                    memory_text[: len(PROMPT.SELF_PREFIX)],
-                    memory_text[len(PROMPT.SELF_PREFIX) + 1 :],
+                    memory_text[: len(cls.self_prefix)],
+                    memory_text[len(cls.self_prefix) + 1 :],
                 )
             else:
                 prfx, mem = (
-                    memory_text[: len(PROMPT.PARTNER_PREFIX)],
-                    memory_text[len(PROMPT.PARTNER_PREFIX) + 1 :],
+                    memory_text[: len(cls.partner_prefix)],
+                    memory_text[len(cls.partner_prefix) + 1 :],
                 )
         return prfx.strip(), mem.strip()
 
-    @staticmethod
+    @classmethod
     def is_valid_memory(
+        cls,
         chatbot_memory: Union[List[str], Dict[str, int]],
         new_memory: str,
         new_memory_prefix: str,
     ) -> bool:
         """
         Return whether the memory is valid.
 
@@ -261,36 +268,34 @@
         ]
         if not person_memories:
             # No memory on record for this person
             return True
 
         return no_overlap(person_memories, new_memory)
 
-    @staticmethod
-    def get_memory_prefix(self_or_partner: str, model_type: str) -> str:
+    @classmethod
+    def get_memory_prefix(cls, self_or_partner: str, model_type: str) -> str:
         """
         Return memory prefix.
         """
         assert self_or_partner in ['self', 'partner']
         assert model_type in ['R2C2', 'OPT']
-        self_prefix = (
-            'your persona' if model_type == 'R2C2' else PROMPT.SELF_MEMORY_PREFIX
-        )
+        self_prefix = 'your persona' if model_type == 'R2C2' else cls.self_memory_prefix
         partner_prefix = (
-            "partner's persona"
-            if model_type == 'R2C2'
-            else PROMPT.PARTNER_MEMORY_PREFIX
+            "partner's persona" if model_type == 'R2C2' else cls.partner_memory_prefix
         )
         if self_or_partner == 'self':
             return self_prefix
         else:
             return partner_prefix
 
-    @staticmethod
-    def add_memory_prefix(memory: str, self_or_partner: str, model_type: str) -> str:
+    @classmethod
+    def add_memory_prefix(
+        cls, memory: str, self_or_partner: str, model_type: str
+    ) -> str:
         """
         Ensure that the memory has a "persona" prefix.
 
         :param memory:
             memory to prefix
         :param self_or_partner:
             string representing if this is a self memory or partner memory
@@ -313,43 +318,43 @@
         else:
             memory = memory.replace("Person 2", "Person 1")
             if not memory.startswith('Person'):
                 memory = f"{prefix}: {memory}"
 
         return memory
 
-    @staticmethod
+    @classmethod
     def maybe_add_memory_prefix(
-        memory: str, self_or_partner: str, model_type: str
+        cls, memory: str, self_or_partner: str, model_type: str
     ) -> str:
         """
         Maybe add it if it's not there.
         """
         if not MemoryUtils.is_opt_ft_mem_format(memory):
             memory = MemoryUtils.add_memory_prefix(memory, self_or_partner, model_type)
         return memory
 
-    @staticmethod
+    @classmethod
     def _build_query_representation(
-        query: str, dictionary: DictionaryAgent
+        cls, query: str, dictionary: DictionaryAgent
     ) -> Dict[str, Any]:
         rep = {}
         rep['words'] = {}
         words = [w for w in dictionary.tokenize(query.lower())]
         rw = rep['words']
         used = {}
         for w in words:
             rw[w] = 1.0 / (1.0 + math.log(1.0 + dictionary.freq[w]))
             used[w] = True
         rep['norm'] = math.sqrt(len(words))
         return rep
 
-    @staticmethod
+    @classmethod
     def maybe_reduce_memories(
-        text: str, memories: List[str], dictionary: DictionaryAgent
+        cls, text: str, memories: List[str], dictionary: DictionaryAgent
     ) -> List[str]:
         """
         TFIDF-Match memories with the textual input to reduce num memories.
 
         :param observation:
             raw observation
         :param memories:
@@ -367,16 +372,17 @@
         query = MemoryUtils._build_query_representation(text, dictionary)
         for m in memories:
             score = score_match(query, m, 0, dictionary)
             mpq.add(m, score)
         new_memories = list(reversed(mpq))[:32]
         return new_memories
 
-    @staticmethod
+    @classmethod
     def get_available_memories(
+        cls,
         text: str,
         memories: Dict[str, int],
         in_session_memories: Set[str],
         dictionary: Optional[DictionaryAgent] = None,
         ignore_in_session_memories: bool = False,
         memory_overlap_threshold: float = 0.0,
         memory_hard_block_for_n_turns: int = 0,
@@ -421,16 +427,16 @@
                 memory_soft_block_decay_factor**turns_since_used
             ):
                 continue
 
             available_memory.append(memory)
         return MemoryUtils.maybe_reduce_memories(text, available_memory, dictionary)
 
-    @staticmethod
-    def add_memory(memory: str, memories: Dict[str, int]) -> Dict[str, int]:
+    @classmethod
+    def add_memory(cls, memory: str, memories: Dict[str, int]) -> Dict[str, int]:
         """
         Add memory to the memory store.
 
         :param memory:
             memory to add
         :param memories:
             all the memories
@@ -440,17 +446,17 @@
         """
         if not memory:
             return memories
         assert memory not in memories
         memories[memory] = 0
         return memories
 
-    @staticmethod
+    @classmethod
     def update_memory_usage(
-        used_memory: str, memories: Dict[str, int]
+        cls, used_memory: str, memories: Dict[str, int]
     ) -> Dict[str, int]:
         """
         Update memories to indicate that a memory was used.
 
         :param memory:
             used memory
         :param memories:
@@ -646,15 +652,19 @@
             # need text offsets to figure out what comes from the prompt
             prompt_len = len(obs['prompt'])
 
             text_off = result['choices'][0]['logprobs']['text_offset']
             start_label = [i for i, off in enumerate(text_off) if off <= prompt_len]
             assert len(start_label) > 0
             start_label = start_label[-1]
-            all_log_probs = result['choices'][0]['logprobs']['token_logprobs']
+            all_log_probs = [
+                lp
+                for lp in result['choices'][0]['logprobs']['token_logprobs']
+                if lp is not None
+            ]
             if not all(l <= 0 for l in all_log_probs):
                 logging.warning(
                     f'Out of {len(all_log_probs)} log probs, {len([l for l in all_log_probs if l > 0])} are > 0. '
                     'Clamping to 0'
                 )
                 all_log_probs = [min(l, 0) for l in all_log_probs]
```

### Comparing `parlai-1.7.1/projects/bb3/constants.py` & `parlai-1.7.2/projects/bb3/constants.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/prompts.py` & `parlai-1.7.2/projects/bb3/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 QUERY_GEN_PREFIX = 'Query'
 MEMORY_GEN_PREFIX = 'Memory'
 MEMORY_KNOWLEDGE_PREFIX = 'Personal Fact'
 CONTEXTUAL_KNOWLEDGE_PREFIX = 'Previous Topic'
 SEARCH_KNOWLEDGE_PREFIX = 'Interesting Fact'
 STYLE_PREFIX = 'Style'
 OPENING_PREFIX = 'Opening'
+CONTEXT_PREFIX = 'Context'
 
 SELF_MEMORY_PREFIX = f"{SELF_PREFIX}'s Persona"
 PARTNER_MEMORY_PREFIX = f"{PARTNER_PREFIX}'s Persona"
 EXTERNAL_KNOWLEDGE_PREFIX = "External Knowledge"
 
 SEARCH = 'search'
 DO_NOT_SEARCH = 'do not search'
@@ -502,14 +503,15 @@
     Module.SEARCH_KNOWLEDGE: SEARCH_KNOWLEDGE_STRING,
     Module.CONTEXTUAL_DIALOGUE: CONTEXTUAL_DIALOGUE_STRING,
     Module.MEMORY_DIALOGUE: MEMORY_DIALOGUE_STRING,
     Module.SEARCH_DIALOGUE: SEARCH_DIALOGUE_STRING,
     Module.VANILLA_DIALOGUE: VANILLA_DIALOGUE_STRING,
     Module.GROUNDED_DIALOGUE: GROUNDED_DIALOGUE_STRING,
     Module.OPENING_DIALOGUE: OPENING_DIALOGUE_STRING,
+    Module.BOT_DIALOGUE: GROUNDED_DIALOGUE_STRING,
 }
 
 
 def extract_docs(d):
     return d['dialog'][0][0]['__retrieved-docs__']
```

### Comparing `parlai-1.7.1/projects/bb3/tasks/mutators.py` & `parlai-1.7.2/projects/bb3/tasks/mutators.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 
 def build_summarizer(opt: Opt) -> Agent:
     """
     Build the Persona Summarizer.
     """
     return create_agent_from_model_file(
-        modelzoo_path(opt['datapath', 'zoo:bb3/persona_summarizer/model']),
+        modelzoo_path(opt['datapath'], 'zoo:bb3/persona_summarizer/model'),
         opt_overrides={
             'skip_generation': False,
             'inference': 'beam',
             'beam_size': 3,
             'beam_block_ngram': 3,
             'beam_min_length': 10,
             'datatype': 'valid',
```

### Comparing `parlai-1.7.1/projects/bb3/tasks/opt_decision_tasks.py` & `parlai-1.7.2/projects/bb3/tasks/opt_decision_tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/tasks/opt_dialogue_tasks.py` & `parlai-1.7.2/projects/bb3/tasks/opt_dialogue_tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/tasks/opt_knowledge_tasks.py` & `parlai-1.7.2/projects/bb3/tasks/opt_knowledge_tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/tasks/opt_memory_generation_tasks.py` & `parlai-1.7.2/projects/bb3/tasks/opt_memory_generation_tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/tasks/opt_search_generation_tasks.py` & `parlai-1.7.2/projects/bb3/tasks/opt_search_generation_tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/tasks/r2c2_decision_tasks.py` & `parlai-1.7.2/projects/bb3/tasks/r2c2_decision_tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/tasks/r2c2_dialogue_tasks.py` & `parlai-1.7.2/projects/bb3/tasks/r2c2_dialogue_tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/tasks/r2c2_knowledge_tasks.py` & `parlai-1.7.2/projects/bb3/tasks/r2c2_knowledge_tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/tasks/r2c2_memory_generation_tasks.py` & `parlai-1.7.2/projects/bb3/tasks/r2c2_memory_generation_tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/bb3/tasks/r2c2_search_generation_tasks.py` & `parlai-1.7.2/projects/bb3/tasks/r2c2_search_generation_tasks.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/blenderbot2/agents/blenderbot2.py` & `parlai-1.7.2/projects/blenderbot2/agents/blenderbot2.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/blenderbot2/agents/modules.py` & `parlai-1.7.2/projects/blenderbot2/agents/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/blenderbot2/agents/sub_modules.py` & `parlai-1.7.2/projects/blenderbot2/agents/sub_modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/dialogue_unlikelihood/agents.py` & `parlai-1.7.2/projects/dialogue_unlikelihood/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/image_chat/interactive.py` & `parlai-1.7.2/projects/image_chat/interactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -223,23 +223,33 @@
         :param data:
             data to send to model
 
         :return:
             model act dictionary
         """
         reply = {}
-        reply["text"] = data["personality"][0].decode()
-        text = data["text"][0].decode()
+        if type(data["personality"][0]) is bytes:
+            reply["text"] = data["personality"][0].decode("utf-8")
+        else:
+            reply["text"] = data["personality"][0]
+        if type(data["text"][0]) is bytes:
+            text = data["text"][0].decode("utf-8")
+        else:
+            text = data["text"][0]
         if text:
             reply["text"] = "\n".join(SHARED["dialog_history"] + [text, reply["text"]])
             SHARED["dialog_history"].append(text)
         if SHARED["image_feats"] is None:
-
-            img_data = str(data["image"][0])
-            _, encoded = img_data.split(",", 1)
+            if type(data["image"][0]) is bytes:
+                img_data = data["image"][0].decode("utf-8")
+                _, encoded = img_data.split(",", 1)
+                encoded = encoded[2:-1]
+            else:
+                img_data = data["image"][0]
+                _, encoded = img_data.split(",", 1)
             image = Image.open(io.BytesIO(b64decode(encoded))).convert("RGB")
             SHARED["image_feats"] = SHARED["image_loader"].extract(image)
 
         reply["image"] = SHARED["image_feats"]
         SHARED["agent"].observe(reply)
         model_res = SHARED["agent"].act()
         return model_res
@@ -257,15 +267,15 @@
         Handle POST.
         """
         if self.path != "/interact":
             return self.respond({"status": 500})
         ctype, pdict = cgi.parse_header(self.headers["content-type"])
         pdict["boundary"] = bytes(pdict["boundary"], "utf-8")
         postvars = cgi.parse_multipart(self.rfile, pdict)
-        if postvars["image"][0].decode() != "":
+        if postvars["image"][0] != "":
             SHARED["dialog_history"] = []
             SHARED["image_feats"] = None
         model_response = self.interactive_running(postvars)
 
         self.send_response(200)
         self.send_header("Content-type", "application/json")
         self.end_headers()
```

### Comparing `parlai-1.7.1/projects/image_chat/transresnet_multimodal/modules.py` & `parlai-1.7.2/projects/image_chat/transresnet_multimodal/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/image_chat/transresnet_multimodal/transresnet_multimodal.py` & `parlai-1.7.2/projects/image_chat/transresnet_multimodal/transresnet_multimodal.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/personality_captions/interactive.py` & `parlai-1.7.2/projects/personality_captions/interactive.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/personality_captions/transresnet/modules.py` & `parlai-1.7.2/projects/personality_captions/transresnet/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/personality_captions/transresnet/transresnet.py` & `parlai-1.7.2/projects/personality_captions/transresnet/transresnet.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/model_wrappers/example_wrapper.py` & `parlai-1.7.2/projects/safety_bench/model_wrappers/example_wrapper.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/model_wrappers/gpt_wrappers.py` & `parlai-1.7.2/projects/safety_bench/model_wrappers/gpt_wrappers.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/model_wrappers/parlai_model_zoo_wrappers.py` & `parlai-1.7.2/projects/safety_bench/model_wrappers/parlai_model_zoo_wrappers.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/prepare_integration_tests.py` & `parlai-1.7.2/projects/safety_bench/prepare_integration_tests.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/run_unit_tests.py` & `parlai-1.7.2/projects/safety_bench/run_unit_tests.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/unit_tests/generate_offensive_language_test.py` & `parlai-1.7.2/projects/safety_bench/unit_tests/generate_offensive_language_test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/unit_tests/response_to_offensive_language_test.py` & `parlai-1.7.2/projects/safety_bench/unit_tests/response_to_offensive_language_test.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/utils/colors.py` & `parlai-1.7.2/projects/safety_bench/utils/colors.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/utils/perspective_api.py` & `parlai-1.7.2/projects/safety_bench/utils/perspective_api.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/utils/safety_testing.py` & `parlai-1.7.2/projects/safety_bench/utils/safety_testing.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/safety_bench/utils/wrapper_loading.py` & `parlai-1.7.2/projects/safety_bench/utils/wrapper_loading.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/agents/gpt2_seeker.py` & `parlai-1.7.2/projects/seeker/agents/gpt2_seeker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/agents/gpt2_seeker_modules.py` & `parlai-1.7.2/projects/seeker/agents/gpt2_seeker_modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/agents/modular_agent.py` & `parlai-1.7.2/projects/seeker/agents/modular_agent.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/agents/seeker.py` & `parlai-1.7.2/projects/seeker/agents/seeker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/agents/seeker_modules.py` & `parlai-1.7.2/projects/seeker/agents/seeker_modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/scripts/generate_lm_data.py` & `parlai-1.7.2/projects/seeker/scripts/generate_lm_data.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/tasks/dialogue.py` & `parlai-1.7.2/projects/seeker/tasks/dialogue.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/tasks/knowledge.py` & `parlai-1.7.2/projects/seeker/tasks/knowledge.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/tasks/lm.py` & `parlai-1.7.2/projects/seeker/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/tasks/mutators.py` & `parlai-1.7.2/projects/seeker/tasks/mutators.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/tasks/search_decision.py` & `parlai-1.7.2/projects/seeker/tasks/search_decision.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/tasks/search_query.py` & `parlai-1.7.2/projects/seeker/tasks/search_query.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/seeker/utils.py` & `parlai-1.7.2/projects/seeker/utils.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/style_gen/classifier.py` & `parlai-1.7.2/projects/style_gen/classifier.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/style_gen/modules.py` & `parlai-1.7.2/projects/style_gen/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/style_gen/style_gen.py` & `parlai-1.7.2/projects/style_gen/style_gen.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/tod_simulator/scripts/cleanup_conversation.py` & `parlai-1.7.2/projects/tod_simulator/scripts/cleanup_conversation.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/tod_simulator/scripts/do_get_passing_only_on_dir.py` & `parlai-1.7.2/projects/tod_simulator/scripts/do_get_passing_only_on_dir.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/tod_simulator/scripts/get_al_samples_for_gsgd.py` & `parlai-1.7.2/projects/tod_simulator/scripts/get_al_samples_for_gsgd.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/tod_simulator/scripts/get_api_data.py` & `parlai-1.7.2/projects/tod_simulator/scripts/get_api_data.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/tod_simulator/scripts/get_interdistinct_on_conversations.py` & `parlai-1.7.2/projects/tod_simulator/scripts/get_interdistinct_on_conversations.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/tod_simulator/scripts/get_passing_only.py` & `parlai-1.7.2/projects/tod_simulator/scripts/get_passing_only.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/tod_simulator/scripts/get_quick_eval_stats.py` & `parlai-1.7.2/projects/tod_simulator/scripts/get_quick_eval_stats.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/tod_simulator/scripts/tod_distributed_uber_script.py` & `parlai-1.7.2/projects/tod_simulator/scripts/tod_distributed_uber_script.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/tod_simulator/world_metrics/extended_world_metrics.py` & `parlai-1.7.2/projects/tod_simulator/world_metrics/extended_world_metrics.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/wizard_of_wikipedia/generator/agents.py` & `parlai-1.7.2/projects/wizard_of_wikipedia/generator/agents.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/wizard_of_wikipedia/generator/modules.py` & `parlai-1.7.2/projects/wizard_of_wikipedia/generator/modules.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/wizard_of_wikipedia/generator/train_end2end.py` & `parlai-1.7.2/projects/wizard_of_wikipedia/generator/train_end2end.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/wizard_of_wikipedia/knowledge_retriever/knowledge_retriever.py` & `parlai-1.7.2/projects/wizard_of_wikipedia/knowledge_retriever/knowledge_retriever.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/wizard_of_wikipedia/scripts/eval_retrieval_model.py` & `parlai-1.7.2/projects/wizard_of_wikipedia/scripts/eval_retrieval_model.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/wizard_of_wikipedia/scripts/interactive_retrieval_model.py` & `parlai-1.7.2/projects/wizard_of_wikipedia/scripts/interactive_retrieval_model.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/wizard_of_wikipedia/wizard_transformer_ranker/wizard_dict.py` & `parlai-1.7.2/projects/wizard_of_wikipedia/wizard_transformer_ranker/wizard_dict.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/projects/wizard_of_wikipedia/wizard_transformer_ranker/wizard_transformer_ranker.py` & `parlai-1.7.2/projects/wizard_of_wikipedia/wizard_transformer_ranker/wizard_transformer_ranker.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/setup.py` & `parlai-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 
 import sys
 
 from setuptools import setup, find_packages
 
-VERSION = '1.7.1'  # if you update, update parlai/__init__.py too!
+VERSION = '1.7.2'  # if you update, update parlai/__init__.py too!
 
 if sys.version_info < (3, 8):
     sys.exit('Sorry, Python >=3.8 is required for ParlAI.')
 
 with open('README.md', encoding="utf8") as f:
     # strip the header and badges etc
     readme = f.read().split('--------------------')[-1]
@@ -29,15 +29,15 @@
     setup(
         name='parlai',
         version=VERSION,
         description='Unified platform for dialogue research.',
         long_description=readme,
         long_description_content_type='text/markdown',
         url='http://parl.ai/',
-        python_requires='>=3.7',
+        python_requires='>=3.8',
         packages=find_packages(exclude=('data', 'docs', 'tests', 'parlai_internal*')),
         install_requires=reqs,
         include_package_data=True,
         package_data={'': ['*.txt', '*.md', '*.opt', '*.cu', '*.cpp']},
         entry_points={
             "flake8.extension": ["PAI = parlai.utils.flake8:ParlAIChecker"],
             "console_scripts": ["parlai=parlai.__main__:main"],
```

### Comparing `parlai-1.7.1/tests/tod/test_tod_agents_and_teachers.py` & `parlai-1.7.2/tests/tod/test_tod_agents_and_teachers.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/tests/tod/test_tod_teacher_metrics.py` & `parlai-1.7.2/tests/tod/test_tod_teacher_metrics.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/tests/tod/test_tod_world_and_script.py` & `parlai-1.7.2/tests/tod/test_tod_world_and_script.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/tests/tod/test_tod_world_metrics.py` & `parlai-1.7.2/tests/tod/test_tod_world_metrics.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/tests/tod/test_tod_world_metrics_in_script.py` & `parlai-1.7.2/tests/tod/test_tod_world_metrics_in_script.py`

 * *Files identical despite different names*

### Comparing `parlai-1.7.1/tests/tod/test_tod_world_script_metrics.py` & `parlai-1.7.2/tests/tod/test_tod_world_script_metrics.py`

 * *Files identical despite different names*

