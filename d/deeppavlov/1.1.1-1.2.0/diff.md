# Comparing `tmp/deeppavlov-1.1.1.tar.gz` & `tmp/deeppavlov-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeppavlov-1.1.1.tar", last modified: Tue Mar 14 17:23:19 2023, max compression
+gzip compressed data, was "deeppavlov-1.2.0.tar", last modified: Tue Jun  6 09:02:55 2023, max compression
```

## Comparing `deeppavlov-1.1.1.tar` & `deeppavlov-1.2.0.tar`

### file list

```diff
@@ -1,372 +1,372 @@
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.449124 deeppavlov-1.1.1/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11434 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/LICENSE
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      167 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/MANIFEST.in
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8668 2023-03-14 17:23:19.449124 deeppavlov-1.1.1/PKG-INFO
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7830 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/README.md
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.417123 deeppavlov-1.1.1/deeppavlov/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1998 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       66 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/__main__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      324 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/_meta.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.417123 deeppavlov-1.1.1/deeppavlov/configs/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2398 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/__init__.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.421123 deeppavlov-1.1.1/deeppavlov/configs/classifiers/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1655 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/boolqa_rubert.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.421123 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2861 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_cola_cased_bert_torch.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2604 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_mnli_cased_bert_torch.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2613 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_mnli_mm_cased_bert_torch.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3116 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_mnli_roberta.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2233 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_mrpc_cased_bert_torch.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2585 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_qnli_cased_bert_torch.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2237 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_qqp_cased_bert_torch.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2583 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_rte_cased_bert_torch.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3085 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_rte_roberta_mnli.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2855 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_sst2_cased_bert_torch.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1941 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_stsb_cased_bert_torch.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3162 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_wnli_roberta.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3229 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/insults_kaggle_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2444 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_2L.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2444 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_6L.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2164 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/paraphraser_rubert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2861 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/query_pr.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3198 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/rusentiment_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3237 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/rusentiment_convers_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3400 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_2L.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3397 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_6L.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3199 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/sentiment_sst_conv_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3540 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/sentiment_twitter.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.421123 deeppavlov-1.1.1/deeppavlov/configs/classifiers/superglue/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3343 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/superglue/superglue_boolq_roberta_mnli.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4136 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/superglue/superglue_copa_roberta.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3640 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/superglue/superglue_record_roberta.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4075 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/classifiers/topics_distilbert_base_uncased.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.421123 deeppavlov-1.1.1/deeppavlov/configs/doc_retrieval/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2429 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/doc_retrieval/en_ranker_pop_enwiki20180211.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1863 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/doc_retrieval/en_ranker_tfidf_wiki.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1906 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/doc_retrieval/ru_ranker_tfidf_wiki.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.421123 deeppavlov-1.1.1/deeppavlov/configs/embedder/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1272 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/embedder/bert_embedder.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1237 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/embedder/bert_sentence_embedder.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.421123 deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1481 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_detection_en.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1348 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_detection_ru.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      754 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_extraction_en.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      754 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_extraction_ru.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2152 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_linking_en.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2184 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_linking_ru.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.421123 deeppavlov-1.1.1/deeppavlov/configs/faq/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2996 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/faq/fasttext_logreg.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.421123 deeppavlov-1.1.1/deeppavlov/configs/kbqa/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3118 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/kbqa/kbqa_cq_en.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4125 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/kbqa/kbqa_cq_ru.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      769 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/kbqa/wiki_parser.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.425123 deeppavlov-1.1.1/deeppavlov/configs/multitask/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7491 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/multitask/mt_glue.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6674 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/multitask/multitask_example.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.425123 deeppavlov-1.1.1/deeppavlov/configs/ner/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2984 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ner/ner_case_agnostic_mdistilbert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3462 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ner/ner_collection3_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3431 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ner/ner_conll2003_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2955 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ner/ner_ontonotes_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2978 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ner/ner_ontonotes_bert_mult.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3408 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ner/ner_rus_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3241 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ner/ner_rus_bert_probas.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3494 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_2L.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3494 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_6L.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.425123 deeppavlov-1.1.1/deeppavlov/configs/odqa/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1373 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/odqa/en_odqa_infer_wiki.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1682 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/odqa/en_odqa_pop_infer_enwiki20180211.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1502 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/odqa/ru_odqa_infer_wiki.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1512 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/odqa/ru_odqa_infer_wiki_retr_noans.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.425123 deeppavlov-1.1.1/deeppavlov/configs/ranking/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2119 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ranking/ranking_ubuntu_v2_torch_bert_uncased.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2955 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ranking/rel_ranking_bert_en.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2969 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/ranking/rel_ranking_bert_ru.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.425123 deeppavlov-1.1.1/deeppavlov/configs/regressors/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2342 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/regressors/translation_ranker.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.425123 deeppavlov-1.1.1/deeppavlov/configs/relation_extraction/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2611 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/relation_extraction/re_docred.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2693 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/relation_extraction/re_rured.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.425123 deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2922 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_danetqa_rubert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2976 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_lidirus_rubert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2924 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_muserc_rubert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2823 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_parus_rubert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2770 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_rcb_rubert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3083 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_rucos_rubert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2789 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_russe_rubert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2737 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_rwsd_rubert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2876 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_terra_rubert.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.425123 deeppavlov-1.1.1/deeppavlov/configs/sentence_segmentation/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3055 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/sentence_segmentation/sentseg_dailydialog_bert.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.425123 deeppavlov-1.1.1/deeppavlov/configs/spelling_correction/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2142 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/spelling_correction/brillmoore_wikitypos_en.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1589 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/spelling_correction/levenshtein_corrector_ru.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.429123 deeppavlov-1.1.1/deeppavlov/configs/squad/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3376 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/squad/qa_multisberquad_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3938 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/squad/qa_squad2_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3198 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/squad/squad_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3912 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/squad/squad_ru_bert.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3992 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/squad/squad_ru_convers_distilrubert_2L.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3994 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/configs/squad/squad_ru_convers_distilrubert_6L.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.429123 deeppavlov-1.1.1/deeppavlov/core/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/__init__.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.429123 deeppavlov-1.1.1/deeppavlov/core/commands/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/commands/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4354 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/commands/infer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4962 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/commands/train.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6310 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/commands/utils.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.429123 deeppavlov-1.1.1/deeppavlov/core/common/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2063 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/aliases.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2679 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/base.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    12027 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/chainer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3703 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/cross_validation.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      895 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/errors.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2997 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/file.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2022 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/log.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2209 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/log_events.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2724 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/metrics_registry.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2280 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/metrics_registry.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3956 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/params.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     9623 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/params_search.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2086 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/paths.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      877 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/prints.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    10487 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/registry.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2778 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/registry.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6141 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/common/requirements_registry.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.429123 deeppavlov-1.1.1/deeppavlov/core/data/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/data/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3594 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/data/data_fitting_iterator.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3673 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/data/data_learning_iterator.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1074 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/data/dataset_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6308 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/data/simple_vocab.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    22486 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/data/utils.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.429123 deeppavlov-1.1.1/deeppavlov/core/models/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/models/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1195 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/models/component.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      911 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/models/estimator.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    19554 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/models/lr_scheduled_model.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      952 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/models/nn_model.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2235 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/models/serializable.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11330 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/models/torch_model.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.433123 deeppavlov-1.1.1/deeppavlov/core/trainers/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      718 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/trainers/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11044 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/trainers/fit_trainer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    16172 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/trainers/nn_trainer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1829 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/trainers/torch_trainer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2463 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/core/trainers/utils.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.433123 deeppavlov-1.1.1/deeppavlov/dataset_iterators/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_iterators/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6724 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_iterators/basic_classification_iterator.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2536 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_iterators/huggingface_dataset_iterator.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    14745 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_iterators/multitask_iterator.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1488 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_iterators/siamese_iterator.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5761 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_iterators/sqlite_iterator.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    12610 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_iterators/squad_iterator.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1464 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_iterators/typos_iterator.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.433123 deeppavlov-1.1.1/deeppavlov/dataset_readers/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4895 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/basic_classification_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3350 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/boolqa_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6262 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/conll2003_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    20084 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/docred_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2021 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/faq_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    21135 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/huggingface_dataset_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2935 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/imdb_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1415 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/line_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2190 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/multitask_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7941 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/odqa_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2393 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/paraphraser_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2412 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/rel_ranking_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7141 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/rured_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1002 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/sq_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5796 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/squad_dataset_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5636 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/typos_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3321 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/dataset_readers/ubuntu_v2_reader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5759 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/deep.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6531 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/download.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.437123 deeppavlov-1.1.1/deeppavlov/metrics/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6650 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/accuracy.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2880 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/bleu.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1201 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/correlation.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1028 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/elmo_metrics.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    16934 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/fmeasure.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4313 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/google_bleu.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1194 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/log_loss.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1275 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/mse.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1912 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/recall_at_k.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2888 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/record_metrics.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1457 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/roc_auc_score.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5646 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/metrics/squad_metrics.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.437123 deeppavlov-1.1.1/deeppavlov/models/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      967 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/__init__.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.437123 deeppavlov-1.1.1/deeppavlov/models/api_requester/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       29 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/api_requester/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3650 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/api_requester/api_requester.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2279 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/api_requester/api_router.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.437123 deeppavlov-1.1.1/deeppavlov/models/classifiers/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/classifiers/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5367 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/classifiers/cos_sim_classifier.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3761 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/classifiers/proba2labels.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8162 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/classifiers/re_bert.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8667 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/classifiers/torch_classification_model.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3251 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/classifiers/torch_nets.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3343 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/classifiers/utils.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.437123 deeppavlov-1.1.1/deeppavlov/models/doc_retrieval/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/doc_retrieval/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6342 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/doc_retrieval/logit_ranker.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4260 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/doc_retrieval/pop_ranker.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3029 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/doc_retrieval/tfidf_ranker.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1202 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/doc_retrieval/utils.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.437123 deeppavlov-1.1.1/deeppavlov/models/embedders/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/embedders/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4128 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/embedders/abstract_embedder.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2032 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/embedders/fasttext_embedder.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11841 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/embedders/tfidf_weighted_embedder.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4920 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/embedders/transformers_embedder.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.437123 deeppavlov-1.1.1/deeppavlov/models/entity_extraction/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/entity_extraction/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     9170 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/entity_extraction/entity_detection_parser.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    28415 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/entity_extraction/entity_linking.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    17300 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/entity_extraction/ner_chunker.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.441124 deeppavlov-1.1.1/deeppavlov/models/kbqa/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/kbqa/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    12903 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/kbqa/query_generator.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    15616 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/kbqa/query_generator_base.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11124 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/kbqa/rel_ranking_infer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7922 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/kbqa/sentence_answer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6832 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/kbqa/template_matcher.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    32658 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/kbqa/tree_to_sparql.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7889 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/kbqa/type_define.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4026 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/kbqa/utils.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    26162 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/kbqa/wiki_parser.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.441124 deeppavlov-1.1.1/deeppavlov/models/preprocessors/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3356 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/dirty_comments_preprocessor.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1249 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/mask.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6025 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/multitask_preprocessor.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4789 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/ner_preprocessor.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6619 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/odqa_preprocessors.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3145 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/one_hotter.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    10960 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/re_preprocessor.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2501 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/response_base_loader.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2471 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/sanitizer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      663 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/sentseg_preprocessor.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5875 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/squad_preprocessor.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1133 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/str_lower.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2606 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/str_token_reverser.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8427 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/str_utf8_encoder.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    38125 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/torch_transformers_preprocessor.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3393 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/preprocessors/transformers_preprocessor.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.441124 deeppavlov-1.1.1/deeppavlov/models/ranking/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/ranking/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1715 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/ranking/metrics.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.441124 deeppavlov-1.1.1/deeppavlov/models/relation_extraction/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/relation_extraction/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2434 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/relation_extraction/losses.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6674 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/relation_extraction/relation_extraction_bert.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.441124 deeppavlov-1.1.1/deeppavlov/models/sklearn/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       33 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/sklearn/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    12929 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/sklearn/sklearn_component.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.441124 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/__init__.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.441124 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/brillmoore/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       36 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/brillmoore/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    10850 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/brillmoore/error_model.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.441124 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/electors/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/electors/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2861 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/electors/kenlm_elector.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1446 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/electors/top1_elector.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.441124 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/levenshtein/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       61 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/levenshtein/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    33386 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/levenshtein/levenshtein_searcher.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3423 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/levenshtein/searcher_component.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    20586 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/spelling_correction/levenshtein/tabled_trie.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.445124 deeppavlov-1.1.1/deeppavlov/models/tokenizers/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/tokenizers/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2061 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/tokenizers/nltk_moses_tokenizer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1718 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/tokenizers/nltk_tokenizer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8783 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/tokenizers/spacy_tokenizer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1447 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/tokenizers/split_tokenizer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2278 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/tokenizers/utils.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.445124 deeppavlov-1.1.1/deeppavlov/models/torch_bert/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/torch_bert/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1166 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/torch_bert/crf.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    30625 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/torch_bert/multitask_transformer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     9011 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_bert_ranker.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    14169 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_transformers_classifier.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    20166 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_transformers_el_ranker.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8955 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_transformers_multiplechoice.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    14003 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_transformers_sequence_tagger.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    13858 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_transformers_squad.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.445124 deeppavlov-1.1.1/deeppavlov/models/vectorizers/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        1 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/vectorizers/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    10022 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/models/vectorizers/hashing_tfidf_vectorizer.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5203 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/paramsearch.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.445124 deeppavlov-1.1.1/deeppavlov/requirements/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       24 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/datasets.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      125 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/en_core_web_sm.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       16 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/fasttext.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        9 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/hdt.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       25 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/kenlm.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       12 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/lxml.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       18 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/opt_einsum.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       21 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/pytorch.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       17 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/rapidfuzz.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      127 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/ru_core_news_sm.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       19 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/sacremoses.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       21 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/slovnet.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       24 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/sortedcontainers.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       19 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/torchcrf.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       29 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/transformers.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       13 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/udapi.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       17 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/requirements/whapi.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1286 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/settings.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.445124 deeppavlov-1.1.1/deeppavlov/utils/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/__init__.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.445124 deeppavlov-1.1.1/deeppavlov/utils/agent/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       41 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/agent/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2746 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/agent/messages.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    12179 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/agent/rabbitmq.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3935 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/agent/server.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.445124 deeppavlov-1.1.1/deeppavlov/utils/connector/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       40 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/connector/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4779 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/connector/dialog_logger.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.445124 deeppavlov-1.1.1/deeppavlov/utils/pip_wrapper/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       27 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/pip_wrapper/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2662 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/pip_wrapper/pip_wrapper.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.449124 deeppavlov-1.1.1/deeppavlov/utils/server/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       97 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/server/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2451 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/server/metrics.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8866 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/server/server.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.449124 deeppavlov-1.1.1/deeppavlov/utils/settings/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/settings/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      150 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/settings/dialog_logger_config.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2005 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/settings/log_config.json
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      603 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/settings/server_config.json
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.449124 deeppavlov-1.1.1/deeppavlov/utils/socket/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       48 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/socket/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     9577 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/utils/socket/socket.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.449124 deeppavlov-1.1.1/deeppavlov/vocabs/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/vocabs/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6141 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/vocabs/typos.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2312 2023-03-14 17:16:16.000000 deeppavlov-1.1.1/deeppavlov/vocabs/wiki_sqlite.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.417123 deeppavlov-1.1.1/deeppavlov.egg-info/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8668 2023-03-14 17:23:19.000000 deeppavlov-1.1.1/deeppavlov.egg-info/PKG-INFO
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    14340 2023-03-14 17:23:19.000000 deeppavlov-1.1.1/deeppavlov.egg-info/SOURCES.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        1 2023-03-14 17:23:19.000000 deeppavlov-1.1.1/deeppavlov.egg-info/dependency_links.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      600 2023-03-14 17:23:19.000000 deeppavlov-1.1.1/deeppavlov.egg-info/requires.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       17 2023-03-14 17:23:19.000000 deeppavlov-1.1.1/deeppavlov.egg-info/top_level.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      307 2023-03-14 17:16:17.000000 deeppavlov-1.1.1/requirements.txt
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       38 2023-03-14 17:23:19.449124 deeppavlov-1.1.1/setup.cfg
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3011 2023-03-14 17:16:17.000000 deeppavlov-1.1.1/setup.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.449124 deeppavlov-1.1.1/tests/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    31011 2023-03-14 17:16:17.000000 deeppavlov-1.1.1/tests/test_quick_start.py
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.417123 deeppavlov-1.1.1/utils/
-drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:23:19.449124 deeppavlov-1.1.1/utils/prepare/
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-03-14 17:16:17.000000 deeppavlov-1.1.1/utils/prepare/__init__.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3408 2023-03-14 17:16:17.000000 deeppavlov-1.1.1/utils/prepare/hashes.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1485 2023-03-14 17:16:17.000000 deeppavlov-1.1.1/utils/prepare/registry.py
--rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2674 2023-03-14 17:16:17.000000 deeppavlov-1.1.1/utils/prepare/upload.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.989082 deeppavlov-1.2.0/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11434 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/LICENSE
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      167 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/MANIFEST.in
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8668 2023-06-06 09:02:55.989082 deeppavlov-1.2.0/PKG-INFO
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7830 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/README.md
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.957081 deeppavlov-1.2.0/deeppavlov/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1998 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       66 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/__main__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      324 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/_meta.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.957081 deeppavlov-1.2.0/deeppavlov/configs/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2398 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/__init__.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.957081 deeppavlov-1.2.0/deeppavlov/configs/classifiers/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1655 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/boolqa_rubert.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.961082 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3068 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_cola_roberta.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2604 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_mnli_cased_bert_torch.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2613 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_mnli_mm_cased_bert_torch.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3116 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_mnli_roberta.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2768 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_mrpc_roberta.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2792 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_qnli_roberta.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2443 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_qqp_roberta.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2583 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_rte_cased_bert_torch.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3085 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_rte_roberta_mnli.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3062 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_sst2_roberta.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2147 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_stsb_roberta.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3162 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_wnli_roberta.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3229 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/insults_kaggle_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2444 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_2L.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2444 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_6L.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2164 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/paraphraser_rubert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2861 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/query_pr.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3198 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/rusentiment_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3237 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/rusentiment_convers_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3400 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_2L.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3397 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_6L.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3199 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/sentiment_sst_conv_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3540 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/sentiment_twitter.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.961082 deeppavlov-1.2.0/deeppavlov/configs/classifiers/superglue/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3343 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/superglue/superglue_boolq_roberta_mnli.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4136 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/superglue/superglue_copa_roberta.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3640 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/superglue/superglue_record_roberta.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4075 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/classifiers/topics_distilbert_base_uncased.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.961082 deeppavlov-1.2.0/deeppavlov/configs/doc_retrieval/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2429 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/doc_retrieval/en_ranker_pop_enwiki20180211.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1863 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/doc_retrieval/en_ranker_tfidf_wiki.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1906 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/doc_retrieval/ru_ranker_tfidf_wiki.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.961082 deeppavlov-1.2.0/deeppavlov/configs/embedder/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1272 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/embedder/bert_embedder.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1237 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/embedder/bert_sentence_embedder.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.961082 deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1406 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_detection_en.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1274 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_detection_ru.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      798 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_extraction_en.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      798 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_extraction_ru.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1981 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_linking_en.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2731 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_linking_ru.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.961082 deeppavlov-1.2.0/deeppavlov/configs/faq/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2996 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/faq/fasttext_logreg.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.961082 deeppavlov-1.2.0/deeppavlov/configs/kbqa/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7337 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/kbqa/kbqa_cq_en.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     9468 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/kbqa/kbqa_cq_ru.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      769 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/kbqa/wiki_parser.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.961082 deeppavlov-1.2.0/deeppavlov/configs/multitask/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7520 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/multitask/mt_glue.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6703 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/multitask/multitask_example.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.961082 deeppavlov-1.2.0/deeppavlov/configs/ner/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2984 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ner/ner_case_agnostic_mdistilbert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3462 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ner/ner_collection3_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3431 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ner/ner_conll2003_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2955 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ner/ner_ontonotes_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2978 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ner/ner_ontonotes_bert_mult.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3408 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ner/ner_rus_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3241 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ner/ner_rus_bert_probas.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3494 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ner/ner_rus_convers_distilrubert_2L.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3494 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ner/ner_rus_convers_distilrubert_6L.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.961082 deeppavlov-1.2.0/deeppavlov/configs/odqa/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1373 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/odqa/en_odqa_infer_wiki.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1682 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/odqa/en_odqa_pop_infer_enwiki20180211.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1502 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/odqa/ru_odqa_infer_wiki.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1512 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/odqa/ru_odqa_infer_wiki_retr_noans.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.965082 deeppavlov-1.2.0/deeppavlov/configs/ranking/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1365 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ranking/path_ranking_nll_roberta_en.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2119 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ranking/ranking_ubuntu_v2_torch_bert_uncased.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1333 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ranking/rel_ranking_nll_bert_ru.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2753 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/ranking/rel_ranking_roberta_en.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.965082 deeppavlov-1.2.0/deeppavlov/configs/regressors/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2342 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/regressors/translation_ranker.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.965082 deeppavlov-1.2.0/deeppavlov/configs/relation_extraction/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2611 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/relation_extraction/re_docred.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2693 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/relation_extraction/re_rured.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.965082 deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3038 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_danetqa_rubert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3092 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_lidirus_rubert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3039 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_muserc_rubert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2937 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_parus_rubert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2882 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_rcb_rubert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3197 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_rucos_rubert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2903 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_russe_rubert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2850 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_rwsd_rubert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2990 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_terra_rubert.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.965082 deeppavlov-1.2.0/deeppavlov/configs/sentence_segmentation/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3055 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/sentence_segmentation/sentseg_dailydialog_bert.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.965082 deeppavlov-1.2.0/deeppavlov/configs/spelling_correction/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2142 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/spelling_correction/brillmoore_wikitypos_en.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1589 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/spelling_correction/levenshtein_corrector_ru.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.965082 deeppavlov-1.2.0/deeppavlov/configs/squad/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3376 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/squad/qa_multisberquad_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3938 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/squad/qa_squad2_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3198 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/squad/squad_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3912 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/squad/squad_ru_bert.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3992 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/squad/squad_ru_convers_distilrubert_2L.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3994 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/configs/squad/squad_ru_convers_distilrubert_6L.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.965082 deeppavlov-1.2.0/deeppavlov/core/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/__init__.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.965082 deeppavlov-1.2.0/deeppavlov/core/commands/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/commands/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4354 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/commands/infer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4962 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/commands/train.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6310 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/commands/utils.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.969082 deeppavlov-1.2.0/deeppavlov/core/common/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2063 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/aliases.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2679 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/base.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    12027 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/chainer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3703 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/cross_validation.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      895 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/errors.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2997 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/file.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2022 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/log.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2209 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/log_events.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2724 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/metrics_registry.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2280 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/metrics_registry.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3956 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/params.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     9623 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/params_search.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2086 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/paths.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      877 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/prints.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11047 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/registry.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2778 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/registry.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6480 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/common/requirements_registry.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.969082 deeppavlov-1.2.0/deeppavlov/core/data/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/data/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3594 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/data/data_fitting_iterator.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3673 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/data/data_learning_iterator.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1074 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/data/dataset_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6308 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/data/simple_vocab.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    22486 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/data/utils.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.969082 deeppavlov-1.2.0/deeppavlov/core/models/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/models/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1195 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/models/component.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      911 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/models/estimator.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    19554 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/models/lr_scheduled_model.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      952 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/models/nn_model.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2235 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/models/serializable.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11253 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/models/torch_model.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.969082 deeppavlov-1.2.0/deeppavlov/core/trainers/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      718 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/trainers/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11044 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/trainers/fit_trainer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    16172 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/trainers/nn_trainer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1829 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/trainers/torch_trainer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2463 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/core/trainers/utils.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.969082 deeppavlov-1.2.0/deeppavlov/dataset_iterators/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_iterators/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6724 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_iterators/basic_classification_iterator.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2536 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_iterators/huggingface_dataset_iterator.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    14745 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_iterators/multitask_iterator.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1488 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_iterators/siamese_iterator.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5683 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_iterators/sqlite_iterator.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    12610 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_iterators/squad_iterator.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1464 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_iterators/typos_iterator.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.973082 deeppavlov-1.2.0/deeppavlov/dataset_readers/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4848 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/basic_classification_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3350 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/boolqa_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6262 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/conll2003_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    20037 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/docred_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2021 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/faq_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    21088 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/huggingface_dataset_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2887 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/imdb_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1415 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/line_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2190 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/multitask_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7941 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/odqa_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2393 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/paraphraser_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2412 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/rel_ranking_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7094 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/rured_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4228 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/sq_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5796 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/squad_dataset_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5636 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/typos_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3321 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/dataset_readers/ubuntu_v2_reader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4162 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/deep.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6531 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/download.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.973082 deeppavlov-1.2.0/deeppavlov/metrics/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7917 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/accuracy.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2880 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/bleu.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1201 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/correlation.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1028 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/elmo_metrics.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    16934 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/fmeasure.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4313 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/google_bleu.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1194 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/log_loss.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1275 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/mse.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1912 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/recall_at_k.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2888 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/record_metrics.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1457 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/roc_auc_score.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5646 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/metrics/squad_metrics.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.973082 deeppavlov-1.2.0/deeppavlov/models/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      967 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/__init__.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.973082 deeppavlov-1.2.0/deeppavlov/models/api_requester/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       29 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/api_requester/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3650 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/api_requester/api_requester.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2279 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/api_requester/api_router.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.973082 deeppavlov-1.2.0/deeppavlov/models/classifiers/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/classifiers/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5367 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/classifiers/cos_sim_classifier.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3761 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/classifiers/proba2labels.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8162 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/classifiers/re_bert.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8620 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/classifiers/torch_classification_model.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3251 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/classifiers/torch_nets.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3343 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/classifiers/utils.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.977082 deeppavlov-1.2.0/deeppavlov/models/doc_retrieval/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/doc_retrieval/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6342 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/doc_retrieval/logit_ranker.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4260 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/doc_retrieval/pop_ranker.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3029 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/doc_retrieval/tfidf_ranker.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1202 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/doc_retrieval/utils.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.977082 deeppavlov-1.2.0/deeppavlov/models/embedders/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/embedders/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4066 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/embedders/abstract_embedder.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1985 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/embedders/fasttext_embedder.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11794 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/embedders/tfidf_weighted_embedder.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4920 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/embedders/transformers_embedder.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.977082 deeppavlov-1.2.0/deeppavlov/models/entity_extraction/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/entity_extraction/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    14144 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/entity_extraction/entity_detection_parser.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    38834 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/entity_extraction/entity_linking.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4073 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/entity_extraction/find_word.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    21819 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/entity_extraction/ner_chunker.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.977082 deeppavlov-1.2.0/deeppavlov/models/kbqa/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    23911 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/query_generator.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    17243 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/query_generator_base.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    15901 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/rel_ranking_infer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4360 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/ru_adj_to_noun.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7922 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/sentence_answer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6832 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/template_matcher.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    46258 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/tree_to_sparql.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     7169 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/type_define.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    11822 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/utils.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    34996 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/kbqa/wiki_parser.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.981082 deeppavlov-1.2.0/deeppavlov/models/preprocessors/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3356 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/dirty_comments_preprocessor.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1249 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/mask.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6025 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/multitask_preprocessor.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4789 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/ner_preprocessor.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6619 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/odqa_preprocessors.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3145 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/one_hotter.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    10960 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/re_preprocessor.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2501 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/response_base_loader.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2471 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/sanitizer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      663 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/sentseg_preprocessor.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5875 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/squad_preprocessor.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1133 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/str_lower.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2606 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/str_token_reverser.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8350 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/str_utf8_encoder.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    40867 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/torch_transformers_preprocessor.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3393 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/preprocessors/transformers_preprocessor.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.981082 deeppavlov-1.2.0/deeppavlov/models/ranking/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/ranking/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1715 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/ranking/metrics.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.981082 deeppavlov-1.2.0/deeppavlov/models/relation_extraction/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/relation_extraction/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2434 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/relation_extraction/losses.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6674 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/relation_extraction/relation_extraction_bert.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.981082 deeppavlov-1.2.0/deeppavlov/models/sklearn/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       33 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/sklearn/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    12929 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/sklearn/sklearn_component.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.981082 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/__init__.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.981082 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/brillmoore/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       36 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/brillmoore/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    10850 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/brillmoore/error_model.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.981082 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/electors/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/electors/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2861 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/electors/kenlm_elector.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1446 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/electors/top1_elector.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.981082 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/levenshtein/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       61 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/levenshtein/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    33386 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/levenshtein/levenshtein_searcher.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3423 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/levenshtein/searcher_component.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    20586 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/spelling_correction/levenshtein/tabled_trie.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.981082 deeppavlov-1.2.0/deeppavlov/models/tokenizers/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/tokenizers/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2061 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/tokenizers/nltk_moses_tokenizer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1718 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/tokenizers/nltk_tokenizer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8783 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/tokenizers/spacy_tokenizer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1447 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/tokenizers/split_tokenizer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2278 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/tokenizers/utils.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.985082 deeppavlov-1.2.0/deeppavlov/models/torch_bert/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/torch_bert/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1166 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/torch_bert/crf.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    30563 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/torch_bert/multitask_transformer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8964 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_bert_ranker.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    14112 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_classifier.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    20166 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_el_ranker.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8908 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_multiplechoice.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     9170 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_nll_ranking.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    14015 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_sequence_tagger.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    13801 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_squad.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.985082 deeppavlov-1.2.0/deeppavlov/models/vectorizers/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        1 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/vectorizers/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    10022 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/models/vectorizers/hashing_tfidf_vectorizer.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     5203 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/paramsearch.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.985082 deeppavlov-1.2.0/deeppavlov/requirements/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       24 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/datasets.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      125 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/en_core_web_sm.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       16 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/fasttext.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        9 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/hdt.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       25 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/kenlm.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       12 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/lxml.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       18 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/opt_einsum.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       21 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/pytorch.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       17 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/rapidfuzz.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       14 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/razdel.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      127 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/ru_core_news_sm.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       19 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/sacremoses.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       21 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/slovnet.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       24 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/sortedcontainers.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       19 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/torchcrf.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       29 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/transformers.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       13 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/udapi.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       17 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/requirements/whapi.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1286 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/settings.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.985082 deeppavlov-1.2.0/deeppavlov/utils/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/__init__.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.985082 deeppavlov-1.2.0/deeppavlov/utils/connector/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       40 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/connector/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     4779 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/connector/dialog_logger.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.985082 deeppavlov-1.2.0/deeppavlov/utils/pip_wrapper/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       27 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/pip_wrapper/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2662 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/pip_wrapper/pip_wrapper.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.985082 deeppavlov-1.2.0/deeppavlov/utils/server/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       97 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/server/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2451 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/server/metrics.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8866 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/server/server.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.985082 deeppavlov-1.2.0/deeppavlov/utils/settings/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/settings/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      150 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/settings/dialog_logger_config.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2005 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/settings/log_config.json
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      309 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/settings/server_config.json
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.985082 deeppavlov-1.2.0/deeppavlov/utils/socket/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       48 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/socket/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     9577 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/utils/socket/socket.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.989082 deeppavlov-1.2.0/deeppavlov/vocabs/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/vocabs/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     6141 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/vocabs/typos.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2312 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/deeppavlov/vocabs/wiki_sqlite.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.957081 deeppavlov-1.2.0/deeppavlov.egg-info/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     8668 2023-06-06 09:02:55.000000 deeppavlov-1.2.0/deeppavlov.egg-info/PKG-INFO
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    14403 2023-06-06 09:02:55.000000 deeppavlov-1.2.0/deeppavlov.egg-info/SOURCES.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        1 2023-06-06 09:02:55.000000 deeppavlov-1.2.0/deeppavlov.egg-info/dependency_links.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      584 2023-06-06 09:02:55.000000 deeppavlov-1.2.0/deeppavlov.egg-info/requires.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       17 2023-06-06 09:02:55.000000 deeppavlov-1.2.0/deeppavlov.egg-info/top_level.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)      270 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/requirements.txt
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)       38 2023-06-06 09:02:55.989082 deeppavlov-1.2.0/setup.cfg
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3051 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/setup.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.989082 deeppavlov-1.2.0/tests/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)    29796 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/tests/test_quick_start.py
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.953081 deeppavlov-1.2.0/utils/
+drwxrwxr-x   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:02:55.989082 deeppavlov-1.2.0/utils/prepare/
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)        0 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/utils/prepare/__init__.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     3408 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/utils/prepare/hashes.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     1485 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/utils/prepare/registry.py
+-rw-rw-r--   0 ignatov   (1000) ignatov   (1000)     2674 2023-06-06 09:00:34.000000 deeppavlov-1.2.0/utils/prepare/upload.py
```

### Comparing `deeppavlov-1.1.1/LICENSE` & `deeppavlov-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/PKG-INFO` & `deeppavlov-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: deeppavlov
-Version: 1.1.1
+Version: 1.2.0
 Summary: An open source library for building end-to-end dialog systems and training chatbots.
 Home-page: https://github.com/deeppavlov/DeepPavlov
-Download-URL: https://github.com/deeppavlov/DeepPavlov/archive/1.1.1.tar.gz
+Download-URL: https://github.com/deeppavlov/DeepPavlov/archive/1.2.0.tar.gz
 Author: Neural Networks and Deep Learning lab, MIPT
 Author-email: info@deeppavlov.ai
 License: Apache License, Version 2.0
 Keywords: NLP,NER,SQUAD,Intents,Chatbot
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
```

### Comparing `deeppavlov-1.1.1/README.md` & `deeppavlov-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/__init__.py` & `deeppavlov-1.2.0/deeppavlov/__init__.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/__init__.py` & `deeppavlov-1.2.0/deeppavlov/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/boolqa_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/boolqa_rubert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_cola_cased_bert_torch.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_sst2_roberta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9173653083028084%*

 * *Differences: {"'chainer'": "{'pipe': {0: {'vocab_file': 'bert-base-cased'}, 3: {'pretrained_bert': "*

 * *              "'bert-base-cased'}}}",*

 * * "'dataset_reader'": "{'path': '{COMPETITION}', 'name': '{TASK}'}",*

 * * "'metadata'": "{'variables': {'MODEL_PATH': '{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}', "*

 * *               "'BASE_MODEL': 'roberta-large', 'COMPETITION': 'glue', 'TASK': 'sst2'}, 'download': "*

 * *               "[OrderedDict([('url', "*

 * *               "'http://files.deeppavlov.ai/v1/glue/glue_sst2_roberta.tar.gz'), […]*

```diff
@@ -16,15 +16,15 @@
                 "in": [
                     "x"
                 ],
                 "max_seq_length": 64,
                 "out": [
                     "bert_features"
                 ],
-                "vocab_file": "{BASE_MODEL}"
+                "vocab_file": "bert-base-cased"
             },
             {
                 "class_name": "simple_vocab",
                 "fit_on": [
                     "y"
                 ],
                 "id": "classes_vocab",
@@ -63,15 +63,15 @@
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
                     "lr": 2e-05
                 },
                 "out": [
                     "y_pred_probas"
                 ],
-                "pretrained_bert": "{BASE_MODEL}",
+                "pretrained_bert": "bert-base-cased",
                 "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
             },
             {
                 "class_name": "proba2labels",
                 "in": [
                     "y_pred_probas"
@@ -96,39 +96,47 @@
         "class_name": "huggingface_dataset_iterator",
         "features": "sentence",
         "label": "label",
         "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
-        "name": "cola",
-        "path": "glue",
+        "name": "{TASK}",
+        "path": "{COMPETITION}",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
+        "download": [
+            {
+                "subdir": "{MODEL_PATH}",
+                "url": "http://files.deeppavlov.ai/v1/glue/glue_sst2_roberta.tar.gz"
+            }
+        ],
         "variables": {
-            "BASE_MODEL": "bert-base-cased",
+            "BASE_MODEL": "roberta-large",
+            "COMPETITION": "glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/glue_cola_torch_cased_bert",
-            "ROOT_PATH": "~/.deeppavlov"
+            "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
+            "ROOT_PATH": "~/.deeppavlov",
+            "TASK": "sst2"
         }
     },
     "train": {
         "batch_size": 128,
         "class_name": "torch_trainer",
         "evaluation_targets": [
             "train",
             "valid"
         ],
         "log_every_n_batches": 250,
         "metrics": [
-            "matthews_correlation"
+            "accuracy"
         ],
         "pytest_max_batches": 2,
         "show_examples": false,
         "tensorboard_log_dir": "{MODEL_PATH}/",
         "val_every_n_batches": 250,
         "validation_patience": 10
     }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_mnli_cased_bert_torch.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_mnli_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_mnli_mm_cased_bert_torch.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_mnli_mm_cased_bert_torch.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_mnli_roberta.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_mnli_roberta.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_mrpc_cased_bert_torch.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_rte_cased_bert_torch.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9295379273504274%*

 * *Differences: {"'chainer'": "{'in_y': ['y'], 'pipe': {0: {'max_seq_length': 256}, 2: {'depth': "*

 * *              "'#classes_vocab.len'}, 3: {'n_classes': '#classes_vocab.len'}, insert: [(1, "*

 * *              "OrderedDict([('id', 'classes_vocab'), ('class_name', 'simple_vocab'), ('fit_on', "*

 * *              "['y']), ('save_path', '{MODEL_PATH}/classes.dict'), ('load_path', "*

 * *              "'{MODEL_PATH}/classes.dict'), ('in', ['y']), ('out', ['y_ids'])])), (5, "*

 * *              "OrderedDict([('in', ['y_pred_ids']), ('out', ['y_pr […]*

```diff
@@ -1,36 +1,51 @@
 {
     "chainer": {
         "in": [
             "sentence1",
             "sentence2"
         ],
         "in_y": [
-            "y_ids"
+            "y"
         ],
         "out": [
-            "y_pred_ids"
+            "y_pred_labels"
         ],
         "pipe": [
             {
                 "class_name": "torch_transformers_preprocessor",
                 "do_lower_case": false,
                 "in": [
                     "sentence1",
                     "sentence2"
                 ],
-                "max_seq_length": 100,
+                "max_seq_length": 256,
                 "out": [
                     "bert_features"
                 ],
                 "vocab_file": "{BASE_MODEL}"
             },
             {
+                "class_name": "simple_vocab",
+                "fit_on": [
+                    "y"
+                ],
+                "id": "classes_vocab",
+                "in": [
+                    "y"
+                ],
+                "load_path": "{MODEL_PATH}/classes.dict",
+                "out": [
+                    "y_ids"
+                ],
+                "save_path": "{MODEL_PATH}/classes.dict"
+            },
+            {
                 "class_name": "one_hotter",
-                "depth": 2,
+                "depth": "#classes_vocab.len",
                 "in": [
                     "y_ids"
                 ],
                 "out": [
                     "y_onehot"
                 ],
                 "single_vector": true
@@ -42,15 +57,15 @@
                 ],
                 "in_y": [
                     "y_ids"
                 ],
                 "learning_rate_drop_div": 2.0,
                 "learning_rate_drop_patience": 3,
                 "load_path": "{MODEL_PATH}/model",
-                "n_classes": 2,
+                "n_classes": "#classes_vocab.len",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
                     "lr": 2e-05
                 },
                 "out": [
                     "y_pred_probas"
                 ],
@@ -63,54 +78,61 @@
                 "in": [
                     "y_pred_probas"
                 ],
                 "max_proba": true,
                 "out": [
                     "y_pred_ids"
                 ]
+            },
+            {
+                "in": [
+                    "y_pred_ids"
+                ],
+                "out": [
+                    "y_pred_labels"
+                ],
+                "ref": "classes_vocab"
             }
         ]
     },
     "dataset_iterator": {
         "class_name": "huggingface_dataset_iterator",
         "features": [
             "sentence1",
             "sentence2"
         ],
         "label": "label",
-        "seed": 42,
-        "use_label_name": false
+        "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
-        "name": "mrpc",
+        "name": "rte",
         "path": "glue",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
         "variables": {
             "BASE_MODEL": "bert-base-cased",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/glue_mrpc_torch_cased_bert",
+            "MODEL_PATH": "{MODELS_PATH}/classifiers/glue_rte_torch_cased_bert",
             "ROOT_PATH": "~/.deeppavlov"
         }
     },
     "train": {
-        "batch_size": 100,
+        "batch_size": 32,
         "class_name": "torch_trainer",
         "evaluation_targets": [
             "train",
             "valid"
         ],
         "log_every_n_epochs": 1,
         "metrics": [
-            "f1",
             "accuracy"
         ],
         "pytest_max_batches": 2,
         "show_examples": false,
         "tensorboard_log_dir": "{MODEL_PATH}/",
         "val_every_n_epochs": 1,
         "validation_patience": 10
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_qnli_cased_bert_torch.json` & `deeppavlov-1.2.0/deeppavlov/configs/ranking/rel_ranking_roberta_en.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7288438413438414%*

 * *Differences: {"'chainer'": "{'in': {insert: [(1, 'rel_list')], delete: [1]}, 'pipe': {0: {'class_name': "*

 * *              "'rel_ranking_preprocessor', 'vocab_file': '{TRANSFORMER}', 'max_seq_length': 64, "*

 * *              "'in': {insert: [(1, 'rel_list')], delete: [1]}}, 3: {'pretrained_bert': "*

 * *              "'{TRANSFORMER}', 'optimizer_parameters': {'lr': 1e-05}, "*

 * *              "'learning_rate_drop_patience': 5}}}",*

 * * "'dataset_iterator'": "{'class_name': 'basic_classification_iterator', delete: ['features', "*

 * *            […]*

```diff
@@ -1,32 +1,32 @@
 {
     "chainer": {
         "in": [
             "question",
-            "sentence"
+            "rel_list"
         ],
         "in_y": [
             "y"
         ],
         "out": [
             "y_pred_labels"
         ],
         "pipe": [
             {
-                "class_name": "torch_transformers_preprocessor",
+                "class_name": "rel_ranking_preprocessor",
                 "do_lower_case": false,
                 "in": [
                     "question",
-                    "sentence"
+                    "rel_list"
                 ],
-                "max_seq_length": 128,
+                "max_seq_length": 64,
                 "out": [
                     "bert_features"
                 ],
-                "vocab_file": "{BASE_MODEL}"
+                "vocab_file": "{TRANSFORMER}"
             },
             {
                 "class_name": "simple_vocab",
                 "fit_on": [
                     "y"
                 ],
                 "id": "classes_vocab",
@@ -55,25 +55,25 @@
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
                 "learning_rate_drop_div": 2.0,
-                "learning_rate_drop_patience": 3,
+                "learning_rate_drop_patience": 5,
                 "load_path": "{MODEL_PATH}/model",
                 "n_classes": "#classes_vocab.len",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "lr": 2e-05
+                    "lr": 1e-05
                 },
                 "out": [
                     "y_pred_probas"
                 ],
-                "pretrained_bert": "{BASE_MODEL}",
+                "pretrained_bert": "{TRANSFORMER}",
                 "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
             },
             {
                 "class_name": "proba2labels",
                 "in": [
                     "y_pred_probas"
@@ -91,50 +91,51 @@
                     "y_pred_labels"
                 ],
                 "ref": "classes_vocab"
             }
         ]
     },
     "dataset_iterator": {
-        "class_name": "huggingface_dataset_iterator",
-        "features": [
-            "question",
-            "sentence"
-        ],
-        "label": "label",
+        "class_name": "basic_classification_iterator",
         "seed": 42
     },
     "dataset_reader": {
-        "class_name": "huggingface_dataset_reader",
-        "name": "qnli",
-        "path": "glue",
-        "test": "test",
-        "train": "train",
-        "valid": "validation"
+        "class_name": "sq_reader",
+        "data_path": "{DOWNLOADS_PATH}/rel_ranking_eng/lcquad_one_rel_ranking.json"
     },
     "metadata": {
+        "download": [
+            {
+                "subdir": "{MODEL_PATH}",
+                "url": "http://files.deeppavlov.ai/kbqa/models/rel_ranking_roberta_en.tar.gz"
+            },
+            {
+                "subdir": "{DOWNLOADS_PATH}/rel_ranking_eng",
+                "url": "http://files.deeppavlov.ai/kbqa/wikidata/lcquad_rel_ranking.pickle"
+            }
+        ],
         "variables": {
-            "BASE_MODEL": "bert-base-cased",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/glue_qnli_torch_cased_bert",
-            "ROOT_PATH": "~/.deeppavlov"
+            "MODEL_PATH": "{MODELS_PATH}/classifiers/rel_ranking_roberta_en",
+            "ROOT_PATH": "~/.deeppavlov",
+            "TRANSFORMER": "haisongzhang/roberta-tiny-cased"
         }
     },
     "train": {
-        "batch_size": 64,
+        "batch_size": 30,
         "class_name": "torch_trainer",
+        "epochs": 3,
         "evaluation_targets": [
-            "train",
-            "valid"
+            "valid",
+            "test"
         ],
-        "log_every_n_batches": 250,
+        "log_every_n_batches": 100,
         "metrics": [
-            "accuracy"
+            "accuracy",
+            "f1_macro"
         ],
-        "pytest_max_batches": 2,
         "show_examples": false,
-        "tensorboard_log_dir": "{MODEL_PATH}/",
-        "val_every_n_batches": 250,
+        "val_every_n_batches": 100,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_qqp_cased_bert_torch.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_qqp_roberta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9226190476190477%*

 * *Differences: {"'dataset_reader'": "{'path': '{COMPETITION}', 'name': '{TASK}'}",*

 * * "'metadata'": "{'variables': {'MODEL_PATH': '{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}', "*

 * *               "'BASE_MODEL': 'roberta-large', 'COMPETITION': 'glue', 'TASK': 'qqp'}, 'download': "*

 * *               "[OrderedDict([('url', "*

 * *               "'http://files.deeppavlov.ai/v1/glue/glue_qqp_roberta.tar.gz'), ('subdir', "*

 * *               "'{MODEL_PATH}')])]}"}*

```diff
@@ -78,27 +78,35 @@
         ],
         "label": "label",
         "seed": 42,
         "use_label_name": false
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
-        "name": "qqp",
-        "path": "glue",
+        "name": "{TASK}",
+        "path": "{COMPETITION}",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
+        "download": [
+            {
+                "subdir": "{MODEL_PATH}",
+                "url": "http://files.deeppavlov.ai/v1/glue/glue_qqp_roberta.tar.gz"
+            }
+        ],
         "variables": {
-            "BASE_MODEL": "bert-base-cased",
+            "BASE_MODEL": "roberta-large",
+            "COMPETITION": "glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/glue_qqp_torch_cased_bert",
-            "ROOT_PATH": "~/.deeppavlov"
+            "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
+            "ROOT_PATH": "~/.deeppavlov",
+            "TASK": "qqp"
         }
     },
     "train": {
         "batch_size": 64,
         "class_name": "torch_trainer",
         "evaluation_targets": [
             "train",
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_rte_cased_bert_torch.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/query_pr.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7094665750915752%*

 * *Differences: {"'chainer'": "{'in': ['x'], 'pipe': {0: {'vocab_file': '{TRANSFORMER}', 'max_seq_length': 64, "*

 * *              "'in': ['x']}, 3: {'pretrained_bert': '{TRANSFORMER}', 'optimizer_parameters': "*

 * *              "{'lr': 1e-05}, 'learning_rate_drop_patience': 5}}}",*

 * * "'dataset_iterator'": "{'class_name': 'basic_classification_iterator', delete: ['features', "*

 * *                       "'label']}",*

 * * "'dataset_reader'": "{'class_name': 'sq_reader', 'data_path': "*

 * *                     "'{DOWNLOADS_PATH}/query_prediction […]*

```diff
@@ -1,32 +1,30 @@
 {
     "chainer": {
         "in": [
-            "sentence1",
-            "sentence2"
+            "x"
         ],
         "in_y": [
             "y"
         ],
         "out": [
             "y_pred_labels"
         ],
         "pipe": [
             {
                 "class_name": "torch_transformers_preprocessor",
                 "do_lower_case": false,
                 "in": [
-                    "sentence1",
-                    "sentence2"
+                    "x"
                 ],
-                "max_seq_length": 256,
+                "max_seq_length": 64,
                 "out": [
                     "bert_features"
                 ],
-                "vocab_file": "{BASE_MODEL}"
+                "vocab_file": "{TRANSFORMER}"
             },
             {
                 "class_name": "simple_vocab",
                 "fit_on": [
                     "y"
                 ],
                 "id": "classes_vocab",
@@ -55,25 +53,25 @@
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
                 "learning_rate_drop_div": 2.0,
-                "learning_rate_drop_patience": 3,
+                "learning_rate_drop_patience": 5,
                 "load_path": "{MODEL_PATH}/model",
                 "n_classes": "#classes_vocab.len",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "lr": 2e-05
+                    "lr": 1e-05
                 },
                 "out": [
                     "y_pred_probas"
                 ],
-                "pretrained_bert": "{BASE_MODEL}",
+                "pretrained_bert": "{TRANSFORMER}",
                 "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
             },
             {
                 "class_name": "proba2labels",
                 "in": [
                     "y_pred_probas"
@@ -91,50 +89,59 @@
                     "y_pred_labels"
                 ],
                 "ref": "classes_vocab"
             }
         ]
     },
     "dataset_iterator": {
-        "class_name": "huggingface_dataset_iterator",
-        "features": [
-            "sentence1",
-            "sentence2"
-        ],
-        "label": "label",
+        "class_name": "basic_classification_iterator",
         "seed": 42
     },
     "dataset_reader": {
-        "class_name": "huggingface_dataset_reader",
-        "name": "rte",
-        "path": "glue",
-        "test": "test",
-        "train": "train",
-        "valid": "validation"
+        "class_name": "sq_reader",
+        "data_path": "{DOWNLOADS_PATH}/query_prediction/query_prediction_eng.pickle"
     },
     "metadata": {
+        "download": [
+            {
+                "subdir": "{MODELS_PATH}/classifiers/query_prediction_eng",
+                "url": "http://files.deeppavlov.ai/kbqa/wikidata/query_prediction_eng.tar.gz"
+            },
+            {
+                "subdir": "{DOWNLOADS_PATH}/query_prediction",
+                "url": "http://files.deeppavlov.ai/kbqa/wikidata/query_prediction_eng.pickle"
+            }
+        ],
         "variables": {
-            "BASE_MODEL": "bert-base-cased",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/glue_rte_torch_cased_bert",
-            "ROOT_PATH": "~/.deeppavlov"
+            "MODEL_PATH": "{MODELS_PATH}/classifiers/query_prediction_eng",
+            "ROOT_PATH": "~/.deeppavlov",
+            "TRANSFORMER": "haisongzhang/roberta-tiny-cased"
         }
     },
     "train": {
-        "batch_size": 32,
+        "batch_size": 64,
         "class_name": "torch_trainer",
+        "epochs": 100,
         "evaluation_targets": [
             "train",
-            "valid"
+            "valid",
+            "test"
         ],
-        "log_every_n_epochs": 1,
+        "log_every_n_batches": 100,
         "metrics": [
-            "accuracy"
+            "f1_macro",
+            "accuracy",
+            {
+                "inputs": [
+                    "y_onehot",
+                    "y_pred_probas"
+                ],
+                "name": "roc_auc"
+            }
         ],
-        "pytest_max_batches": 2,
         "show_examples": false,
-        "tensorboard_log_dir": "{MODEL_PATH}/",
-        "val_every_n_epochs": 1,
+        "val_every_n_batches": 100,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_rte_roberta_mnli.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_rte_roberta_mnli.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_sst2_cased_bert_torch.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/superglue/superglue_boolq_roberta_mnli.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.843964629120879%*

 * *Differences: {"'chainer'": "{'in': ['question', 'passage'], 'pipe': {0: {'vocab_file': '{BASE_MODEL}', "*

 * *              "'max_seq_length': 256, 'in': ['question', 'passage']}, 3: {'pretrained_bert': "*

 * *              "'{BASE_MODEL}', 'optimizer_parameters': {'weight_decay': 0.1}, 'is_binary': "*

 * *              "'{BINARY_CLASSIFICATION}'}, 4: {'is_binary': '{BINARY_CLASSIFICATION}', "*

 * *              "'confidence_threshold': 0.5, delete: ['max_proba']}}}",*

 * * "'dataset_iterator'": "{'features': ['question', 'passage']}",*

 * * "'datas […]*

```diff
@@ -1,30 +1,32 @@
 {
     "chainer": {
         "in": [
-            "x"
+            "question",
+            "passage"
         ],
         "in_y": [
             "y"
         ],
         "out": [
             "y_pred_labels"
         ],
         "pipe": [
             {
                 "class_name": "torch_transformers_preprocessor",
                 "do_lower_case": false,
                 "in": [
-                    "x"
+                    "question",
+                    "passage"
                 ],
-                "max_seq_length": 64,
+                "max_seq_length": 256,
                 "out": [
                     "bert_features"
                 ],
-                "vocab_file": "bert-base-cased"
+                "vocab_file": "{BASE_MODEL}"
             },
             {
                 "class_name": "simple_vocab",
                 "fit_on": [
                     "y"
                 ],
                 "id": "classes_vocab",
@@ -52,35 +54,38 @@
                 "class_name": "torch_transformers_classifier",
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
+                "is_binary": "{BINARY_CLASSIFICATION}",
                 "learning_rate_drop_div": 2.0,
                 "learning_rate_drop_patience": 3,
                 "load_path": "{MODEL_PATH}/model",
                 "n_classes": "#classes_vocab.len",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "lr": 2e-05
+                    "lr": 2e-05,
+                    "weight_decay": 0.1
                 },
                 "out": [
                     "y_pred_probas"
                 ],
-                "pretrained_bert": "bert-base-cased",
+                "pretrained_bert": "{BASE_MODEL}",
                 "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
             },
             {
                 "class_name": "proba2labels",
+                "confidence_threshold": 0.5,
                 "in": [
                     "y_pred_probas"
                 ],
-                "max_proba": true,
+                "is_binary": "{BINARY_CLASSIFICATION}",
                 "out": [
                     "y_pred_ids"
                 ]
             },
             {
                 "in": [
                     "y_pred_ids"
@@ -90,46 +95,58 @@
                 ],
                 "ref": "classes_vocab"
             }
         ]
     },
     "dataset_iterator": {
         "class_name": "huggingface_dataset_iterator",
-        "features": "sentence",
+        "features": [
+            "question",
+            "passage"
+        ],
         "label": "label",
         "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
-        "name": "sst2",
-        "path": "glue",
+        "dev_percentage": 50,
+        "name": "boolq",
+        "path": "super_glue",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
+        "download": [
+            {
+                "subdir": "{MODELS_PATH}",
+                "url": "http://files.deeppavlov.ai/v1/superglue/superglue_boolq_roberta_mnli.tar.gz"
+            }
+        ],
         "variables": {
-            "BASE_MODEL": "bert-base-cased",
+            "BASE_MODEL": "roberta-large-mnli",
+            "BINARY_CLASSIFICATION": true,
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/glue_sst2_torch_cased_bert",
+            "MODEL_PATH": "{MODELS_PATH}/classifiers/superglue_boolq_roberta_mnli",
             "ROOT_PATH": "~/.deeppavlov"
         }
     },
     "train": {
-        "batch_size": 128,
+        "batch_size": 24,
         "class_name": "torch_trainer",
         "evaluation_targets": [
             "train",
             "valid"
         ],
-        "log_every_n_batches": 250,
+        "log_every_n_epochs": 1,
         "metrics": [
             "accuracy"
         ],
+        "pytest_batch_size": 2,
         "pytest_max_batches": 2,
         "show_examples": false,
         "tensorboard_log_dir": "{MODEL_PATH}/",
-        "val_every_n_batches": 250,
+        "val_every_n_epochs": 1,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_stsb_cased_bert_torch.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_stsb_roberta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9176190476190478%*

 * *Differences: {"'dataset_reader'": "{'path': '{COMPETITION}', 'name': '{TASK}'}",*

 * * "'metadata'": "{'variables': {'MODEL_PATH': '{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}', "*

 * *               "'BASE_MODEL': 'roberta-large', 'COMPETITION': 'glue', 'TASK': 'stsb'}, 'download': "*

 * *               "[OrderedDict([('url', "*

 * *               "'http://files.deeppavlov.ai/v1/glue/glue_stsb_roberta.tar.gz'), ('subdir', "*

 * *               "'{MODEL_PATH}')])]}",*

 * * "'train'": "{'batch_size': 32}"}*

```diff
@@ -57,31 +57,39 @@
         ],
         "label": "label",
         "seed": 42,
         "use_label_name": false
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
-        "name": "stsb",
-        "path": "glue",
+        "name": "{TASK}",
+        "path": "{COMPETITION}",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
+        "download": [
+            {
+                "subdir": "{MODEL_PATH}",
+                "url": "http://files.deeppavlov.ai/v1/glue/glue_stsb_roberta.tar.gz"
+            }
+        ],
         "variables": {
-            "BASE_MODEL": "bert-base-cased",
+            "BASE_MODEL": "roberta-large",
+            "COMPETITION": "glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/glue_stsb_torch_cased_bert",
-            "ROOT_PATH": "~/.deeppavlov"
+            "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
+            "ROOT_PATH": "~/.deeppavlov",
+            "TASK": "stsb"
         }
     },
     "train": {
-        "batch_size": 128,
+        "batch_size": 32,
         "class_name": "torch_trainer",
         "evaluation_targets": [
             "train",
             "valid"
         ],
         "log_every_n_epochs": 1,
         "metrics": [
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/glue/glue_wnli_roberta.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_wnli_roberta.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/insults_kaggle_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/insults_kaggle_bert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_2L.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_2L.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_6L.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/paraphraser_convers_distilrubert_6L.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/paraphraser_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/paraphraser_rubert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/query_pr.json` & `deeppavlov-1.2.0/deeppavlov/configs/sentence_segmentation/sentseg_dailydialog_bert.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7757612663287005%*

 * *Differences: {"'chainer'": "{'pipe': {0: {'class_name': 'torch_transformers_ner_preprocessor', 'do_lower_case': "*

 * *              "True, 'max_seq_length': 512, 'out': ['x_tokens', 'x_subword_tokens', "*

 * *              "'x_subword_tok_ids', 'startofword_markers', 'attention_mask', 'tokens_offsets'], "*

 * *              "'max_subword_length': 15, 'token_masking_prob': 0.0}, 1: {'id': 'tag_vocab', "*

 * *              "'save_path': '{MODEL_PATH}/tag.dict', 'load_path': '{MODEL_PATH}/tag.dict', 'out': "*

 * *              "['y_ind'], 'unk_to […]*

```diff
@@ -3,145 +3,161 @@
         "in": [
             "x"
         ],
         "in_y": [
             "y"
         ],
         "out": [
-            "y_pred_labels"
+            "x_tokens",
+            "punctuated_sents"
         ],
         "pipe": [
             {
-                "class_name": "torch_transformers_preprocessor",
-                "do_lower_case": false,
+                "class_name": "torch_transformers_ner_preprocessor",
+                "do_lower_case": true,
                 "in": [
                     "x"
                 ],
-                "max_seq_length": 64,
+                "max_seq_length": 512,
+                "max_subword_length": 15,
                 "out": [
-                    "bert_features"
+                    "x_tokens",
+                    "x_subword_tokens",
+                    "x_subword_tok_ids",
+                    "startofword_markers",
+                    "attention_mask",
+                    "tokens_offsets"
                 ],
+                "token_masking_prob": 0.0,
                 "vocab_file": "{TRANSFORMER}"
             },
             {
                 "class_name": "simple_vocab",
                 "fit_on": [
                     "y"
                 ],
-                "id": "classes_vocab",
+                "id": "tag_vocab",
                 "in": [
                     "y"
                 ],
-                "load_path": "{MODEL_PATH}/classes.dict",
+                "load_path": "{MODEL_PATH}/tag.dict",
                 "out": [
-                    "y_ids"
+                    "y_ind"
                 ],
-                "save_path": "{MODEL_PATH}/classes.dict"
+                "pad_with_zeros": true,
+                "save_path": "{MODEL_PATH}/tag.dict",
+                "unk_token": [
+                    "O"
+                ]
             },
             {
-                "class_name": "one_hotter",
-                "depth": "#classes_vocab.len",
-                "in": [
-                    "y_ids"
-                ],
-                "out": [
-                    "y_onehot"
+                "attention_probs_keep_prob": 0.5,
+                "class_name": "torch_transformers_sequence_tagger",
+                "clip_norm": 1.0,
+                "encoder_layer_ids": [
+                    -1
                 ],
-                "single_vector": true
-            },
-            {
-                "class_name": "torch_transformers_classifier",
                 "in": [
-                    "bert_features"
+                    "x_subword_tok_ids",
+                    "attention_mask",
+                    "startofword_markers"
                 ],
                 "in_y": [
-                    "y_ids"
+                    "y_ind"
                 ],
-                "learning_rate_drop_div": 2.0,
-                "learning_rate_drop_patience": 5,
+                "learning_rate_drop_div": 1.5,
+                "learning_rate_drop_patience": 6,
+                "load_before_drop": true,
                 "load_path": "{MODEL_PATH}/model",
-                "n_classes": "#classes_vocab.len",
+                "min_learning_rate": 1e-07,
+                "n_tags": "#tag_vocab.len",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "lr": 1e-05
+                    "betas": [
+                        0.9,
+                        0.999
+                    ],
+                    "eps": 1e-06,
+                    "lr": 2e-05,
+                    "weight_decay": 1e-06
                 },
                 "out": [
-                    "y_pred_probas"
+                    "y_pred_ind",
+                    "probas"
                 ],
                 "pretrained_bert": "{TRANSFORMER}",
-                "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
             },
             {
-                "class_name": "proba2labels",
                 "in": [
-                    "y_pred_probas"
+                    "y_pred_ind"
                 ],
-                "max_proba": true,
                 "out": [
-                    "y_pred_ids"
-                ]
+                    "y_pred"
+                ],
+                "ref": "tag_vocab"
             },
             {
+                "class_name": "sentseg_restore_sent",
                 "in": [
-                    "y_pred_ids"
+                    "x_tokens",
+                    "y_pred"
                 ],
-                "out": [
-                    "y_pred_labels"
-                ],
-                "ref": "classes_vocab"
+                "out": "punctuated_sents"
             }
         ]
     },
     "dataset_iterator": {
-        "class_name": "basic_classification_iterator",
-        "seed": 42
+        "class_name": "data_learning_iterator"
     },
     "dataset_reader": {
-        "class_name": "sq_reader",
-        "data_path": "{DOWNLOADS_PATH}/query_prediction/query_prediction_eng.pickle"
+        "class_name": "conll2003_reader",
+        "data_path": "{DOWNLOADS_PATH}/dailydialog/",
+        "dataset_name": "dailydialog"
     },
     "metadata": {
         "download": [
             {
-                "subdir": "{MODELS_PATH}/classifiers/query_prediction_eng",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/query_prediction_eng.tar.gz"
-            },
-            {
-                "subdir": "{DOWNLOADS_PATH}/query_prediction",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/query_prediction_eng.pickle"
+                "subdir": "{MODEL_PATH}",
+                "url": "http://files.deeppavlov.ai/deeppavlov_data/sentseg_dailydialog_bert.tar.gz"
             }
         ],
         "variables": {
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/query_prediction_eng",
+            "MODEL_PATH": "{MODELS_PATH}/sentseg_dailydialog_bert",
             "ROOT_PATH": "~/.deeppavlov",
-            "TRANSFORMER": "haisongzhang/roberta-tiny-cased"
+            "TRANSFORMER": "bert-base-uncased"
         }
     },
     "train": {
-        "batch_size": 64,
+        "batch_size": 30,
         "class_name": "torch_trainer",
-        "epochs": 100,
+        "epochs": 30,
         "evaluation_targets": [
-            "train",
             "valid",
             "test"
         ],
         "log_every_n_batches": 100,
         "metrics": [
-            "f1_macro",
-            "accuracy",
             {
                 "inputs": [
-                    "y_onehot",
-                    "y_pred_probas"
+                    "y",
+                    "y_pred"
+                ],
+                "name": "ner_f1"
+            },
+            {
+                "inputs": [
+                    "y",
+                    "y_pred"
                 ],
-                "name": "roc_auc"
+                "name": "ner_token_f1"
             }
         ],
+        "pytest_batch_size": 8,
+        "pytest_max_batches": 2,
         "show_examples": false,
         "val_every_n_batches": 100,
-        "validation_patience": 10
+        "validation_patience": 20
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/rusentiment_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/rusentiment_bert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/rusentiment_convers_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/rusentiment_convers_bert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_2L.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_2L.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_6L.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_6L.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/sentiment_sst_conv_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/sentiment_sst_conv_bert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/sentiment_twitter.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/sentiment_twitter.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/superglue/superglue_boolq_roberta_mnli.json` & `deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_danetqa_rubert.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9184151785714285%*

 * *Differences: {"'chainer'": "{'pipe': {0: {'max_seq_length': 512}, 3: {'optimizer_parameters': {delete: "*

 * *              "['weight_decay']}, delete: ['learning_rate_drop_patience', "*

 * *              "'learning_rate_drop_div']}, 4: {'max_proba': True, delete: "*

 * *              "['confidence_threshold']}}}",*

 * * "'dataset_reader'": "{'path': '{COMPETITION}', 'name': '{TASK}', 'data_url': "*

 * *                     "'http://files.deeppavlov.ai/datasets/russian_super_glue/DaNetQA', "*

 * *                     "'ignore_verifications': True, d […]*

```diff
@@ -14,15 +14,15 @@
             {
                 "class_name": "torch_transformers_preprocessor",
                 "do_lower_case": false,
                 "in": [
                     "question",
                     "passage"
                 ],
-                "max_seq_length": 256,
+                "max_seq_length": 512,
                 "out": [
                     "bert_features"
                 ],
                 "vocab_file": "{BASE_MODEL}"
             },
             {
                 "class_name": "simple_vocab",
@@ -55,37 +55,34 @@
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
                 "is_binary": "{BINARY_CLASSIFICATION}",
-                "learning_rate_drop_div": 2.0,
-                "learning_rate_drop_patience": 3,
                 "load_path": "{MODEL_PATH}/model",
                 "n_classes": "#classes_vocab.len",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "lr": 2e-05,
-                    "weight_decay": 0.1
+                    "lr": 2e-05
                 },
                 "out": [
                     "y_pred_probas"
                 ],
                 "pretrained_bert": "{BASE_MODEL}",
                 "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
             },
             {
                 "class_name": "proba2labels",
-                "confidence_threshold": 0.5,
                 "in": [
                     "y_pred_probas"
                 ],
                 "is_binary": "{BINARY_CLASSIFICATION}",
+                "max_proba": true,
                 "out": [
                     "y_pred_ids"
                 ]
             },
             {
                 "in": [
                     "y_pred_ids"
@@ -104,40 +101,44 @@
             "passage"
         ],
         "label": "label",
         "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
-        "dev_percentage": 50,
-        "name": "boolq",
-        "path": "super_glue",
+        "data_url": "http://files.deeppavlov.ai/datasets/russian_super_glue/DaNetQA",
+        "ignore_verifications": true,
+        "name": "{TASK}",
+        "path": "{COMPETITION}",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
         "download": [
             {
-                "subdir": "{MODELS_PATH}",
-                "url": "http://files.deeppavlov.ai/v1/superglue/superglue_boolq_roberta_mnli.tar.gz"
+                "subdir": "{MODEL_PATH}",
+                "url": "http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_danetqa_rubert.tar.gz"
             }
         ],
         "variables": {
-            "BASE_MODEL": "roberta-large-mnli",
-            "BINARY_CLASSIFICATION": true,
+            "BASE_MODEL": "DeepPavlov/rubert-base-cased",
+            "BINARY_CLASSIFICATION": false,
+            "COMPETITION": "russian_super_glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/superglue_boolq_roberta_mnli",
-            "ROOT_PATH": "~/.deeppavlov"
+            "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
+            "ROOT_PATH": "~/.deeppavlov",
+            "TASK": "danetqa"
         }
     },
     "train": {
-        "batch_size": 24,
+        "batch_size": 4,
         "class_name": "torch_trainer",
+        "epochs": 10,
         "evaluation_targets": [
             "train",
             "valid"
         ],
         "log_every_n_epochs": 1,
         "metrics": [
             "accuracy"
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/superglue/superglue_copa_roberta.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/superglue/superglue_copa_roberta.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/superglue/superglue_record_roberta.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/superglue/superglue_record_roberta.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/classifiers/topics_distilbert_base_uncased.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/topics_distilbert_base_uncased.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/doc_retrieval/en_ranker_pop_enwiki20180211.json` & `deeppavlov-1.2.0/deeppavlov/configs/doc_retrieval/en_ranker_pop_enwiki20180211.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/doc_retrieval/en_ranker_tfidf_wiki.json` & `deeppavlov-1.2.0/deeppavlov/configs/doc_retrieval/en_ranker_tfidf_wiki.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/doc_retrieval/ru_ranker_tfidf_wiki.json` & `deeppavlov-1.2.0/deeppavlov/configs/doc_retrieval/ru_ranker_tfidf_wiki.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/embedder/bert_embedder.json` & `deeppavlov-1.2.0/deeppavlov/configs/embedder/bert_embedder.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/embedder/bert_sentence_embedder.json` & `deeppavlov-1.2.0/deeppavlov/configs/embedder/bert_sentence_embedder.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_detection_en.json` & `deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_detection_en.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945436507936508%*

 * *Differences: {"'chainer'": "{'pipe': {0: {delete: ['max_chunk_len']}, 1: {'thres_proba': 0.6, delete: "*

 * *              "['return_entities_with_tags']}}}"}*

```diff
@@ -15,31 +15,29 @@
         "pipe": [
             {
                 "batch_size": 16,
                 "class_name": "ner_chunker",
                 "in": [
                     "x"
                 ],
-                "max_chunk_len": 180,
                 "max_seq_len": 300,
                 "out": [
                     "x_chunk",
                     "chunk_nums",
                     "chunk_sentences_offsets",
                     "chunk_sentences"
                 ],
                 "vocab_file": "{TRANSFORMER}"
             },
             {
                 "class_name": "entity_detection_parser",
                 "id": "edp",
                 "o_tag": "O",
-                "return_entities_with_tags": true,
                 "tags_file": "{NER_PATH}/tag.dict",
-                "thres_proba": 0.05
+                "thres_proba": 0.6
             },
             {
                 "class_name": "ner_chunk_model",
                 "in": [
                     "x_chunk",
                     "chunk_nums",
                     "chunk_sentences_offsets",
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_detection_ru.json` & `deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_detection_ru.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957010582010583%*

 * *Differences: {"'chainer'": "{'pipe': {0: {delete: ['max_chunk_len']}, 1: {delete: "*

 * *              "['return_entities_with_tags']}}}"}*

```diff
@@ -15,29 +15,27 @@
         "pipe": [
             {
                 "batch_size": 16,
                 "class_name": "ner_chunker",
                 "in": [
                     "x"
                 ],
-                "max_chunk_len": 180,
                 "max_seq_len": 300,
                 "out": [
                     "x_chunk",
                     "chunk_nums",
                     "chunk_sentences_offsets",
                     "chunk_sentences"
                 ],
                 "vocab_file": "{TRANSFORMER}"
             },
             {
                 "class_name": "entity_detection_parser",
                 "id": "edp",
                 "o_tag": "O",
-                "return_entities_with_tags": true,
                 "tags_file": "{NER_PATH}/tag.dict",
                 "thres_proba": 0.05
             },
             {
                 "class_name": "ner_chunk_model",
                 "in": [
                     "x_chunk",
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_extraction_en.json` & `deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_extraction_ru.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9856564153439153%*

 * *Differences: {"'chainer'": "{'pipe': {0: {'config_path': "*

 * *              "'{CONFIGS_PATH}/entity_extraction/entity_detection_ru.json'}, 1: {'config_path': "*

 * *              "'{CONFIGS_PATH}/entity_extraction/entity_linking_ru.json', 'in': {insert: [(2, "*

 * *              "'probas')]}, 'out': {insert: [(3, 'entity_labels')]}}}, 'out': {insert: [(6, "*

 * *              "'entity_labels')]}}"}*

```diff
@@ -5,45 +5,48 @@
         ],
         "out": [
             "entity_substr",
             "tags",
             "entity_offsets",
             "entity_ids",
             "entity_conf",
-            "entity_pages"
+            "entity_pages",
+            "entity_labels"
         ],
         "pipe": [
             {
-                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_detection_en.json",
+                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_detection_ru.json",
                 "in": [
                     "x"
                 ],
                 "out": [
                     "entity_substr",
                     "entity_offsets",
                     "entity_positions",
                     "tags",
                     "sentences_offsets",
                     "sentences",
                     "probas"
                 ]
             },
             {
-                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_linking_en.json",
+                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_linking_ru.json",
                 "in": [
                     "entity_substr",
                     "tags",
+                    "probas",
                     "sentences",
                     "entity_offsets",
                     "sentences_offsets"
                 ],
                 "out": [
                     "entity_ids",
                     "entity_conf",
-                    "entity_pages"
+                    "entity_pages",
+                    "entity_labels"
                 ]
             }
         ]
     },
     "metadata": {
         "variables": {
             "CONFIGS_PATH": "{DEEPPAVLOV_PATH}/configs"
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_extraction_ru.json` & `deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_extraction_en.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9856564153439153%*

 * *Differences: {"'chainer'": "{'pipe': {0: {'config_path': "*

 * *              "'{CONFIGS_PATH}/entity_extraction/entity_detection_en.json'}, 1: {'config_path': "*

 * *              "'{CONFIGS_PATH}/entity_extraction/entity_linking_en.json', 'in': {insert: [(2, "*

 * *              "'probas')]}, 'out': {insert: [(3, 'entity_labels')]}}}, 'out': {insert: [(6, "*

 * *              "'entity_labels')]}}"}*

```diff
@@ -5,45 +5,48 @@
         ],
         "out": [
             "entity_substr",
             "tags",
             "entity_offsets",
             "entity_ids",
             "entity_conf",
-            "entity_pages"
+            "entity_pages",
+            "entity_labels"
         ],
         "pipe": [
             {
-                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_detection_ru.json",
+                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_detection_en.json",
                 "in": [
                     "x"
                 ],
                 "out": [
                     "entity_substr",
                     "entity_offsets",
                     "entity_positions",
                     "tags",
                     "sentences_offsets",
                     "sentences",
                     "probas"
                 ]
             },
             {
-                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_linking_ru.json",
+                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_linking_en.json",
                 "in": [
                     "entity_substr",
                     "tags",
+                    "probas",
                     "sentences",
                     "entity_offsets",
                     "sentences_offsets"
                 ],
                 "out": [
                     "entity_ids",
                     "entity_conf",
-                    "entity_pages"
+                    "entity_pages",
+                    "entity_labels"
                 ]
             }
         ]
     },
     "metadata": {
         "variables": {
             "CONFIGS_PATH": "{DEEPPAVLOV_PATH}/configs"
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_linking_en.json` & `deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_linking_ru.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9427083333333333%*

 * *Differences: {"'chainer'": "{'in': {insert: [(2, 'probas')]}, 'pipe': {0: {'encoder_weights_path': "*

 * *              "'{MODELS_PATH}/entity_linking_rus/encoder.pth.tar', 'bilinear_weights_path': "*

 * *              "'{MODELS_PATH}/entity_linking_rus/bilinear.pth.tar', 'emb_size': 264, 'block_size': "*

 * *              "6}, 1: {'in': {insert: [(2, 'probas')]}, 'out': {insert: [(3, 'entity_labels')]}, "*

 * *              "'load_path': '{DOWNLOADS_PATH}/entity_linking_rus', 'entities_database_filename': "*

 * *              "'el_rus_v2.db',  […]*

```diff
@@ -1,81 +1,98 @@
 {
     "chainer": {
         "in": [
             "entity_substr",
             "tags",
+            "probas",
             "sentences",
             "entity_offsets",
             "sentences_offsets"
         ],
         "out": [
             "entity_ids",
             "entity_conf",
-            "entity_pages"
+            "entity_pages",
+            "entity_labels"
         ],
         "pipe": [
             {
-                "bilinear_weights_path": "{MODELS_PATH}/entity_linking_eng/bilinear.pth.tar",
-                "block_size": 8,
+                "bilinear_weights_path": "{MODELS_PATH}/entity_linking_rus/bilinear.pth.tar",
+                "block_size": 6,
                 "class_name": "torch_transformers_entity_ranker_infer",
-                "emb_size": 512,
-                "encoder_weights_path": "{MODELS_PATH}/entity_linking_eng/encoder.pth.tar",
+                "emb_size": 264,
+                "encoder_weights_path": "{MODELS_PATH}/entity_linking_rus/encoder.pth.tar",
                 "id": "entity_descr_ranking",
                 "pretrained_bert": "{TRANSFORMER}",
                 "special_token_id": 30522
             },
             {
                 "class_name": "entity_linker",
-                "entities_database_filename": "el_eng.db",
+                "entities_database_filename": "el_rus_v2.db",
                 "entity_ranker": "#entity_descr_ranking",
                 "full_paragraph": true,
                 "in": [
                     "entity_substr",
                     "tags",
+                    "probas",
                     "sentences",
                     "entity_offsets",
                     "sentences_offsets"
                 ],
                 "include_mention": false,
+                "kb_filename": "{DOWNLOADS_PATH}/wikidata/wikidata_lite.hdt",
                 "lang": "ru",
                 "lemmatize": true,
-                "load_path": "{DOWNLOADS_PATH}/entity_linking_eng",
-                "num_entities_for_bert_ranking": 20,
+                "load_path": "{DOWNLOADS_PATH}/entity_linking_rus",
+                "ngrams_matrix_filename": "{DOWNLOADS_PATH}/entity_linking_rus/ngrams_matrix.npz",
+                "num_entities_for_bert_ranking": 30,
                 "num_entities_to_return": 3,
                 "out": [
                     "entity_ids",
                     "entity_conf",
-                    "entity_pages"
+                    "entity_pages",
+                    "entity_labels"
                 ],
+                "prefixes": {
+                    "entity": [
+                        "http://we"
+                    ],
+                    "rels": {
+                        "direct": "http://wpd",
+                        "no_type": "http://wp",
+                        "qualifier": "http://wpq",
+                        "statement": "http://wps"
+                    }
+                },
                 "rank_in_runtime": true,
                 "return_confidences": true,
                 "use_connections": true,
                 "use_descriptions": true,
                 "use_gpu": false,
                 "use_tags": true,
-                "wikidata_file": "{DOWNLOADS_PATH}/wikidata/wikidata_lite.hdt"
+                "words_dict_filename": "{DOWNLOADS_PATH}/entity_linking_rus/words_dict.pickle"
             }
         ]
     },
     "metadata": {
         "download": [
             {
-                "subdir": "{DOWNLOADS_PATH}/entity_linking_eng",
-                "url": "http://files.deeppavlov.ai/deeppavlov_data/entity_linking/el_db_eng.tar.gz"
+                "subdir": "{DOWNLOADS_PATH}/entity_linking_rus",
+                "url": "http://files.deeppavlov.ai/kbqa/downloads/el_files_rus_v2.tar.gz"
             },
             {
-                "subdir": "{MODELS_PATH}/entity_linking_eng",
-                "url": "http://files.deeppavlov.ai/deeppavlov_data/entity_linking/el_ranker_eng.tar.gz"
+                "subdir": "{MODELS_PATH}/entity_linking_rus",
+                "url": "http://files.deeppavlov.ai/deeppavlov_data/entity_linking/el_ranker_rus.tar.gz"
             },
             {
                 "subdir": "{DOWNLOADS_PATH}/wikidata",
                 "url": "http://files.deeppavlov.ai/kbqa/wikidata/wikidata_lite.tar.gz"
             }
         ],
         "variables": {
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
             "ROOT_PATH": "~/.deeppavlov",
-            "TRANSFORMER": "prajjwal1/bert-small"
+            "TRANSFORMER": "DeepPavlov/distilrubert-tiny-cased-conversational-v1"
         }
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/entity_extraction/entity_linking_ru.json` & `deeppavlov-1.2.0/deeppavlov/configs/relation_extraction/re_docred.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.31554271708683473%*

 * *Differences: {"'chainer'": "{'in': ['tokens', 'entity_pos', 'entity_tags'], 'pipe': {1: {'class_name': "*

 * *              "'re_classifier', 'pretrained_bert': 'bert-base-cased', 'in': ['input_ids', "*

 * *              "'attention_mask', 'upd_entity_pos', 'upd_entity_tags'], 'in_y': ['y_ids'], 'out': "*

 * *              "['model_output'], 'save_path': '{MODEL_PATH}/model', 'load_path': "*

 * *              "'{MODEL_PATH}/model', 'model_name': 're_model', 'n_classes': 97, 'num_ner_tags': 6, "*

 * *              "'return_probas': True, delete: […]*

```diff
@@ -1,81 +1,123 @@
 {
     "chainer": {
         "in": [
-            "entity_substr",
-            "tags",
-            "sentences",
-            "entity_offsets",
-            "sentences_offsets"
+            "tokens",
+            "entity_pos",
+            "entity_tags"
+        ],
+        "in_y": [
+            "y_ids"
         ],
         "out": [
-            "entity_ids",
-            "entity_conf",
-            "entity_pages"
+            "wikidata_relation_id",
+            "relation_name"
         ],
         "pipe": [
             {
-                "bilinear_weights_path": "{MODELS_PATH}/entity_linking_rus/bilinear.pth.tar",
-                "block_size": 6,
-                "class_name": "torch_transformers_entity_ranker_infer",
-                "emb_size": 264,
-                "encoder_weights_path": "{MODELS_PATH}/entity_linking_rus/encoder.pth.tar",
-                "id": "entity_descr_ranking",
-                "pretrained_bert": "{TRANSFORMER}",
-                "special_token_id": 30522
+                "class_name": "re_preprocessor",
+                "default_tag": "PER",
+                "in": [
+                    "tokens",
+                    "entity_pos",
+                    "entity_tags"
+                ],
+                "out": [
+                    "input_ids",
+                    "attention_mask",
+                    "upd_entity_pos",
+                    "upd_entity_tags",
+                    "nf_samples"
+                ],
+                "vocab_file": "bert-base-cased"
+            },
+            {
+                "class_name": "re_classifier",
+                "in": [
+                    "input_ids",
+                    "attention_mask",
+                    "upd_entity_pos",
+                    "upd_entity_tags"
+                ],
+                "in_y": [
+                    "y_ids"
+                ],
+                "load_path": "{MODEL_PATH}/model",
+                "model_name": "re_model",
+                "n_classes": 97,
+                "num_ner_tags": 6,
+                "out": [
+                    "model_output"
+                ],
+                "pretrained_bert": "bert-base-cased",
+                "return_probas": true,
+                "save_path": "{MODEL_PATH}/model"
             },
             {
-                "class_name": "entity_linker",
-                "entities_database_filename": "el_rus.db",
-                "entity_ranker": "#entity_descr_ranking",
-                "full_paragraph": true,
+                "class_name": "re_postprocessor",
                 "in": [
-                    "entity_substr",
-                    "tags",
-                    "sentences",
-                    "entity_offsets",
-                    "sentences_offsets"
-                ],
-                "include_mention": false,
-                "lang": "ru",
-                "lemmatize": true,
-                "load_path": "{DOWNLOADS_PATH}/entity_linking_rus",
-                "num_entities_for_bert_ranking": 20,
-                "num_entities_to_return": 3,
+                    "model_output",
+                    "nf_samples"
+                ],
                 "out": [
-                    "entity_ids",
-                    "entity_conf",
-                    "entity_pages"
-                ],
-                "rank_in_runtime": true,
-                "return_confidences": true,
-                "use_connections": true,
-                "use_descriptions": true,
-                "use_gpu": false,
-                "use_tags": true,
-                "wikidata_file": "{DOWNLOADS_PATH}/wikidata/wikidata_lite.hdt"
+                    "wikidata_relation_id",
+                    "relation_name"
+                ],
+                "rel2id_path": "{DOWNLOADS_PATH}/docred/meta/rel2id.json",
+                "rel2label_path": "{DOWNLOADS_PATH}/docred/rel_info.json"
             }
         ]
     },
+    "dataset_iterator": {
+        "class_name": "basic_classification_iterator"
+    },
+    "dataset_reader": {
+        "class_name": "docred_reader",
+        "data_path": "{DOWNLOADS_PATH}/docred/",
+        "rel2id_path": "{DOWNLOADS_PATH}/docred/meta/rel2id.json",
+        "rel_info_path": "{DOWNLOADS_PATH}/docred/rel_info.json",
+        "valid_test_data_size": 150
+    },
     "metadata": {
         "download": [
             {
-                "subdir": "{DOWNLOADS_PATH}/entity_linking_rus",
-                "url": "http://files.deeppavlov.ai/deeppavlov_data/entity_linking/el_db_rus.tar.gz"
+                "subdir": "{DOWNLOADS_PATH}/docred",
+                "url": "http://files.deeppavlov.ai/deeppavlov_data/relation_extraction/docred.tar.gz"
             },
             {
-                "subdir": "{MODELS_PATH}/entity_linking_rus",
-                "url": "http://files.deeppavlov.ai/deeppavlov_data/entity_linking/el_ranker_rus.tar.gz"
+                "subdir": "{MODELS_PATH}/re_docred",
+                "url": "http://files.deeppavlov.ai/deeppavlov_data/relation_extraction/re_docred_model_v1.tar.gz"
             },
             {
-                "subdir": "{DOWNLOADS_PATH}/wikidata",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/wikidata_lite.tar.gz"
+                "subdir": "{DOWNLOADS_PATH}/docred",
+                "url": "http://files.deeppavlov.ai/deeppavlov_data/relation_extraction/rel2label.json"
             }
         ],
         "variables": {
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "ROOT_PATH": "~/.deeppavlov",
-            "TRANSFORMER": "DeepPavlov/distilrubert-tiny-cased-conversational-v1"
+            "MODEL_PATH": "{MODELS_PATH}/re_docred",
+            "ROOT_PATH": "~/.deeppavlov"
         }
+    },
+    "train": {
+        "batch_size": 30,
+        "class_name": "torch_trainer",
+        "epochs": 50,
+        "evaluation_targets": [
+            "valid",
+            "train"
+        ],
+        "log_every_n_batches": 100,
+        "metrics": [
+            "f1_weighted",
+            "acc"
+        ],
+        "show_examples": false,
+        "train_metrics": [
+            "f1_weighted",
+            "acc"
+        ],
+        "val_every_n_batches": 200,
+        "validation_patience": 50
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/faq/fasttext_logreg.json` & `deeppavlov-1.2.0/deeppavlov/configs/faq/fasttext_logreg.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/kbqa/kbqa_cq_en.json` & `deeppavlov-1.2.0/deeppavlov/configs/entity_extraction/entity_linking_en.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7755952380952381%*

 * *Differences: {"'chainer'": "{'in': ['entity_substr', 'tags', 'probas', 'sentences', 'entity_offsets', "*

 * *              "'sentences_offsets'], 'pipe': {0: {'class_name': "*

 * *              "'torch_transformers_entity_ranker_infer', 'id': 'entity_descr_ranking', "*

 * *              "'pretrained_bert': '{TRANSFORMER}', 'encoder_weights_path': "*

 * *              "'{MODELS_PATH}/entity_linking_eng/encoder.pth.tar', 'bilinear_weights_path': "*

 * *              "'{MODELS_PATH}/entity_linking_eng/bilinear.pth.tar', 'special_token_id': 30522,  […]*

```diff
@@ -1,137 +1,80 @@
 {
     "chainer": {
         "in": [
-            "x"
-        ],
-        "in_y": [
-            "y"
+            "entity_substr",
+            "tags",
+            "probas",
+            "sentences",
+            "entity_offsets",
+            "sentences_offsets"
         ],
         "out": [
-            "answers"
+            "entity_ids",
+            "entity_conf",
+            "entity_pages",
+            "entity_labels"
         ],
         "pipe": [
             {
-                "class_name": "question_sign_checker",
-                "in": [
-                    "x"
-                ],
-                "out": [
-                    "x_punct"
-                ]
+                "bilinear_weights_path": "{MODELS_PATH}/entity_linking_eng/bilinear.pth.tar",
+                "block_size": 8,
+                "class_name": "torch_transformers_entity_ranker_infer",
+                "emb_size": 512,
+                "encoder_weights_path": "{MODELS_PATH}/entity_linking_eng/encoder.pth.tar",
+                "id": "entity_descr_ranking",
+                "pretrained_bert": "{TRANSFORMER}",
+                "special_token_id": 30522
             },
             {
-                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_detection_en.json",
+                "class_name": "entity_linker",
+                "entities_database_filename": "el_eng_v2.db",
+                "entity_ranker": "#entity_descr_ranking",
+                "full_paragraph": true,
                 "in": [
-                    "x_punct"
-                ],
-                "out": [
                     "entity_substr",
-                    "entity_offsets",
-                    "entity_positions",
                     "tags",
-                    "sentences_offsets",
+                    "probas",
                     "sentences",
-                    "probas"
-                ]
-            },
-            {
-                "class_name": "answer_types_extractor",
-                "in": [
-                    "x_punct",
-                    "entity_substr",
-                    "tags"
-                ],
-                "lang": "@en",
-                "out": [
-                    "answer_types",
-                    "f_entity_substr",
-                    "f_tags"
-                ],
-                "types_filename": "{DOWNLOADS_PATH}/wikidata_eng/types_labels_dict_en.pickle",
-                "types_sets_filename": "{DOWNLOADS_PATH}/wikidata_eng/answer_types.pickle"
-            },
-            {
-                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_linking_en.json",
-                "id": "entity_linker"
-            },
-            {
-                "class_name": "wiki_parser",
-                "id": "wiki_p",
-                "lang": "@en",
-                "wiki_filename": "{DOWNLOADS_PATH}/wikidata/wikidata_lite.hdt"
-            },
-            {
-                "class_name": "template_matcher",
-                "id": "template_m",
-                "load_path": "{DOWNLOADS_PATH}/wikidata_eng",
-                "num_processors": 16,
-                "templates_filename": "templates_eng.json"
-            },
-            {
-                "config_path": "{CONFIGS_PATH}/classifiers/query_pr.json",
-                "in": [
-                    "x_punct"
-                ],
-                "out": [
-                    "template_type"
-                ]
-            },
-            {
-                "batch_size": 32,
-                "class_name": "rel_ranking_infer",
-                "id": "rel_r_inf",
-                "load_path": "{DOWNLOADS_PATH}/wikidata_eng",
-                "rank_answers": true,
-                "ranker": {
-                    "config_path": "{CONFIGS_PATH}/ranking/rel_ranking_bert_en.json"
-                },
-                "rel_q2name_filename": "wiki_dict_properties_eng.pickle",
-                "return_all_possible_answers": true,
-                "return_answer_ids": false,
-                "wiki_parser": "#wiki_p"
-            },
-            {
-                "class_name": "query_generator",
-                "entities_to_leave": 5,
-                "entity_linker": "#entity_linker",
-                "id": "query_g",
-                "in": [
-                    "x_punct",
-                    "x_punct",
-                    "template_type",
-                    "f_entity_substr",
-                    "f_tags",
-                    "answer_types"
+                    "entity_offsets",
+                    "sentences_offsets"
                 ],
-                "load_path": "{DOWNLOADS_PATH}/wikidata",
+                "include_mention": false,
+                "lang": "en",
+                "lemmatize": true,
+                "load_path": "{DOWNLOADS_PATH}/entity_linking_eng",
+                "num_entities_for_bert_ranking": 20,
+                "num_entities_to_return": 3,
                 "out": [
-                    "answers"
-                ],
-                "rank_rels_filename_1": "rels_0.txt",
-                "rank_rels_filename_2": "rels_1.txt",
-                "rel_ranker": "#rel_r_inf",
-                "rels_to_leave": 10,
-                "sparql_queries_filename": "{DOWNLOADS_PATH}/wikidata/sparql_queries.json",
-                "template_matcher": "#template_m",
-                "wiki_parser": "#wiki_p"
+                    "entity_ids",
+                    "entity_conf",
+                    "entity_pages",
+                    "entity_labels"
+                ],
+                "rank_in_runtime": true,
+                "return_confidences": true,
+                "use_connections": true,
+                "use_descriptions": true,
+                "use_gpu": false,
+                "use_tags": true
             }
         ]
     },
     "metadata": {
         "download": [
             {
-                "subdir": "{DOWNLOADS_PATH}/wikidata",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/queries_and_rels.tar.gz"
+                "subdir": "{DOWNLOADS_PATH}/entity_linking_eng",
+                "url": "http://files.deeppavlov.ai/kbqa/downloads/el_db_eng_v2.tar.gz"
             },
             {
-                "subdir": "{DOWNLOADS_PATH}/wikidata_eng",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/kbqa_files_en.tar.gz"
+                "subdir": "{MODELS_PATH}/entity_linking_eng",
+                "url": "http://files.deeppavlov.ai/deeppavlov_data/entity_linking/el_ranker_eng.tar.gz"
             }
         ],
         "variables": {
-            "CONFIGS_PATH": "{DEEPPAVLOV_PATH}/configs",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
-            "ROOT_PATH": "~/.deeppavlov"
+            "MODELS_PATH": "{ROOT_PATH}/models",
+            "ROOT_PATH": "~/.deeppavlov",
+            "TRANSFORMER": "prajjwal1/bert-small"
         }
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/kbqa/kbqa_cq_ru.json` & `deeppavlov-1.2.0/deeppavlov/configs/ner/ner_rus_convers_distilrubert_6L.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.34236877705627705%*

 * *Differences: {"'chainer'": "{'pipe': {0: {'class_name': 'torch_transformers_ner_preprocessor', 'out': "*

 * *              "['x_tokens', 'x_subword_tokens', 'x_subword_tok_ids', 'startofword_markers', "*

 * *              "'attention_mask', 'tokens_offsets'], 'vocab_file': '{TRANSFORMER}', "*

 * *              "'do_lower_case': False, 'max_seq_length': 512, 'max_subword_length': 15, "*

 * *              "'token_masking_prob': 0.0}, 1: {'class_name': 'simple_vocab', 'in': ['y'], 'out': "*

 * *              "['y_ind'], 'id': 'tag_vocab', 'unk_tok […]*

```diff
@@ -3,166 +3,154 @@
         "in": [
             "x"
         ],
         "in_y": [
             "y"
         ],
         "out": [
-            "answers"
+            "x_tokens",
+            "y_pred"
         ],
         "pipe": [
             {
-                "class_name": "question_sign_checker",
+                "class_name": "torch_transformers_ner_preprocessor",
+                "do_lower_case": false,
                 "in": [
                     "x"
                 ],
+                "max_seq_length": 512,
+                "max_subword_length": 15,
                 "out": [
-                    "x_punct"
-                ]
-            },
-            {
-                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_detection_ru.json",
-                "in": [
-                    "x_punct"
+                    "x_tokens",
+                    "x_subword_tokens",
+                    "x_subword_tok_ids",
+                    "startofword_markers",
+                    "attention_mask",
+                    "tokens_offsets"
                 ],
-                "out": [
-                    "entity_substr",
-                    "entity_offsets",
-                    "entity_positions",
-                    "tags",
-                    "sentences_offsets",
-                    "sentences",
-                    "probas"
-                ]
+                "token_masking_prob": 0.0,
+                "vocab_file": "{TRANSFORMER}"
             },
             {
-                "class_name": "answer_types_extractor",
-                "in": [
-                    "x_punct",
-                    "entity_substr",
-                    "tags"
+                "class_name": "simple_vocab",
+                "fit_on": [
+                    "y"
                 ],
-                "lang": "@ru",
-                "out": [
-                    "answer_types",
-                    "f_entity_substr",
-                    "f_tags"
-                ],
-                "types_filename": "{DOWNLOADS_PATH}/wikidata_rus/types_labels_dict_ru.pickle",
-                "types_sets_filename": "{DOWNLOADS_PATH}/wikidata_rus/answer_types.pickle"
-            },
-            {
-                "config_path": "{CONFIGS_PATH}/entity_extraction/entity_linking_ru.json",
-                "id": "entity_linker"
-            },
-            {
-                "class_name": "wiki_parser",
-                "id": "wiki_p",
-                "lang": "@ru",
-                "wiki_filename": "{DOWNLOADS_PATH}/wikidata/wikidata_lite.hdt"
-            },
-            {
-                "class_name": "slovnet_syntax_parser",
+                "id": "tag_vocab",
                 "in": [
-                    "x_punct",
-                    "entity_offsets"
+                    "y"
                 ],
-                "load_path": "{MODELS_PATH}/slovnet_syntax_parser",
-                "navec_filename": "{MODELS_PATH}/slovnet_syntax_parser/navec_news_v1_1B_250K_300d_100q.tar",
+                "load_path": "{MODEL_PATH}/tag.dict",
                 "out": [
-                    "syntax_info"
+                    "y_ind"
                 ],
-                "syntax_parser_filename": "{MODELS_PATH}/slovnet_syntax_parser/slovnet_syntax_news_v1.tar"
-            },
-            {
-                "class_name": "ru_adj_to_noun",
-                "freq_dict_filename": "{DOWNLOADS_PATH}/wikidata_rus/freqrnc2011.csv",
-                "id": "adj2noun"
+                "pad_with_zeros": true,
+                "save_path": "{MODEL_PATH}/tag.dict",
+                "unk_token": [
+                    "O"
+                ]
             },
             {
-                "adj_to_noun": "#adj2noun",
-                "class_name": "tree_to_sparql",
-                "in": [
-                    "syntax_info",
-                    "entity_positions"
-                ],
-                "lang": "rus",
+                "attention_probs_keep_prob": 0.44,
+                "class_name": "torch_transformers_sequence_tagger",
+                "clip_norm": 1.0,
+                "encoder_layer_ids": [
+                    -1
+                ],
+                "hidden_keep_prob": 0.89,
+                "in": [
+                    "x_subword_tok_ids",
+                    "attention_mask",
+                    "startofword_markers"
+                ],
+                "in_y": [
+                    "y_ind"
+                ],
+                "learning_rate_drop_div": 1.5,
+                "learning_rate_drop_patience": 30,
+                "load_before_drop": true,
+                "load_path": "{MODEL_PATH}/model",
+                "min_learning_rate": 1e-07,
+                "n_tags": "#tag_vocab.len",
+                "optimizer": "AdamW",
+                "optimizer_parameters": {
+                    "betas": [
+                        0.9,
+                        0.999
+                    ],
+                    "eps": 1e-06,
+                    "lr": 2.78e-05,
+                    "weight_decay": 1e-06
+                },
                 "out": [
-                    "x_sanitized",
-                    "query_nums",
-                    "entities_dict",
-                    "types_dict"
+                    "y_pred_ind",
+                    "probas"
                 ],
-                "sparql_queries_filename": "{DOWNLOADS_PATH}/wikidata/sparql_queries.json"
-            },
-            {
-                "class_name": "template_matcher",
-                "id": "template_m",
-                "load_path": "{DOWNLOADS_PATH}/wikidata_rus",
-                "num_processors": 8,
-                "templates_filename": "templates_rus.json"
-            },
-            {
-                "batch_size": 32,
-                "class_name": "rel_ranking_infer",
-                "id": "rel_r_inf",
-                "load_path": "{DOWNLOADS_PATH}/wikidata_rus",
-                "ranker": {
-                    "config_path": "{CONFIGS_PATH}/ranking/rel_ranking_bert_ru.json"
-                },
-                "rel_q2name_filename": "wiki_dict_properties_rus.pickle",
-                "return_all_possible_answers": true,
-                "return_answer_ids": false,
-                "wiki_parser": "#wiki_p"
+                "pretrained_bert": "{TRANSFORMER}",
+                "save_path": "{MODEL_PATH}/model"
             },
             {
-                "class_name": "query_generator",
-                "entities_to_leave": 9,
-                "entity_linker": "#entity_linker",
-                "id": "query_g",
                 "in": [
-                    "x_punct",
-                    "x_sanitized",
-                    "query_nums",
-                    "f_entity_substr",
-                    "f_tags",
-                    "answer_types"
+                    "y_pred_ind"
                 ],
-                "load_path": "{DOWNLOADS_PATH}/wikidata",
                 "out": [
-                    "answers"
+                    "y_pred"
                 ],
-                "rank_rels_filename_1": "rels_0.txt",
-                "rank_rels_filename_2": "rels_1.txt",
-                "rel_ranker": "#rel_r_inf",
-                "rels_to_leave": 10,
-                "return_all_possible_answers": false,
-                "sparql_queries_filename": "{DOWNLOADS_PATH}/wikidata/sparql_queries.json",
-                "syntax_structure_known": true,
-                "template_matcher": "#template_m",
-                "wiki_parser": "#wiki_p"
+                "ref": "tag_vocab"
             }
         ]
     },
+    "dataset_iterator": {
+        "class_name": "data_learning_iterator"
+    },
+    "dataset_reader": {
+        "class_name": "conll2003_reader",
+        "data_path": "{DOWNLOADS_PATH}/total_rus/",
+        "dataset_name": "collection_rus",
+        "provide_pos": false
+    },
     "metadata": {
         "download": [
             {
-                "subdir": "{DOWNLOADS_PATH}/wikidata",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/queries_and_rels.tar.gz"
-            },
-            {
-                "subdir": "{DOWNLOADS_PATH}/wikidata_rus",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/kbqa_files_ru.tar.gz"
-            },
-            {
-                "subdir": "{MODELS_PATH}/slovnet_syntax_parser",
-                "url": "http://files.deeppavlov.ai/deeppavlov_data/slovnet_syntax_parser.tar.gz"
+                "subdir": "{MODELS_PATH}",
+                "url": "http://files.deeppavlov.ai/v1/ner/ner_rus_conversational_distilrubert_6L.tar.gz"
             }
         ],
         "variables": {
-            "CONFIGS_PATH": "{DEEPPAVLOV_PATH}/configs",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "ROOT_PATH": "~/.deeppavlov"
+            "MODEL_PATH": "{MODELS_PATH}/ner_rus_conversational_distilrubert_6L",
+            "ROOT_PATH": "~/.deeppavlov",
+            "TRANSFORMER": "DeepPavlov/distilrubert-base-cased-conversational"
         }
+    },
+    "train": {
+        "batch_size": 10,
+        "class_name": "torch_trainer",
+        "epochs": 30,
+        "evaluation_targets": [
+            "valid",
+            "test"
+        ],
+        "log_every_n_batches": 20,
+        "metrics": [
+            {
+                "inputs": [
+                    "y",
+                    "y_pred"
+                ],
+                "name": "ner_f1"
+            },
+            {
+                "inputs": [
+                    "y",
+                    "y_pred"
+                ],
+                "name": "ner_token_f1"
+            }
+        ],
+        "show_examples": false,
+        "tensorboard_log_dir": "{MODEL_PATH}/",
+        "val_every_n_batches": 20,
+        "validation_patience": 100
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/kbqa/wiki_parser.json` & `deeppavlov-1.2.0/deeppavlov/configs/kbqa/wiki_parser.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/multitask/mt_glue.json` & `deeppavlov-1.2.0/deeppavlov/configs/multitask/mt_glue.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99%*

 * *Differences: {"'train'": "{'pytest_max_batches': 2}"}*

```diff
@@ -381,12 +381,13 @@
                 "inputs": [
                     "y_stsb",
                     "y_stsb_pred"
                 ],
                 "name": "spearman_correlation"
             }
         ],
+        "pytest_max_batches": 2,
         "show_examples": false,
         "val_every_n_epochs": 1,
         "validation_patience": 3
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/multitask/multitask_example.json` & `deeppavlov-1.2.0/deeppavlov/configs/multitask/multitask_example.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99%*

 * *Differences: {"'train'": "{'pytest_max_batches': 2}"}*

```diff
@@ -336,12 +336,13 @@
                 "inputs": [
                     "y_stsb",
                     "y_stsb_pred"
                 ],
                 "name": "spearman_correlation"
             }
         ],
+        "pytest_max_batches": 2,
         "show_examples": false,
         "val_every_n_epochs": 1,
         "validation_patience": 3
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ner/ner_case_agnostic_mdistilbert.json` & `deeppavlov-1.2.0/deeppavlov/configs/ner/ner_case_agnostic_mdistilbert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ner/ner_collection3_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/ner/ner_collection3_bert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ner/ner_conll2003_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/ner/ner_conll2003_bert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ner/ner_ontonotes_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/ner/ner_ontonotes_bert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ner/ner_ontonotes_bert_mult.json` & `deeppavlov-1.2.0/deeppavlov/configs/ner/ner_ontonotes_bert_mult.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ner/ner_rus_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/ner/ner_rus_bert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ner/ner_rus_bert_probas.json` & `deeppavlov-1.2.0/deeppavlov/configs/ner/ner_rus_bert_probas.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_2L.json` & `deeppavlov-1.2.0/deeppavlov/configs/ner/ner_rus_convers_distilrubert_2L.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ner/ner_rus_convers_distilrubert_6L.json` & `deeppavlov-1.2.0/deeppavlov/configs/squad/squad_ru_convers_distilrubert_6L.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7378142361111111%*

 * *Differences: {"'chainer'": "{'in': ['context_raw', 'question_raw'], 'in_y': ['ans_raw', 'ans_raw_start'], "*

 * *              "'pipe': {0: {'class_name': 'torch_squad_transformers_preprocessor', "*

 * *              "'do_lower_case': '{lowercase}', 'max_seq_length': 384, 'in': ['question_raw', "*

 * *              "'context_raw'], 'out': ['bert_features', 'subtokens', 'split_context'], "*

 * *              "'add_token_type_ids': True, delete: ['max_subword_length', 'token_masking_prob']}, "*

 * *              "2: {'class_name': 'squad_bert_ans […]*

```diff
@@ -1,156 +1,175 @@
 {
     "chainer": {
         "in": [
-            "x"
+            "context_raw",
+            "question_raw"
         ],
         "in_y": [
-            "y"
+            "ans_raw",
+            "ans_raw_start"
         ],
         "out": [
-            "x_tokens",
-            "y_pred"
+            "ans_predicted",
+            "ans_start_predicted",
+            "scores"
         ],
         "pipe": [
             {
-                "class_name": "torch_transformers_ner_preprocessor",
-                "do_lower_case": false,
+                "add_token_type_ids": true,
+                "class_name": "torch_squad_transformers_preprocessor",
+                "do_lower_case": "{lowercase}",
                 "in": [
-                    "x"
+                    "question_raw",
+                    "context_raw"
                 ],
-                "max_seq_length": 512,
-                "max_subword_length": 15,
+                "max_seq_length": 384,
                 "out": [
-                    "x_tokens",
-                    "x_subword_tokens",
-                    "x_subword_tok_ids",
-                    "startofword_markers",
-                    "attention_mask",
-                    "tokens_offsets"
+                    "bert_features",
+                    "subtokens",
+                    "split_context"
                 ],
-                "token_masking_prob": 0.0,
                 "vocab_file": "{TRANSFORMER}"
             },
             {
-                "class_name": "simple_vocab",
-                "fit_on": [
-                    "y"
-                ],
-                "id": "tag_vocab",
+                "class_name": "squad_bert_mapping",
+                "do_lower_case": "{lowercase}",
                 "in": [
-                    "y"
+                    "split_context",
+                    "bert_features",
+                    "subtokens"
                 ],
-                "load_path": "{MODEL_PATH}/tag.dict",
                 "out": [
-                    "y_ind"
-                ],
-                "pad_with_zeros": true,
-                "save_path": "{MODEL_PATH}/tag.dict",
-                "unk_token": [
-                    "O"
+                    "subtok2chars",
+                    "char2subtoks"
                 ]
             },
             {
-                "attention_probs_keep_prob": 0.44,
-                "class_name": "torch_transformers_sequence_tagger",
-                "clip_norm": 1.0,
-                "encoder_layer_ids": [
-                    -1
+                "class_name": "squad_bert_ans_preprocessor",
+                "do_lower_case": "{lowercase}",
+                "in": [
+                    "ans_raw",
+                    "ans_raw_start",
+                    "char2subtoks"
                 ],
-                "hidden_keep_prob": 0.89,
+                "out": [
+                    "ans",
+                    "ans_start",
+                    "ans_end"
+                ]
+            },
+            {
+                "attention_probs_keep_prob": 0.0,
+                "class_name": "torch_transformers_squad",
+                "hidden_keep_prob": 0.33,
                 "in": [
-                    "x_subword_tok_ids",
-                    "attention_mask",
-                    "startofword_markers"
+                    "bert_features"
                 ],
                 "in_y": [
-                    "y_ind"
+                    "ans_start",
+                    "ans_end"
                 ],
                 "learning_rate_drop_div": 1.5,
-                "learning_rate_drop_patience": 30,
-                "load_before_drop": true,
+                "learning_rate_drop_patience": 2,
                 "load_path": "{MODEL_PATH}/model",
-                "min_learning_rate": 1e-07,
-                "n_tags": "#tag_vocab.len",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "betas": [
-                        0.9,
-                        0.999
-                    ],
-                    "eps": 1e-06,
-                    "lr": 2.78e-05,
-                    "weight_decay": 1e-06
+                    "lr": 3.67e-05
                 },
                 "out": [
-                    "y_pred_ind",
-                    "probas"
+                    "ans_start_predicted",
+                    "ans_end_predicted",
+                    "logits",
+                    "scores",
+                    "inds"
                 ],
                 "pretrained_bert": "{TRANSFORMER}",
                 "save_path": "{MODEL_PATH}/model"
             },
             {
+                "class_name": "squad_bert_ans_postprocessor",
                 "in": [
-                    "y_pred_ind"
+                    "ans_start_predicted",
+                    "ans_end_predicted",
+                    "split_context",
+                    "subtok2chars",
+                    "subtokens",
+                    "inds"
                 ],
                 "out": [
-                    "y_pred"
-                ],
-                "ref": "tag_vocab"
+                    "ans_predicted",
+                    "ans_start_predicted",
+                    "ans_end_predicted"
+                ]
             }
         ]
     },
     "dataset_iterator": {
-        "class_name": "data_learning_iterator"
+        "class_name": "squad_iterator",
+        "seed": 1337,
+        "shuffle": true
     },
     "dataset_reader": {
-        "class_name": "conll2003_reader",
-        "data_path": "{DOWNLOADS_PATH}/total_rus/",
-        "dataset_name": "collection_rus",
-        "provide_pos": false
+        "class_name": "squad_dataset_reader",
+        "data_path": "{DOWNLOADS_PATH}/squad_ru_clean/",
+        "dataset": "SberSQuADClean",
+        "url": "http://files.deeppavlov.ai/datasets/sber_squad_clean-v1.1.tar.gz"
     },
     "metadata": {
         "download": [
             {
                 "subdir": "{MODELS_PATH}",
-                "url": "http://files.deeppavlov.ai/v1/ner/ner_rus_conversational_distilrubert_6L.tar.gz"
+                "url": "http://files.deeppavlov.ai/deeppavlov_data/squad_ru_convers_distilrubert_6L.tar.gz"
             }
         ],
         "variables": {
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/ner_rus_conversational_distilrubert_6L",
+            "MODEL_PATH": "{MODELS_PATH}/squad_ru_convers_distilrubert_6L",
             "ROOT_PATH": "~/.deeppavlov",
-            "TRANSFORMER": "DeepPavlov/distilrubert-base-cased-conversational"
+            "TRANSFORMER": "DeepPavlov/distilrubert-base-cased-conversational",
+            "lowercase": false
         }
     },
     "train": {
         "batch_size": 10,
         "class_name": "torch_trainer",
-        "epochs": 30,
         "evaluation_targets": [
-            "valid",
-            "test"
+            "valid"
         ],
-        "log_every_n_batches": 20,
+        "log_every_n_batches": 250,
         "metrics": [
             {
                 "inputs": [
-                    "y",
-                    "y_pred"
+                    "ans",
+                    "ans_predicted"
+                ],
+                "name": "squad_v2_f1"
+            },
+            {
+                "inputs": [
+                    "ans",
+                    "ans_predicted"
+                ],
+                "name": "squad_v2_em"
+            },
+            {
+                "inputs": [
+                    "ans",
+                    "ans_predicted"
                 ],
-                "name": "ner_f1"
+                "name": "squad_v1_f1"
             },
             {
                 "inputs": [
-                    "y",
-                    "y_pred"
+                    "ans",
+                    "ans_predicted"
                 ],
-                "name": "ner_token_f1"
+                "name": "squad_v1_em"
             }
         ],
         "show_examples": false,
-        "tensorboard_log_dir": "{MODEL_PATH}/",
-        "val_every_n_batches": 20,
-        "validation_patience": 100
+        "tensorboard_log_dir": "{MODEL_PATH}/logs",
+        "val_every_n_batches": 500,
+        "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/odqa/en_odqa_infer_wiki.json` & `deeppavlov-1.2.0/deeppavlov/configs/odqa/en_odqa_infer_wiki.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/odqa/en_odqa_pop_infer_enwiki20180211.json` & `deeppavlov-1.2.0/deeppavlov/configs/odqa/en_odqa_pop_infer_enwiki20180211.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/odqa/ru_odqa_infer_wiki.json` & `deeppavlov-1.2.0/deeppavlov/configs/odqa/ru_odqa_infer_wiki.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/odqa/ru_odqa_infer_wiki_retr_noans.json` & `deeppavlov-1.2.0/deeppavlov/configs/odqa/ru_odqa_infer_wiki_retr_noans.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ranking/ranking_ubuntu_v2_torch_bert_uncased.json` & `deeppavlov-1.2.0/deeppavlov/configs/ranking/ranking_ubuntu_v2_torch_bert_uncased.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ranking/rel_ranking_bert_en.json` & `deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_russe_rubert.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7277195894383395%*

 * *Differences: {"'chainer'": "{'in': ['sentence1', 'sentence2'], 'pipe': {0: {'class_name': "*

 * *              "'torch_transformers_preprocessor', 'vocab_file': '{BASE_MODEL}', 'do_lower_case': "*

 * *              "False, 'max_seq_length': 256, 'in': ['sentence1', 'sentence2'], delete: "*

 * *              "['add_special_tokens']}, 3: {'return_probas': True, 'pretrained_bert': "*

 * *              "'{BASE_MODEL}', 'optimizer_parameters': {'lr': 2e-05}, delete: "*

 * *              "['num_special_tokens', 'learning_rate_drop_patience', 'learnin […]*

```diff
@@ -1,37 +1,32 @@
 {
     "chainer": {
         "in": [
-            "question",
-            "rel_list"
+            "sentence1",
+            "sentence2"
         ],
         "in_y": [
             "y"
         ],
         "out": [
-            "y_pred_probas"
+            "y_pred_labels"
         ],
         "pipe": [
             {
-                "add_special_tokens": [
-                    "<q>",
-                    "</q>",
-                    "<rel_sep>"
-                ],
-                "class_name": "rel_ranking_preprocessor",
-                "do_lower_case": true,
+                "class_name": "torch_transformers_preprocessor",
+                "do_lower_case": false,
                 "in": [
-                    "question",
-                    "rel_list"
+                    "sentence1",
+                    "sentence2"
                 ],
-                "max_seq_length": 64,
+                "max_seq_length": 256,
                 "out": [
                     "bert_features"
                 ],
-                "vocab_file": "{TRANSFORMER}"
+                "vocab_file": "{BASE_MODEL}"
             },
             {
                 "class_name": "simple_vocab",
                 "fit_on": [
                     "y"
                 ],
                 "id": "classes_vocab",
@@ -59,28 +54,25 @@
                 "class_name": "torch_transformers_classifier",
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
-                "learning_rate_drop_div": 2.0,
-                "learning_rate_drop_patience": 5,
                 "load_path": "{MODEL_PATH}/model",
                 "n_classes": "#classes_vocab.len",
-                "num_special_tokens": 3,
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "lr": 1e-05
+                    "lr": 2e-05
                 },
                 "out": [
                     "y_pred_probas"
                 ],
-                "pretrained_bert": "{TRANSFORMER}",
-                "return_probas": "true",
+                "pretrained_bert": "{BASE_MODEL}",
+                "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
             },
             {
                 "class_name": "proba2labels",
                 "in": [
                     "y_pred_probas"
                 ],
@@ -97,59 +89,61 @@
                     "y_pred_labels"
                 ],
                 "ref": "classes_vocab"
             }
         ]
     },
     "dataset_iterator": {
-        "class_name": "basic_classification_iterator",
+        "class_name": "huggingface_dataset_iterator",
+        "features": [
+            "sentence1",
+            "sentence2"
+        ],
+        "label": "label",
         "seed": 42
     },
     "dataset_reader": {
-        "class_name": "sq_reader",
-        "data_path": "{DOWNLOADS_PATH}/rel_ranking_eng/lcquad_rel_ranking.pickle"
+        "class_name": "huggingface_dataset_reader",
+        "data_url": "http://files.deeppavlov.ai/datasets/russian_super_glue/RUSSE",
+        "ignore_verifications": true,
+        "name": "{TASK}",
+        "path": "{COMPETITION}",
+        "test": "test",
+        "train": "train",
+        "valid": "validation"
     },
     "metadata": {
         "download": [
             {
                 "subdir": "{MODEL_PATH}",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/rel_ranking_bert_eng_torch.tar.gz"
-            },
-            {
-                "subdir": "{DOWNLOADS_PATH}/rel_ranking_eng",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/lcquad_rel_ranking.pickle"
+                "url": "http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_russe_rubert.tar.gz"
             }
         ],
         "variables": {
+            "BASE_MODEL": "DeepPavlov/rubert-base-cased",
+            "COMPETITION": "russian_super_glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/rel_ranking_bert_eng_torch",
+            "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
             "ROOT_PATH": "~/.deeppavlov",
-            "TRANSFORMER": "haisongzhang/roberta-tiny-cased"
+            "TASK": "russe"
         }
     },
     "train": {
-        "batch_size": 30,
+        "batch_size": 4,
         "class_name": "torch_trainer",
-        "epochs": 3,
+        "epochs": 10,
         "evaluation_targets": [
-            "train",
-            "valid",
-            "test"
+            "valid"
         ],
-        "log_every_n_batches": 100,
+        "log_every_n_epochs": 1,
         "metrics": [
-            {
-                "inputs": [
-                    "y_onehot",
-                    "y_pred_probas"
-                ],
-                "name": "roc_auc"
-            },
-            "accuracy",
-            "f1_macro"
+            "accuracy"
         ],
+        "pytest_max_batches": 2,
         "show_examples": false,
-        "val_every_n_batches": 100,
-        "validation_patience": 5
+        "tensorboard_log_dir": "{MODEL_PATH}/",
+        "val_every_n_batches": 1000,
+        "val_every_n_epochs": 1,
+        "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/ranking/rel_ranking_bert_ru.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_mrpc_roberta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7218377976190475%*

 * *Differences: {"'chainer'": "{'in': ['sentence1', 'sentence2'], 'pipe': {0: {'class_name': "*

 * *              "'torch_transformers_preprocessor', 'vocab_file': '{BASE_MODEL}', 'do_lower_case': "*

 * *              "False, 'max_seq_length': 256, 'in': ['sentence1', 'sentence2'], delete: "*

 * *              "['add_special_tokens']}, 3: {'return_probas': True, 'pretrained_bert': "*

 * *              "'{BASE_MODEL}', 'optimizer_parameters': {'lr': 1e-06}, "*

 * *              "'learning_rate_drop_patience': 3, delete: ['num_special_tokens']}}, 'o […]*

```diff
@@ -1,37 +1,32 @@
 {
     "chainer": {
         "in": [
-            "question",
-            "rel_list"
+            "sentence1",
+            "sentence2"
         ],
         "in_y": [
             "y"
         ],
         "out": [
-            "y_pred_probas"
+            "y_pred_labels"
         ],
         "pipe": [
             {
-                "add_special_tokens": [
-                    "<q>",
-                    "</q>",
-                    "<rel_sep>"
-                ],
-                "class_name": "rel_ranking_preprocessor",
-                "do_lower_case": true,
+                "class_name": "torch_transformers_preprocessor",
+                "do_lower_case": false,
                 "in": [
-                    "question",
-                    "rel_list"
+                    "sentence1",
+                    "sentence2"
                 ],
-                "max_seq_length": 64,
+                "max_seq_length": 256,
                 "out": [
                     "bert_features"
                 ],
-                "vocab_file": "{TRANSFORMER}"
+                "vocab_file": "{BASE_MODEL}"
             },
             {
                 "class_name": "simple_vocab",
                 "fit_on": [
                     "y"
                 ],
                 "id": "classes_vocab",
@@ -60,27 +55,26 @@
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
                 "learning_rate_drop_div": 2.0,
-                "learning_rate_drop_patience": 5,
+                "learning_rate_drop_patience": 3,
                 "load_path": "{MODEL_PATH}/model",
                 "n_classes": "#classes_vocab.len",
-                "num_special_tokens": 3,
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "lr": 1e-05
+                    "lr": 1e-06
                 },
                 "out": [
                     "y_pred_probas"
                 ],
-                "pretrained_bert": "{TRANSFORMER}",
-                "return_probas": "true",
+                "pretrained_bert": "{BASE_MODEL}",
+                "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
             },
             {
                 "class_name": "proba2labels",
                 "in": [
                     "y_pred_probas"
                 ],
@@ -97,59 +91,57 @@
                     "y_pred_labels"
                 ],
                 "ref": "classes_vocab"
             }
         ]
     },
     "dataset_iterator": {
-        "class_name": "basic_classification_iterator",
+        "class_name": "huggingface_dataset_iterator",
+        "features": [
+            "sentence1",
+            "sentence2"
+        ],
+        "label": "label",
         "seed": 42
     },
     "dataset_reader": {
-        "class_name": "sq_reader",
-        "data_path": "{DOWNLOADS_PATH}/rel_ranking_rus/rubq_rel_ranking.pickle"
+        "class_name": "huggingface_dataset_reader",
+        "name": "{TASK}",
+        "path": "{COMPETITION}",
+        "test": "test",
+        "train": "train",
+        "valid": "validation"
     },
     "metadata": {
         "download": [
             {
                 "subdir": "{MODEL_PATH}",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/rel_ranking_bert_rus_torch.tar.gz"
-            },
-            {
-                "subdir": "{DOWNLOADS_PATH}/rel_ranking_rus",
-                "url": "http://files.deeppavlov.ai/kbqa/wikidata/rubq_rel_ranking.pickle"
+                "url": "http://files.deeppavlov.ai/v1/glue/glue_mrpc_roberta.tar.gz"
             }
         ],
         "variables": {
+            "BASE_MODEL": "roberta-large",
+            "COMPETITION": "glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/classifiers/rel_ranking_bert_rus_torch",
+            "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
             "ROOT_PATH": "~/.deeppavlov",
-            "TRANSFORMER": "DeepPavlov/distilrubert-tiny-cased-conversational"
+            "TASK": "mrpc"
         }
     },
     "train": {
-        "batch_size": 30,
+        "batch_size": 4,
         "class_name": "torch_trainer",
-        "epochs": 3,
+        "epochs": 2,
         "evaluation_targets": [
-            "train",
-            "valid",
-            "test"
+            "valid"
         ],
-        "log_every_n_batches": 100,
+        "log_every_n_epochs": 1,
         "metrics": [
-            {
-                "inputs": [
-                    "y_onehot",
-                    "y_pred_probas"
-                ],
-                "name": "roc_auc"
-            },
-            "accuracy",
-            "f1_macro"
+            "accuracy"
         ],
+        "pytest_max_batches": 2,
         "show_examples": false,
-        "val_every_n_batches": 100,
-        "validation_patience": 5
+        "tensorboard_log_dir": "{MODEL_PATH}/",
+        "val_every_n_epochs": 1
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/regressors/translation_ranker.json` & `deeppavlov-1.2.0/deeppavlov/configs/regressors/translation_ranker.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/relation_extraction/re_docred.json` & `deeppavlov-1.2.0/deeppavlov/configs/relation_extraction/re_rured.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8772673160173159%*

 * *Differences: {"'chainer'": "{'pipe': {0: {'vocab_file': '{TRANSFORMER}', 'default_tag': 'PERSON', 'ner_tags': "*

 * *              "['WORK_OF_ART', 'NORP', 'GROUP', 'LAW', 'NATIONALITY', 'EVENT', 'DATE', 'CURRENCY', "*

 * *              "'GPE', 'QUANTITY', 'FAMILY', 'ORDINAL', 'RELIGION', 'CITY', 'MONEY', 'AGE', "*

 * *              "'LOCATION', 'PERCENT', 'BOROUGH', 'STREET', 'PERSON', 'REGION', 'COUNTRY', "*

 * *              "'PROFESSION', 'ORGANIZATION', 'FAC', 'CARDINAL', 'PRODUCT', 'TIME'], "*

 * *              "'max_seq_length': 512}, 1: […]*

```diff
@@ -11,113 +11,136 @@
         "out": [
             "wikidata_relation_id",
             "relation_name"
         ],
         "pipe": [
             {
                 "class_name": "re_preprocessor",
-                "default_tag": "PER",
+                "default_tag": "PERSON",
                 "in": [
                     "tokens",
                     "entity_pos",
                     "entity_tags"
                 ],
+                "max_seq_length": 512,
+                "ner_tags": [
+                    "WORK_OF_ART",
+                    "NORP",
+                    "GROUP",
+                    "LAW",
+                    "NATIONALITY",
+                    "EVENT",
+                    "DATE",
+                    "CURRENCY",
+                    "GPE",
+                    "QUANTITY",
+                    "FAMILY",
+                    "ORDINAL",
+                    "RELIGION",
+                    "CITY",
+                    "MONEY",
+                    "AGE",
+                    "LOCATION",
+                    "PERCENT",
+                    "BOROUGH",
+                    "STREET",
+                    "PERSON",
+                    "REGION",
+                    "COUNTRY",
+                    "PROFESSION",
+                    "ORGANIZATION",
+                    "FAC",
+                    "CARDINAL",
+                    "PRODUCT",
+                    "TIME"
+                ],
                 "out": [
                     "input_ids",
                     "attention_mask",
                     "upd_entity_pos",
                     "upd_entity_tags",
                     "nf_samples"
                 ],
-                "vocab_file": "bert-base-cased"
+                "vocab_file": "{TRANSFORMER}"
             },
             {
                 "class_name": "re_classifier",
                 "in": [
                     "input_ids",
                     "attention_mask",
                     "upd_entity_pos",
                     "upd_entity_tags"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
                 "load_path": "{MODEL_PATH}/model",
                 "model_name": "re_model",
-                "n_classes": 97,
-                "num_ner_tags": 6,
+                "n_classes": 30,
+                "num_ner_tags": 29,
                 "out": [
                     "model_output"
                 ],
-                "pretrained_bert": "bert-base-cased",
-                "return_probas": true,
+                "pretrained_bert": "{TRANSFORMER}",
                 "save_path": "{MODEL_PATH}/model"
             },
             {
                 "class_name": "re_postprocessor",
                 "in": [
                     "model_output",
                     "nf_samples"
                 ],
                 "out": [
                     "wikidata_relation_id",
                     "relation_name"
                 ],
-                "rel2id_path": "{DOWNLOADS_PATH}/docred/meta/rel2id.json",
-                "rel2label_path": "{DOWNLOADS_PATH}/docred/rel_info.json"
+                "rel2id_path": "{DOWNLOADS_PATH}/rured/rel2id.json",
+                "rel2label_path": "{DOWNLOADS_PATH}/rured/rel2label.json"
             }
         ]
     },
     "dataset_iterator": {
         "class_name": "basic_classification_iterator"
     },
     "dataset_reader": {
-        "class_name": "docred_reader",
-        "data_path": "{DOWNLOADS_PATH}/docred/",
-        "rel2id_path": "{DOWNLOADS_PATH}/docred/meta/rel2id.json",
-        "rel_info_path": "{DOWNLOADS_PATH}/docred/rel_info.json",
-        "valid_test_data_size": 150
+        "class_name": "rured_reader",
+        "data_path": "{DOWNLOADS_PATH}/rured/"
     },
     "metadata": {
         "download": [
             {
-                "subdir": "{DOWNLOADS_PATH}/docred",
-                "url": "http://files.deeppavlov.ai/deeppavlov_data/relation_extraction/docred.tar.gz"
-            },
-            {
-                "subdir": "{MODELS_PATH}/re_docred",
-                "url": "http://files.deeppavlov.ai/deeppavlov_data/relation_extraction/re_docred_model_v1.tar.gz"
+                "subdir": "{DOWNLOADS_PATH}/rured",
+                "url": "http://files.deeppavlov.ai/deeppavlov_data/relation_extraction/rured.tar.gz"
             },
             {
-                "subdir": "{DOWNLOADS_PATH}/docred",
-                "url": "http://files.deeppavlov.ai/deeppavlov_data/relation_extraction/rel2label.json"
+                "subdir": "{MODELS_PATH}/re_rured",
+                "url": "http://files.deeppavlov.ai/deeppavlov_data/relation_extraction/re_rured_model_v1.tar.gz"
             }
         ],
         "variables": {
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/re_docred",
-            "ROOT_PATH": "~/.deeppavlov"
+            "MODEL_PATH": "{MODELS_PATH}/re_rured",
+            "ROOT_PATH": "~/.deeppavlov",
+            "TRANSFORMER": "DeepPavlov/rubert-base-cased"
         }
     },
     "train": {
-        "batch_size": 30,
+        "batch_size": 16,
         "class_name": "torch_trainer",
         "epochs": 50,
         "evaluation_targets": [
             "valid",
             "train"
         ],
         "log_every_n_batches": 100,
         "metrics": [
-            "f1_weighted",
             "acc"
         ],
         "show_examples": false,
         "train_metrics": [
-            "f1_weighted",
             "acc"
         ],
-        "val_every_n_batches": 200,
+        "val_every_n_batches": 100,
         "validation_patience": 50
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/relation_extraction/re_rured.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_qnli_roberta.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6818216765873015%*

 * *Differences: {"'chainer'": "{'in': ['question', 'sentence'], 'in_y': ['y'], 'pipe': {0: {'in': ['question', "*

 * *              "'sentence'], 'out': ['bert_features'], 'class_name': "*

 * *              "'torch_transformers_preprocessor', 'max_seq_length': 128, 'vocab_file': "*

 * *              "'{BASE_MODEL}', 'do_lower_case': False, delete: ['ner_tags', 'default_tag']}, 3: "*

 * *              "{'class_name': 'torch_transformers_classifier', 'in': ['bert_features'], 'out': "*

 * *              "['y_pred_probas'], 'n_classes': '#classes_voca […]*

```diff
@@ -1,146 +1,148 @@
 {
     "chainer": {
         "in": [
-            "tokens",
-            "entity_pos",
-            "entity_tags"
+            "question",
+            "sentence"
         ],
         "in_y": [
-            "y_ids"
+            "y"
         ],
         "out": [
-            "wikidata_relation_id",
-            "relation_name"
+            "y_pred_labels"
         ],
         "pipe": [
             {
-                "class_name": "re_preprocessor",
-                "default_tag": "PERSON",
+                "class_name": "torch_transformers_preprocessor",
+                "do_lower_case": false,
                 "in": [
-                    "tokens",
-                    "entity_pos",
-                    "entity_tags"
-                ],
-                "max_seq_length": 512,
-                "ner_tags": [
-                    "WORK_OF_ART",
-                    "NORP",
-                    "GROUP",
-                    "LAW",
-                    "NATIONALITY",
-                    "EVENT",
-                    "DATE",
-                    "CURRENCY",
-                    "GPE",
-                    "QUANTITY",
-                    "FAMILY",
-                    "ORDINAL",
-                    "RELIGION",
-                    "CITY",
-                    "MONEY",
-                    "AGE",
-                    "LOCATION",
-                    "PERCENT",
-                    "BOROUGH",
-                    "STREET",
-                    "PERSON",
-                    "REGION",
-                    "COUNTRY",
-                    "PROFESSION",
-                    "ORGANIZATION",
-                    "FAC",
-                    "CARDINAL",
-                    "PRODUCT",
-                    "TIME"
-                ],
-                "out": [
-                    "input_ids",
-                    "attention_mask",
-                    "upd_entity_pos",
-                    "upd_entity_tags",
-                    "nf_samples"
+                    "question",
+                    "sentence"
                 ],
-                "vocab_file": "{TRANSFORMER}"
+                "max_seq_length": 128,
+                "out": [
+                    "bert_features"
+                ],
+                "vocab_file": "{BASE_MODEL}"
+            },
+            {
+                "class_name": "simple_vocab",
+                "fit_on": [
+                    "y"
+                ],
+                "id": "classes_vocab",
+                "in": [
+                    "y"
+                ],
+                "load_path": "{MODEL_PATH}/classes.dict",
+                "out": [
+                    "y_ids"
+                ],
+                "save_path": "{MODEL_PATH}/classes.dict"
+            },
+            {
+                "class_name": "one_hotter",
+                "depth": "#classes_vocab.len",
+                "in": [
+                    "y_ids"
+                ],
+                "out": [
+                    "y_onehot"
+                ],
+                "single_vector": true
             },
             {
-                "class_name": "re_classifier",
+                "class_name": "torch_transformers_classifier",
                 "in": [
-                    "input_ids",
-                    "attention_mask",
-                    "upd_entity_pos",
-                    "upd_entity_tags"
+                    "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
+                "learning_rate_drop_div": 2.0,
+                "learning_rate_drop_patience": 3,
                 "load_path": "{MODEL_PATH}/model",
-                "model_name": "re_model",
-                "n_classes": 30,
-                "num_ner_tags": 29,
+                "n_classes": "#classes_vocab.len",
+                "optimizer": "AdamW",
+                "optimizer_parameters": {
+                    "lr": 2e-05
+                },
                 "out": [
-                    "model_output"
+                    "y_pred_probas"
                 ],
-                "pretrained_bert": "{TRANSFORMER}",
+                "pretrained_bert": "{BASE_MODEL}",
+                "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
             },
             {
-                "class_name": "re_postprocessor",
+                "class_name": "proba2labels",
                 "in": [
-                    "model_output",
-                    "nf_samples"
+                    "y_pred_probas"
                 ],
+                "max_proba": true,
                 "out": [
-                    "wikidata_relation_id",
-                    "relation_name"
+                    "y_pred_ids"
+                ]
+            },
+            {
+                "in": [
+                    "y_pred_ids"
                 ],
-                "rel2id_path": "{DOWNLOADS_PATH}/rured/rel2id.json",
-                "rel2label_path": "{DOWNLOADS_PATH}/rured/rel2label.json"
+                "out": [
+                    "y_pred_labels"
+                ],
+                "ref": "classes_vocab"
             }
         ]
     },
     "dataset_iterator": {
-        "class_name": "basic_classification_iterator"
+        "class_name": "huggingface_dataset_iterator",
+        "features": [
+            "question",
+            "sentence"
+        ],
+        "label": "label",
+        "seed": 42
     },
     "dataset_reader": {
-        "class_name": "rured_reader",
-        "data_path": "{DOWNLOADS_PATH}/rured/"
+        "class_name": "huggingface_dataset_reader",
+        "name": "{TASK}",
+        "path": "{COMPETITION}",
+        "test": "test",
+        "train": "train",
+        "valid": "validation"
     },
     "metadata": {
         "download": [
             {
-                "subdir": "{DOWNLOADS_PATH}/rured",
-                "url": "http://files.deeppavlov.ai/deeppavlov_data/relation_extraction/rured.tar.gz"
-            },
-            {
-                "subdir": "{MODELS_PATH}/re_rured",
-                "url": "http://files.deeppavlov.ai/deeppavlov_data/relation_extraction/re_rured_model_v1.tar.gz"
+                "subdir": "{MODEL_PATH}",
+                "url": "http://files.deeppavlov.ai/v1/glue/glue_qnli_roberta.tar.gz"
             }
         ],
         "variables": {
+            "BASE_MODEL": "roberta-large",
+            "COMPETITION": "glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/re_rured",
+            "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
             "ROOT_PATH": "~/.deeppavlov",
-            "TRANSFORMER": "DeepPavlov/rubert-base-cased"
+            "TASK": "qnli"
         }
     },
     "train": {
-        "batch_size": 16,
+        "batch_size": 64,
         "class_name": "torch_trainer",
-        "epochs": 50,
         "evaluation_targets": [
-            "valid",
-            "train"
+            "train",
+            "valid"
         ],
-        "log_every_n_batches": 100,
+        "log_every_n_batches": 250,
         "metrics": [
-            "acc"
+            "accuracy"
         ],
+        "pytest_max_batches": 2,
         "show_examples": false,
-        "train_metrics": [
-            "acc"
-        ],
-        "val_every_n_batches": 100,
-        "validation_patience": 50
+        "tensorboard_log_dir": "{MODEL_PATH}/",
+        "val_every_n_batches": 250,
+        "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_danetqa_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_rwsd_rubert.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9295312499999999%*

 * *Differences: {"'chainer'": "{'in': ['text', 'answer'], 'pipe': {0: {'do_lower_case': True, 'max_seq_length': "*

 * *              "256, 'in': ['text', 'answer']}, 3: {'optimizer': 'Adam', delete: ['is_binary']}, 4: "*

 * *              "{delete: ['is_binary']}}}",*

 * * "'dataset_iterator'": "{'features': ['text', 'answer']}",*

 * * "'dataset_reader'": "{'data_url': 'http://files.deeppavlov.ai/datasets/russian_super_glue/RWSD', "*

 * *                     "'ignore_verifications': True}",*

 * * "'metadata'": "{'variables': {'TASK': 'rwsd', delete: [' […]*

```diff
@@ -1,28 +1,28 @@
 {
     "chainer": {
         "in": [
-            "question",
-            "passage"
+            "text",
+            "answer"
         ],
         "in_y": [
             "y"
         ],
         "out": [
             "y_pred_labels"
         ],
         "pipe": [
             {
                 "class_name": "torch_transformers_preprocessor",
-                "do_lower_case": false,
+                "do_lower_case": true,
                 "in": [
-                    "question",
-                    "passage"
+                    "text",
+                    "answer"
                 ],
-                "max_seq_length": 512,
+                "max_seq_length": 256,
                 "out": [
                     "bert_features"
                 ],
                 "vocab_file": "{BASE_MODEL}"
             },
             {
                 "class_name": "simple_vocab",
@@ -54,18 +54,17 @@
                 "class_name": "torch_transformers_classifier",
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
-                "is_binary": "{BINARY_CLASSIFICATION}",
                 "load_path": "{MODEL_PATH}/model",
                 "n_classes": "#classes_vocab.len",
-                "optimizer": "AdamW",
+                "optimizer": "Adam",
                 "optimizer_parameters": {
                     "lr": 2e-05
                 },
                 "out": [
                     "y_pred_probas"
                 ],
                 "pretrained_bert": "{BASE_MODEL}",
@@ -73,15 +72,14 @@
                 "save_path": "{MODEL_PATH}/model"
             },
             {
                 "class_name": "proba2labels",
                 "in": [
                     "y_pred_probas"
                 ],
-                "is_binary": "{BINARY_CLASSIFICATION}",
                 "max_proba": true,
                 "out": [
                     "y_pred_ids"
                 ]
             },
             {
                 "in": [
@@ -93,59 +91,59 @@
                 "ref": "classes_vocab"
             }
         ]
     },
     "dataset_iterator": {
         "class_name": "huggingface_dataset_iterator",
         "features": [
-            "question",
-            "passage"
+            "text",
+            "answer"
         ],
         "label": "label",
         "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
+        "data_url": "http://files.deeppavlov.ai/datasets/russian_super_glue/RWSD",
+        "ignore_verifications": true,
         "name": "{TASK}",
         "path": "{COMPETITION}",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
         "download": [
             {
                 "subdir": "{MODEL_PATH}",
-                "url": "http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_danetqa_rubert.tar.gz"
+                "url": "http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_rwsd_rubert.tar.gz"
             }
         ],
         "variables": {
             "BASE_MODEL": "DeepPavlov/rubert-base-cased",
-            "BINARY_CLASSIFICATION": false,
             "COMPETITION": "russian_super_glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
             "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
             "ROOT_PATH": "~/.deeppavlov",
-            "TASK": "danetqa"
+            "TASK": "rwsd"
         }
     },
     "train": {
         "batch_size": 4,
         "class_name": "torch_trainer",
         "epochs": 10,
         "evaluation_targets": [
             "train",
             "valid"
         ],
         "log_every_n_epochs": 1,
         "metrics": [
             "accuracy"
         ],
-        "pytest_batch_size": 2,
         "pytest_max_batches": 2,
         "show_examples": false,
         "tensorboard_log_dir": "{MODEL_PATH}/",
         "val_every_n_epochs": 1,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_lidirus_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_lidirus_rubert.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666666%*

 * *Differences: {"'dataset_reader'": "{'data_url': "*

 * *                     "'http://files.deeppavlov.ai/datasets/russian_super_glue/LiDiRus', "*

 * *                     "'ignore_verifications': True}"}*

```diff
@@ -104,14 +104,16 @@
             "sentence2"
         ],
         "label": "label",
         "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
+        "data_url": "http://files.deeppavlov.ai/datasets/russian_super_glue/LiDiRus",
+        "ignore_verifications": true,
         "name": "{TASK}",
         "path": "{COMPETITION}",
         "test": "test"
     },
     "metadata": {
         "download": [
             {
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_muserc_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_muserc_rubert.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'dataset_reader'": "{'data_url': "*

 * *                     "'http://files.deeppavlov.ai/datasets/russian_super_glue/MuSeRC', "*

 * *                     "'ignore_verifications': True}"}*

```diff
@@ -103,14 +103,16 @@
             "idx"
         ],
         "label": "label",
         "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
+        "data_url": "http://files.deeppavlov.ai/datasets/russian_super_glue/MuSeRC",
+        "ignore_verifications": true,
         "name": "{TASK}",
         "path": "{COMPETITION}",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_parus_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_parus_rubert.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'dataset_reader'": "{'data_url': 'http://files.deeppavlov.ai/datasets/russian_super_glue/PARus', "*

 * *                     "'ignore_verifications': True}"}*

```diff
@@ -99,14 +99,16 @@
             "choices"
         ],
         "label": "label",
         "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
+        "data_url": "http://files.deeppavlov.ai/datasets/russian_super_glue/PARus",
+        "ignore_verifications": true,
         "name": "{TASK}",
         "path": "{COMPETITION}",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_rcb_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_terra_rubert.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9534288194444445%*

 * *Differences: {"'chainer'": "{'pipe': {3: {'optimizer_parameters': {'lr': 2e-05}, 'is_binary': "*

 * *              "'{BINARY_CLASSIFICATION}'}}}",*

 * * "'dataset_reader'": "{'data_url': 'http://files.deeppavlov.ai/datasets/russian_super_glue/TERRa', "*

 * *                     "'ignore_verifications': True}",*

 * * "'metadata'": "{'variables': {'TASK': 'terra', 'BINARY_CLASSIFICATION': False}, 'download': {0: "*

 * *               "{'url': "*

 * *               "'http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_terra_rubert.tar.gz […]*

```diff
@@ -54,19 +54,20 @@
                 "class_name": "torch_transformers_classifier",
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
+                "is_binary": "{BINARY_CLASSIFICATION}",
                 "load_path": "{MODEL_PATH}/model",
                 "n_classes": "#classes_vocab.len",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "lr": 4e-05
+                    "lr": 2e-05
                 },
                 "out": [
                     "y_pred_probas"
                 ],
                 "pretrained_bert": "{BASE_MODEL}",
                 "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
@@ -99,50 +100,53 @@
             "hypothesis"
         ],
         "label": "label",
         "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
+        "data_url": "http://files.deeppavlov.ai/datasets/russian_super_glue/TERRa",
+        "ignore_verifications": true,
         "name": "{TASK}",
         "path": "{COMPETITION}",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
         "download": [
             {
                 "subdir": "{MODEL_PATH}",
-                "url": "http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_rcb_rubert.tar.gz"
+                "url": "http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_terra_rubert.tar.gz"
             }
         ],
         "variables": {
             "BASE_MODEL": "DeepPavlov/rubert-base-cased",
+            "BINARY_CLASSIFICATION": false,
             "COMPETITION": "russian_super_glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
             "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
             "ROOT_PATH": "~/.deeppavlov",
-            "TASK": "rcb"
+            "TASK": "terra"
         }
     },
     "train": {
         "batch_size": 4,
         "class_name": "torch_trainer",
         "epochs": 10,
         "evaluation_targets": [
             "train",
             "valid"
         ],
         "log_every_n_epochs": 1,
         "metrics": [
-            "accuracy",
-            "f1_macro"
+            "accuracy"
         ],
+        "pytest_batch_size": 2,
         "pytest_max_batches": 2,
         "show_examples": false,
         "tensorboard_log_dir": "{MODEL_PATH}/",
         "val_every_n_epochs": 1,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_rucos_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_rucos_rubert.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9800000000000001%*

 * *Differences: {"'dataset_reader'": "{'data_url': 'http://files.deeppavlov.ai/datasets/russian_super_glue/RuCoS', "*

 * *                     "'ignore_verifications': True}"}*

```diff
@@ -86,20 +86,22 @@
             "num_examples"
         ],
         "label": "label",
         "use_label_name": false
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
+        "data_url": "http://files.deeppavlov.ai/datasets/russian_super_glue/RuCoS",
         "do_index_correction": false,
         "downsample_ratio": [
             1.8,
             1.8,
             1
         ],
+        "ignore_verifications": true,
         "name": "{TASK}",
         "path": "{COMPETITION}",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_russe_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/classifiers/glue/glue_cola_roberta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9184943528693529%*

 * *Differences: {"'chainer'": "{'in': ['x'], 'pipe': {0: {'max_seq_length': 64, 'in': ['x']}, 3: "*

 * *              "{'learning_rate_drop_patience': 3, 'learning_rate_drop_div': 2.0}}}",*

 * * "'dataset_iterator'": "{'features': 'sentence'}",*

 * * "'metadata'": "{'variables': {'BASE_MODEL': 'roberta-large', 'COMPETITION': 'glue', 'TASK': "*

 * *               "'cola'}, 'download': {0: {'url': "*

 * *               "'http://files.deeppavlov.ai/v1/glue/glue_cola_roberta.tar.gz'}}}",*

 * * "'train'": "{'batch_size': 128, 'metrics': ['matthews_correlati […]*

```diff
@@ -1,28 +1,26 @@
 {
     "chainer": {
         "in": [
-            "sentence1",
-            "sentence2"
+            "x"
         ],
         "in_y": [
             "y"
         ],
         "out": [
             "y_pred_labels"
         ],
         "pipe": [
             {
                 "class_name": "torch_transformers_preprocessor",
                 "do_lower_case": false,
                 "in": [
-                    "sentence1",
-                    "sentence2"
+                    "x"
                 ],
-                "max_seq_length": 256,
+                "max_seq_length": 64,
                 "out": [
                     "bert_features"
                 ],
                 "vocab_file": "{BASE_MODEL}"
             },
             {
                 "class_name": "simple_vocab",
@@ -54,14 +52,16 @@
                 "class_name": "torch_transformers_classifier",
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
+                "learning_rate_drop_div": 2.0,
+                "learning_rate_drop_patience": 3,
                 "load_path": "{MODEL_PATH}/model",
                 "n_classes": "#classes_vocab.len",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
                     "lr": 2e-05
                 },
                 "out": [
@@ -90,18 +90,15 @@
                 ],
                 "ref": "classes_vocab"
             }
         ]
     },
     "dataset_iterator": {
         "class_name": "huggingface_dataset_iterator",
-        "features": [
-            "sentence1",
-            "sentence2"
-        ],
+        "features": "sentence",
         "label": "label",
         "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
         "name": "{TASK}",
         "path": "{COMPETITION}",
@@ -109,39 +106,38 @@
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
         "download": [
             {
                 "subdir": "{MODEL_PATH}",
-                "url": "http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_russe_rubert.tar.gz"
+                "url": "http://files.deeppavlov.ai/v1/glue/glue_cola_roberta.tar.gz"
             }
         ],
         "variables": {
-            "BASE_MODEL": "DeepPavlov/rubert-base-cased",
-            "COMPETITION": "russian_super_glue",
+            "BASE_MODEL": "roberta-large",
+            "COMPETITION": "glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
             "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
             "ROOT_PATH": "~/.deeppavlov",
-            "TASK": "russe"
+            "TASK": "cola"
         }
     },
     "train": {
-        "batch_size": 4,
+        "batch_size": 128,
         "class_name": "torch_trainer",
-        "epochs": 10,
         "evaluation_targets": [
+            "train",
             "valid"
         ],
-        "log_every_n_epochs": 1,
+        "log_every_n_batches": 250,
         "metrics": [
-            "accuracy"
+            "matthews_correlation"
         ],
         "pytest_max_batches": 2,
         "show_examples": false,
         "tensorboard_log_dir": "{MODEL_PATH}/",
-        "val_every_n_batches": 1000,
-        "val_every_n_epochs": 1,
+        "val_every_n_batches": 250,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_rwsd_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/squad/qa_multisberquad_bert.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6883968317562068%*

 * *Differences: {"'chainer'": "{'in': ['context_raw', 'question_raw'], 'in_y': ['ans_raw', 'ans_raw_start'], "*

 * *              "'pipe': {0: {'class_name': 'torch_squad_transformers_preprocessor', 'vocab_file': "*

 * *              "'{TRANSFORMER}', 'do_lower_case': '{LOWERCASE}', 'max_seq_length': 384, 'in': "*

 * *              "['question_raw', 'context_raw'], 'out': {insert: [(1, 'subtokens'), (2, "*

 * *              "'split_context')]}}, 1: {'class_name': 'squad_bert_mapping', 'in': "*

 * *              "['split_context', 'bert_features',  […]*

```diff
@@ -1,147 +1,179 @@
 {
     "chainer": {
         "in": [
-            "text",
-            "answer"
+            "context_raw",
+            "question_raw"
         ],
         "in_y": [
-            "y"
+            "ans_raw",
+            "ans_raw_start"
         ],
         "out": [
-            "y_pred_labels"
+            "ans_predicted",
+            "ans_start_predicted",
+            "scores"
         ],
         "pipe": [
             {
-                "class_name": "torch_transformers_preprocessor",
-                "do_lower_case": true,
+                "class_name": "torch_squad_transformers_preprocessor",
+                "do_lower_case": "{LOWERCASE}",
                 "in": [
-                    "text",
-                    "answer"
+                    "question_raw",
+                    "context_raw"
                 ],
-                "max_seq_length": 256,
+                "max_seq_length": 384,
                 "out": [
-                    "bert_features"
+                    "bert_features",
+                    "subtokens",
+                    "split_context"
                 ],
-                "vocab_file": "{BASE_MODEL}"
+                "vocab_file": "{TRANSFORMER}"
             },
             {
-                "class_name": "simple_vocab",
-                "fit_on": [
-                    "y"
-                ],
-                "id": "classes_vocab",
+                "class_name": "squad_bert_mapping",
+                "do_lower_case": "{LOWERCASE}",
                 "in": [
-                    "y"
+                    "split_context",
+                    "bert_features",
+                    "subtokens"
                 ],
-                "load_path": "{MODEL_PATH}/classes.dict",
                 "out": [
-                    "y_ids"
-                ],
-                "save_path": "{MODEL_PATH}/classes.dict"
+                    "subtok2chars",
+                    "char2subtoks"
+                ]
             },
             {
-                "class_name": "one_hotter",
-                "depth": "#classes_vocab.len",
+                "class_name": "squad_bert_ans_preprocessor",
+                "do_lower_case": "{LOWERCASE}",
                 "in": [
-                    "y_ids"
+                    "ans_raw",
+                    "ans_raw_start",
+                    "char2subtoks"
                 ],
                 "out": [
-                    "y_onehot"
-                ],
-                "single_vector": true
+                    "ans",
+                    "ans_start",
+                    "ans_end"
+                ]
             },
             {
-                "class_name": "torch_transformers_classifier",
+                "class_name": "torch_transformers_squad",
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
-                    "y_ids"
+                    "ans_start",
+                    "ans_end"
                 ],
+                "learning_rate_drop_div": 2.0,
+                "learning_rate_drop_patience": 3,
                 "load_path": "{MODEL_PATH}/model",
-                "n_classes": "#classes_vocab.len",
-                "optimizer": "Adam",
+                "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "lr": 2e-05
+                    "betas": [
+                        0.9,
+                        0.999
+                    ],
+                    "eps": 1e-06,
+                    "lr": 2e-05,
+                    "weight_decay": 0.01
                 },
                 "out": [
-                    "y_pred_probas"
+                    "ans_start_predicted",
+                    "ans_end_predicted",
+                    "logits",
+                    "scores",
+                    "inds"
                 ],
-                "pretrained_bert": "{BASE_MODEL}",
-                "return_probas": true,
+                "pretrained_bert": "{TRANSFORMER}",
                 "save_path": "{MODEL_PATH}/model"
             },
             {
-                "class_name": "proba2labels",
+                "class_name": "squad_bert_ans_postprocessor",
                 "in": [
-                    "y_pred_probas"
+                    "ans_start_predicted",
+                    "ans_end_predicted",
+                    "split_context",
+                    "subtok2chars",
+                    "subtokens",
+                    "inds"
                 ],
-                "max_proba": true,
                 "out": [
-                    "y_pred_ids"
+                    "ans_predicted",
+                    "ans_start_predicted",
+                    "ans_end_predicted"
                 ]
-            },
-            {
-                "in": [
-                    "y_pred_ids"
-                ],
-                "out": [
-                    "y_pred_labels"
-                ],
-                "ref": "classes_vocab"
             }
         ]
     },
     "dataset_iterator": {
-        "class_name": "huggingface_dataset_iterator",
-        "features": [
-            "text",
-            "answer"
-        ],
-        "label": "label",
-        "seed": 42
+        "class_name": "multi_squad_retr_iterator",
+        "seed": 1337,
+        "shuffle": false,
+        "with_answer_rate": 0.666
     },
     "dataset_reader": {
-        "class_name": "huggingface_dataset_reader",
-        "name": "{TASK}",
-        "path": "{COMPETITION}",
-        "test": "test",
-        "train": "train",
-        "valid": "validation"
+        "class_name": "multi_squad_dataset_reader",
+        "data_path": "{DOWNLOADS_PATH}/multi_squad_ru_retr_clean/",
+        "dataset": "MultiSQuADRuRetrClean",
+        "url": "http://files.deeppavlov.ai/datasets/multi_squad_ru_retr_clean.tar.gz"
     },
     "metadata": {
         "download": [
             {
                 "subdir": "{MODEL_PATH}",
-                "url": "http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_rwsd_rubert.tar.gz"
+                "url": "http://files.deeppavlov.ai/v1/squad/multi_squad_ru_torch_bert_retr_noans.tar.gz"
             }
         ],
         "variables": {
-            "BASE_MODEL": "DeepPavlov/rubert-base-cased",
-            "COMPETITION": "russian_super_glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
+            "LOWERCASE": false,
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
+            "MODEL_PATH": "{MODELS_PATH}/multi_squad_ru_torch_bert_retr_noans/{TRANSFORMER}",
             "ROOT_PATH": "~/.deeppavlov",
-            "TASK": "rwsd"
+            "TRANSFORMER": "DeepPavlov/rubert-base-cased"
         }
     },
     "train": {
-        "batch_size": 4,
+        "batch_size": 20,
         "class_name": "torch_trainer",
-        "epochs": 10,
         "evaluation_targets": [
-            "train",
             "valid"
         ],
-        "log_every_n_epochs": 1,
+        "log_every_n_batches": 250,
         "metrics": [
-            "accuracy"
+            {
+                "inputs": [
+                    "ans",
+                    "ans_predicted"
+                ],
+                "name": "squad_v1_f1"
+            },
+            {
+                "inputs": [
+                    "ans",
+                    "ans_predicted"
+                ],
+                "name": "squad_v1_em"
+            },
+            {
+                "inputs": [
+                    "ans",
+                    "ans_predicted"
+                ],
+                "name": "squad_v2_f1"
+            },
+            {
+                "inputs": [
+                    "ans",
+                    "ans_predicted"
+                ],
+                "name": "squad_v2_em"
+            }
         ],
-        "pytest_max_batches": 2,
         "show_examples": false,
-        "tensorboard_log_dir": "{MODEL_PATH}/",
-        "val_every_n_epochs": 1,
+        "val_every_n_batches": 500,
+        "valid_batch_size": 64,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/russian_super_glue/russian_superglue_terra_rubert.json` & `deeppavlov-1.2.0/deeppavlov/configs/russian_super_glue/russian_superglue_rcb_rubert.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9534288194444445%*

 * *Differences: {"'chainer'": "{'pipe': {3: {'optimizer_parameters': {'lr': 4e-05}, delete: ['is_binary']}}}",*

 * * "'dataset_reader'": "{'data_url': 'http://files.deeppavlov.ai/datasets/russian_super_glue/RCB', "*

 * *                     "'ignore_verifications': True}",*

 * * "'metadata'": "{'variables': {'TASK': 'rcb', delete: ['BINARY_CLASSIFICATION']}, 'download': {0: "*

 * *               "{'url': "*

 * *               "'http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_rcb_rubert.tar.gz'}}}",*

 * * "'train'": "{'metrics': {inse […]*

```diff
@@ -54,20 +54,19 @@
                 "class_name": "torch_transformers_classifier",
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "y_ids"
                 ],
-                "is_binary": "{BINARY_CLASSIFICATION}",
                 "load_path": "{MODEL_PATH}/model",
                 "n_classes": "#classes_vocab.len",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "lr": 2e-05
+                    "lr": 4e-05
                 },
                 "out": [
                     "y_pred_probas"
                 ],
                 "pretrained_bert": "{BASE_MODEL}",
                 "return_probas": true,
                 "save_path": "{MODEL_PATH}/model"
@@ -100,51 +99,52 @@
             "hypothesis"
         ],
         "label": "label",
         "seed": 42
     },
     "dataset_reader": {
         "class_name": "huggingface_dataset_reader",
+        "data_url": "http://files.deeppavlov.ai/datasets/russian_super_glue/RCB",
+        "ignore_verifications": true,
         "name": "{TASK}",
         "path": "{COMPETITION}",
         "test": "test",
         "train": "train",
         "valid": "validation"
     },
     "metadata": {
         "download": [
             {
                 "subdir": "{MODEL_PATH}",
-                "url": "http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_terra_rubert.tar.gz"
+                "url": "http://files.deeppavlov.ai/v1/russian_super_glue/russian_superglue_rcb_rubert.tar.gz"
             }
         ],
         "variables": {
             "BASE_MODEL": "DeepPavlov/rubert-base-cased",
-            "BINARY_CLASSIFICATION": false,
             "COMPETITION": "russian_super_glue",
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "MODELS_PATH": "{ROOT_PATH}/models",
             "MODEL_PATH": "{MODELS_PATH}/{COMPETITION}/{TASK}/{BASE_MODEL}",
             "ROOT_PATH": "~/.deeppavlov",
-            "TASK": "terra"
+            "TASK": "rcb"
         }
     },
     "train": {
         "batch_size": 4,
         "class_name": "torch_trainer",
         "epochs": 10,
         "evaluation_targets": [
             "train",
             "valid"
         ],
         "log_every_n_epochs": 1,
         "metrics": [
-            "accuracy"
+            "accuracy",
+            "f1_macro"
         ],
-        "pytest_batch_size": 2,
         "pytest_max_batches": 2,
         "show_examples": false,
         "tensorboard_log_dir": "{MODEL_PATH}/",
         "val_every_n_epochs": 1,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/spelling_correction/brillmoore_wikitypos_en.json` & `deeppavlov-1.2.0/deeppavlov/configs/spelling_correction/brillmoore_wikitypos_en.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/spelling_correction/levenshtein_corrector_ru.json` & `deeppavlov-1.2.0/deeppavlov/configs/spelling_correction/levenshtein_corrector_ru.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/squad/qa_multisberquad_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/squad/squad_bert.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8324526515151515%*

 * *Differences: {"'chainer'": "{'pipe': {3: {'learning_rate_drop_patience': 2, 'batch_size': 10}}}",*

 * * "'dataset_iterator'": "{'class_name': 'squad_iterator', 'shuffle': True, delete: "*

 * *                       "['with_answer_rate']}",*

 * * "'dataset_reader'": "{'class_name': 'squad_dataset_reader', 'data_path': "*

 * *                     "'{DOWNLOADS_PATH}/squad/', delete: ['dataset', 'url']}",*

 * * "'metadata'": "{'variables': {'TRANSFORMER': 'bert-base-cased', 'MODEL_PATH': "*

 * *               "'{MODELS_PATH}/squad_torch_bert/cased/{TRAN […]*

```diff
@@ -53,24 +53,25 @@
                 "out": [
                     "ans",
                     "ans_start",
                     "ans_end"
                 ]
             },
             {
+                "batch_size": 10,
                 "class_name": "torch_transformers_squad",
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "ans_start",
                     "ans_end"
                 ],
                 "learning_rate_drop_div": 2.0,
-                "learning_rate_drop_patience": 3,
+                "learning_rate_drop_patience": 2,
                 "load_path": "{MODEL_PATH}/model",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
                     "betas": [
                         0.9,
                         0.999
                     ],
@@ -103,43 +104,40 @@
                     "ans_start_predicted",
                     "ans_end_predicted"
                 ]
             }
         ]
     },
     "dataset_iterator": {
-        "class_name": "multi_squad_retr_iterator",
+        "class_name": "squad_iterator",
         "seed": 1337,
-        "shuffle": false,
-        "with_answer_rate": 0.666
+        "shuffle": true
     },
     "dataset_reader": {
-        "class_name": "multi_squad_dataset_reader",
-        "data_path": "{DOWNLOADS_PATH}/multi_squad_ru_retr_clean/",
-        "dataset": "MultiSQuADRuRetrClean",
-        "url": "http://files.deeppavlov.ai/datasets/multi_squad_ru_retr_clean.tar.gz"
+        "class_name": "squad_dataset_reader",
+        "data_path": "{DOWNLOADS_PATH}/squad/"
     },
     "metadata": {
         "download": [
             {
                 "subdir": "{MODEL_PATH}",
-                "url": "http://files.deeppavlov.ai/v1/squad/multi_squad_ru_torch_bert_retr_noans.tar.gz"
+                "url": "http://files.deeppavlov.ai/v1/squad/squad_torch_bert_cased.tar.gz"
             }
         ],
         "variables": {
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "LOWERCASE": false,
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/multi_squad_ru_torch_bert_retr_noans/{TRANSFORMER}",
+            "MODEL_PATH": "{MODELS_PATH}/squad_torch_bert/cased/{TRANSFORMER}",
             "ROOT_PATH": "~/.deeppavlov",
-            "TRANSFORMER": "DeepPavlov/rubert-base-cased"
+            "TRANSFORMER": "bert-base-cased"
         }
     },
     "train": {
-        "batch_size": 20,
+        "batch_size": 10,
         "class_name": "torch_trainer",
         "evaluation_targets": [
             "valid"
         ],
         "log_every_n_batches": 250,
         "metrics": [
             {
@@ -167,13 +165,14 @@
                 "inputs": [
                     "ans",
                     "ans_predicted"
                 ],
                 "name": "squad_v2_em"
             }
         ],
+        "pytest_batch_size": 5,
+        "pytest_max_batches": 2,
         "show_examples": false,
         "val_every_n_batches": 500,
-        "valid_batch_size": 64,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/squad/qa_squad2_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/squad/qa_squad2_bert.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/squad/squad_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/squad/squad_ru_bert.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9005208333333334%*

 * *Differences: {"'chainer'": "{'pipe': {3: {'learning_rate_drop_patience': 3, delete: ['batch_size']}}}",*

 * * "'dataset_reader'": "{'data_path': '{DOWNLOADS_PATH}/squad_ru_clean/', 'dataset': "*

 * *                     "'SberSQuADClean', 'url': "*

 * *                     "'http://files.deeppavlov.ai/datasets/sber_squad_clean-v1.1.tar.gz'}",*

 * * "'metadata'": "{'variables': {'TRANSFORMER': 'DeepPavlov/rubert-base-cased', 'MODEL_PATH': "*

 * *               "'{MODELS_PATH}/squad_ru_torch_bert/{TRANSFORMER}'}, 'download': {0: {'url': "*

 * *        […]*

```diff
@@ -53,25 +53,24 @@
                 "out": [
                     "ans",
                     "ans_start",
                     "ans_end"
                 ]
             },
             {
-                "batch_size": 10,
                 "class_name": "torch_transformers_squad",
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "ans_start",
                     "ans_end"
                 ],
                 "learning_rate_drop_div": 2.0,
-                "learning_rate_drop_patience": 2,
+                "learning_rate_drop_patience": 3,
                 "load_path": "{MODEL_PATH}/model",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
                     "betas": [
                         0.9,
                         0.999
                     ],
@@ -110,30 +109,32 @@
     "dataset_iterator": {
         "class_name": "squad_iterator",
         "seed": 1337,
         "shuffle": true
     },
     "dataset_reader": {
         "class_name": "squad_dataset_reader",
-        "data_path": "{DOWNLOADS_PATH}/squad/"
+        "data_path": "{DOWNLOADS_PATH}/squad_ru_clean/",
+        "dataset": "SberSQuADClean",
+        "url": "http://files.deeppavlov.ai/datasets/sber_squad_clean-v1.1.tar.gz"
     },
     "metadata": {
         "download": [
             {
-                "subdir": "{MODEL_PATH}",
-                "url": "http://files.deeppavlov.ai/v1/squad/squad_torch_bert_cased.tar.gz"
+                "subdir": "{MODELS_PATH}",
+                "url": "http://files.deeppavlov.ai/v1/squad/squad_ru_torch_bert.tar.gz"
             }
         ],
         "variables": {
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
             "LOWERCASE": false,
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/squad_torch_bert/cased/{TRANSFORMER}",
+            "MODEL_PATH": "{MODELS_PATH}/squad_ru_torch_bert/{TRANSFORMER}",
             "ROOT_PATH": "~/.deeppavlov",
-            "TRANSFORMER": "bert-base-cased"
+            "TRANSFORMER": "DeepPavlov/rubert-base-cased"
         }
     },
     "train": {
         "batch_size": 10,
         "class_name": "torch_trainer",
         "evaluation_targets": [
             "valid"
@@ -165,14 +166,12 @@
                 "inputs": [
                     "ans",
                     "ans_predicted"
                 ],
                 "name": "squad_v2_em"
             }
         ],
-        "pytest_batch_size": 5,
-        "pytest_max_batches": 2,
         "show_examples": false,
         "val_every_n_batches": 500,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/configs/squad/squad_ru_bert.json` & `deeppavlov-1.2.0/deeppavlov/configs/squad/squad_ru_convers_distilrubert_2L.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9687139423076923%*

 * *Differences: {"'chainer'": "{'pipe': {0: {'do_lower_case': '{lowercase}', 'add_token_type_ids': True}, 1: "*

 * *              "{'do_lower_case': '{lowercase}'}, 2: {'do_lower_case': '{lowercase}'}, 3: "*

 * *              "{'optimizer_parameters': {'lr': 9e-05, delete: ['weight_decay', 'betas', 'eps']}, "*

 * *              "'learning_rate_drop_patience': 2, 'learning_rate_drop_div': 1.5, "*

 * *              "'attention_probs_keep_prob': 0.11, 'hidden_keep_prob': 0.33}}}",*

 * * "'metadata'": "{'variables': {'TRANSFORMER': 'DeepPavlov/distilr […]*

```diff
@@ -11,76 +11,73 @@
         "out": [
             "ans_predicted",
             "ans_start_predicted",
             "scores"
         ],
         "pipe": [
             {
+                "add_token_type_ids": true,
                 "class_name": "torch_squad_transformers_preprocessor",
-                "do_lower_case": "{LOWERCASE}",
+                "do_lower_case": "{lowercase}",
                 "in": [
                     "question_raw",
                     "context_raw"
                 ],
                 "max_seq_length": 384,
                 "out": [
                     "bert_features",
                     "subtokens",
                     "split_context"
                 ],
                 "vocab_file": "{TRANSFORMER}"
             },
             {
                 "class_name": "squad_bert_mapping",
-                "do_lower_case": "{LOWERCASE}",
+                "do_lower_case": "{lowercase}",
                 "in": [
                     "split_context",
                     "bert_features",
                     "subtokens"
                 ],
                 "out": [
                     "subtok2chars",
                     "char2subtoks"
                 ]
             },
             {
                 "class_name": "squad_bert_ans_preprocessor",
-                "do_lower_case": "{LOWERCASE}",
+                "do_lower_case": "{lowercase}",
                 "in": [
                     "ans_raw",
                     "ans_raw_start",
                     "char2subtoks"
                 ],
                 "out": [
                     "ans",
                     "ans_start",
                     "ans_end"
                 ]
             },
             {
+                "attention_probs_keep_prob": 0.11,
                 "class_name": "torch_transformers_squad",
+                "hidden_keep_prob": 0.33,
                 "in": [
                     "bert_features"
                 ],
                 "in_y": [
                     "ans_start",
                     "ans_end"
                 ],
-                "learning_rate_drop_div": 2.0,
-                "learning_rate_drop_patience": 3,
+                "learning_rate_drop_div": 1.5,
+                "learning_rate_drop_patience": 2,
                 "load_path": "{MODEL_PATH}/model",
                 "optimizer": "AdamW",
                 "optimizer_parameters": {
-                    "betas": [
-                        0.9,
-                        0.999
-                    ],
-                    "eps": 1e-06,
-                    "lr": 2e-05,
-                    "weight_decay": 0.01
+                    "lr": 9e-05
                 },
                 "out": [
                     "ans_start_predicted",
                     "ans_end_predicted",
                     "logits",
                     "scores",
                     "inds"
@@ -117,24 +114,24 @@
         "dataset": "SberSQuADClean",
         "url": "http://files.deeppavlov.ai/datasets/sber_squad_clean-v1.1.tar.gz"
     },
     "metadata": {
         "download": [
             {
                 "subdir": "{MODELS_PATH}",
-                "url": "http://files.deeppavlov.ai/v1/squad/squad_ru_torch_bert.tar.gz"
+                "url": "http://files.deeppavlov.ai/deeppavlov_data/squad_ru_convers_distilrubert_2L.tar.gz"
             }
         ],
         "variables": {
             "DOWNLOADS_PATH": "{ROOT_PATH}/downloads",
-            "LOWERCASE": false,
             "MODELS_PATH": "{ROOT_PATH}/models",
-            "MODEL_PATH": "{MODELS_PATH}/squad_ru_torch_bert/{TRANSFORMER}",
+            "MODEL_PATH": "{MODELS_PATH}/squad_ru_convers_distilrubert_2L",
             "ROOT_PATH": "~/.deeppavlov",
-            "TRANSFORMER": "DeepPavlov/rubert-base-cased"
+            "TRANSFORMER": "DeepPavlov/distilrubert-tiny-cased-conversational",
+            "lowercase": false
         }
     },
     "train": {
         "batch_size": 10,
         "class_name": "torch_trainer",
         "evaluation_targets": [
             "valid"
@@ -142,36 +139,37 @@
         "log_every_n_batches": 250,
         "metrics": [
             {
                 "inputs": [
                     "ans",
                     "ans_predicted"
                 ],
-                "name": "squad_v1_f1"
+                "name": "squad_v2_f1"
             },
             {
                 "inputs": [
                     "ans",
                     "ans_predicted"
                 ],
-                "name": "squad_v1_em"
+                "name": "squad_v2_em"
             },
             {
                 "inputs": [
                     "ans",
                     "ans_predicted"
                 ],
-                "name": "squad_v2_f1"
+                "name": "squad_v1_f1"
             },
             {
                 "inputs": [
                     "ans",
                     "ans_predicted"
                 ],
-                "name": "squad_v2_em"
+                "name": "squad_v1_em"
             }
         ],
         "show_examples": false,
+        "tensorboard_log_dir": "{MODEL_PATH}/logs",
         "val_every_n_batches": 500,
         "validation_patience": 10
     }
 }
```

### Comparing `deeppavlov-1.1.1/deeppavlov/core/commands/infer.py` & `deeppavlov-1.2.0/deeppavlov/core/commands/infer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/commands/train.py` & `deeppavlov-1.2.0/deeppavlov/core/commands/train.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/commands/utils.py` & `deeppavlov-1.2.0/deeppavlov/core/commands/utils.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/aliases.py` & `deeppavlov-1.2.0/deeppavlov/core/common/aliases.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/base.py` & `deeppavlov-1.2.0/deeppavlov/core/common/base.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/chainer.py` & `deeppavlov-1.2.0/deeppavlov/core/common/chainer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/cross_validation.py` & `deeppavlov-1.2.0/deeppavlov/core/common/cross_validation.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/errors.py` & `deeppavlov-1.2.0/deeppavlov/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/file.py` & `deeppavlov-1.2.0/deeppavlov/core/common/file.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/log.py` & `deeppavlov-1.2.0/deeppavlov/core/common/log.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/log_events.py` & `deeppavlov-1.2.0/deeppavlov/core/common/log_events.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/metrics_registry.json` & `deeppavlov-1.2.0/deeppavlov/core/common/metrics_registry.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/metrics_registry.py` & `deeppavlov-1.2.0/deeppavlov/core/common/metrics_registry.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/params.py` & `deeppavlov-1.2.0/deeppavlov/core/common/params.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/params_search.py` & `deeppavlov-1.2.0/deeppavlov/core/common/params_search.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/paths.py` & `deeppavlov-1.2.0/deeppavlov/core/common/paths.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/prints.py` & `deeppavlov-1.2.0/deeppavlov/core/common/prints.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/registry.json` & `deeppavlov-1.2.0/deeppavlov/core/common/registry.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9353448275862069%*

 * *Differences: {"'entity_type_split'": "'deeppavlov.models.entity_extraction.entity_detection_parser:entity_type_split'",*

 * * "'lcquad_reader'": "'deeppavlov.dataset_readers.sq_reader:LCQuADReader'",*

 * * "'path_ranking_preprocessor'": "'deeppavlov.models.preprocessors.torch_transformers_preprocessor:PathRankingPreprocessor'",*

 * * "'query_formatter'": "'deeppavlov.models.kbqa.query_generator:QueryFormatter'",*

 * * "'question_sign_checker'": "'deeppavlov.models.entity_extraction.entity_detection_parser:QuestionSignChecker'",*

 * * "'ru_adj_t […]*

```diff
@@ -10,22 +10,24 @@
     "data_fitting_iterator": "deeppavlov.core.data.data_fitting_iterator:DataFittingIterator",
     "data_learning_iterator": "deeppavlov.core.data.data_learning_iterator:DataLearningIterator",
     "dirty_comments_preprocessor": "deeppavlov.models.preprocessors.dirty_comments_preprocessor:DirtyCommentsPreprocessor",
     "docred_reader": "deeppavlov.dataset_readers.docred_reader:DocREDDatasetReader",
     "document_chunker": "deeppavlov.models.preprocessors.odqa_preprocessors:DocumentChunker",
     "entity_detection_parser": "deeppavlov.models.entity_extraction.entity_detection_parser:EntityDetectionParser",
     "entity_linker": "deeppavlov.models.entity_extraction.entity_linking:EntityLinker",
+    "entity_type_split": "deeppavlov.models.entity_extraction.entity_detection_parser:entity_type_split",
     "faq_reader": "deeppavlov.dataset_readers.faq_reader:FaqDatasetReader",
     "fasttext": "deeppavlov.models.embedders.fasttext_embedder:FasttextEmbedder",
     "fit_trainer": "deeppavlov.core.trainers.fit_trainer:FitTrainer",
     "hashing_tfidf_vectorizer": "deeppavlov.models.vectorizers.hashing_tfidf_vectorizer:HashingTfIdfVectorizer",
     "huggingface_dataset_iterator": "deeppavlov.dataset_iterators.huggingface_dataset_iterator:HuggingFaceDatasetIterator",
     "huggingface_dataset_reader": "deeppavlov.dataset_readers.huggingface_dataset_reader:HuggingFaceDatasetReader",
     "imdb_reader": "deeppavlov.dataset_readers.imdb_reader:ImdbReader",
     "kenlm_elector": "deeppavlov.models.spelling_correction.electors.kenlm_elector:KenlmElector",
+    "lcquad_reader": "deeppavlov.dataset_readers.sq_reader:LCQuADReader",
     "line_reader": "deeppavlov.dataset_readers.line_reader:LineReader",
     "logit_ranker": "deeppavlov.models.doc_retrieval.logit_ranker:LogitRanker",
     "mask": "deeppavlov.models.preprocessors.mask:Mask",
     "multi_squad_dataset_reader": "deeppavlov.dataset_readers.squad_dataset_reader:MultiSquadDatasetReader",
     "multi_squad_iterator": "deeppavlov.dataset_iterators.squad_iterator:MultiSquadIterator",
     "multi_squad_retr_iterator": "deeppavlov.dataset_iterators.squad_iterator:MultiSquadRetrIterator",
     "multitask_iterator": "deeppavlov.dataset_iterators.multitask_iterator:MultiTaskIterator",
@@ -38,38 +40,41 @@
     "nltk_moses_tokenizer": "deeppavlov.models.tokenizers.nltk_moses_tokenizer:NLTKMosesTokenizer",
     "nltk_tokenizer": "deeppavlov.models.tokenizers.nltk_tokenizer:NLTKTokenizer",
     "nn_trainer": "deeppavlov.core.trainers.nn_trainer:NNTrainer",
     "odqa_reader": "deeppavlov.dataset_readers.odqa_reader:ODQADataReader",
     "one_hotter": "deeppavlov.models.preprocessors.one_hotter:OneHotter",
     "params_search": "deeppavlov.core.common.params_search:ParamsSearch",
     "paraphraser_reader": "deeppavlov.dataset_readers.paraphraser_reader:ParaphraserReader",
+    "path_ranking_preprocessor": "deeppavlov.models.preprocessors.torch_transformers_preprocessor:PathRankingPreprocessor",
     "pop_ranker": "deeppavlov.models.doc_retrieval.pop_ranker:PopRanker",
     "proba2labels": "deeppavlov.models.classifiers.proba2labels:Proba2Labels",
+    "query_formatter": "deeppavlov.models.kbqa.query_generator:QueryFormatter",
     "query_generator": "deeppavlov.models.kbqa.query_generator:QueryGenerator",
-    "question_sign_checker": "deeppavlov.models.entity_extraction.entity_detection_parser:question_sign_checker",
+    "question_sign_checker": "deeppavlov.models.entity_extraction.entity_detection_parser:QuestionSignChecker",
     "re_classifier": "deeppavlov.models.relation_extraction.relation_extraction_bert:REBertModel",
     "re_postprocessor": "deeppavlov.models.preprocessors.re_preprocessor:REPostprocessor",
     "re_preprocessor": "deeppavlov.models.preprocessors.re_preprocessor:REPreprocessor",
     "rel_ranking_infer": "deeppavlov.models.kbqa.rel_ranking_infer:RelRankerInfer",
     "rel_ranking_preprocessor": "deeppavlov.models.preprocessors.torch_transformers_preprocessor:RelRankingPreprocessor",
     "rel_ranking_reader": "deeppavlov.dataset_readers.rel_ranking_reader:ParaphraserReader",
     "response_base_loader": "deeppavlov.models.preprocessors.response_base_loader:ResponseBaseLoader",
-    "ru_adj_to_noun": "deeppavlov.models.kbqa.tree_to_sparql:RuAdjToNoun",
+    "ru_adj_to_noun": "deeppavlov.models.kbqa.ru_adj_to_noun:RuAdjToNoun",
+    "rubq_reader": "deeppavlov.dataset_readers.sq_reader:RuBQReader",
     "rured_reader": "deeppavlov.dataset_readers.rured_reader:RuREDDatasetReader",
     "russian_words_vocab": "deeppavlov.vocabs.typos:RussianWordsVocab",
     "sanitizer": "deeppavlov.models.preprocessors.sanitizer:Sanitizer",
     "sentseg_restore_sent": "deeppavlov.models.preprocessors.sentseg_preprocessor:SentSegRestoreSent",
     "siamese_iterator": "deeppavlov.dataset_iterators.siamese_iterator:SiameseIterator",
     "simple_vocab": "deeppavlov.core.data.simple_vocab:SimpleVocabulary",
     "sklearn_component": "deeppavlov.models.sklearn.sklearn_component:SklearnComponent",
     "slovnet_syntax_parser": "deeppavlov.models.kbqa.tree_to_sparql:SlovnetSyntaxParser",
     "spelling_error_model": "deeppavlov.models.spelling_correction.brillmoore.error_model:ErrorModel",
     "spelling_levenshtein": "deeppavlov.models.spelling_correction.levenshtein.searcher_component:LevenshteinSearcherComponent",
     "split_tokenizer": "deeppavlov.models.tokenizers.split_tokenizer:SplitTokenizer",
-    "sq_reader": "deeppavlov.dataset_readers.sq_reader:OntonotesReader",
+    "sq_reader": "deeppavlov.dataset_readers.sq_reader:SQReader",
     "sqlite_iterator": "deeppavlov.dataset_iterators.sqlite_iterator:SQLiteDataIterator",
     "squad_bert_ans_postprocessor": "deeppavlov.models.preprocessors.squad_preprocessor:SquadBertAnsPostprocessor",
     "squad_bert_ans_preprocessor": "deeppavlov.models.preprocessors.squad_preprocessor:SquadBertAnsPreprocessor",
     "squad_bert_mapping": "deeppavlov.models.preprocessors.squad_preprocessor:SquadBertMappingPreprocessor",
     "squad_dataset_reader": "deeppavlov.dataset_readers.squad_dataset_reader:SquadDatasetReader",
     "squad_iterator": "deeppavlov.dataset_iterators.squad_iterator:SquadIterator",
     "static_dictionary": "deeppavlov.vocabs.typos:StaticDictionary",
@@ -91,14 +96,15 @@
     "torch_transformers_classifier": "deeppavlov.models.torch_bert.torch_transformers_classifier:TorchTransformersClassifierModel",
     "torch_transformers_el_ranker": "deeppavlov.models.torch_bert.torch_transformers_el_ranker:TorchTransformersElRanker",
     "torch_transformers_entity_ranker_infer": "deeppavlov.models.torch_bert.torch_transformers_el_ranker:TorchTransformersEntityRankerInfer",
     "torch_transformers_entity_ranker_preprocessor": "deeppavlov.models.preprocessors.torch_transformers_preprocessor:TorchTransformersEntityRankerPreprocessor",
     "torch_transformers_multiplechoice": "deeppavlov.models.torch_bert.torch_transformers_multiplechoice:TorchTransformersMultiplechoiceModel",
     "torch_transformers_multiplechoice_preprocessor": "deeppavlov.models.preprocessors.torch_transformers_preprocessor:TorchTransformersMultiplechoicePreprocessor",
     "torch_transformers_ner_preprocessor": "deeppavlov.models.preprocessors.torch_transformers_preprocessor:TorchTransformersNerPreprocessor",
+    "torch_transformers_nll_ranker": "deeppavlov.models.torch_bert.torch_transformers_nll_ranking:TorchTransformersNLLRanker",
     "torch_transformers_preprocessor": "deeppavlov.models.preprocessors.torch_transformers_preprocessor:TorchTransformersPreprocessor",
     "torch_transformers_sequence_tagger": "deeppavlov.models.torch_bert.torch_transformers_sequence_tagger:TorchTransformersSequenceTagger",
     "torch_transformers_squad": "deeppavlov.models.torch_bert.torch_transformers_squad:TorchTransformersSquad",
     "transformers_bert_embedder": "deeppavlov.models.embedders.transformers_embedder:TransformersBertEmbedder",
     "transformers_bert_preprocessor": "deeppavlov.models.preprocessors.transformers_preprocessor:TransformersBertPreprocessor",
     "tree_to_sparql": "deeppavlov.models.kbqa.tree_to_sparql:TreeToSparql",
     "typos_custom_reader": "deeppavlov.dataset_readers.typos_reader:TyposCustom",
```

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/registry.py` & `deeppavlov-1.2.0/deeppavlov/core/common/registry.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/common/requirements_registry.json` & `deeppavlov-1.2.0/deeppavlov/core/common/requirements_registry.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9421768707482994%*

 * *Differences: {"'path_ranking_preprocessor'": "['{DEEPPAVLOV_PATH}/requirements/pytorch.txt', "*

 * *                                "'{DEEPPAVLOV_PATH}/requirements/transformers.txt']",*

 * * "'ru_adj_to_noun'": '{delete: [1]}',*

 * * "'slovnet_syntax_parser'": "{insert: [(1, '{DEEPPAVLOV_PATH}/requirements/razdel.txt'), (2, "*

 * *                            "'{DEEPPAVLOV_PATH}/requirements/ru_core_news_sm.txt')]}",*

 * * "'torch_transformers_nll_ranker'": "['{DEEPPAVLOV_PATH}/requirements/pytorch.txt', "*

 * *                                    "' […]*

```diff
@@ -37,14 +37,18 @@
     "ner_chunker": [
         "{DEEPPAVLOV_PATH}/requirements/pytorch.txt",
         "{DEEPPAVLOV_PATH}/requirements/transformers.txt"
     ],
     "nltk_moses_tokenizer": [
         "{DEEPPAVLOV_PATH}/requirements/sacremoses.txt"
     ],
+    "path_ranking_preprocessor": [
+        "{DEEPPAVLOV_PATH}/requirements/pytorch.txt",
+        "{DEEPPAVLOV_PATH}/requirements/transformers.txt"
+    ],
     "query_generator": [
         "{DEEPPAVLOV_PATH}/requirements/en_core_web_sm.txt",
         "{DEEPPAVLOV_PATH}/requirements/hdt.txt",
         "{DEEPPAVLOV_PATH}/requirements/rapidfuzz.txt",
         "{DEEPPAVLOV_PATH}/requirements/whapi.txt"
     ],
     "re_classifier": [
@@ -65,22 +69,23 @@
         "{DEEPPAVLOV_PATH}/requirements/hdt.txt"
     ],
     "rel_ranking_preprocessor": [
         "{DEEPPAVLOV_PATH}/requirements/pytorch.txt",
         "{DEEPPAVLOV_PATH}/requirements/transformers.txt"
     ],
     "ru_adj_to_noun": [
-        "{DEEPPAVLOV_PATH}/requirements/ru_core_news_sm.txt",
-        "{DEEPPAVLOV_PATH}/requirements/udapi.txt"
+        "{DEEPPAVLOV_PATH}/requirements/ru_core_news_sm.txt"
     ],
     "russian_words_vocab": [
         "{DEEPPAVLOV_PATH}/requirements/lxml.txt"
     ],
     "slovnet_syntax_parser": [
-        "{DEEPPAVLOV_PATH}/requirements/slovnet.txt"
+        "{DEEPPAVLOV_PATH}/requirements/slovnet.txt",
+        "{DEEPPAVLOV_PATH}/requirements/razdel.txt",
+        "{DEEPPAVLOV_PATH}/requirements/ru_core_news_sm.txt"
     ],
     "spelling_error_model": [
         "{DEEPPAVLOV_PATH}/requirements/lxml.txt"
     ],
     "spelling_levenshtein": [
         "{DEEPPAVLOV_PATH}/requirements/sortedcontainers.txt"
     ],
@@ -134,14 +139,18 @@
         "{DEEPPAVLOV_PATH}/requirements/pytorch.txt",
         "{DEEPPAVLOV_PATH}/requirements/transformers.txt"
     ],
     "torch_transformers_ner_preprocessor": [
         "{DEEPPAVLOV_PATH}/requirements/pytorch.txt",
         "{DEEPPAVLOV_PATH}/requirements/transformers.txt"
     ],
+    "torch_transformers_nll_ranker": [
+        "{DEEPPAVLOV_PATH}/requirements/pytorch.txt",
+        "{DEEPPAVLOV_PATH}/requirements/transformers.txt"
+    ],
     "torch_transformers_preprocessor": [
         "{DEEPPAVLOV_PATH}/requirements/pytorch.txt",
         "{DEEPPAVLOV_PATH}/requirements/transformers.txt"
     ],
     "torch_transformers_sequence_tagger": [
         "{DEEPPAVLOV_PATH}/requirements/pytorch.txt",
         "{DEEPPAVLOV_PATH}/requirements/torchcrf.txt",
@@ -157,15 +166,15 @@
     ],
     "transformers_bert_preprocessor": [
         "{DEEPPAVLOV_PATH}/requirements/pytorch.txt",
         "{DEEPPAVLOV_PATH}/requirements/transformers.txt"
     ],
     "tree_to_sparql": [
         "{DEEPPAVLOV_PATH}/requirements/udapi.txt",
-        "{DEEPPAVLOV_PATH}/requirements/en_core_web_sm.txt",
+        "{DEEPPAVLOV_PATH}/requirements/razdel.txt",
         "{DEEPPAVLOV_PATH}/requirements/ru_core_news_sm.txt"
     ],
     "typos_custom_reader": [
         "{DEEPPAVLOV_PATH}/requirements/lxml.txt"
     ],
     "typos_kartaslov_reader": [
         "{DEEPPAVLOV_PATH}/requirements/lxml.txt"
```

### Comparing `deeppavlov-1.1.1/deeppavlov/core/data/data_fitting_iterator.py` & `deeppavlov-1.2.0/deeppavlov/core/data/data_fitting_iterator.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/data/data_learning_iterator.py` & `deeppavlov-1.2.0/deeppavlov/core/data/data_learning_iterator.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/data/dataset_reader.py` & `deeppavlov-1.2.0/deeppavlov/core/data/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/data/simple_vocab.py` & `deeppavlov-1.2.0/deeppavlov/core/data/simple_vocab.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/data/utils.py` & `deeppavlov-1.2.0/deeppavlov/core/data/utils.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/models/component.py` & `deeppavlov-1.2.0/deeppavlov/core/models/component.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/models/estimator.py` & `deeppavlov-1.2.0/deeppavlov/core/models/estimator.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/models/lr_scheduled_model.py` & `deeppavlov-1.2.0/deeppavlov/core/models/lr_scheduled_model.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/models/nn_model.py` & `deeppavlov-1.2.0/deeppavlov/core/models/nn_model.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/models/serializable.py` & `deeppavlov-1.2.0/deeppavlov/core/models/serializable.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/models/torch_model.py` & `deeppavlov-1.2.0/deeppavlov/core/models/torch_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from abc import abstractmethod
 from copy import deepcopy
 from logging import getLogger
 from pathlib import Path
 from typing import Optional
 
 import torch
-from overrides import overrides
 
 from deeppavlov.core.common.errors import ConfigError
 from deeppavlov.core.models.nn_model import NNModel
 
 log = getLogger(__name__)
 
 
@@ -126,15 +125,14 @@
         else:
             raise AttributeError("Model is not defined.")
 
     @property
     def is_data_parallel(self) -> bool:
         return isinstance(self.model, torch.nn.DataParallel)
 
-    @overrides
     def load(self, fname: Optional[str] = None, *args, **kwargs) -> None:
         """Load model from `fname` (if `fname` is not given, use `self.load_path`) to `self.model` along with
             the optimizer `self.optimizer`, optionally `self.lr_scheduler`.
             If `fname` (if `fname` is not given, use `self.load_path`) does not exist, initialize model from scratch.
 
         Args:
             fname: string path to checkpoint
@@ -183,15 +181,14 @@
             elif model_func:
                 log.debug(f"Init from scratch. Load path {weights_path} does not exist.")
                 self.init_from_opt(model_func)
         elif model_func:
             log.debug(f"Init from scratch. Load path {self.load_path} is not provided.")
             self.init_from_opt(model_func)
 
-    @overrides
     def save(self, fname: Optional[str] = None, *args, **kwargs) -> None:
         """Save torch model to `fname` (if `fname` is not given, use `self.save_path`). Checkpoint includes
             `model_state_dict`, `optimizer_state_dict`, and `epochs_done` (number of training epochs).
 
         Args:
             fname:
             *args:
@@ -220,15 +217,14 @@
                 "model_state_dict": self.model.cpu().state_dict(),
                 "optimizer_state_dict": self.optimizer.state_dict(),
                 "epochs_done": self.epochs_done
             }, weights_path)
         # return it back to device (necessary if it was on `cuda`)
         self.model.to(self.device)
 
-    @overrides
     def process_event(self, event_name: str, data: dict) -> None:
         """Process event. After epoch, increase `self.epochs_done`. After validation, decrease learning rate in
             `self.learning_rate_drop_div` times (not lower than `self.min_learning_rate`)
             if given `self.learning_rate_drop_patience`.
 
         Args:
             event_name: whether event is send after epoch or batch.
```

### Comparing `deeppavlov-1.1.1/deeppavlov/core/trainers/__init__.py` & `deeppavlov-1.2.0/deeppavlov/core/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/trainers/fit_trainer.py` & `deeppavlov-1.2.0/deeppavlov/core/trainers/fit_trainer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/trainers/nn_trainer.py` & `deeppavlov-1.2.0/deeppavlov/core/trainers/nn_trainer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/trainers/torch_trainer.py` & `deeppavlov-1.2.0/deeppavlov/core/trainers/torch_trainer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/core/trainers/utils.py` & `deeppavlov-1.2.0/deeppavlov/core/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_iterators/basic_classification_iterator.py` & `deeppavlov-1.2.0/deeppavlov/dataset_iterators/basic_classification_iterator.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_iterators/huggingface_dataset_iterator.py` & `deeppavlov-1.2.0/deeppavlov/dataset_iterators/huggingface_dataset_iterator.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_iterators/multitask_iterator.py` & `deeppavlov-1.2.0/deeppavlov/dataset_iterators/multitask_iterator.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_iterators/siamese_iterator.py` & `deeppavlov-1.2.0/deeppavlov/dataset_iterators/siamese_iterator.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_iterators/sqlite_iterator.py` & `deeppavlov-1.2.0/deeppavlov/dataset_iterators/sqlite_iterator.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 import sqlite3
 from logging import getLogger
 from pathlib import Path
 from random import Random
 from typing import List, Any, Dict, Optional, Union, Generator, Tuple
 
-from overrides import overrides
-
 from deeppavlov.core.commands.utils import expand_path
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.data.data_fitting_iterator import DataFittingIterator
 
 logger = getLogger(__name__)
 
 
@@ -69,15 +67,14 @@
             raise e
         self.doc_ids = self.get_doc_ids()
         self.doc2index = self.map_doc2idx()
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.random = Random(seed)
 
-    @overrides
     def get_doc_ids(self) -> List[Any]:
         """Get document ids.
 
         Returns:
             document ids
         """
         cursor = self.connect.cursor()
@@ -108,15 +105,14 @@
 
         """
         doc2idx = {doc_id: i for i, doc_id in enumerate(self.doc_ids)}
         logger.info(
             "SQLite iterator: The size of the database is {} documents".format(len(doc2idx)))
         return doc2idx
 
-    @overrides
     def get_doc_content(self, doc_id: Any) -> Optional[str]:
         """Get document content by id.
 
         Args:
             doc_id: a document id
 
         Returns:
@@ -128,15 +124,14 @@
             "SELECT text FROM {} WHERE id = ?".format(self.db_name),
             (doc_id,)
         )
         result = cursor.fetchone()
         cursor.close()
         return result if result is None else result[0]
 
-    @overrides
     def gen_batches(self, batch_size: int, shuffle: bool = None) \
             -> Generator[Tuple[List[str], List[int]], Any, None]:
         """Gen batches of documents.
 
         Args:
             batch_size: a number of samples in a single batch
             shuffle: whether to shuffle data during batching
```

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_iterators/squad_iterator.py` & `deeppavlov-1.2.0/deeppavlov/dataset_iterators/squad_iterator.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_iterators/typos_iterator.py` & `deeppavlov-1.2.0/deeppavlov/dataset_iterators/typos_iterator.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/basic_classification_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/basic_classification_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,28 @@
 # limitations under the License.
 
 
 from logging import getLogger
 from pathlib import Path
 
 import pandas as pd
-from overrides import overrides
 
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.data.dataset_reader import DatasetReader
 from deeppavlov.core.data.utils import download
 
 log = getLogger(__name__)
 
 
 @register('basic_classification_reader')
 class BasicClassificationDatasetReader(DatasetReader):
     """
     Class provides reading dataset in .csv format
     """
 
-    @overrides
     def read(self, data_path: str, url: str = None,
              format: str = "csv", class_sep: str = None,
              *args, **kwargs) -> dict:
         """
         Read dataset from data_path directory.
         Reading files are all data_types + extension
         (i.e for data_types=["train", "valid"] files "train.csv" and "valid.csv" form
```

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/boolqa_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/boolqa_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/conll2003_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/conll2003_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/docred_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/docred_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,28 +18,26 @@
 import random
 from logging import getLogger
 from pathlib import Path
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from overrides import overrides
 
 from deeppavlov.core.commands.utils import expand_path
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.data.dataset_reader import DatasetReader
 
 logger = getLogger(__name__)
 
 
 @register('docred_reader')
 class DocREDDatasetReader(DatasetReader):
     """ Class to read the datasets in DocRED format"""
 
-    @overrides
     def read(
             self,
             data_path: str,
             rel2id_path: str,
             rel_info_path: str,
             negative_label: str = "Na",
             train_valid_test_proportion: int = None,
```

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/faq_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/faq_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/huggingface_dataset_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/huggingface_dataset_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 
 import re
 from collections import Counter
 from math import floor
 from typing import Dict, Optional, List, Union
 
 from datasets import load_dataset, Dataset, Features, ClassLabel, concatenate_datasets
-from overrides import overrides
 
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.data.dataset_reader import DatasetReader
 
 
 @register('huggingface_dataset_reader')
 class HuggingFaceDatasetReader(DatasetReader):
     """Adds HuggingFace Datasets https://huggingface.co/datasets/ to DeepPavlov
     """
 
-    @overrides
     def read(self,
              path: str,
              name: Optional[str] = None,
              train: Optional[str] = None,  # for lidirus with no train
              valid: Optional[str] = None,
              test: Optional[str] = None,
              **kwargs) -> Dict[str, Dataset]:
```

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/imdb_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/imdb_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # limitations under the License.
 
 
 from logging import getLogger
 from typing import List, Dict, Any, Optional, Tuple
 from pathlib import Path
 
-from overrides import overrides
-
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.data.dataset_reader import DatasetReader
 from deeppavlov.core.data.utils import download_decompress, mark_done, is_done
 
 log = getLogger(__name__)
 
 
@@ -31,15 +29,14 @@
     https://ai.stanford.edu/~amaas/data/sentiment/
 
     Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts.
     (2011). Learning Word Vectors for Sentiment Analysis. The 49th Annual Meeting of the Association
     for Computational Linguistics (ACL 2011).
     """
 
-    @overrides
     def read(self, data_path: str, url: Optional[str] = None,
              *args, **kwargs) -> Dict[str, List[Tuple[Any, Any]]]:
         """
         Args:
             data_path: A path to a folder with dataset files.
             url: A url to the archive with the dataset to download if the data folder is empty.
         """
```

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/line_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/line_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/multitask_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/multitask_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/odqa_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/odqa_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/paraphraser_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/paraphraser_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/rel_ranking_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/rel_ranking_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/rured_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/rured_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import json
 import os
 import random
 from typing import Dict, List, Tuple
 from pathlib import Path
 from logging import getLogger
-from overrides import overrides
 
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.data.dataset_reader import DatasetReader
 
 logger = getLogger(__name__)
 
 
 @register('rured_reader')
 class RuREDDatasetReader(DatasetReader):
     """ Class to read the datasets in RuRED format"""
 
-    @overrides
     def read(self, data_path: str, rel2id: Dict = None) -> Dict[str, List[Tuple]]:
         """
         This class processes the RuRED relation extraction dataset
         (http://www.dialog-21.ru/media/5093/gordeevdiplusetal-031.pdf).
         Args:
             data_path: a path to a folder with dataset files.
             rel2id: a path to a file where information about relation to relation id corresponding is stored.
```

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/squad_dataset_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/squad_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/typos_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/typos_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/dataset_readers/ubuntu_v2_reader.py` & `deeppavlov-1.2.0/deeppavlov/dataset_readers/ubuntu_v2_reader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/deep.py` & `deeppavlov-1.2.0/deeppavlov/deep.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,26 +16,25 @@
 from logging import getLogger
 
 from deeppavlov.core.commands.infer import interact_model, predict_on_stream
 from deeppavlov.core.commands.train import train_evaluate_model_from_config
 from deeppavlov.core.common.cross_validation import calc_cv_score
 from deeppavlov.core.common.file import find_config
 from deeppavlov.download import deep_download
-from deeppavlov.utils.agent import start_rabbit_service
 from deeppavlov.utils.pip_wrapper import install_from_config
 from deeppavlov.utils.server import start_model_server
 from deeppavlov.utils.socket import start_socket_server
 
 log = getLogger(__name__)
 
 parser = argparse.ArgumentParser()
 
 parser.add_argument("mode", help="select a mode, train or interact", type=str,
-                    choices={'train', 'evaluate', 'interact', 'predict', 'riseapi', 'risesocket', 'agent-rabbit',
-                             'download', 'install', 'crossval'})
+                    choices={'train', 'evaluate', 'interact', 'predict', 'riseapi', 'risesocket', 'download', 'install',
+                             'crossval'})
 parser.add_argument("config_path", help="path to a pipeline json config", type=str)
 
 parser.add_argument("-e", "--start-epoch-num", dest="start_epoch_num", default=None,
                     help="Start epoch number", type=int)
 parser.add_argument("--recursive", action="store_true", help="Train nested configs")
 
 parser.add_argument("-b", "--batch-size", dest="batch_size", default=None, help="inference batch size", type=int)
@@ -50,23 +49,14 @@
 parser.add_argument("--cert", default=None, help="ssl certificate", type=str)
 
 parser.add_argument("-p", "--port", default=None, help="api port", type=int)
 
 parser.add_argument("--socket-type", default="TCP", type=str, choices={"TCP", "UNIX"})
 parser.add_argument("--socket-file", default="/tmp/deeppavlov_socket.s", type=str)
 
-parser.add_argument("-sn", "--service-name", default=None, help="service name for agent-rabbit mode", type=str)
-parser.add_argument("-an", "--agent-namespace", default=None, help="dp-agent namespace name", type=str)
-parser.add_argument("-ul", "--utterance-lifetime", default=None, help="message expiration in seconds", type=int)
-parser.add_argument("-rh", "--rabbit-host", default=None, help="RabbitMQ server host", type=str)
-parser.add_argument("-rp", "--rabbit-port", default=None, help="RabbitMQ server port", type=int)
-parser.add_argument("-rl", "--rabbit-login", default=None, help="RabbitMQ server login", type=str)
-parser.add_argument("-rpwd", "--rabbit-password", default=None, help="RabbitMQ server password", type=str)
-parser.add_argument("-rvh", "--rabbit-virtualhost", default=None, help="RabbitMQ server virtualhost", type=str)
-
 
 def main():
     args = parser.parse_args()
     pipeline_config_path = find_config(args.config_path)
 
     if args.install or args.mode == 'install':
         install_from_config(pipeline_config_path)
@@ -81,25 +71,14 @@
         train_evaluate_model_from_config(pipeline_config_path, to_train=False, start_epoch_num=args.start_epoch_num)
     elif args.mode == 'interact':
         interact_model(pipeline_config_path)
     elif args.mode == 'riseapi':
         start_model_server(pipeline_config_path, args.https, args.key, args.cert, port=args.port)
     elif args.mode == 'risesocket':
         start_socket_server(pipeline_config_path, args.socket_type, port=args.port, socket_file=args.socket_file)
-    elif args.mode == 'agent-rabbit':
-        start_rabbit_service(model_config=pipeline_config_path,
-                             service_name=args.service_name,
-                             agent_namespace=args.agent_namespace,
-                             batch_size=args.batch_size,
-                             utterance_lifetime_sec=args.utterance_lifetime,
-                             rabbit_host=args.rabbit_host,
-                             rabbit_port=args.rabbit_port,
-                             rabbit_login=args.rabbit_login,
-                             rabbit_password=args.rabbit_password,
-                             rabbit_virtualhost=args.rabbit_virtualhost)
     elif args.mode == 'predict':
         predict_on_stream(pipeline_config_path, args.batch_size, args.file_path)
     elif args.mode == 'crossval':
         if args.folds < 2:
             log.error('Minimum number of Folds is 2')
         else:
             calc_cv_score(pipeline_config_path, n_folds=args.folds, is_loo=False)
```

### Comparing `deeppavlov-1.1.1/deeppavlov/download.py` & `deeppavlov-1.2.0/deeppavlov/download.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/accuracy.py` & `deeppavlov-1.2.0/deeppavlov/metrics/accuracy.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import itertools
-from typing import List, Iterable
+import re
+from logging import getLogger
+from typing import List
 
 import numpy as np
 
 from deeppavlov.core.common.metrics_registry import register_metric
 
+log = getLogger(__name__)
+
 
 @register_metric('accuracy')
 def accuracy(y_true: [list, np.ndarray], y_predicted: [list, np.ndarray]) -> float:
     """
     Calculate accuracy in terms of absolute coincidence
 
     Args:
@@ -43,14 +47,39 @@
         return answer
 
     equalities = [_are_equal(y1, y2) for y1, y2 in zip(y_true, y_predicted)]
     correct = sum(equalities)
     return correct / examples_len if examples_len else 0
 
 
+@register_metric('kbqa_accuracy')
+def kbqa_accuracy(questions_batch, pred_answer_labels_batch, pred_answer_ids_batch, pred_query_batch,
+                  gold_answer_labels_batch, gold_answer_ids_batch, gold_query_batch) -> float:
+    num_samples = len(pred_answer_ids_batch)
+    correct = 0
+    for question, pred_answer_label, pred_answer_ids, pred_query, gold_answer_labels, gold_answer_ids, gold_query in \
+            zip(questions_batch, pred_answer_labels_batch, pred_answer_ids_batch, pred_query_batch,
+                gold_answer_labels_batch, gold_answer_ids_batch, gold_query_batch):
+        found_date = False
+        if pred_answer_ids and gold_answer_ids and re.findall(r"[\d]{3,4}", pred_answer_ids[0]) and \
+                re.findall(r"[\d]{3,4}", pred_answer_ids[0]) == re.findall(r"[\d]{3,4}", gold_answer_ids[0]):
+            found_date = True
+        found_label = False
+        if len(gold_answer_labels) == 1 and len(pred_answer_label) > 1 and pred_answer_label == gold_answer_labels[0]:
+            found_label = True
+        no_answer = False
+        if pred_answer_label == "Not Found" and not gold_answer_ids:
+            no_answer = True
+        if set(pred_answer_ids) == set(gold_answer_ids) or gold_query in pred_query or found_date or found_label \
+                or no_answer:
+            correct += 1
+        log.debug(f"question: {question} -- gold_answer_ids: {gold_answer_ids} -- pred_answer_ids: {pred_answer_ids}")
+    return correct / num_samples if num_samples else 0
+
+
 @register_metric('multitask_accuracy')
 def multitask_accuracy(*args) -> float:
     """
     Accuracy for multiple simultaneous tasks.
 
     Args:
         *args: a list of `2n` inputs. The first `n` inputs are the correct answers for `n` tasks,
@@ -174,17 +203,7 @@
     if isinstance(y_predicted[0], np.ndarray):
         predictions = [np.round(x) for x in y_predicted]
     else:
         predictions = [round(x) for x in y_predicted]
     examples_len = len(y_true)
     correct = sum([y1 == y2 for y1, y2 in zip(y_true, predictions)])
     return correct / examples_len if examples_len else 0
-
-
-@register_metric('kbqa_accuracy')
-def kbqa_accuracy(y_true, y_predicted):
-    total_correct = 0
-    for answer_true, answer_predicted in zip(y_true, y_predicted):
-        if answer_predicted in answer_true:
-            total_correct += 1
-
-    return total_correct / len(y_true) if len(y_true) else 0
```

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/bleu.py` & `deeppavlov-1.2.0/deeppavlov/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/correlation.py` & `deeppavlov-1.2.0/deeppavlov/metrics/correlation.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/elmo_metrics.py` & `deeppavlov-1.2.0/deeppavlov/metrics/elmo_metrics.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/fmeasure.py` & `deeppavlov-1.2.0/deeppavlov/metrics/fmeasure.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/google_bleu.py` & `deeppavlov-1.2.0/deeppavlov/metrics/google_bleu.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/log_loss.py` & `deeppavlov-1.2.0/deeppavlov/metrics/log_loss.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/mse.py` & `deeppavlov-1.2.0/deeppavlov/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/recall_at_k.py` & `deeppavlov-1.2.0/deeppavlov/metrics/recall_at_k.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/record_metrics.py` & `deeppavlov-1.2.0/deeppavlov/metrics/record_metrics.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/roc_auc_score.py` & `deeppavlov-1.2.0/deeppavlov/metrics/roc_auc_score.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/metrics/squad_metrics.py` & `deeppavlov-1.2.0/deeppavlov/metrics/squad_metrics.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/__init__.py` & `deeppavlov-1.2.0/deeppavlov/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/api_requester/api_requester.py` & `deeppavlov-1.2.0/deeppavlov/models/api_requester/api_requester.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/api_requester/api_router.py` & `deeppavlov-1.2.0/deeppavlov/models/api_requester/api_router.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/classifiers/cos_sim_classifier.py` & `deeppavlov-1.2.0/deeppavlov/models/classifiers/cos_sim_classifier.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/classifiers/proba2labels.py` & `deeppavlov-1.2.0/deeppavlov/models/classifiers/proba2labels.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/classifiers/re_bert.py` & `deeppavlov-1.2.0/deeppavlov/models/classifiers/re_bert.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/classifiers/torch_classification_model.py` & `deeppavlov-1.2.0/deeppavlov/models/classifiers/torch_classification_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-from overrides import overrides
 from typing import List, Union, Optional
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 from deeppavlov.core.common.errors import ConfigError
@@ -129,15 +128,14 @@
 
         outputs = outputs.cpu().detach().numpy()
         if self.opt["return_probas"]:
             return outputs.tolist()
         else:
             return np.argmax(outputs, axis=-1).tolist()
 
-    @overrides
     def process_event(self, event_name: str, data: dict):
         """Process event after epoch
 
         Args:
             event_name: whether event is send after epoch or batch.
                     Set of values: ``"after_epoch", "after_batch"``
             data: event data (dictionary)
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/classifiers/torch_nets.py` & `deeppavlov-1.2.0/deeppavlov/models/classifiers/torch_nets.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/classifiers/utils.py` & `deeppavlov-1.2.0/deeppavlov/models/classifiers/utils.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/doc_retrieval/logit_ranker.py` & `deeppavlov-1.2.0/deeppavlov/models/doc_retrieval/logit_ranker.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/doc_retrieval/pop_ranker.py` & `deeppavlov-1.2.0/deeppavlov/models/doc_retrieval/pop_ranker.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/doc_retrieval/tfidf_ranker.py` & `deeppavlov-1.2.0/deeppavlov/models/doc_retrieval/tfidf_ranker.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/doc_retrieval/utils.py` & `deeppavlov-1.2.0/deeppavlov/models/doc_retrieval/utils.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/embedders/abstract_embedder.py` & `deeppavlov-1.2.0/deeppavlov/models/embedders/abstract_embedder.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from abc import ABCMeta, abstractmethod
 from logging import getLogger
 from pathlib import Path
 from typing import List, Union, Iterator
 
 import numpy as np
-from overrides import overrides
 
 from deeppavlov.core.data.utils import zero_pad
 from deeppavlov.core.models.component import Component
 from deeppavlov.core.models.serializable import Serializable
 
 log = getLogger(__name__)
 
@@ -52,22 +51,20 @@
         self.tok2emb = {}
         self.pad_zero = pad_zero
         self.mean = mean
         self.dim = None
         self.model = None
         self.load()
 
-    @overrides
     def save(self) -> None:
         """
         Class does not save loaded model again as it is not trained during usage
         """
         raise NotImplementedError
 
-    @overrides
     def __call__(self, batch: List[List[str]], mean: bool = None) -> List[Union[list, np.ndarray]]:
         """
         Embed sentences from batch
 
         Args:
             batch: list of tokenized text samples
             mean: whether to return mean embedding of tokens per sample
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/embedders/fasttext_embedder.py` & `deeppavlov-1.2.0/deeppavlov/models/embedders/fasttext_embedder.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from logging import getLogger
 from typing import Iterator
 
 import fasttext
 
 import numpy as np
-from overrides import overrides
 
 from deeppavlov.core.common.registry import register
 from deeppavlov.models.embedders.abstract_embedder import Embedder
 
 log = getLogger(__name__)
 
 
@@ -50,15 +49,14 @@
         """
         Load fastText binary model from self.load_path
         """
         log.debug(f"[loading fastText embeddings from `{self.load_path}`]")
         self.model = fasttext.load_model(str(self.load_path))
         self.dim = self.model.get_dimension()
 
-    @overrides
     def __iter__(self) -> Iterator[str]:
         """
         Iterate over all words from fastText model vocabulary
 
         Returns:
             iterator
         """
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/embedders/tfidf_weighted_embedder.py` & `deeppavlov-1.2.0/deeppavlov/models/embedders/tfidf_weighted_embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from logging import getLogger
 from typing import List, Union, Optional, Tuple
 
 import numpy as np
-from overrides import overrides
 
 from deeppavlov.core.commands.utils import expand_path
 from deeppavlov.core.common.errors import ConfigError
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.data.utils import zero_pad
 from deeppavlov.core.models.component import Component
 
@@ -173,15 +172,14 @@
             batch: batch of tokenized texts
 
         Returns:
             batch of detokenized texts
         """
         return [" ".join(tokens) for tokens in batch]
 
-    @overrides
     def __call__(self, batch: List[List[str]], tags_batch: Optional[List[List[str]]] = None, mean: bool = None,
                  *args, **kwargs) -> List[Union[list, np.ndarray]]:
         """
         Infer on the given data
 
         Args:
             batch: tokenized text samples
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/embedders/transformers_embedder.py` & `deeppavlov-1.2.0/deeppavlov/models/embedders/transformers_embedder.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/kbqa/rel_ranking_infer.py` & `deeppavlov-1.2.0/deeppavlov/models/kbqa/rel_ranking_infer.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from logging import getLogger
 from typing import Tuple, List, Any, Optional
 
 from scipy.special import softmax
 
 from deeppavlov.core.common.chainer import Chainer
-from deeppavlov.core.common.file import load_pickle
+from deeppavlov.core.common.file import load_pickle, read_json
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.models.component import Component
 from deeppavlov.core.models.serializable import Serializable
 from deeppavlov.models.kbqa.sentence_answer import sentence_answer
 from deeppavlov.models.kbqa.wiki_parser import WikiParser
 
 log = getLogger(__name__)
@@ -30,188 +30,265 @@
 
 @register('rel_ranking_infer')
 class RelRankerInfer(Component, Serializable):
     """Class for ranking of paths in subgraph"""
 
     def __init__(self, load_path: str,
                  rel_q2name_filename: str,
+                 return_elements: List[str] = None,
                  ranker: Chainer = None,
                  wiki_parser: Optional[WikiParser] = None,
                  batch_size: int = 32,
-                 rels_to_leave: int = 40,
                  softmax: bool = False,
-                 return_all_possible_answers: bool = False,
-                 return_answer_ids: bool = False,
                  use_api_requester: bool = False,
-                 return_sentence_answer: bool = False,
                  rank: bool = True,
-                 return_confidences: bool = False, **kwargs):
+                 nll_rel_ranking: bool = False,
+                 nll_path_ranking: bool = False,
+                 top_possible_answers: int = -1,
+                 top_n: int = 1,
+                 pos_class_num: int = 1,
+                 rel_thres: float = 0.0,
+                 type_rels: List[str] = None, **kwargs):
         """
 
         Args:
             load_path: path to folder with wikidata files
             rel_q2name_filename: name of file which maps relation id to name
+            return_elements: what elements return in output
             ranker: component deeppavlov.models.ranking.rel_ranker
             wiki_parser: component deeppavlov.models.wiki_parser
             batch_size: infering batch size
-            rels_to_leave: how many relations to leave after relation ranking
             softmax: whether to process relation scores with softmax function
-            return_all_possible_answers: whether to return all found answers
-            return_answer_ids: whether to return answer ids from Wikidata
             use_api_requester: whether wiki parser will be used as external api
-            return_sentence_answer: whether to return answer as a sentence
             rank: whether to rank relations or simple copy input
-            return_confidences: whether to return confidences of candidate answers
+            nll_rel_ranking: whether use components trained with nll loss for relation ranking
+            nll_path_ranking: whether use components trained with nll loss for relation path ranking
+            top_possible_answers: number of answers returned for a question in each list of candidate answers
+            top_n: number of lists of candidate answers returned for a question
+            pos_class_num: index of positive class in the output of relation ranking model
+            rel_thres: threshold of relation confidence
+            type_rels: list of relations in the knowledge base which connect an entity and its type 
             **kwargs:
         """
         super().__init__(save_path=None, load_path=load_path)
         self.rel_q2name_filename = rel_q2name_filename
         self.ranker = ranker
         self.wiki_parser = wiki_parser
         self.batch_size = batch_size
-        self.rels_to_leave = rels_to_leave
         self.softmax = softmax
-        self.return_all_possible_answers = return_all_possible_answers
-        self.return_answer_ids = return_answer_ids
+        self.return_elements = return_elements or list()
         self.use_api_requester = use_api_requester
-        self.return_sentence_answer = return_sentence_answer
         self.rank = rank
-        self.return_confidences = return_confidences
+        self.nll_rel_ranking = nll_rel_ranking
+        self.nll_path_ranking = nll_path_ranking
+        self.top_possible_answers = top_possible_answers
+        self.top_n = top_n
+        self.pos_class_num = pos_class_num
+        self.rel_thres = rel_thres
+        self.type_rels = type_rels or set()
         self.load()
 
     def load(self) -> None:
-        self.rel_q2name = load_pickle(self.load_path / self.rel_q2name_filename)
+        if self.rel_q2name_filename.endswith("pickle"):
+            self.rel_q2name = load_pickle(self.load_path / self.rel_q2name_filename)
+        elif self.rel_q2name_filename.endswith("json"):
+            self.rel_q2name = read_json(self.load_path / self.rel_q2name_filename)
 
     def save(self) -> None:
         pass
 
-    def __call__(self, questions_list: List[str],
-                 candidate_answers_list: List[List[Tuple[str]]],
-                 entities_list: List[List[str]] = None,
-                 template_answers_list: List[str] = None) -> List[str]:
-        answers = []
-        confidence = 0.0
-        if entities_list is None:
-            entities_list = [[] for _ in questions_list]
-        if template_answers_list is None:
-            template_answers_list = ["" for _ in questions_list]
-        for question, candidate_answers, entities, template_answer in \
-                zip(questions_list, candidate_answers_list, entities_list, template_answers_list):
+    def __call__(self, questions_batch: List[str],
+                 template_type_batch: List[str],
+                 raw_answers_batch: List[List[Tuple[str]]],
+                 entity_substr_batch: List[List[str]],
+                 template_answers_batch: List[str]) -> List[str]:
+        answers_batch, outp_confidences_batch, answer_ids_batch = [], [], []
+        entities_and_rels_batch, queries_batch, triplets_batch = [], [], []
+        for question, template_type, raw_answers, entities, template_answer in \
+                zip(questions_batch, template_type_batch, raw_answers_batch, entity_substr_batch,
+                    template_answers_batch):
             answers_with_scores = []
-            answer = "Not Found"
-            if self.rank:
-                n_batches = len(candidate_answers) // self.batch_size + int(
-                    len(candidate_answers) % self.batch_size > 0)
-                for i in range(n_batches):
-                    questions_batch = []
-                    rels_batch = []
-                    rels_labels_batch = []
-                    answers_batch = []
-                    entities_batch = []
-                    confidences_batch = []
-                    for candidate_ans_and_rels in candidate_answers[i * self.batch_size: (i + 1) * self.batch_size]:
-                        candidate_rels = []
-                        candidate_rels_str, candidate_answer = "", ""
-                        candidate_entities, candidate_confidence = [], []
-                        if candidate_ans_and_rels:
-                            candidate_rels = candidate_ans_and_rels["relations"]
-                            candidate_rels = [candidate_rel.split('/')[-1] for candidate_rel in candidate_rels]
-                            candidate_answer = candidate_ans_and_rels["answers"]
-                            candidate_entities = candidate_ans_and_rels["entities"]
-                            candidate_confidence = candidate_ans_and_rels["rel_conf"]
-                            candidate_rels_str = " # ".join([self.rel_q2name[candidate_rel] \
-                                                             for candidate_rel in candidate_rels if
-                                                             candidate_rel in self.rel_q2name])
-                        if candidate_rels_str:
-                            questions_batch.append(question)
-                            rels_batch.append(candidate_rels)
-                            rels_labels_batch.append(candidate_rels_str)
-                            answers_batch.append(candidate_answer)
-                            entities_batch.append(candidate_entities)
-                            confidences_batch.append(candidate_confidence)
-
-                    if questions_batch:
-                        probas = self.ranker(questions_batch, rels_labels_batch)
-                        probas = [proba[1] for proba in probas]
-                        for j, (answer, entities, confidence, rels_ids, rels_labels) in \
-                                enumerate(zip(answers_batch, entities_batch, confidences_batch, rels_batch,
-                                              rels_labels_batch)):
-                            answers_with_scores.append(
-                                (answer, entities, rels_labels, rels_ids, max(probas[j], confidence)))
-
-                answers_with_scores = sorted(answers_with_scores, key=lambda x: x[-1], reverse=True)
-            else:
-                answers_with_scores = [(answer, rels, conf) for *rels, answer, conf in candidate_answers]
+            l_questions, l_rels, l_rels_labels, l_cur_answers, l_entities, l_types, l_sparql_queries, l_triplets, \
+            l_confs = self.preprocess_ranking_input(question, raw_answers)
 
-            answer_ids = tuple()
-            if answers_with_scores:
-                log.debug(f"answers: {answers_with_scores[0]}")
-                answer_ids = answers_with_scores[0][0]
-                if self.return_all_possible_answers and isinstance(answer_ids, tuple):
-                    answer_ids_input = [(answer_id, question) for answer_id in answer_ids]
-                    answer_ids = list(map(lambda x: x.split("/")[-1] if str(x).startswith("http") else x, answer_ids))
+            n_batches = len(l_questions) // self.batch_size + int(len(l_questions) % self.batch_size > 0)
+            for i in range(n_batches):
+                if self.rank:
+                    if self.nll_path_ranking:
+                        probas = self.ranker([l_questions[0]],
+                                             [l_rels_labels[self.batch_size * i:self.batch_size * (i + 1)]])
+                        probas = probas[0]
+                    else:
+                        probas = self.ranker(l_questions[self.batch_size * i:self.batch_size * (i + 1)],
+                                             l_rels_labels[self.batch_size * i:self.batch_size * (i + 1)])
+                        probas = [proba[0] for proba in probas]
                 else:
-                    answer_ids_input = [(answer_ids, question)]
-                    if str(answer_ids).startswith("http:"):
-                        answer_ids = answer_ids.split("/")[-1]
+                    probas = [rel_conf for rel_conf, entity_conf in
+                              l_confs[self.batch_size * i:self.batch_size * (i + 1)]]
+                for j in range(self.batch_size * i, self.batch_size * (i + 1)):
+                    if j < len(l_cur_answers) and (probas[j - self.batch_size * i] > self.rel_thres or
+                                                   (len(l_rels[j]) > 1 and not set(l_rels[j]).intersection(
+                                                       self.type_rels))):
+                        answers_with_scores.append((l_cur_answers[j], l_sparql_queries[j], l_triplets[j],
+                                                    l_entities[j], l_types[j], l_rels_labels[j], l_rels[j],
+                                                    round(probas[j - self.batch_size * i], 3),
+                                                    round(l_confs[j][0], 3), l_confs[j][1]))
+            answers_with_scores = sorted(answers_with_scores, key=lambda x: x[-1] * x[-3], reverse=True)
+            if template_type == "simple_boolean" and not answers_with_scores:
+                answers_with_scores = [(["No"], "", [], [], [], [], [], 1.0, 1.0, 1.0)]
+            res_answers_list, res_answer_ids_list, res_confidences_list, res_entities_and_rels_list = [], [], [], []
+            res_queries_list, res_triplets_list = [], []
+            for n, ans_sc_elem in enumerate(answers_with_scores):
+                init_answer_ids, query, triplets, q_entities, q_types, _, q_rels, p_conf, r_conf, e_conf = ans_sc_elem
+                answer_ids = []
+                for answer_id in init_answer_ids:
+                    answer_id = str(answer_id).replace("@en", "").strip('"')
+                    if answer_id not in answer_ids:
+                        answer_ids.append(answer_id)
+
+                if self.top_possible_answers > 0:
+                    answer_ids = answer_ids[:self.top_possible_answers]
+                answer_ids_input = [(answer_id, question) for answer_id in answer_ids]
+                answer_ids = [str(answer_id).split("/")[-1] for answer_id in answer_ids]
                 parser_info_list = ["find_label" for _ in answer_ids_input]
-                answer_labels = self.wiki_parser(parser_info_list, answer_ids_input)
-                log.debug(f"answer_labels {answer_labels}")
-                if self.return_all_possible_answers:
-                    answer_labels = list(set(answer_labels))
-                    answer_labels = [label for label in answer_labels if (label and label != "Not Found")][:5]
-                    answer_labels = [str(label) for label in answer_labels]
-                    if len(answer_labels) > 2:
-                        answer = f"{', '.join(answer_labels[:-1])} and {answer_labels[-1]}"
-                    else:
-                        answer = ', '.join(answer_labels)
+                init_answer_labels = self.wiki_parser(parser_info_list, answer_ids_input)
+                if n < 7:
+                    log.debug(f"answers: {init_answer_ids[:3]} --- query {query} --- entities {q_entities} --- "
+                              f"types {q_types[:3]} --- q_rels {q_rels} --- {ans_sc_elem[5:]} --- "
+                              f"answer_labels {init_answer_labels[:3]}")
+                answer_labels = []
+                for label in init_answer_labels:
+                    if label not in answer_labels:
+                        answer_labels.append(label)
+                answer_labels = [label for label in answer_labels if (label and label != "Not Found")][:5]
+                answer_labels = [str(label) for label in answer_labels]
+                if len(answer_labels) > 2:
+                    answer = f"{', '.join(answer_labels[:-1])} and {answer_labels[-1]}"
                 else:
-                    answer = answer_labels[0]
-                if self.return_sentence_answer:
+                    answer = ', '.join(answer_labels)
+
+                if "sentence_answer" in self.return_elements:
                     try:
                         answer = sentence_answer(question, answer, entities, template_answer)
-                    except:
-                        log.warning("Error in sentence answer")
-                confidence = answers_with_scores[0][2]
-            if self.return_confidences:
-                answers.append((answer, confidence))
-            else:
-                if self.return_answer_ids:
-                    if not answer_ids:
-                        answer_ids = "Not found"
-                    answers.append((answer, answer_ids))
+                    except ValueError as e:
+                        log.warning(f"Error in sentence answer, {e}")
+
+                res_answers_list.append(answer)
+                res_answer_ids_list.append(answer_ids)
+                if "several_confidences" in self.return_elements:
+                    res_confidences_list.append((p_conf, r_conf, e_conf))
+                else:
+                    res_confidences_list.append(p_conf)
+                res_entities_and_rels_list.append([q_entities[:-1], q_rels])
+                res_queries_list.append(query)
+                res_triplets_list.append(triplets)
+
+            if self.top_n == 1:
+                if answers_with_scores:
+                    answers_batch.append(res_answers_list[0])
+                    outp_confidences_batch.append(res_confidences_list[0])
+                    answer_ids_batch.append(res_answer_ids_list[0])
+                    entities_and_rels_batch.append(res_entities_and_rels_list[0])
+                    queries_batch.append(res_queries_list[0])
+                    triplets_batch.append(res_triplets_list[0])
                 else:
-                    answers.append(answer)
-        if not answers:
-            if self.return_confidences:
-                answers.append(("Not found", 0.0))
+                    answers_batch.append("Not Found")
+                    outp_confidences_batch.append(0.0)
+                    answer_ids_batch.append([])
+                    entities_and_rels_batch.append([])
+                    queries_batch.append([])
+                    triplets_batch.append([])
             else:
-                answers.append("Not found")
-
-        return answers
+                answers_batch.append(res_answers_list[:self.top_n])
+                outp_confidences_batch.append(res_confidences_list[:self.top_n])
+                answer_ids_batch.append(res_answer_ids_list[:self.top_n])
+                entities_and_rels_batch.append(res_entities_and_rels_list[:self.top_n])
+                queries_batch.append(res_queries_list[:self.top_n])
+                triplets_batch.append(res_triplets_list[:self.top_n])
+
+        answer_tuple = (answers_batch,)
+        if "confidences" in self.return_elements:
+            answer_tuple += (outp_confidences_batch,)
+        if "answer_ids" in self.return_elements:
+            answer_tuple += (answer_ids_batch,)
+        if "entities_and_rels" in self.return_elements:
+            answer_tuple += (entities_and_rels_batch,)
+        if "queries" in self.return_elements:
+            answer_tuple += (queries_batch,)
+        if "triplets" in self.return_elements:
+            answer_tuple += (triplets_batch,)
+
+        return answer_tuple
+
+    def preprocess_ranking_input(self, question, answers):
+        l_questions, l_rels, l_rels_labels, l_cur_answers = [], [], [], []
+        l_entities, l_types, l_sparql_queries, l_triplets, l_confs = [], [], [], [], []
+        for ans_and_rels in answers:
+            answer, sparql_query, confidence = "", "", []
+            entities, types, rels, rels_labels, triplets = [], [], [], [], []
+            if ans_and_rels:
+                rels = [rel.split('/')[-1] for rel in ans_and_rels["relations"]]
+                answer = ans_and_rels["answers"]
+                entities = ans_and_rels["entities"]
+                types = ans_and_rels["types"]
+                sparql_query = ans_and_rels["sparql_query"]
+                triplets = ans_and_rels["triplets"]
+                confidence = ans_and_rels["output_conf"]
+                rels_labels = []
+                for rel in rels:
+                    if rel in self.rel_q2name:
+                        label = self.rel_q2name[rel]
+                        if isinstance(label, list):
+                            label = label[0]
+                        rels_labels.append(label.lower())
+            if rels_labels:
+                l_questions.append(question)
+                l_rels.append(rels)
+                l_rels_labels.append(rels_labels)
+                l_cur_answers.append(answer)
+                l_entities.append(entities)
+                l_types.append(types)
+                l_sparql_queries.append(sparql_query)
+                l_triplets.append(triplets)
+                l_confs.append(confidence)
+        return l_questions, l_rels, l_rels_labels, l_cur_answers, l_entities, l_types, l_sparql_queries, l_triplets, \
+               l_confs
 
     def rank_rels(self, question: str, candidate_rels: List[str]) -> List[Tuple[str, Any]]:
         rels_with_scores = []
         if question is not None:
-            n_batches = len(candidate_rels) // self.batch_size + int(len(candidate_rels) % self.batch_size > 0)
-            for i in range(n_batches):
-                questions_batch = []
-                rels_labels_batch = []
-                rels_batch = []
-                for candidate_rel in candidate_rels[i * self.batch_size: (i + 1) * self.batch_size]:
-                    if candidate_rel in self.rel_q2name:
-                        questions_batch.append(question)
-                        rels_batch.append(candidate_rel)
-                        rels_labels_batch.append(self.rel_q2name[candidate_rel])
-                if questions_batch:
-                    probas = self.ranker(questions_batch, rels_labels_batch)
-                    probas = [proba[1] for proba in probas]
-                    for j, rel in enumerate(rels_batch):
+            questions, rels_labels, rels = [], [], []
+            for candidate_rel in candidate_rels:
+                if candidate_rel in self.rel_q2name:
+                    cur_rels_labels = self.rel_q2name[candidate_rel]
+                    if isinstance(cur_rels_labels, str):
+                        cur_rels_labels = [cur_rels_labels]
+                    for cur_rel in cur_rels_labels:
+                        questions.append(question)
+                        rels.append(candidate_rel)
+                        rels_labels.append(cur_rel)
+            if questions:
+                n_batches = len(rels) // self.batch_size + int(len(rels) % self.batch_size > 0)
+                for i in range(n_batches):
+                    if self.nll_rel_ranking:
+                        probas = self.ranker([questions[0]],
+                                             [rels_labels[i * self.batch_size:(i + 1) * self.batch_size]])
+                        probas = probas[0]
+                    else:
+                        probas = self.ranker(questions[i * self.batch_size:(i + 1) * self.batch_size],
+                                             rels_labels[i * self.batch_size:(i + 1) * self.batch_size])
+                        probas = [proba[self.pos_class_num] for proba in probas]
+                    for j, rel in enumerate(rels[i * self.batch_size:(i + 1) * self.batch_size]):
                         rels_with_scores.append((rel, probas[j]))
             if self.softmax:
                 scores = [score for rel, score in rels_with_scores]
                 softmax_scores = softmax(scores)
                 rels_with_scores = [(rel, softmax_score) for (rel, score), softmax_score in
                                     zip(rels_with_scores, softmax_scores)]
+            rels_with_scores_dict = {}
+            for rel, score in rels_with_scores:
+                if rel not in rels_with_scores_dict:
+                    rels_with_scores_dict[rel] = []
+                rels_with_scores_dict[rel].append(score)
+            rels_with_scores = [(rel, max(scores)) for rel, scores in rels_with_scores_dict.items()]
             rels_with_scores = sorted(rels_with_scores, key=lambda x: x[1], reverse=True)
-
-        return rels_with_scores[:self.rels_to_leave]
+        return rels_with_scores
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/kbqa/sentence_answer.py` & `deeppavlov-1.2.0/deeppavlov/models/kbqa/sentence_answer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/kbqa/template_matcher.py` & `deeppavlov-1.2.0/deeppavlov/models/kbqa/template_matcher.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/kbqa/tree_to_sparql.py` & `deeppavlov-1.2.0/deeppavlov/models/kbqa/tree_to_sparql.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,338 +8,537 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import copy
 import re
 from collections import defaultdict
 from io import StringIO
 from logging import getLogger
 from typing import Any, List, Tuple, Dict, Union
 
-import numpy as np
 import spacy
 from navec import Navec
-from scipy.sparse import csr_matrix
+from razdel import tokenize
 from slovnet import Syntax
 from udapi.block.read.conllu import Conllu
 from udapi.core.node import Node
 
 from deeppavlov.core.commands.utils import expand_path
 from deeppavlov.core.common.file import read_json
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.models.component import Component
 from deeppavlov.core.models.serializable import Serializable
+from deeppavlov.models.kbqa.ru_adj_to_noun import RuAdjToNoun
+from deeppavlov.models.kbqa.utils import preprocess_template_queries
 
 log = getLogger(__name__)
 
 
-@register('ru_adj_to_noun')
-class RuAdjToNoun:
-    """
-        Class for converting an adjective in Russian to the corresponding noun, for example:
-        "московский" -> "Москва", "африканский" -> "Африка"
-    """
-
-    def __init__(self, freq_dict_filename: str, candidate_nouns: int = 10, **kwargs):
-        """
-
-        Args:
-            freq_dict_filename: file with the dictionary of Russian words with the corresponding frequencies
-            candidate_nouns: how many candidate nouns to leave after search
-            **kwargs:
-        """
-        self.candidate_nouns = candidate_nouns
-        alphabet = "абвгдеёжзийклмнопрстуфхцчшщъыьэюя-"
-        self.alphabet_length = len(alphabet)
-        self.max_word_length = 24
-        self.letter_nums = {letter: num for num, letter in enumerate(alphabet)}
-        with open(str(expand_path(freq_dict_filename)), 'r') as fl:
-            lines = fl.readlines()
-        pos_freq_dict = defaultdict(list)
-        for line in lines:
-            line_split = line.strip('\n').split('\t')
-            if re.match("[\d]+\.[\d]+", line_split[2]):
-                pos_freq_dict[line_split[1]].append((line_split[0], float(line_split[2])))
-        self.nouns_with_freq = pos_freq_dict["s.PROP"]
-        self.adj_set = set([word for word, freq in pos_freq_dict["a"]])
-        self.nouns = [noun[0] for noun in self.nouns_with_freq]
-        self.matrix = self.make_sparse_matrix(self.nouns).transpose()
-        self.nlp = spacy.load("ru_core_news_sm")
-
-    def search(self, word: str):
-        word = self.nlp(word)[0].lemma_
-        if word in self.adj_set:
-            q_matrix = self.make_sparse_matrix([word])
-            scores = q_matrix * self.matrix
-            scores = np.squeeze(scores.toarray() + 0.0001)
-            indices = np.argsort(-scores)[:self.candidate_nouns]
-            scores = list(scores[indices])
-            candidates = [self.nouns_with_freq[indices[i]] + (scores[i],) for i in range(len(indices))]
-            candidates = sorted(candidates, key=lambda x: x[1] * x[2], reverse=True)
-            log.debug(f"AdjToNoun, found nouns: {candidates}")
-            if candidates[0][2] > 2.5:
-                return candidates[0][0]
-        return ""
-
-    def make_sparse_matrix(self, words: List[str]):
-        indptr = []
-        indices = []
-        data = []
-
-        total_length = 0
-
-        for n, word in enumerate(words):
-            indptr.append(total_length)
-            for cnt, letter in enumerate(word.lower()):
-                col = self.alphabet_length * cnt + self.letter_nums[letter]
-                indices.append(col)
-                init_value = 1.0 - cnt * 0.05
-                if init_value < 0:
-                    init_value = 0
-                data.append(init_value)
-            total_length += len(word)
-
-        indptr.append(total_length)
-
-        data = np.array(data)
-        indptr = np.array(indptr)
-        indices = np.array(indices)
-
-        matrix = csr_matrix((data, indices, indptr), shape=(len(words), self.max_word_length * self.alphabet_length))
-
-        return matrix
-
-
 @register('slovnet_syntax_parser')
 class SlovnetSyntaxParser(Component, Serializable):
     """Class for syntax parsing using Slovnet library"""
 
-    def __init__(self, load_path: str, navec_filename: str, syntax_parser_filename: str, **kwargs):
+    def __init__(self, load_path: str, navec_filename: str, syntax_parser_filename: str, tree_patterns_filename: str,
+                 **kwargs):
         super().__init__(save_path=None, load_path=load_path)
         self.navec_filename = expand_path(navec_filename)
         self.syntax_parser_filename = expand_path(syntax_parser_filename)
+        self.tree_patterns = read_json(expand_path(tree_patterns_filename))
         self.re_tokenizer = re.compile(r"[\w']+|[^\w ]")
+        self.pronouns = {"q_pronouns": {"какой", "какая", "какое", "каком", "каким", "какую", "кто", "что", "как",
+                                        "когда", "где", "чем", "сколько"},
+                         "how_many": {"сколько"}}
+        self.first_tokens = {"первый", "первая", "первое"}
+        self.nlp = spacy.load("ru_core_news_sm")
         self.load()
 
     def load(self) -> None:
         navec = Navec.load(self.navec_filename)
         self.syntax = Syntax.load(self.syntax_parser_filename)
         self.syntax.navec(navec)
 
     def save(self) -> None:
         pass
 
-    def __call__(self, sentences, entity_offsets_batch):
-        sentences_tok = []
+    def preprocess_sentences(self, sentences, entity_offsets_batch):
+        sentences_tokens_batch, replace_dict_batch = [], []
         for sentence, entity_offsets in zip(sentences, entity_offsets_batch):
-            for start, end in entity_offsets:
-                entity_old = sentence[start:end]
-                entity_new = entity_old.capitalize()
-                sentence = sentence.replace(entity_old, entity_new)
-            sentence = sentence.capitalize()
-            sentences_tok.append(re.findall(self.re_tokenizer, sentence))
-        markup = list(self.syntax.map(sentences_tok))
+            if sentence.islower():
+                for start, end in entity_offsets:
+                    entity_old = sentence[start:end]
+                    if entity_old:
+                        entity_new = f"{entity_old[0].upper()}{entity_old[1:]}"
+                        sentence = sentence.replace(entity_old, entity_new)
+                sentence = f"{sentence[0].upper()}{sentence[1:]}"
+            names3 = re.findall(r"([\w]{1}\.)([ ]?)([\w]{1}\.)([ ])([\w]{3,})", sentence)
+            replace_dict = {}
+            for name in names3:
+                names_str = "".join(name)
+                replace_dict[name[-1]] = (names_str, "name")
+                sentence = sentence.replace(names_str, name[-1])
+            names2 = re.findall(r"([\w]{1}\.)([ ])([\w]{3,})", sentence)
+            for name in names2:
+                names_str = "".join(name)
+                replace_dict[name[-1]] = (names_str, "name")
+                sentence = sentence.replace(names_str, name[-1])
+            works_of_art = re.findall(r'(["«])(.*?)(["»])', sentence)
+            for symb_start, work_of_art, symb_end in works_of_art:
+                work_of_art_tokens = re.findall(self.re_tokenizer, work_of_art)
+                if len(work_of_art.split()) > 1:
+                    short_substr = ""
+                    for tok in work_of_art_tokens:
+                        if self.nlp(tok)[0].pos_ == "NOUN":
+                            short_substr = tok
+                            break
+                    if not short_substr:
+                        short_substr = work_of_art_tokens[0]
+                    replace_dict[short_substr] = (work_of_art, "name")
+                    sentence = sentence.replace(work_of_art, short_substr)
+            while True:
+                tokens = sentence.split()
+                found_substr = False
+                for i in range(len(tokens) - 2):
+                    found = True
+                    for j in range(i, i + 3):
+                        if len(tokens[j]) < 2 or tokens[j][0] in '("' or tokens[j][-1] in '"),.?':
+                            found = False
+                    if found and i > 0:
+                        token_tags = [self.nlp(tokens[j])[0].pos_ for j in range(i, i + 3)]
+                        lemm_tokens = {self.nlp(tok)[0].lemma_ for tok in tokens[i:i + 3]}
+                        if token_tags == ["DET", "DET", "NOUN"] and not lemm_tokens & self.first_tokens:
+                            long_substr = " ".join(tokens[i:i + 3])
+                            replace_dict[tokens[i + 2]] = (long_substr, "adj")
+                            sentence = sentence.replace(long_substr, tokens[i + 2])
+                            found_substr = True
+                    if found_substr:
+                        break
+                if not found_substr:
+                    break
+            sentence_tokens = [tok.text for tok in tokenize(sentence)]
+            sentences_tokens_batch.append(sentence_tokens)
+            log.debug(f"replace_dict: {replace_dict} --- sentence: {sentence_tokens}")
+            replace_dict_batch.append(replace_dict)
+        return sentences_tokens_batch, replace_dict_batch
+
+    def get_markup(self, proc_syntax_batch, replace_dict_batch):
+        markup_batch = []
+        for proc_syntax, replace_dict in zip(proc_syntax_batch, replace_dict_batch):
+            markup_list = []
+            for elem in proc_syntax.tokens:
+                markup_list.append({"id": elem.id, "text": elem.text, "head_id": int(elem.head_id), "rel": elem.rel})
+            ids, words, head_ids, rels = self.get_elements(markup_list)
+            head_ids, markup_list = self.correct_cycle(ids, head_ids, rels, markup_list)
+            for substr in replace_dict:
+                substr_full, substr_type = replace_dict[substr]
+                found_n = -1
+                for n, markup_elem in enumerate(markup_list):
+                    if markup_elem["text"] == substr:
+                        found_n = n
+                if found_n > -1:
+                    before_markup_list = copy.deepcopy(markup_list[:found_n])
+                    after_markup_list = copy.deepcopy(markup_list[found_n + 1:])
+                    substr_tokens = [tok.text for tok in tokenize(substr_full)]
+                    new_markup_list = []
+                    if substr_type == "name":
+                        for j in range(len(substr_tokens)):
+                            new_markup_elem = {"id": str(found_n + j + 1), "text": substr_tokens[j]}
+                            if j == 0:
+                                new_markup_elem["rel"] = markup_list[found_n]["rel"]
+                                if int(markup_list[found_n]["head_id"]) < found_n + 1:
+                                    new_markup_elem["head_id"] = markup_list[found_n]["head_id"]
+                                else:
+                                    new_markup_elem["head_id"] = str(int(markup_list[found_n]["head_id"]) + len(
+                                        substr_tokens) - 1)
+                            else:
+                                new_markup_elem["rel"] = "flat:name"
+                                new_markup_elem["head_id"] = str(found_n + 1)
+                            new_markup_list.append(new_markup_elem)
+                    elif substr_type == "adj":
+                        for j in range(len(substr_tokens)):
+                            new_elem = {"id": str(found_n + j + 1), "text": substr_tokens[j]}
+                            if j == len(substr_tokens) - 1:
+                                new_elem["rel"] = markup_list[found_n]["rel"]
+                                if markup_list[found_n]["head_id"] < found_n + 1:
+                                    new_elem["head_id"] = markup_list[found_n]["head_id"]
+                                else:
+                                    new_elem["head_id"] = markup_list[found_n]["head_id"] + len(substr_tokens) - 1
+                            else:
+                                new_elem["rel"] = "amod"
+                                new_elem["head_id"] = str(found_n + len(substr_tokens))
+                            new_markup_list.append(new_elem)
+
+                    for j in range(len(before_markup_list)):
+                        if int(before_markup_list[j]["head_id"]) > found_n + 1:
+                            before_markup_list[j]["head_id"] = int(before_markup_list[j]["head_id"]) + \
+                                                               len(substr_tokens) - 1
+                        if before_markup_list[j]["head_id"] == found_n + 1 and substr_type == "adj":
+                            before_markup_list[j]["head_id"] = found_n + len(substr_tokens)
+                    for j in range(len(after_markup_list)):
+                        after_markup_list[j]["id"] = str(int(after_markup_list[j]["id"]) + len(substr_tokens) - 1)
+                        if int(after_markup_list[j]["head_id"]) > found_n + 1:
+                            after_markup_list[j]["head_id"] = int(after_markup_list[j]["head_id"]) + \
+                                                              len(substr_tokens) - 1
+                        if after_markup_list[j]["head_id"] == found_n + 1 and substr_type == "adj":
+                            after_markup_list[j]["head_id"] = found_n + len(substr_tokens)
+
+                    markup_list = before_markup_list + new_markup_list + after_markup_list
+            for j in range(len(markup_list)):
+                markup_list[j]["head_id"] = str(markup_list[j]["head_id"])
+            markup_batch.append(markup_list)
+        return markup_batch
+
+    def find_cycle(self, ids, head_ids):
+        for i in range(len(ids)):
+            for j in range(len(ids)):
+                if i < j and head_ids[j] == str(i + 1) and head_ids[i] == str(j + 1):
+                    return i + 1
+        return -1
+
+    def correct_markup(self, words, head_ids, rels, root_n):
+        if len(words) > 3:
+            pos = [self.nlp(words[i])[0].pos_ for i in range(len(words))]
+            for tree_pattern in self.tree_patterns:
+                first_word = tree_pattern.get("first_word", "")
+                (r_start, r_end), rel_info = tree_pattern.get("rels", [[0, 0], ""])
+                (p_start, p_end), pos_info = tree_pattern.get("pos", [[0, 0], ""])
+                if (not first_word or words[0].lower() in self.pronouns[first_word]) \
+                        and (not rel_info or rels[r_start:r_end] == rel_info) \
+                        and (not pos_info or pos[p_start:p_end] == pos_info):
+                    for ind, deprel in tree_pattern.get("rel_ids", {}).items():
+                        rels[int(ind)] = deprel
+                    for ind, head_id in tree_pattern.get("head_ids", {}).items():
+                        head_ids[int(ind)] = head_id
+                    root_n = tree_pattern["root_n"]
+                    break
+            if words[0].lower() in {"какой", "какая", "какое"} and rels[:3] == ["det", "obj", "root"] \
+                    and pos[1:3] == ["NOUN", "VERB"] and "nsubj" not in rels:
+                rels[1] = "nsubj"
+        return head_ids, rels, root_n
+
+    def find_root(self, rels):
+        root_n = -1
+        for n in range(len(rels)):
+            if rels[n] == "root":
+                root_n = n + 1
+                break
+        return root_n
+
+    def get_elements(self, markup_elem):
+        ids, words, head_ids, rels = [], [], [], []
+        for elem in markup_elem:
+            ids.append(elem["id"])
+            words.append(elem["text"])
+            head_ids.append(elem["head_id"])
+            rels.append(elem["rel"])
+        return ids, words, head_ids, rels
+
+    def correct_cycle(self, ids, head_ids, rels, markup_elem):
+        cycle_num = -1
+        for n, (elem_id, head_id) in enumerate(zip(ids, head_ids)):
+            if str(head_id) == str(elem_id):
+                cycle_num = n
+        root_n = self.find_root(rels)
+        if cycle_num > 0 and root_n > -1:
+            head_ids[cycle_num] = root_n
+        markup_elem[cycle_num]["head_id"] = root_n
+        return head_ids, markup_elem
 
+    def process_markup(self, markup_batch):
         processed_markup_batch = []
-        for markup_elem in markup:
+        for markup_elem in markup_batch:
             processed_markup = []
-            ids, words, head_ids, rels = [], [], [], []
-            for elem in markup_elem.tokens:
-                ids.append(elem.id)
-                words.append(elem.text)
-                head_ids.append(elem.head_id)
-                rels.append(elem.rel)
+            ids, words, head_ids, rels = self.get_elements(markup_elem)
             if "root" not in {rel.lower() for rel in rels}:
+                found_root = False
                 for n, (elem_id, head_id) in enumerate(zip(ids, head_ids)):
                     if elem_id == head_id:
                         rels[n] = "root"
                         head_ids[n] = 0
+                        found_root = True
+                if not found_root:
+                    for n in range(len(ids)):
+                        if rels[n] == "nsubj":
+                            rels[n] = "root"
+                            head_ids[n] = 0
+                            found_root = True
+                if not found_root:
+                    for n in range(len(ids)):
+                        if self.nlp(words[n])[0].pos_ == "VERB":
+                            rels[n] = "root"
+                            head_ids[n] = 0
+
+            root_n = self.find_root(rels)
+            head_ids, rels, root_n = self.correct_markup(words, head_ids, rels, root_n)
+            if words[-1] == "?" and -1 < root_n != head_ids[-1]:
+                head_ids[-1] = root_n
+
+            head_ids, markup_elem = self.correct_cycle(ids, head_ids, rels, markup_elem)
+            i = self.find_cycle(ids, head_ids)
+            if i == 1 and root_n > -1:
+                head_ids[i - 1] = root_n
             for elem_id, word, head_id, rel in zip(ids, words, head_ids, rels):
                 processed_markup.append(f"{elem_id}\t{word}\t_\t_\t_\t_\t{head_id}\t{rel}\t_\t_")
             processed_markup_batch.append("\n".join(processed_markup))
+        return processed_markup_batch
 
+    def __call__(self, sentences, entity_offsets_batch):
+        sentences_tokens_batch, substr_dict_batch = self.preprocess_sentences(sentences, entity_offsets_batch)
+        proc_syntax_batch = list(self.syntax.map(sentences_tokens_batch))
+        markup_batch = self.get_markup(proc_syntax_batch, substr_dict_batch)
+        processed_markup_batch = self.process_markup(markup_batch)
         return processed_markup_batch
 
 
 @register('tree_to_sparql')
 class TreeToSparql(Component):
     """
         Class for building of sparql query template using syntax parser
     """
 
-    def __init__(self, sparql_queries_filename: str, lang: str = "rus", adj_to_noun: RuAdjToNoun = None, **kwargs):
+    def __init__(self, sparql_queries_filename: str, syntax_parser: Component, kb_prefixes: Dict[str, str],
+                 adj_to_noun: RuAdjToNoun = None, **kwargs):
         """
 
         Args:
             sparql_queries_filename: file with sparql query templates
-            lang: english or russian
+            syntax_parser: component for syntactic parsing of the input question
+            kb_prefixes: prefixes for entities, relations and types in the knowledge base
             adj_to_noun: component deeppavlov.models.kbqa.tree_to_sparql:RuAdjToNoun
             **kwargs:
         """
-        self.lang = lang
-        if self.lang == "rus":
-            self.q_pronouns = {"какой", "какая", "какое", "каком", "каким", "какую", "кто", "что", "как", "когда",
-                               "где", "чем", "сколько"}
-            self.how_many = "сколько"
-            self.change_root_tokens = {"каким был", "какой была"}
-            self.first_tokens = {"первый"}
-            self.last_tokens = {"последний"}
-            self.begin_tokens = {"начинать", "начать"}
-            self.end_tokens = {"завершить", "завершать", "закончить"}
-            self.ranking_tokens = {"самый"}
-            self.nlp = spacy.load("ru_core_news_sm")
-        elif self.lang == "eng":
-            self.q_pronouns = {"what", "who", "how", "when", "where", "which"}
-            self.how_many = "how many"
-            self.change_root_tokens = ""
-            self.first_tokens = {"first"}
-            self.last_tokens = {"last"}
-            self.begin_tokens = set()
-            self.end_tokens = set()
-            self.ranking_tokens = set()
-            self.nlp = spacy.load("en_core_web_sm")
-        else:
-            raise ValueError(f"unsupported language {lang}")
+        self.q_pronouns = {"какой", "какая", "какое", "каком", "каким", "какую", "кто", "что", "как", "когда",
+                           "где", "чем", "сколько"}
+        self.how_many = "сколько"
+        self.change_root_tokens = {"каким был", "какой была"}
+        self.first_tokens = {"первый", "первая", "первое"}
+        self.last_tokens = {"последний"}
+        self.begin_tokens = {"начинать", "начать"}
+        self.end_tokens = {"завершить", "завершать", "закончить"}
+        self.ranking_tokens = {"самый"}
+        self.date_tokens = {"год", "месяц"}
+        self.nlp = spacy.load("ru_core_news_sm")
+        self.re_tokenizer = re.compile(r"[\w']+|[^\w ]")
         self.sparql_queries_filename = expand_path(sparql_queries_filename)
-        self.template_queries = read_json(self.sparql_queries_filename)
+        template_queries = read_json(self.sparql_queries_filename)
+        self.template_queries = preprocess_template_queries(template_queries, kb_prefixes)
+        self.syntax_parser = syntax_parser
         self.adj_to_noun = adj_to_noun
 
-    def __call__(self, syntax_tree_batch: List[str],
-                 positions_batch: List[List[List[int]]]) -> Tuple[
-        List[str], List[List[str]], List[List[str]], List[List[str]]]:
-        log.debug(f"positions of entity tokens {positions_batch}")
-        query_nums_batch = []
-        entities_dict_batch = []
-        types_dict_batch = []
-        questions_batch = []
+    def __call__(self, questions_batch: List[str], substr_batch: List[List[str]], tags_batch: List[List[str]],
+                 offsets_batch: List[List[List[int]]], positions_batch: List[List[List[int]]],
+                 probas_batch: List[List[float]]) -> Tuple[
+        List[Union[str, Any]], List[Union[List[str], List[Union[str, Any]]]], List[Union[List[str], Any]], List[
+            Union[List[Union[str, Any]], Any]], List[Union[List[Union[float, Any]], Any]], List[List[int]], List[
+            Union[List[str], List[Any]]]]:
+        substr_batch, tags_batch, offsets_batch, positions_batch, probas_batch = \
+            self.sort_substr(substr_batch, tags_batch, offsets_batch, positions_batch, probas_batch)
+        log.debug(f"substr: {substr_batch} tags: {tags_batch} positions: {positions_batch}")
+        query_nums_batch, s_substr_batch, s_tags_batch, s_probas_batch, types_batch = [], [], [], [], []
+        entities_to_link_batch = []
+        clean_questions_batch = []
         count = False
-        for syntax_tree, positions in zip(syntax_tree_batch, positions_batch):
-            log.debug(f"\n{syntax_tree}")
-            try:
-                tree = Conllu(filehandle=StringIO(syntax_tree)).read_tree()
-                root = self.find_root(tree)
-                tree_desc = tree.descendants
-            except ValueError:
-                root = ""
-            unknown_node = ""
-            if root:
-                log.debug(f"syntax tree info, root: {root.form}")
-                unknown_node, unknown_branch = self.find_branch_with_unknown(root)
-            positions = [num for position in positions for num in position]
+        for question, substr_list, tags_list, offsets_list, probas_list, positions in \
+                zip(questions_batch, substr_batch, tags_batch, offsets_batch, probas_batch, positions_batch):
+            entities_dict, probas_dict = {}, {}
+            for substr, tag, proba in zip(substr_list, tags_list, probas_list):
+                entities_dict[substr.lower()] = tag
+                probas_dict[substr.lower()] = proba
+            for i in range(len(substr_list)):
+                substr = substr_list[i]
+                if len(substr) > 2 and ("-" in substr or f"{substr}-" in question) and " - " not in substr:
+                    if "-" in substr:
+                        length = len(re.findall(self.re_tokenizer, substr))
+                    else:
+                        length = 3
+                    substr_tokens = list(tokenize(substr))
+                    positions[i] = [positions[i][j] for j in range(len(substr_tokens))]
+                    if i < len(substr_list) - 1:
+                        for j in range(i + 1, len(substr_list)):
+                            pos_inds = positions[j]
+                            pos_inds = [ind - length + 1 for ind in pos_inds]
+                            positions[j] = pos_inds
+
+            root, tree, tree_desc, unknown_node, unknown_branch = self.syntax_parse(question, offsets_list)
+            query_nums = ["7"]
+            s_substr_list = substr_list
+            s_tags_list = tags_list
+            s_probas_list = probas_list
+            types_list = []
             if unknown_node:
-                log.debug(f"syntax tree info, unknown node: {unknown_node.form}, unknown branch: {unknown_branch.form}")
+                log.debug(f"syntax tree info 1, unknown node: {unknown_node.form}, unkn branch: {unknown_branch.form}")
                 log.debug(f"wh_leaf: {self.wh_leaf}")
                 clause_node, clause_branch = self.find_clause_node(root, unknown_branch)
-                if clause_node:
-                    log.debug(f"clause node {clause_node.form}")
-                else:
-                    log.debug(f"clause node not found")
-                modifiers, clause_modifiers = self.find_modifiers_of_unknown(unknown_node)
-                modifiers_debug_list = []
-                for modifier in modifiers:
-                    if isinstance(modifier, str):
-                        modifiers_debug_list.append(modifier)
-                    else:
-                        modifiers_debug_list.append(modifier.form)
-                log.debug(f"modifiers: {' '.join(modifiers_debug_list)}")
-                if f"{tree_desc[0].form.lower()} {tree_desc[1].form.lower()}" in self.change_root_tokens:
-                    new_root = root.children[0]
-                else:
-                    new_root = root
-                root_desc = defaultdict(list)
-                for node in new_root.children:
-                    if node.deprel not in ["punct", "advmod", "cop", "mark"]:
-                        if node == unknown_branch:
-                            root_desc[node.deprel].append(node)
-                        else:
-                            if self.find_entities(node, positions, cut_clause=False) or \
-                                    (self.find_year_or_number(node) and node.deprel in ["obl", "nummod"]):
-                                root_desc[node.deprel].append(node)
-
-                if root.form.lower() == self.how_many or ("nsubj" in root_desc.keys() and
-                                                          self.how_many in [nd.form.lower() for nd in
-                                                                            root_desc["nsubj"]]):
-                    count = True
-                log.debug(f"root_desc {root_desc.keys()}")
-                appos_token_nums = sorted(self.find_appos_tokens(root, []))
+                log.debug(f"clause node: {clause_node}")
+                tok_and_ord = {node.ord: node for node in tree.descendants}
+                appos_token_nums = sorted(self.find_appos_tokens(root, tok_and_ord, []))
                 appos_tokens = [elem.form for elem in tree_desc if elem.ord in appos_token_nums]
-                clause_token_nums = sorted(self.find_clause_tokens(root, clause_node, []))
+                clause_token_nums = sorted(self.find_clause_tokens(root, tok_and_ord, clause_node))
                 clause_tokens = [elem.form for elem in tree_desc if elem.ord in clause_token_nums]
                 log.debug(f"appos tokens: {appos_tokens}")
                 log.debug(f"clause_tokens: {clause_tokens}")
-                self.root_entity = False
-                if root.ord - 1 in positions:
-                    self.root_entity = True
-
-                temporal_order = self.find_first_last(new_root)
-                new_root_nf = self.nlp(new_root.form)[0].lemma_
-                if new_root_nf in self.begin_tokens or new_root_nf in self.end_tokens:
-                    temporal_order = new_root_nf
-                ranking_tokens = self.find_ranking_tokens(new_root)
-                query_nums, entities_dict, types_dict = self.build_query(new_root, unknown_branch, root_desc,
-                                                                         unknown_node, modifiers, clause_modifiers,
-                                                                         clause_node, positions, count,
-                                                                         temporal_order, ranking_tokens)
-
-                if self.lang == "rus":
-                    if ranking_tokens:
-                        question = []
-                        for node in tree.descendants:
-                            if node.ord in ranking_tokens or node.form.lower() in self.q_pronouns:
-                                question.append(self.nlp(node.form)[0].lemma_)
-                            else:
-                                question.append(node.form)
-                        question = ' '.join(question)
+                question, ranking_tokens = self.sanitize_question(tree, root, appos_token_nums, clause_token_nums)
+                if appos_token_nums or clause_token_nums:
+                    root, tree, tree_desc, unknown_node, unknown_branch = self.syntax_parse(question, offsets_list)
+                    log.debug(f"syntax tree info 2, unknown node: {unknown_node}, unkn branch: {unknown_branch}")
+
+                if unknown_node:
+                    modifiers, clause_modifiers = self.find_modifiers_of_unknown(unknown_node)
+                    log.debug(f"modifiers: {modifiers} --- clause modifiers: {[nd.form for nd in clause_modifiers]}")
+                    if f"{tree_desc[0].form.lower()} {tree_desc[1].form.lower()}" in self.change_root_tokens:
+                        new_root = root.children[0]
                     else:
-                        question = ' '.join([node.form for node in tree.descendants
-                                             if
-                                             (node.ord not in appos_token_nums or node.ord not in clause_token_nums)])
+                        new_root = root
+                    root_desc = defaultdict(list)
+                    for node in new_root.children:
+                        if node.deprel not in ["punct", "advmod", "cop", "mark"]:
+                            if node == unknown_branch:
+                                root_desc[node.deprel].append(node)
+                            else:
+                                if self.find_entities(node, positions) or \
+                                        (self.find_year_or_number(node) and node.deprel in ["obl", "nummod"]):
+                                    root_desc[node.deprel].append(node)
+
+                    if root.form.lower() == self.how_many or ("nsubj" in root_desc.keys() and
+                                                              self.how_many in [nd.form.lower() for nd in
+                                                                                root_desc["nsubj"]]):
+                        count = True
+                    log.debug(f"root_desc {root_desc.keys()}")
+                    self.root_entity = False
+                    if root.ord - 1 in positions:
+                        self.root_entity = True
+
+                    temporal_order = self.find_first_last(new_root)
+                    new_root_nf = self.nlp(new_root.form)[0].lemma_
+                    if new_root_nf in self.begin_tokens or new_root_nf in self.end_tokens:
+                        temporal_order = new_root_nf
+                    query_nums, s_substr_list, types_list = self.build_query(new_root, unknown_branch, root_desc,
+                                                                             unknown_node, modifiers, clause_modifiers,
+                                                                             clause_node, positions, entities_dict,
+                                                                             count, temporal_order, ranking_tokens)
+                    s_tags_list, s_probas_list = [], []
+                    for substr in s_substr_list:
+                        substr = substr.replace(" - ", "-")
+                        s_tags_list.append(entities_dict.get(substr.lower(), "E"))
+                        s_probas_list.append(probas_dict.get(substr.lower(), 1.0))
+            clean_questions_batch.append(question)
+            if query_nums and s_substr_list:
+                entities_to_link = [1 for _ in s_substr_list]
+                s_substr_list_lower = [s.lower() for s in s_substr_list]
+                for substr, tag, proba in zip(substr_list, tags_list, probas_list):
+                    if substr.lower() not in s_substr_list_lower:
+                        s_substr_list.append(substr)
+                        s_tags_list.append(tag)
+                        s_probas_list.append(proba)
+                        entities_to_link.append(0)
+                s_substr_batch.append(s_substr_list)
+                s_tags_batch.append(s_tags_list)
+                s_probas_batch.append(s_probas_list)
+                entities_to_link_batch.append(entities_to_link)
+            else:
+                mod_len = 0
+                gr_len = 1
+                if all([tags_list[i] == tags_list[0] for i in range(len(tags_list))]):
+                    gr_len = len(substr_list)
+                elif len(substr_list) > 1:
+                    mod_len = 1
+                for num, template in self.template_queries.items():
+                    syntax_info = [gr_len, 0, mod_len, 0, False, False, False]
+                    if syntax_info == list(template["syntax_structure"].values()):
+                        query_nums.append(num)
+                entities_to_link = [1 for _ in s_substr_list]
+                s_substr_batch.append(substr_list)
+                s_tags_batch.append(tags_list)
+                s_probas_batch.append(probas_list)
+                entities_to_link_batch.append(entities_to_link)
+            query_nums_batch.append(query_nums)
+            types_batch.append(types_list)
+        log.debug(f"clean_questions: {clean_questions_batch} --- substr: {s_substr_batch} --- tags: {s_tags_batch} "
+                  f"--- entities_to_link {entities_to_link_batch} --- types: {types_batch}")
+        return clean_questions_batch, query_nums_batch, s_substr_batch, s_tags_batch, s_probas_batch, \
+               entities_to_link_batch, types_batch
+
+    def sort_substr(self, substr_batch: List[List[str]], tags_batch: List[List[str]],
+                    offsets_batch: List[List[List[int]]], positions_batch: List[List[List[int]]],
+                    probas_batch: List[List[float]]) -> Tuple[
+        List[List[str]], List[List[str]], List[List[List[int]]], List[List[List[int]]], List[List[float]]]:
+        s_substr_batch, s_tags_batch, s_offsets_batch, s_positions_batch, s_probas_batch = [], [], [], [], []
+        for substr_list, tags_list, offsets_list, positions_list, probas_list \
+                in zip(substr_batch, tags_batch, offsets_batch, positions_batch, probas_batch):
+            substr_info = [(substr, tag, offsets, positions, proba) for substr, tag, offsets, positions, proba
+                           in zip(substr_list, tags_list, offsets_list, positions_list, probas_list)]
+            substr_info = sorted(substr_info, key=lambda x: x[3][0])
+            s_substr_batch.append([elem[0] for elem in substr_info])
+            s_tags_batch.append([elem[1] for elem in substr_info])
+            s_offsets_batch.append([elem[2] for elem in substr_info])
+            s_positions_batch.append([elem[3] for elem in substr_info])
+            s_probas_batch.append([elem[4] for elem in substr_info])
+        return s_substr_batch, s_tags_batch, s_offsets_batch, s_positions_batch, s_probas_batch
+
+    def syntax_parse(self, question: str, entity_offsets_list: List[List[int]]) -> Tuple[
+        Union[str, Any], Union[str, Any], Union[str, Any], str, str]:
+        syntax_tree = self.syntax_parser([question], [entity_offsets_list])[0]
+        log.debug(f"syntax tree: \n{syntax_tree}")
+        root, tree, tree_desc, unknown_node, unknown_branch = "", "", "", "", ""
+        try:
+            tree = Conllu(filehandle=StringIO(syntax_tree)).read_tree()
+            root = self.find_root(tree)
+            tree_desc = tree.descendants
+        except ValueError as e:
+            log.warning(f"error in parsing syntax tree, {e}")
+        if root:
+            unknown_node, unknown_branch = self.find_branch_with_unknown(root)
+            log.debug(f"syntax tree info, root: {root.form} unk_node: {unknown_node} unk_branch: {unknown_branch}")
+        return root, tree, tree_desc, unknown_node, unknown_branch
+
+    def sanitize_question(self, tree: Node, root: Node, appos_token_nums: List[int], clause_token_nums: List[int]) -> \
+            Tuple[str, list]:
+        ranking_tokens = self.find_ranking_tokens(root, appos_token_nums, clause_token_nums)
+        question_tokens = []
+        for node in tree.descendants:
+            if node.ord not in appos_token_nums + clause_token_nums:
+                if ranking_tokens and (node.ord in ranking_tokens or node.form.lower() in self.q_pronouns):
+                    question_tokens.append(self.nlp(node.form)[0].lemma_)
                 else:
-                    question = ' '.join([node.form for node in tree.descendants])
-                log.debug(f"sanitized question: {question}")
-                query_nums_batch.append(query_nums)
-                entities_dict_batch.append(entities_dict)
-                types_dict_batch.append(types_dict)
-                questions_batch.append(question)
-        return questions_batch, query_nums_batch, entities_dict_batch, types_dict_batch
+                    question_tokens.append(node.form)
+        question = " ".join(question_tokens)
+        log.debug(f"sanitized question: {question}")
+        return question, ranking_tokens
 
     def find_root(self, tree: Node) -> Node:
         for node in tree.descendants:
             if node.deprel == "root" and node.children:
                 return node
 
     def find_branch_with_unknown(self, root: Node) -> Tuple[str, str]:
         self.wh_leaf = False
         self.one_chain = False
-
         if root.form.lower() in self.q_pronouns:
             if "nsubj" in [node.deprel for node in root.children] or root.form.lower() in self.how_many:
                 self.one_chain = True
             else:
                 for node in root.children:
                     if node.deprel == "nsubj":
                         return node, node
-
         if not self.one_chain:
             for node in root.children:
                 if node.form.lower() in self.q_pronouns:
                     if node.children:
                         for child in node.children:
                             if child.deprel in ["nmod", "obl"]:
                                 return child, node
                     else:
                         self.wh_leaf = True
                 else:
                     for child in node.descendants:
                         if child.form.lower() in self.q_pronouns:
                             return child.parent, node
-
         if self.wh_leaf or self.one_chain:
             for node in root.children:
                 if node.deprel in ["nsubj", "obl", "obj", "nmod", "xcomp"] and node.form.lower() not in self.q_pronouns:
                     return node, node
 
         return "", ""
 
@@ -363,183 +562,138 @@
         for node in root.children:
             if node.deprel == "obl" and node != unknown_branch:
                 for elem in node.children:
                     if elem.deprel == "acl":
                         return elem, node
         return "", ""
 
-    def find_named_entity(self, node: Node, conj_list: List[Node], desc_list: List[Tuple[str, int]],
-                          positions: List[int], cut_clause: bool) -> List[Tuple[str, int]]:
-        if node.children:
-            if self.find_nmod_appos(node, positions):
-                used_desc = [elem for elem in node.children if elem.deprel == "appos"]
-            else:
-                used_desc = node.children
-
-            for elem in used_desc:
-                if self.check_node(elem, conj_list, cut_clause):
-                    desc_list = self.find_named_entity(elem, conj_list, desc_list, positions, cut_clause)
-        log.debug(f"find_named_entity: node.ord, {node.ord - 1}, {node.form}, positions, {positions}")
-        log.debug(f"find nmod appos {self.find_nmod_appos(node, positions)}")
-        if node.ord - 1 in positions:
-            initials_3 = re.findall("([А-Яа-я]{1}\.)([А-Яа-я]{1}\.)([А-Яа-я]{3,15})", node.form)
-            initials_2 = re.findall("([А-Яа-я]{1}\.)([А-Яа-я]{3,15})", node.form)
-            if initials_3:
-                entity_substring = ' '.join(initials_3[0])
-            elif initials_2:
-                entity_substring = ' '.join(initials_2[0])
-            else:
-                entity_substring = node.form
-            desc_list.append((entity_substring, node.ord))
-
-        return desc_list
-
-    def check_node(self, elem: Node, conj_list: List[Node], cut_clause: bool) -> bool:
-        """
-        This function defines whether to go deeper in the syntactic tree to look for named entity tokens
-        If all the conditions are true, then we recursively look for named entity tokens in elem's descendants.
-        Args:
-            elem: node of the syntactic tree for which we decide whether to look for named entities in its descendants
-            conj_list: list of nodes, connected with the "elem" node with "conj" deprel
-            cut_clause: if cut_clause is True, we do not want to look for named entities in adjective clauses ("acl")
-        """
-        move_deeper = False
-        if not cut_clause or (cut_clause and elem.deprel != "acl"):
-            if elem not in conj_list:
-                if elem.deprel != "appos" or \
-                        (elem.deprel == "appos"
-                         and (not elem.children or
-                              (len(elem.children) == 1 and elem.children[0].deprel in ["flat:name", "parataxis"]) or
-                              (len(elem.children) > 1 and {"«", '"', '``', '('} & {nd.form for nd in
-                                                                                   elem.descendants}))):
-                    move_deeper = True
-        return move_deeper
-
-    def find_conj(self, node: Node, conj_list: List[Node], positions: List[int], cut_clause: bool) -> List[Node]:
-        if node.children:
-            for elem in node.children:
-                if not cut_clause or (cut_clause and elem.deprel != "acl"):
-                    conj_list = self.find_conj(elem, conj_list, positions, cut_clause)
-
-        if node.deprel == "conj":
-            conj_in_ner = False
-            for elem in node.children:
-                if elem.deprel == "cc" and (elem.ord - 1) in positions:
-                    conj_in_ner = True
-            if not conj_in_ner:
-                conj_list.append(node)
-
-        return conj_list
-
-    def find_entities(self, node: Node, positions: List[int], cut_clause: bool = True) -> List[str]:
-        entities_list = []
-        conj_list = self.find_conj(node, [], positions, cut_clause)
-        entity = self.find_entity(node, conj_list, positions, cut_clause)
-        if entity:
-            entities_list.append(entity)
-        if conj_list:
-            for conj_node in conj_list:
-                curr_conj_list = [elem for elem in conj_list if elem != conj_node]
-                entity = self.find_entity(conj_node, curr_conj_list, positions, cut_clause)
+    def find_entities(self, node: Node, positions: List[List[int]]) -> List[str]:
+        node_desc = [(node.form, node.ord, node.parent)] + \
+                    [(elem.form, elem.ord, elem.parent) for elem in node.descendants]
+        node_desc = sorted(node_desc, key=lambda x: x[1])
+        entities_list, heads_list = [], []
+        for pos_elem in positions:
+            entity, parents = [], []
+            for ind in pos_elem:
+                for node_elem in node_desc:
+                    if ind + 1 == node_elem[1]:
+                        entity.append(node_elem[0])
+                        parents.append(node_elem[2])
+                        break
+            if len(entity) == len(pos_elem):
+                entity = " ".join(entity).replace(" .", ".")
                 entities_list.append(entity)
-        log.debug(f"found_entities, {entities_list}")
+                heads_list.append(parents[0])
+        log.debug(f"node: {node.form} --- found_entities: {entities_list} --- node_desc: {node_desc} --- "
+                  f"positions: {positions}")
         return entities_list
 
-    def find_entity(self, node: Node, conj_list: List[Node], positions: List[int], cut_clause: bool) -> str:
-        grounded_entity_tokens = self.find_named_entity(node, conj_list, [], positions, cut_clause)
-        grounded_entity = sorted(grounded_entity_tokens, key=lambda x: x[1])
-        grounded_entity = " ".join([entity[0] for entity in grounded_entity])
-        return grounded_entity
-
-    def find_nmod_appos(self, node: Node, positions: List[int]) -> bool:
-        node_desc = {elem.deprel: elem for elem in node.children}
-        node_deprels = sorted([elem.deprel for elem in node.children if elem.deprel != "case"])
-        if node.ord - 1 in positions:
-            return False
-        elif node_deprels == ["appos", "nmod"] and node_desc["appos"].ord - 1 in positions \
-                and node_desc["nmod"].ord in positions:
-            return True
-        return False
-
     def find_year_or_number(self, node: Node) -> bool:
         found = False
         for elem in node.descendants:
-            if elem.deprel == "nummod":
+            if elem.deprel == "nummod" or re.findall(r"[\d]{4}", elem.form):
                 return True
         return found
 
-    def find_appos_tokens(self, node: Node, appos_token_nums: List[int]) -> List[int]:
+    def find_year_constraint(self, node: Node) -> list:
+        node_desc = [(node.form, node.ord)] + [(elem.form, elem.ord) for elem in node.descendants]
+        node_desc = sorted(node_desc, key=lambda x: x[1])
+        desc_text = " ".join([elem[0] for elem in node_desc])
+        for symb in ".,:;)":
+            desc_text = desc_text.replace(f" {symb}", symb)
+        for pattern in [r"в ([\d]{3,4}) году", r"с ([\d]{3,4}) по ([\d]{3,4})"]:
+            fnd = re.findall(pattern, desc_text)
+            if fnd:
+                return fnd
+        return []
+
+    def find_appos_tokens(self, node: Node, tok_and_ord: List[Tuple[Node, int]],
+                          appos_token_nums: List[int]) -> List[int]:
         for elem in node.children:
-            if elem.deprel == "appos" and (len(elem.descendants) > 1 and
-                                           not {"«", '"', '``', '('} & {nd.form for nd in elem.descendants} or
-                                           (len(elem.descendants) == 1 and elem.descendants[0].deprel != "flat:name")):
+            e_desc = elem.descendants
+            if elem.deprel == "appos" and elem.ord > 1 and tok_and_ord[elem.ord - 1].deprel == "punct" \
+                    and not all([nd.deprel in {"appos", "flat:name"} for nd in e_desc]) \
+                    and not ({"«", '"', '``', '('} & {nd.form for nd in e_desc}):
                 appos_token_nums.append(elem.ord)
                 for desc in elem.descendants:
                     appos_token_nums.append(desc.ord)
             else:
-                appos_token_nums = self.find_appos_tokens(elem, appos_token_nums)
+                appos_token_nums = self.find_appos_tokens(elem, tok_and_ord, appos_token_nums)
         return appos_token_nums
 
-    def find_clause_tokens(self, node: Node, clause_node: Node, clause_token_nums: List[int]) -> List[int]:
+    def find_clause_tokens(self, node: Node, tok_and_ord: Dict[int, Node], clause_node: Node) -> List[int]:
+        clause_token_nums = []
         for elem in node.children:
             if elem != clause_node and elem.deprel == "acl":
                 clause_token_nums.append(elem.ord)
                 for desc in elem.descendants:
                     clause_token_nums.append(desc.ord)
             else:
-                clause_token_nums = self.find_appos_tokens(elem, clause_token_nums)
+                clause_token_nums = self.find_appos_tokens(elem, tok_and_ord, clause_token_nums)
         return clause_token_nums
 
     def find_first_last(self, node: Node) -> str:
         first_or_last = ""
         nodes = [node]
         while nodes:
             for node in nodes:
                 node_desc = defaultdict(set)
                 for elem in node.children:
-                    parsed_elem = self.nlp(elem.form.lower())[0].lemma_
-                    if parsed_elem is not None:
-                        node_desc[elem.deprel].add(parsed_elem)
-                    else:
-                        node_desc[elem.deprel].add(elem.form)
+                    normal_form = self.nlp(elem.form.lower())[0].lemma_
+                    node_desc[elem.deprel].add(normal_form)
+                log.debug(f"find_first_last {node_desc}")
                 if "amod" in node_desc.keys() and "nmod" in node_desc.keys() and \
                         node_desc["amod"].intersection(self.first_tokens | self.last_tokens):
                     first_or_last = ' '.join(node_desc["amod"].intersection(self.first_tokens | self.last_tokens))
                     return first_or_last
             nodes = [elem for node in nodes for elem in node.children]
         return first_or_last
 
-    def find_ranking_tokens(self, node: Node) -> list:
+    def find_ranking_tokens(self, node: Node, appos_token_nums: List[int], clause_token_nums: List[int]) -> list:
         ranking_tokens = []
         for elem in node.descendants:
-            if self.nlp(elem.form)[0].lemma_ in self.ranking_tokens:
+            if self.nlp(elem.form)[0].lemma_ in self.ranking_tokens \
+                    and elem.ord not in appos_token_nums + clause_token_nums:
                 ranking_tokens.append(elem.ord)
                 ranking_tokens.append(elem.parent.ord)
                 return ranking_tokens
         return ranking_tokens
 
-    def build_query(self, root: Node, unknown_branch: Node, root_desc: Dict[str, List[Node]],
-                    unknown_node: Node, unknown_modifiers: List[Node], clause_modifiers: List[Node],
-                    clause_node: Node, positions: List[int],
-                    count: bool = False, temporal_order: str = "",
-                    ranking_tokens: List[str] = None) -> Tuple[List[str], List[str], List[str]]:
+    @staticmethod
+    def choose_grounded_entity(grounded_entities: List[str], entities_dict: Dict[str, str]):
+        tags = [entities_dict.get(entity.lower(), "") for entity in grounded_entities]
+        if len(grounded_entities) > 1:
+            if not all([tags[i] == tags[0] for i in range(1, len(tags))]):
+                for f_tag in ["WORK_OF_ART", "FAC", "PERSON", "GPE"]:
+                    for entity, tag in zip(grounded_entities, tags):
+                        if tag == f_tag:
+                            return [entity]
+            elif not all([entity[0].islower() for entity in grounded_entities]):
+                for entity in grounded_entities:
+                    if entity[0].isupper():
+                        return [entity]
+        return grounded_entities
+
+    def build_query(self, root: Node, unknown_branch: Node, root_desc: Dict[str, List[Node]], unknown_node: Node,
+                    unknown_modifiers: List[Node], clause_modifiers: List[Node], clause_node: Node,
+                    positions: List[List[int]], entities_dict: Dict[str, str], count: bool = False,
+                    temporal_order: str = "", ranking_tokens: List[str] = None) -> Tuple[
+        List[str], List[str], List[str]]:
         query_nums = []
-        grounded_entities_list = []
-        types_list = []
-        modifiers_list = []
-        qualifier_entities_list = []
+        grounded_entities_list, types_list, modifiers_list, qualifier_entities_list = [], [], [], []
         found_year_or_number = False
         order = False
         root_desc_deprels = []
         for key in root_desc.keys():
             for i in range(len(root_desc[key])):
-                root_desc_deprels.append(key)
+                if key in {"nsubj", "obj", "obl", "iobj", "acl", "nmod", "xcomp", "cop"}:
+                    root_desc_deprels.append(key)
         root_desc_deprels = sorted(root_desc_deprels)
-        log.debug(f"build_query: root_desc.keys, {root_desc_deprels}, positions {positions}")
-        log.debug(f"temporal order {temporal_order}, ranking tokens {ranking_tokens}")
+        log.debug(f"build_query: root_desc.keys, {root_desc_deprels}, positions {positions}, wh_leaf {self.wh_leaf}, "
+                  f"one_chain {self.one_chain}, temporal order {temporal_order}, ranking tokens {ranking_tokens}")
         if root_desc_deprels in [["nsubj", "obl"],
                                  ["nsubj", "obj"],
                                  ["nsubj", "xcomp"],
                                  ["obj", "xcomp"],
                                  ["nmod", "nsubj"],
                                  ["obj", "obl"],
                                  ["iobj", "nsubj"],
@@ -548,129 +702,155 @@
                                  ["obj"],
                                  ["obl"],
                                  ["nmod"],
                                  ["xcomp"],
                                  ["nsubj"]]:
             if self.wh_leaf or self.one_chain:
                 if root_desc_deprels == ["nsubj", "obl"]:
-                    grounded_entities_list = self.find_entities(root_desc["nsubj"][0], positions, cut_clause=True)
+                    grounded_entities_list = self.find_entities(root_desc["nsubj"][0], positions)
                     if not grounded_entities_list:
-                        grounded_entities_list = self.find_entities(root_desc["obl"][0], positions, cut_clause=True)
+                        grounded_entities_list = self.find_entities(root_desc["obl"][0], positions)
                 else:
                     for nodes in root_desc.values():
                         if nodes[0].form not in self.q_pronouns:
-                            grounded_entities_list = self.find_entities(nodes[0], positions, cut_clause=True)
+                            grounded_entities_list = self.find_entities(nodes[0], positions)
                             if grounded_entities_list:
                                 break
             else:
                 if self.root_entity:
                     grounded_entities_list = [root.form]
                 for nodes in root_desc.values():
                     if nodes[0] != unknown_branch:
-                        grounded_entities_list = self.find_entities(nodes[0], positions, cut_clause=True)
+                        grounded_entities_list = self.find_entities(nodes[0], positions)
                         if grounded_entities_list:
                             type_entity = unknown_node.form
                             types_list.append(type_entity)
                             break
 
                 if unknown_modifiers:
                     for n, modifier in enumerate(unknown_modifiers):
                         if isinstance(modifier, str):
                             modifiers_list.append(modifier)
                         else:
-                            modifier_entities = self.find_entities(modifier, positions, cut_clause=True)
+                            modifier_entities = self.find_entities(modifier, positions)
                             if modifier_entities:
                                 modifiers_list += modifier_entities
                 if clause_modifiers:
                     found_year_or_number = self.find_year_or_number(clause_modifiers[0])
                     if found_year_or_number:
                         query_nums.append("0")
-                    qualifier_entities_list = self.find_entities(clause_modifiers[0], positions, cut_clause=True)
+                    qualifier_entities_list = self.find_entities(clause_modifiers[0], positions)
 
         if root_desc_deprels == ["nsubj", "obl", "obl"]:
-            grounded_entities_list = self.find_entities(root_desc["nsubj"][0], positions, cut_clause=True)
+            grounded_entities_list = self.find_entities(root_desc["nsubj"][0], positions)
             for node in root_desc["obl"]:
                 if node == unknown_branch:
                     types_list.append(node.form)
                 else:
-                    grounded_entities_list += self.find_entities(node, positions, cut_clause=True)
+                    grounded_entities_list += self.find_entities(node, positions)
+
+        if root_desc_deprels == ["nsubj", "obj", "obj"]:
+            obj_desc = root_desc["obj"]
+            qualifier_entities_list = self.find_entities(obj_desc[0], positions)
+            grounded_entities_list = self.find_entities(obj_desc[1], positions)
+
+        year_constraint = self.find_year_constraint(root)
+        if root_desc_deprels == ["nmod", "nsubj"] and year_constraint:
+            if len(year_constraint[0]) == 2:
+                query_nums.append("24")
+            elif len(year_constraint[0]) == 1:
+                query_nums.append("0")
 
         if root_desc_deprels == ["obj", "xcomp"]:
-            grounded_entities_list = self.find_entities(root_desc["xcomp"][0], positions, cut_clause=True)
+            grounded_entities_list = self.find_entities(root_desc["xcomp"][0], positions)
 
-        if root_desc_deprels == ["nsubj", "obj", "obl"] or root_desc_deprels == ["obj", "obl"] and self.wh_leaf:
+        if (self.wh_leaf and root_desc_deprels in [["nsubj", "obj", "obl"], ["obj", "obl"]]) \
+                or (root_desc_deprels in [["nsubj", "obj", "obl"], ["obl", "xcomp"]]
+                    and self.find_year_or_number(root_desc["obl"][0])):
             found_year_or_number = self.find_year_or_number(root_desc["obl"][0])
+            nsubj_ent_list, obj_ent_list = [], []
+            if "nsubj" in root_desc_deprels:
+                nsubj_ent_list = self.find_entities(root_desc["nsubj"][0], positions)
+            if "obj" in root_desc:
+                obj_ent_list = self.find_entities(root_desc["obj"][0], positions)
+            obl_ent_list = self.find_entities(root_desc["obl"][0], positions)
+            log.debug(f"nsubj_ent: {nsubj_ent_list} --- obj_ent: {obj_ent_list} obl_ent: {obl_ent_list}")
             if self.wh_leaf:
-                grounded_entities_list = self.find_entities(root_desc["obl"][0], positions, cut_clause=True)
-                qualifier_entities_list = self.find_entities(root_desc["obj"][0], positions, cut_clause=True)
+                grounded_entities_list = obl_ent_list
+                qualifier_entities_list = obj_ent_list
+            elif not found_year_or_number and nsubj_ent_list and obl_ent_list:
+                grounded_entities_list = nsubj_ent_list
+                modifiers_list = obl_ent_list
             else:
-                grounded_entities_list = self.find_entities(root_desc["obj"][0], positions, cut_clause=True)
-                if found_year_or_number:
-                    query_nums.append("0")
+                grounded_entities_list = obj_ent_list
+            if found_year_or_number:
+                query_nums.append("0")
+            if not grounded_entities_list:
+                grounded_entities_list = self.find_entities(root, positions)
+                grounded_entities_list = self.choose_grounded_entity(grounded_entities_list, entities_dict)
 
         if clause_node:
             for node in clause_node.children:
                 if node.deprel == "obj":
-                    grounded_entities_list = self.find_entities(node, positions, cut_clause=False)
+                    grounded_entities_list = self.find_entities(node, positions)
                 if self.find_year_or_number(node):
                     query_nums.append("0")
 
             if not self.wh_leaf:
                 type_entity = unknown_node.form
                 types_list.append(type_entity)
 
         if root_desc_deprels == ["nmod", "nmod"]:
-            grounded_entities_list = self.find_entities(root_desc["nmod"][0], positions, cut_clause=True)
-            modifiers_list = self.find_entities(root_desc["nmod"][1], positions, cut_clause=True)
+            grounded_entities_list = self.find_entities(root_desc["nmod"][0], positions)
+            modifiers_list = self.find_entities(root_desc["nmod"][1], positions)
 
         if root_desc_deprels == ["nmod", "nsubj", "nummod"]:
             if not self.wh_leaf:
-                grounded_entities_list = self.find_entities(root_desc["nmod"][0], positions, cut_clause=True)
+                grounded_entities_list = self.find_entities(root_desc["nmod"][0], positions)
                 found_year_or_number = self.find_year_or_number(root_desc["nummod"][0])
 
-        if temporal_order:
+        if temporal_order and not query_nums:
             for deprel in root_desc:
                 for node in root_desc[deprel]:
-                    entities = self.find_entities(node, positions, cut_clause=True)
+                    entities = self.find_entities(node, positions)
                     if entities:
                         grounded_entities_list = entities
                         break
                 if grounded_entities_list:
                     break
-            if temporal_order in self.first_tokens:
-                query_nums.append("22")
-                query_nums.append("23")
-            if temporal_order in self.last_tokens:
-                query_nums.append("24")
-            if temporal_order in self.begin_tokens:
-                query_nums.append("22")
-                query_nums.append("25")
-            if temporal_order in self.end_tokens:
-                query_nums.append("24")
-                query_nums.append("26")
+            if temporal_order in self.first_tokens | self.begin_tokens:
+                query_nums += ["22"]
+            if temporal_order in self.last_tokens | self.end_tokens:
+                query_nums += ["23"]
+        log.debug(f"query_nums: {query_nums} --- year_constraint: {year_constraint}")
 
         if count:
-            grounded_entities_list = self.find_entities(root, positions, cut_clause=True)
+            grounded_entities_list = self.find_entities(root, positions)
 
+        grounded_entities_list = self.choose_grounded_entity(grounded_entities_list, entities_dict)
         entities_list = grounded_entities_list + qualifier_entities_list + modifiers_list
+        types_list = [tp for tp in types_list
+                      if not (len(tp.split()) == 1 and self.nlp(tp)[0].lemma_ in self.date_tokens)]
 
-        grounded_entities_length = len(grounded_entities_list)
-        types_length = len(types_list)
-        modifiers_length = len(modifiers_list)
-        qualifiers_length = len(qualifier_entities_list)
-        if qualifiers_length > 0 or modifiers_length or count:
-            types_length = 0
+        gr_len = len(grounded_entities_list)
+        types_len = len(types_list)
+        mod_len = len(modifiers_list)
+        qua_len = len(qualifier_entities_list)
+        if qua_len or count:
+            types_len = 0
 
-        if not temporal_order:
+        if not temporal_order and not query_nums:
             for num, template in self.template_queries.items():
-                if [grounded_entities_length, types_length, modifiers_length,
-                    qualifiers_length, found_year_or_number, count, order] == list(
-                    template["syntax_structure"].values()):
+                syntax_info = [gr_len, types_len, mod_len, qua_len, found_year_or_number, count, order]
+                if syntax_info == list(template["syntax_structure"].values()):
                     query_nums.append(num)
-
-        log.debug(f"tree_to_sparql, grounded entities {grounded_entities_list}")
-        log.debug(f"tree_to_sparql, types {types_list}")
-        log.debug(f"tree_to_sparql, modifier entities {modifiers_list}")
-        log.debug(f"tree_to_sparql, qualifier entities {qualifier_entities_list}")
-        log.debug(f"tree to sparql, query nums {query_nums}")
+                if mod_len:
+                    syntax_info[1] = 0
+                    if syntax_info == list(template["syntax_structure"].values()):
+                        query_nums.append(num)
+
+        log.debug(f"tree_to_sparql, grounded entities: {grounded_entities_list} --- types: {types_list} --- "
+                  f"modifier entities: {modifiers_list} --- qualifier entities: {qualifier_entities_list} --- "
+                  f"year_or_number {found_year_or_number} --- count: {count} --- order: {order} --- "
+                  f"query nums: {query_nums}")
 
         return query_nums, entities_list, types_list
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/kbqa/type_define.py` & `deeppavlov-1.2.0/deeppavlov/models/kbqa/type_define.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         with open(self.types_filename, 'rb') as fl:
             self.types_dict = pickle.load(fl)
         with open(self.types_sets_filename, 'rb') as fl:
             self.types_sets = pickle.load(fl)
 
     def __call__(self, questions_batch: List[str], entity_substr_batch: List[List[str]],
                  tags_batch: List[List[str]], types_substr_batch: List[List[str]] = None):
-        types_sets_batch = []
         if types_substr_batch is None:
             types_substr_batch = []
             for question, entity_substr_list in zip(questions_batch, entity_substr_batch):
                 types_substr = []
                 type_noun = ""
                 doc = self.nlp(question)
                 token_pos_dict = {}
@@ -79,64 +78,47 @@
                             type_adj = token.text
                             if not any([type_adj.lower() in entity_substr.lower() for entity_substr in
                                         entity_substr_list]):
                                 types_substr.append(type_adj)
                             break
                         elif token.head.text == type_noun and token.dep_ == "prep":
                             if len(list(token.children)) == 1 \
-                                    and not any([[tok.text for tok in token.children][0] in entity_substr.lower()
+                                    and not any([list(token.children)[0].text in entity_substr.lower()
                                                  for entity_substr in entity_substr_list]):
-                                types_substr += [token.text, [tok.text for tok in token.children][0]]
+                                types_substr += [token.text, list(token.children)[0].text]
                 elif any([word in question for word in self.pronouns]):
                     for token in doc:
                         if token.dep_ == "nsubj" and not any([token.text in entity_substr.lower()
                                                               for entity_substr in entity_substr_list]):
                             types_substr.append(token.text)
-
                 types_substr = [(token, token_pos_dict[token]) for token in types_substr]
                 types_substr = sorted(types_substr, key=lambda x: x[1])
                 types_substr = " ".join([elem[0] for elem in types_substr])
                 types_substr_batch.append(types_substr)
-        for types_substr in types_substr_batch:
-            types_substr_tokens = types_substr.split()
-            types_substr_tokens = [tok for tok in types_substr_tokens if tok not in self.stopwords]
-            if self.lang == "@ru":
-                types_substr_tokens = [self.nlp(tok)[0].lemma_ for tok in types_substr_tokens]
-            types_substr_tokens = set(types_substr_tokens)
-            types_scores = []
-            for entity in self.types_dict:
-                labels, cnt = self.types_dict[entity]
-                cur_cnts = []
-                for label in labels:
-                    label_tokens = label.lower().split()
-                    if len(types_substr_tokens) == 1 and len(label_tokens) == 2 and \
-                            list(types_substr_tokens)[0] == label_tokens[0]:
-                        cur_cnts.append(0.3)
-                    else:
-                        inters = types_substr_tokens.intersection(set(label_tokens))
-                        cur_cnts.append(len(inters) / max(len(types_substr_tokens), len(label_tokens)))
-
-                types_scores.append([entity, max(cur_cnts), cnt])
-            types_scores = sorted(types_scores, key=lambda x: (x[1], x[2]), reverse=True)
-            cur_types = [elem[0] for elem in types_scores if elem[1] > 0][:self.num_types_to_return]
-            types_sets_batch.append(cur_types)
-
+        types_sets_batch = [set() for _ in questions_batch]
         for n, (question, types_sets) in enumerate(zip(questions_batch, types_sets_batch)):
             question = question.lower()
             if not types_sets:
                 if self.lang == "@ru":
                     if question.startswith("кто"):
                         types_sets_batch[n] = self.types_sets["PER"]
                     elif question.startswith("где"):
                         types_sets_batch[n] = self.types_sets["LOC"]
+                    elif any([question.startswith(elem) for elem in ["когда", "в каком году", "в каком месяце"]]):
+                        types_sets_batch[n] = {"date"}
+                    elif len(question.split()) > 1 and (any([question.startswith(elem) for elem in ["кем ", "как"]]) \
+                                                        or question.split()[1].startswith("как")):
+                        types_sets_batch[n] = {"not_date"}
                 elif self.lang == "@en":
                     if question.startswith("who"):
                         types_sets_batch[n] = self.types_sets["PER"]
                     elif question.startswith("where"):
                         types_sets_batch[n] = self.types_sets["LOC"]
+                    elif any([question.startswith(elem) for elem in ["when", "what year", "what month"]]):
+                        types_sets_batch[n] = {"date"}
 
         new_entity_substr_batch, new_entity_offsets_batch, new_tags_batch = [], [], []
         for question, entity_substr_list, tags_list in zip(questions_batch, entity_substr_batch, tags_batch):
             new_entity_substr, new_tags = [], []
             if not entity_substr_list:
                 doc = self.nlp(question)
                 for token in doc:
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/kbqa/wiki_parser.py` & `deeppavlov-1.2.0/deeppavlov/models/kbqa/wiki_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,34 +10,35 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 import re
+from collections import namedtuple
 from logging import getLogger
 from typing import List, Tuple, Dict, Any, Union
-from collections import namedtuple
 
 from hdt import HDTDocument
 
-from deeppavlov.core.common.file import load_pickle
 from deeppavlov.core.commands.utils import expand_path
+from deeppavlov.core.common.file import load_pickle, read_json
 from deeppavlov.core.common.registry import register
 
 log = getLogger(__name__)
 
 
 @register('wiki_parser')
 class WikiParser:
     """This class extract relations, objects or triplets from Wikidata HDT file."""
 
     def __init__(self, wiki_filename: str,
                  file_format: str = "hdt",
                  prefixes: Dict[str, Union[str, Dict[str, str]]] = None,
+                 rel_q2name_filename: str = None,
                  max_comb_num: int = 1e6,
                  lang: str = "@en", **kwargs) -> None:
         """
 
         Args:
             wiki_filename: file with Wikidata
             file_format: format of Wikidata file
@@ -51,57 +52,77 @@
                 "label": "http://wl",
                 "alias": "http://wal",
                 "description": "http://wd",
                 "rels": {
                     "direct": "http://wpd",
                     "no_type": "http://wp",
                     "statement": "http://wps",
-                    "qualifier": "http://wpq"
+                    "qualifier": "http://wpq",
+                    "type": "http://wpd/P31"
                 },
                 "statement": "http://ws"
             }
         self.prefixes = prefixes
         self.file_format = file_format
         self.wiki_filename = str(expand_path(wiki_filename))
         if self.file_format == "hdt":
             self.document = HDTDocument(self.wiki_filename)
         elif self.file_format == "pickle":
             self.document = load_pickle(self.wiki_filename)
             self.parsed_document = {}
         else:
             raise ValueError("Unsupported file format")
+        self.used_rels = set()
+        self.rel_q2name = dict()
+        if rel_q2name_filename:
+            if rel_q2name_filename.endswith("json"):
+                self.rel_q2name = read_json(str(expand_path(rel_q2name_filename)))
+            elif rel_q2name_filename.endswith("pickle"):
+                self.rel_q2name = load_pickle(str(expand_path(rel_q2name_filename)))
+            else:
+                raise ValueError(f"Unsupported file format: {rel_q2name_filename}")
 
         self.max_comb_num = max_comb_num
         self.lang = lang
+        self.replace_tokens = [('"', ''), (self.lang, " "), ('$', ' '), ('  ', ' ')]
 
     def __call__(self, parser_info_list: List[str], queries_list: List[Any]) -> List[Any]:
         wiki_parser_output = self.execute_queries_list(parser_info_list, queries_list)
         return wiki_parser_output
 
     def execute_queries_list(self, parser_info_list: List[str], queries_list: List[Any]):
         wiki_parser_output = []
         query_answer_types = []
         for parser_info, query in zip(parser_info_list, queries_list):
             if parser_info == "query_execute":
-                candidate_output = []
+                answers, found_rels, found_combs = [], [], []
                 try:
-                    what_return, query_seq, filter_info, order_info, answer_types, rel_types, return_if_found = query
+                    what_return, rels_from_query, query_seq, filter_info, order_info, answer_types, rel_types, \
+                    return_if_found = query
                     if answer_types:
                         query_answer_types = answer_types
-                    candidate_output = self.execute(what_return, query_seq, filter_info, order_info,
-                                                    query_answer_types, rel_types)
-                except:
+                    answers, found_rels, found_combs = \
+                        self.execute(what_return, rels_from_query, query_seq, filter_info, order_info,
+                                     query_answer_types, rel_types)
+                except ValueError:
                     log.warning("Wrong arguments are passed to wiki_parser")
-                wiki_parser_output.append(candidate_output)
+                wiki_parser_output.append([answers, found_rels, found_combs])
             elif parser_info == "find_rels":
                 rels = []
                 try:
                     rels = self.find_rels(*query)
                 except:
                     log.warning("Wrong arguments are passed to wiki_parser")
+                wiki_parser_output.append(rels)
+            elif parser_info == "find_rels_2hop":
+                rels = []
+                try:
+                    rels = self.find_rels_2hop(*query)
+                except ValueError:
+                    log.warning("Wrong arguments are passed to wiki_parser")
                 wiki_parser_output += rels
             elif parser_info == "find_object":
                 objects = []
                 try:
                     objects = self.find_object(*query)
                 except:
                     log.warning("Wrong arguments are passed to wiki_parser")
@@ -123,14 +144,21 @@
             elif parser_info == "find_types":
                 types = []
                 try:
                     types = self.find_types(query)
                 except:
                     log.warning("Wrong arguments are passed to wiki_parser")
                 wiki_parser_output.append(types)
+            elif parser_info == "fill_triplets":
+                filled_triplets = []
+                try:
+                    filled_triplets = self.fill_triplets(*query)
+                except ValueError:
+                    log.warning("Wrong arguments are passed to wiki_parser")
+                wiki_parser_output.append(filled_triplets)
             elif parser_info == "find_triplets":
                 if self.file_format == "hdt":
                     triplets = []
                     try:
                         triplets_forw, c = self.document.search_triples(f"{self.prefixes['entity']}/{query}", "", "")
                         triplets.extend([triplet for triplet in triplets_forw
                                          if not triplet[2].startswith(self.prefixes["statement"])])
@@ -167,49 +195,50 @@
                 wiki_parser_output.append("ok")
             else:
                 raise ValueError("Unsupported query type")
 
         return wiki_parser_output
 
     def execute(self, what_return: List[str],
+                rels_from_query: List[str],
                 query_seq: List[List[str]],
                 filter_info: List[Tuple[str]] = None,
                 order_info: namedtuple = None,
                 answer_types: List[str] = None,
-                rel_types: List[str] = None) -> List[List[str]]:
+                rel_types: List[str] = None):
         """
             Let us consider an example of the question "What is the deepest lake in Russia?"
             with the corresponding SPARQL query            
             "SELECT ?ent WHERE { ?ent wdt:P31 wd:T1 . ?ent wdt:R1 ?obj . ?ent wdt:R2 wd:E1 } ORDER BY ASC(?obj) LIMIT 5"
 
             arguments:
                 what_return: ["?obj"]
                 query_seq: [["?ent", "http://www.wikidata.org/prop/direct/P17", "http://www.wikidata.org/entity/Q159"]
                             ["?ent", "http://www.wikidata.org/prop/direct/P31", "http://www.wikidata.org/entity/Q23397"],
                             ["?ent", "http://www.wikidata.org/prop/direct/P4511", "?obj"]]
                 filter_info: []
                 order_info: order_info(variable='?obj', sorting_order='asc')
         """
         extended_combs = []
-        combs = []
+        answers, found_rels, found_combs = [], [], []
 
         for n, (query, rel_type) in enumerate(zip(query_seq, rel_types)):
             unknown_elem_positions = [(pos, elem) for pos, elem in enumerate(query) if elem.startswith('?')]
             """
                 n = 0, query = ["?ent", "http://www.wikidata.org/prop/direct/P17",
-                                                                            "http://www.wikidata.org/entity/Q159"]
+                                "http://www.wikidata.org/entity/Q159"]
                        unknown_elem_positions = ["?ent"]
                 n = 1, query = ["?ent", "http://www.wikidata.org/prop/direct/P31",
-                                                                        "http://www.wikidata.org/entity/Q23397"]
+                                "http://www.wikidata.org/entity/Q23397"]
                        unknown_elem_positions = [(0, "?ent")]
                 n = 2, query = ["?ent", "http://www.wikidata.org/prop/direct/P4511", "?obj"]
                        unknown_elem_positions = [(0, "?ent"), (2, "?obj")]
             """
             if n == 0:
-                combs = self.search(query, unknown_elem_positions, rel_type)
+                combs, triplets = self.search(query, unknown_elem_positions, rel_type)
                 # combs = [{"?ent": "http://www.wikidata.org/entity/Q5513"}, ...]
             else:
                 if combs:
                     known_elements = []
                     extended_combs = []
                     if query[0].startswith("?"):
                         for elem in query:
@@ -226,79 +255,130 @@
                                                 "http://www.wikidata.org/prop/direct/P31", 
                                                 "http://www.wikidata.org/entity/Q23397"]
                                 new_combs = [["http://www.wikidata.org/entity/Q5513", 
                                               "http://www.wikidata.org/prop/direct/P31", 
                                               "http://www.wikidata.org/entity/Q23397"], ...]
                                 extended_combs = [{"?ent": "http://www.wikidata.org/entity/Q5513"}, ...]
                             """
-                            known_values = [comb[known_elem] for known_elem in known_elements]
-                            for known_elem, known_value in zip(known_elements, known_values):
-                                filled_query = [elem.replace(known_elem, known_value) for elem in query]
-                                new_combs = self.search(filled_query, unknown_elem_positions, rel_type)
-                                for new_comb in new_combs:
-                                    extended_combs.append({**comb, **new_comb})
+                            if comb:
+                                known_values = [comb[known_elem] for known_elem in known_elements]
+                                for known_elem, known_value in zip(known_elements, known_values):
+                                    filled_query = [elem.replace(known_elem, known_value) for elem in query]
+                                    new_combs, triplets = self.search(filled_query, unknown_elem_positions, rel_type)
+                                    for new_comb in new_combs:
+                                        extended_combs.append(self.merge_combs(comb, new_comb))
                     else:
-                        new_combs = self.search(query, unknown_elem_positions, rel_type)
+                        new_combs, triplets = self.search(query, unknown_elem_positions, rel_type)
                         for comb in combs:
                             for new_comb in new_combs:
-                                extended_combs.append({**comb, **new_comb})
+                                extended_combs.append(self.merge_combs(comb, new_comb))
                 combs = extended_combs
 
-        if combs:
+        is_boolean = self.define_is_boolean(query_seq)
+        if combs or is_boolean:
             if filter_info:
                 for filter_elem, filter_value in filter_info:
                     if filter_value == "qualifier":
                         filter_value = "wpq/"
                     combs = [comb for comb in combs if filter_value in comb[filter_elem]]
 
             if order_info and not isinstance(order_info, list) and order_info.variable is not None:
                 reverse = True if order_info.sorting_order == "desc" else False
                 sort_elem = order_info.variable
-                for i in range(len(combs)):
-                    value_str = combs[i][sort_elem].split('^^')[0].strip('"')
-                    fnd = re.findall(r"[\d]{3,4}-[\d]{1,2}-[\d]{1,2}", value_str)
-                    if fnd:
-                        combs[i][sort_elem] = fnd[0]
-                    else:
-                        combs[i][sort_elem] = float(value_str)
-                combs = sorted(combs, key=lambda x: x[sort_elem], reverse=reverse)
-                combs = [combs[0]]
+                if combs and "?p" in combs[0]:
+                    rel_combs = {}
+                    for comb in combs:
+                        if comb["?p"] not in rel_combs:
+                            rel_combs[comb["?p"]] = []
+                        rel_combs[comb["?p"]].append(comb)
+                    rel_combs_list = rel_combs.values()
+                else:
+                    rel_combs_list = [combs]
+                new_rel_combs_list = []
+                for rel_combs in rel_combs_list:
+                    new_rel_combs = []
+                    for rel_comb in rel_combs:
+                        value_str = rel_comb[sort_elem].split('^^')[0].strip('"+')
+                        fnd_date = re.findall(r"[\d]{3,4}-[\d]{1,2}-[\d]{1,2}", value_str)
+                        fnd_num = re.findall(r"([\d]+)\.([\d]+)", value_str)
+                        if fnd_date:
+                            rel_comb[sort_elem] = fnd_date[0]
+                        elif fnd_num or value_str.isdigit():
+                            rel_comb[sort_elem] = float(value_str)
+                        new_rel_combs.append(rel_comb)
+                    new_rel_combs = [(elem, n) for n, elem in enumerate(new_rel_combs)]
+                    new_rel_combs = sorted(new_rel_combs, key=lambda x: (x[0][sort_elem], x[1]), reverse=reverse)
+                    new_rel_combs = [elem[0] for elem in new_rel_combs]
+                    new_rel_combs_list.append(new_rel_combs)
+                combs = [new_rel_combs[0] for new_rel_combs in new_rel_combs_list]
 
-            if what_return[-1].startswith("count"):
-                combs = [[combs[0][key] for key in what_return[:-1]] + [len(combs)]]
+            if what_return and what_return[-1].startswith("count"):
+                answers = [[len(combs)]]
             else:
-                combs = [[elem[key] for key in what_return] for elem in combs]
+                answers = [[elem[key] for key in what_return if key in elem] for elem in combs]
 
             if answer_types:
-                if answer_types == ["date"]:
-                    combs = [[entity for entity in comb
-                              if re.findall(r"[\d]{3,4}-[\d]{1,2}-[\d]{1,2}", entity)] for comb in combs]
+                if list(answer_types) == ["date"]:
+                    answers = [[entity for entity in answer
+                                if re.findall(r"[\d]{3,4}-[\d]{1,2}-[\d]{1,2}", entity)] for answer in answers]
+                elif list(answer_types) == ["not_date"]:
+                    answers = [[entity for entity in answer
+                                if not re.findall(r"[\d]{3,4}-[\d]{1,2}-[\d]{1,2}", entity)] for answer in answers]
                 else:
                     answer_types = set(answer_types)
-                    combs = [[entity for entity in comb
-                              if answer_types.intersection(self.find_types(entity))] for comb in combs]
-                combs = [comb for comb in combs if any([entity for entity in comb])]
+                    answers = [[entity for entity in answer
+                                if answer_types.intersection(self.find_types(entity))] for answer in answers]
+            if is_boolean:
+                answers = [["Yes" if len(triplets) > 0 else "No"]]
+            found_rels = [[elem[key] for key in rels_from_query if key in elem] for elem in combs]
+            ans_rels_combs = [(answer, rel, comb) for answer, rel, comb in zip(answers, found_rels, combs)
+                              if any([entity for entity in answer])]
+            answers = [elem[0] for elem in ans_rels_combs]
+            found_rels = [elem[1] for elem in ans_rels_combs]
+            found_combs = [elem[2] for elem in ans_rels_combs]
+
+        return answers, found_rels, found_combs
+
+    @staticmethod
+    def define_is_boolean(query_hdt_seq):
+        return len(query_hdt_seq) == 1 and all([not query_hdt_seq[0][i].startswith("?") for i in [0, 2]])
+
+    @staticmethod
+    def merge_combs(comb1, comb2):
+        new_comb = {}
+        for key in comb1:
+            if (key in comb2 and comb1[key] == comb2[key]) or key not in comb2:
+                new_comb[key] = comb1[key]
+        for key in comb2:
+            if (key in comb1 and comb2[key] == comb1[key]) or key not in comb1:
+                new_comb[key] = comb2[key]
+        return new_comb
 
-        return combs
-
-    def search(self, query: List[str], unknown_elem_positions: List[Tuple[int, str]], rel_type) -> List[Dict[str, str]]:
+    def search(self, query: List[str], unknown_elem_positions: List[Tuple[int, str]], rel_type):
         query = list(map(lambda elem: "" if elem.startswith('?') else elem, query))
         subj, rel, obj = query
         if self.file_format == "hdt":
             combs = []
             triplets, cnt = self.document.search_triples(subj, rel, obj)
             if cnt < self.max_comb_num:
+                triplets = list(triplets)
                 if rel == self.prefixes["description"] or rel == self.prefixes["label"]:
                     triplets = [triplet for triplet in triplets if triplet[2].endswith(self.lang)]
                     combs = [{elem: triplet[pos] for pos, elem in unknown_elem_positions} for triplet in triplets]
                 else:
-                    combs = [{elem: triplet[pos] for pos, elem in unknown_elem_positions} for triplet in triplets
-                             if triplet[1].startswith(self.prefixes["rels"][rel_type])]
+                    if isinstance(self.prefixes["rels"][rel_type], str):
+                        combs = [{elem: triplet[pos] for pos, elem in unknown_elem_positions} for triplet in triplets
+                                 if (triplet[1].startswith(self.prefixes["rels"][rel_type])
+                                     or triplet[1].startswith(self.prefixes["rels"]["type"]))]
+                    else:
+                        combs = [{elem: triplet[pos] for pos, elem in unknown_elem_positions} for triplet in triplets
+                                 if (any(triplet[1].startswith(tp) for tp in self.prefixes["rels"][rel_type])
+                                     or triplet[1].startswith(self.prefixes["rels"]["type"]))]
             else:
-                log.debug("max comb num exceede")
+                log.debug("max comb num exceeds")
         else:
             triplets = []
             if subj:
                 subj, triplets = self.find_triplets(subj, "forw")
                 triplets = [[subj, triplet[0], obj] for triplet in triplets for obj in triplet[1:]]
             if obj:
                 obj, triplets = self.find_triplets(obj, "backw")
@@ -307,35 +387,34 @@
                 if rel == self.prefixes["description"]:
                     triplets = [triplet for triplet in triplets if triplet[1] == "descr_en"]
                 else:
                     rel = rel.split('/')[-1]
                     triplets = [triplet for triplet in triplets if triplet[1] == rel]
             combs = [{elem: triplet[pos] for pos, elem in unknown_elem_positions} for triplet in triplets]
 
-        return combs
+        return combs, triplets
 
-    def find_label(self, entity: str, question: str) -> str:
+    def find_label(self, entity: str, question: str = "") -> str:
         entity = str(entity).replace('"', '')
         if self.file_format == "hdt":
             if entity.startswith("Q") or entity.startswith("P"):
                 # example: "Q5513"
                 entity = f"{self.prefixes['entity']}/{entity}"
                 # "http://www.wikidata.org/entity/Q5513"
 
             if entity.startswith(self.prefixes["entity"]):
                 labels, c = self.document.search_triples(entity, self.prefixes["label"], "")
                 # labels = [["http://www.wikidata.org/entity/Q5513", "http://www.w3.org/2000/01/rdf-schema#label",
                 #                                                    '"Lake Baikal"@en'], ...]
                 for label in labels:
                     if label[2].endswith(self.lang):
-                        found_label = label[2].strip(self.lang).replace('"', '').replace('$', ' ').replace('  ', ' ')
-                        return found_label
-                for label in labels:
-                    if label[2].endswith("@en"):
-                        found_label = label[2].strip("@en").replace('"', '').replace('$', ' ').replace('  ', ' ')
+                        found_label = label[2].strip(self.lang)
+                        for old_tok, new_tok in self.replace_tokens:
+                            found_label = found_label.replace(old_tok, new_tok)
+                        found_label = found_label.strip()
                         return found_label
 
             elif entity.endswith(self.lang):
                 # entity: '"Lake Baikal"@en'
                 entity = entity[:-3].replace('$', ' ').replace('  ', ' ')
                 return entity
 
@@ -345,19 +424,25 @@
                         '"1799-06-06T00:00:00Z"^^<http://www.w3.org/2001/XMLSchema#dateTime>' (date)
                         '"+1642"^^<http://www.w3.org/2001/XMLSchema#decimal>' (number)
                 """
                 entity = entity.split("^^")[0]
                 for token in ["T00:00:00Z", "+"]:
                     entity = entity.replace(token, '')
                 entity = self.format_date(entity, question).replace('$', '')
+                return entity
 
+            elif re.findall(r"[\d]{3,4}-[\d]{2}-[\d]{2}", entity):
+                entity = self.format_date(entity, question).replace('$', '')
+                return entity
+
+            elif entity in ["Yes", "No"]:
                 return entity
 
             elif entity.isdigit():
-                entity = str(entity).replace('.', ',')
+                entity = entity.replace('.', ',')
                 return entity
 
         if self.file_format == "pickle":
             if entity:
                 if entity.startswith("Q") or entity.startswith("P"):
                     triplets = self.document.get(entity, {}).get("forw", [])
                     triplets = self.uncompress(triplets)
@@ -380,15 +465,15 @@
             year, month, day = date_info[0]
             if "how old" in question.lower() or "сколько лет" in question.lower():
                 entity = datetime.datetime.now().year - int(year)
             elif "в каком году" in question.lower():
                 entity = year
             elif "в каком месяце" in question.lower():
                 entity = month
-            elif day != "00":
+            elif day not in {"00", "0"}:
                 date = datetime.datetime.strptime(f"{year}-{month}-{day}", "%Y-%m-%d")
                 entity = date.strftime("%d %B %Y")
             else:
                 entity = year
             if self.lang == "@ru":
                 for mnth, mnth_replace in dates_dict.items():
                     entity = entity.replace(mnth, mnth_replace)
@@ -399,32 +484,58 @@
     def find_alias(self, entity: str) -> List[str]:
         aliases = []
         if entity.startswith(self.prefixes["entity"]):
             labels, cardinality = self.document.search_triples(entity, self.prefixes["alias"], "")
             aliases = [label[2].strip(self.lang).strip('"') for label in labels if label[2].endswith(self.lang)]
         return aliases
 
-    def find_rels(self, entity: str, direction: str, rel_type: str = "no_type", save: bool = False) -> List[str]:
+    def find_rels(self, entity: str, direction: str, rel_type: str = "no_type") -> List[str]:
         rels = []
         if self.file_format == "hdt":
             if not rel_type:
                 rel_type = "direct"
             if direction == "forw":
                 query = [f"{self.prefixes['entity']}/{entity}", "", ""]
             else:
                 query = ["", "", f"{self.prefixes['entity']}/{entity}"]
             triplets, c = self.document.search_triples(*query)
-
-            start_str = f"{self.prefixes['rels'][rel_type]}/P"
-            rels = {triplet[1] for triplet in triplets if triplet[1].startswith(start_str)}
+            triplets = list(triplets)
+            if isinstance(self.prefixes['rels'][rel_type], str):
+                start_str = f"{self.prefixes['rels'][rel_type]}/P"
+                rels = {triplet[1] for triplet in triplets if triplet[1].startswith(start_str)}
+            else:
+                rels = {triplet[1] for triplet in triplets
+                        if any([triplet[1].startswith(tp) for tp in self.prefixes['rels'][rel_type]])}
             rels = list(rels)
-        if self.file_format == "pickle":
-            triplets = self.document.get(entity, {}).get(direction, [])
-            triplets = self.uncompress(triplets)
-            rels = [triplet[0] for triplet in triplets if triplet[0].startswith("P")]
+            if self.used_rels:
+                rels = [rel for rel in rels if rel.split("/")[-1] in self.used_rels]
+        return rels
+
+    def find_rels_2hop(self, entity_ids, rels_1hop):
+        rels = []
+        for entity_id in entity_ids:
+            for rel_1hop in rels_1hop:
+                triplets, cnt = self.document.search_triples(f"{self.prefixes['entity']}/{entity_id}", rel_1hop, "")
+                triplets = [triplet for triplet in triplets if triplet[2].startswith(self.prefixes['entity'])]
+                objects_1hop = [triplet[2].split("/")[-1] for triplet in triplets]
+                triplets, cnt = self.document.search_triples("", rel_1hop, f"{self.prefixes['entity']}/{entity_id}")
+                triplets = [triplet for triplet in triplets if triplet[0].startswith(self.prefixes['entity'])]
+                objects_1hop += [triplet[0].split("/")[-1] for triplet in triplets]
+                for object_1hop in objects_1hop[:5]:
+                    tr_2hop, cnt = self.document.search_triples(f"{self.prefixes['entity']}/{object_1hop}", "", "")
+                    rels_2hop = [elem[1] for elem in tr_2hop if elem[1] != rel_1hop]
+                    if self.used_rels:
+                        rels_2hop = [elem for elem in rels_2hop if elem.split("/")[-1] in self.used_rels]
+                    rels += rels_2hop
+                    tr_2hop, cnt = self.document.search_triples("", "", f"{self.prefixes['entity']}/{object_1hop}")
+                    rels_2hop = [elem[1] for elem in tr_2hop if elem[1] != rel_1hop]
+                    if self.used_rels:
+                        rels_2hop = [elem for elem in rels_2hop if elem.split("/")[-1] in self.used_rels]
+                    rels += rels_2hop
+        rels = list(set(rels))
         return rels
 
     def find_object(self, entity: str, rel: str, direction: str) -> List[str]:
         objects = []
         if not direction:
             direction = "forw"
         if self.file_format == "hdt":
@@ -473,17 +584,18 @@
     def find_types(self, entity: str):
         types = []
         if self.file_format == "hdt":
             if not entity.startswith("http"):
                 entity = f"{self.prefixes['entity']}/{entity}"
             tr, c = self.document.search_triples(entity, f"{self.prefixes['rels']['direct']}/P31", "")
             types = [triplet[2].split('/')[-1] for triplet in tr]
-            if "Q5" in types:
-                tr, c = self.document.search_triples(entity, f"{self.prefixes['rels']['direct']}/P106", "")
+            for rel in ["P106", "P21"]:
+                tr, c = self.document.search_triples(entity, f"{self.prefixes['rels']['direct']}/{rel}", "")
                 types += [triplet[2].split('/')[-1] for triplet in tr]
+
         if self.file_format == "pickle":
             entity = entity.split('/')[-1]
             triplets = self.document.get(entity, {}).get("forw", [])
             triplets = self.uncompress(triplets)
             for triplet in triplets:
                 if triplet[0] == "P31":
                     types = triplet[1:]
@@ -528,7 +640,49 @@
         subj = subj.split('/')[-1]
         if subj in self.parsed_document:
             triplets = self.parsed_document.get(subj, {}).get(direction, [])
         else:
             triplets = self.document.get(subj, {}).get(direction, [])
             triplets = self.uncompress(triplets)
         return subj, triplets
+
+    def fill_triplets(self, init_triplets, what_to_return, comb):
+        filled_triplets = []
+        for n, (subj, rel, obj) in enumerate(init_triplets):
+            if "statement" in self.prefixes and subj.startswith("?") \
+                    and comb.get(subj, "").startswith(self.prefixes["statement"]) and not rel.startswith("?") \
+                    and (obj == what_to_return[0] or re.findall(r"[\d]{3,4}", comb.get(what_to_return[0], ""))):
+                continue
+            else:
+                if "statement" in self.prefixes and subj.startswith("?") \
+                        and str(comb.get(subj, "")).startswith(self.prefixes["statement"]):
+                    if not comb.get(what_to_return[0], "").startswith("http") \
+                            and re.findall(r"[\d]{3,4}", comb.get(what_to_return[0], "")):
+                        subj = init_triplets[1][2]
+                    else:
+                        subj = what_to_return[0]
+                if "statement" in self.prefixes and obj.startswith("?") \
+                        and str(comb.get(obj, "")).startswith(self.prefixes["statement"]):
+                    if not str(comb.get(what_to_return[0], "")).startswith("http") \
+                            and re.findall(r"[\d]{3,4}", str(comb.get(what_to_return[0], ""))):
+                        obj = init_triplets[1][2]
+                    else:
+                        obj = what_to_return[0]
+                subj, obj = str(subj), str(obj)
+                if subj.startswith("?"):
+                    subj = comb.get(subj, "")
+                if obj.startswith("?"):
+                    obj = comb.get(obj, "")
+                if rel.startswith("?"):
+                    rel = comb.get(rel, "")
+                subj_label = self.find_label(subj)
+                obj_label = self.find_label(obj)
+                if rel in self.rel_q2name:
+                    rel_label = self.rel_q2name[rel]
+                elif rel.split("/")[-1] in self.rel_q2name:
+                    rel_label = self.rel_q2name[rel.split("/")[-1]]
+                else:
+                    rel_label = self.find_label(rel)
+                if isinstance(rel_label, list) and rel_label:
+                    rel_label = rel_label[0]
+                filled_triplets.append([subj_label, rel_label, obj_label])
+        return filled_triplets
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/dirty_comments_preprocessor.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/dirty_comments_preprocessor.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/mask.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/mask.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/multitask_preprocessor.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/multitask_preprocessor.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/ner_preprocessor.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/ner_preprocessor.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/odqa_preprocessors.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/odqa_preprocessors.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/one_hotter.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/one_hotter.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/re_preprocessor.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/re_preprocessor.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/response_base_loader.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/response_base_loader.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/sanitizer.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/sanitizer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/sentseg_preprocessor.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/sentseg_preprocessor.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/squad_preprocessor.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/squad_preprocessor.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/str_lower.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/str_lower.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/str_token_reverser.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/str_token_reverser.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/str_utf8_encoder.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/str_utf8_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from collections import Counter, OrderedDict
 from itertools import chain
 from logging import getLogger
 from typing import Union, List, Tuple
 
 import numpy as np
-from overrides import overrides
 
 from deeppavlov.core.common.errors import ConfigError
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.models.estimator import Estimator
 
 log = getLogger(__name__)
 
@@ -126,36 +125,33 @@
             if isinstance(batch[-1], str):
                 return self._encode_chars(batch)
             else:
                 return [self(line) for line in batch]
         raise RuntimeError(f'The objects passed to the reverser are not list or tuple of str! '
                            f' But they are {type(batch)}.')
 
-    @overrides
     def load(self) -> None:
         if self.load_path:
             if self.load_path.is_file():
                 log.debug(f"[loading vocabulary from {self.load_path}]")
                 self.tokens = []
                 for ln in self.load_path.open('r', encoding='utf8'):
                     token = ln.strip().split()[0]
                     self.tokens.append(token)
             else:
                 raise ConfigError(f"Provided `load_path` for {self.__class__.__name__} doesn't exist!")
         else:
             raise ConfigError(f"`load_path` for {self} is not provided!")
 
-    @overrides
     def save(self) -> None:
         log.info(f"[saving vocabulary to {self.save_path}]")
         with self.save_path.open('wt', encoding='utf8') as f:
             for token in self._word_char_ids.keys():
                 f.write('{}\n'.format(token))
 
-    @overrides
     def fit(self, *args) -> None:
         words = chain(*args)
         # filter(None, <>) -- to filter empty words
         freqs = Counter(filter(None, chain(*words)))
         for token, _ in freqs.most_common():
             if not (token in self._word_char_ids):
                 self._word_char_ids[token] = self._convert_word_to_char_ids(token)
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/torch_transformers_preprocessor.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/torch_transformers_preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -364,70 +364,117 @@
         add_special_tokens: special_tokens_list
         do_lower_case: set True if lowercasing is needed
         max_seq_length: max sequence length in subtokens, including [SEP] and [CLS] tokens
     """
 
     def __init__(self,
                  vocab_file: str,
-                 add_special_tokens: List[str],
                  do_lower_case: bool = True,
                  max_seq_length: int = 512,
                  **kwargs) -> None:
         self.max_seq_length = max_seq_length
         self.tokenizer = AutoTokenizer.from_pretrained(vocab_file, do_lower_case=do_lower_case)
-        self.add_special_tokens = add_special_tokens
-        special_tokens_dict = {'additional_special_tokens': add_special_tokens}
-        self.tokenizer.add_special_tokens(special_tokens_dict)
 
     def __call__(self, questions_batch: List[List[str]], rels_batch: List[List[str]] = None) -> Dict[str, torch.tensor]:
         """Tokenize questions and relations
         texts_a and texts_b are separated by [SEP] token
         Args:
             questions_batch: list of texts,
             rels_batch: list of relations list
-
         Returns:
             batch of :class:`transformers.data.processors.utils.InputFeatures` with subtokens, subtoken ids, \
                 subtoken mask, segment mask, or tuple of batch of InputFeatures and Batch of subtokens
         """
-        lengths = []
+        lengths, proc_rels_batch = [], []
         for question, rels_list in zip(questions_batch, rels_batch):
             if isinstance(rels_list, list):
-                rels_str = self.add_special_tokens[2].join(rels_list)
+                rels_str = " ".join(rels_list)
             else:
                 rels_str = rels_list
-            text_input = f"{self.add_special_tokens[0]} {question} {self.add_special_tokens[1]} {rels_str}"
-            encoding = self.tokenizer.encode_plus(text=text_input,
+            encoding = self.tokenizer.encode_plus(text=question, text_pair=rels_str,
                                                   return_attention_mask=True, add_special_tokens=True,
                                                   truncation=True)
             lengths.append(len(encoding["input_ids"]))
+            proc_rels_batch.append(rels_str)
         max_len = max(lengths)
-        input_ids_batch = []
-        attention_mask_batch = []
-        token_type_ids_batch = []
-        for question, rels_list in zip(questions_batch, rels_batch):
-            if isinstance(rels_list, list):
-                rels_str = self.add_special_tokens[2].join(rels_list)
-            else:
-                rels_str = rels_list
-            text_input = f"{self.add_special_tokens[0]} {question} {self.add_special_tokens[1]} {rels_str}"
-            encoding = self.tokenizer.encode_plus(text=text_input,
-                                                  truncation = True, max_length=max_len,
-                                                  pad_to_max_length=True, return_attention_mask = True)
+        input_ids_batch, attention_mask_batch, token_type_ids_batch = [], [], []
+        for question, rels_list in zip(questions_batch, proc_rels_batch):
+            encoding = self.tokenizer.encode_plus(text=question, text_pair=rels_list,
+                                                  truncation=True, max_length=max_len,
+                                                  pad_to_max_length=True, return_attention_mask=True)
             input_ids_batch.append(encoding["input_ids"])
             attention_mask_batch.append(encoding["attention_mask"])
             if "token_type_ids" in encoding:
                 token_type_ids_batch.append(encoding["token_type_ids"])
             else:
                 token_type_ids_batch.append([0])
-
         input_features = {"input_ids": torch.LongTensor(input_ids_batch),
                           "attention_mask": torch.LongTensor(attention_mask_batch),
                           "token_type_ids": torch.LongTensor(token_type_ids_batch)}
+        return input_features
+
 
+@register('path_ranking_preprocessor')
+class PathRankingPreprocessor(Component):
+    def __init__(self,
+                 vocab_file: str,
+                 additional_special_tokens: List[str] = None,
+                 do_lower_case: bool = True,
+                 max_seq_length: int = 67,
+                 **kwargs) -> None:
+        self.max_seq_length = max_seq_length
+        self.tokenizer = AutoTokenizer.from_pretrained(vocab_file, do_lower_case=do_lower_case)
+        self.additional_special_tokens = additional_special_tokens
+        if self.additional_special_tokens:
+            self.tokenizer.add_special_tokens({'additional_special_tokens': additional_special_tokens})
+
+    def __call__(self, questions_batch: List[str], rels_batch: List[List[List[str]]]):
+        lengths, proc_rels_batch = [], []
+        for question, rels_list in zip(questions_batch, rels_batch):
+            proc_rels_list = []
+            for rels in rels_list:
+                if isinstance(rels, str):
+                    rels = [rels]
+                rels_str = ""
+                if len(rels) == 1:
+                    if self.additional_special_tokens:
+                        rels_str = f"<one_rel> {rels[0]} </one_rel>"
+                    else:
+                        rels_str = rels[0]
+                elif len(rels) == 2:
+                    if rels[0] == rels[1]:
+                        rels_str = f"<double> {rels[0]} </double>"
+                    else:
+                        rels_str = f"<first_rel> {rels[0]} <mid> {rels[1]} </second_rel>"
+                encoding = self.tokenizer.encode_plus(text=question, text_pair=rels_str,
+                                                      return_attention_mask=True, add_special_tokens=True,
+                                                      truncation=True)
+                lengths.append(len(encoding["input_ids"]))
+                proc_rels_list.append(rels_str)
+            proc_rels_batch.append(proc_rels_list)
+
+        max_len = min(max(lengths), self.max_seq_length)
+        input_ids_batch, attention_mask_batch, token_type_ids_batch = [], [], []
+        for question, rels_list in zip(questions_batch, proc_rels_batch):
+            input_ids_list, attention_mask_list, token_type_ids_list = [], [], []
+            for rels_str in rels_list:
+                encoding = self.tokenizer.encode_plus(text=question, text_pair=rels_str,
+                                                      truncation=True, max_length=max_len, add_special_tokens=True,
+                                                      pad_to_max_length=True, return_attention_mask=True)
+                input_ids_list.append(encoding["input_ids"])
+                attention_mask_list.append(encoding["attention_mask"])
+                if "token_type_ids" in encoding:
+                    token_type_ids_list.append(encoding["token_type_ids"])
+                else:
+                    token_type_ids_list.append([0])
+            input_ids_batch.append(input_ids_list)
+            attention_mask_batch.append(attention_mask_list)
+            token_type_ids_batch.append(token_type_ids_list)
+        input_features = {"input_ids": input_ids_batch, "attention_mask": attention_mask_batch,
+                          "token_type_ids": token_type_ids_batch}
         return input_features
 
 
 @register('torch_transformers_ner_preprocessor')
 class TorchTransformersNerPreprocessor(Component):
     """
     Takes tokens and splits them into bert subtokens, encodes subtokens with their indices.
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/preprocessors/transformers_preprocessor.py` & `deeppavlov-1.2.0/deeppavlov/models/preprocessors/transformers_preprocessor.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/ranking/metrics.py` & `deeppavlov-1.2.0/deeppavlov/models/ranking/metrics.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/relation_extraction/losses.py` & `deeppavlov-1.2.0/deeppavlov/models/relation_extraction/losses.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/relation_extraction/relation_extraction_bert.py` & `deeppavlov-1.2.0/deeppavlov/models/relation_extraction/relation_extraction_bert.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/sklearn/sklearn_component.py` & `deeppavlov-1.2.0/deeppavlov/models/sklearn/sklearn_component.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/spelling_correction/brillmoore/error_model.py` & `deeppavlov-1.2.0/deeppavlov/models/spelling_correction/brillmoore/error_model.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/spelling_correction/electors/kenlm_elector.py` & `deeppavlov-1.2.0/deeppavlov/models/spelling_correction/electors/kenlm_elector.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/spelling_correction/electors/top1_elector.py` & `deeppavlov-1.2.0/deeppavlov/models/spelling_correction/electors/top1_elector.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/spelling_correction/levenshtein/levenshtein_searcher.py` & `deeppavlov-1.2.0/deeppavlov/models/spelling_correction/levenshtein/levenshtein_searcher.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/spelling_correction/levenshtein/searcher_component.py` & `deeppavlov-1.2.0/deeppavlov/models/spelling_correction/levenshtein/searcher_component.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/spelling_correction/levenshtein/tabled_trie.py` & `deeppavlov-1.2.0/deeppavlov/models/spelling_correction/levenshtein/tabled_trie.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/tokenizers/nltk_moses_tokenizer.py` & `deeppavlov-1.2.0/deeppavlov/models/tokenizers/nltk_moses_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/tokenizers/nltk_tokenizer.py` & `deeppavlov-1.2.0/deeppavlov/models/tokenizers/nltk_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/tokenizers/spacy_tokenizer.py` & `deeppavlov-1.2.0/deeppavlov/models/tokenizers/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/tokenizers/split_tokenizer.py` & `deeppavlov-1.2.0/deeppavlov/models/tokenizers/split_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/tokenizers/utils.py` & `deeppavlov-1.2.0/deeppavlov/models/tokenizers/utils.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/torch_bert/crf.py` & `deeppavlov-1.2.0/deeppavlov/models/torch_bert/crf.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/torch_bert/multitask_transformer.py` & `deeppavlov-1.2.0/deeppavlov/models/torch_bert/multitask_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from logging import getLogger
 from pathlib import Path
 from typing import Dict, Optional
 
 import numpy as np
 import torch
 import torch.nn as nn
-from overrides import overrides
 from torch.nn import CrossEntropyLoss, MSELoss, BCEWithLogitsLoss
 from transformers import AutoConfig, AutoModel
 
 from deeppavlov.core.common.errors import ConfigError
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.models.torch_model import TorchModel
 from deeppavlov.models.torch_bert.torch_transformers_sequence_tagger import token_from_subtoken, \
@@ -338,15 +337,14 @@
             lr_scheduler_parameters=self.lr_scheduler_parameters,
             **kwargs,
         )
 
     def _reset_cache(self):
         self.preds_cache = {index_: None for index_ in self.types_to_cache if index_ != -1}
 
-    @overrides
     def init_from_opt(self) -> None:
         """
         Initialize from scratch `self.model` with the architecture built
         in `model_func (MultitaskBert)` method of this class along with
         `self.optimizer` as `self.optimizer_name` from `torch.optim` and
         parameters `self.optimizer_parameters`, optionally initialize
         `self.lr_scheduler` as `self.lr_scheduler_name` from
@@ -397,15 +395,14 @@
         )
 
         if self.lr_scheduler_name:
             self.lr_scheduler = getattr(
                 torch.optim.lr_scheduler, self.lr_scheduler_name
             )(self.optimizer, **self.lr_scheduler_parameters)
 
-    @overrides
     def load(self, fname: Optional[str] = None) -> None:
         """
         Loads weights.
         """
         if fname is not None:
             self.load_path = fname
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_bert_ranker.py` & `deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_bert_ranker.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from logging import getLogger
 from pathlib import Path
 from typing import List, Dict, Union, Optional
 
 import numpy as np
 import torch
-from overrides import overrides
 from transformers import AutoModelForSequenceClassification, AutoConfig
 from transformers.data.processors.utils import InputFeatures
 
 from deeppavlov.core.commands.utils import expand_path
 from deeppavlov.core.common.errors import ConfigError
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.models.torch_model import TorchModel
@@ -151,15 +150,14 @@
         if len(features_li) == 1:
             predictions = predictions[0]
         else:
             predictions = np.hstack([np.expand_dims(el, 1) for el in predictions])
 
         return predictions
 
-    @overrides
     def load(self, fname=None):
         if fname is not None:
             self.load_path = fname
 
         if self.pretrained_bert:
             log.debug(f"From pretrained {self.pretrained_bert}.")
             if Path(expand_path(self.pretrained_bert)).exists():
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_transformers_classifier.py` & `deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
 from logging import getLogger
 from pathlib import Path
 from typing import List, Dict, Union, Optional, Tuple
 
 import numpy as np
 import torch
-from overrides import overrides
 from torch.nn import BCEWithLogitsLoss
 from transformers import AutoModelForSequenceClassification, AutoConfig, AutoModel, AutoTokenizer
 from transformers.modeling_outputs import SequenceClassifierOutput
 
-from deeppavlov.core.common.errors import ConfigError
 from deeppavlov.core.commands.utils import expand_path
+from deeppavlov.core.common.errors import ConfigError
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.models.torch_model import TorchModel
 
 log = getLogger(__name__)
 
 
 @register('torch_transformers_classifier')
@@ -192,15 +190,14 @@
 
     # TODO move to the super class
     @property
     def is_data_parallel(self) -> bool:
         return isinstance(self.model, torch.nn.DataParallel)
 
     # TODO this method requires massive refactoring
-    @overrides
     def load(self, fname=None):
         if fname is not None:
             self.load_path = fname
 
         if self.pretrained_bert:
             log.debug(f"From pretrained {self.pretrained_bert}.")
             config = AutoConfig.from_pretrained(self.pretrained_bert,
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_transformers_el_ranker.py` & `deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_el_ranker.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_transformers_multiplechoice.py` & `deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_multiplechoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from logging import getLogger
 from pathlib import Path
 from typing import List, Dict, Union, Optional
 
 import numpy as np
 import torch
-from overrides import overrides
 from transformers import AutoModelForMultipleChoice, AutoConfig
 
 from deeppavlov.core.common.errors import ConfigError
 from deeppavlov.core.commands.utils import expand_path
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.models.torch_model import TorchModel
 
@@ -154,15 +153,14 @@
             logits = logits.detach().cpu().numpy()
             pred = np.argmax(logits, axis=1)
         else:  # regression
             pred = logits.squeeze(-1).detach().cpu().numpy()
 
         return pred
 
-    @overrides
     def load(self, fname = None):
         if fname is not None:
             self.load_path = fname
 
         if self.pretrained_bert:
             log.debug(f"From pretrained {self.pretrained_bert}.")
             config = AutoConfig.from_pretrained(self.pretrained_bert, num_labels=self.n_classes,
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_transformers_sequence_tagger.py` & `deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_sequence_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from logging import getLogger
 from pathlib import Path
 from typing import List, Union, Dict, Optional, Tuple
 
 import numpy as np
 import torch
-from overrides import overrides
 from transformers import AutoModelForTokenClassification, AutoConfig
 
 from deeppavlov.core.commands.utils import expand_path
 from deeppavlov.core.common.errors import ConfigError
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.models.torch_model import TorchModel
 from deeppavlov.models.torch_bert.crf import CRF
@@ -266,15 +265,14 @@
             logits = logits.detach().cpu().numpy()
             pred = np.argmax(logits, axis=-1)
         seq_lengths = np.sum(y_masks, axis=1)
         pred = [p[:l] for l, p in zip(seq_lengths, pred)]
 
         return pred, probas
 
-    @overrides
     def load(self, fname=None):
         if fname is not None:
             self.load_path = fname
 
         if self.pretrained_bert:
             config = AutoConfig.from_pretrained(self.pretrained_bert, num_labels=self.n_classes,
                                                 output_attentions=False, output_hidden_states=False)
@@ -307,15 +305,16 @@
                 weights_path_crf = weights_path_crf.with_suffix(".pth.tar")
                 if weights_path_crf.exists():
                     checkpoint = torch.load(weights_path_crf, map_location=self.device)
                     self.crf.load_state_dict(checkpoint["model_state_dict"], strict=False)
                 else:
                     log.warning(f"Init from scratch. Load path {weights_path_crf} does not exist.")
 
-    @overrides
     def save(self, fname: Optional[str] = None, *args, **kwargs) -> None:
-        super().save()
+        super().save(fname)
         if self.use_crf:
+            if fname is None:
+                fname = self.save_path
             weights_path_crf = Path(f"{fname}_crf").resolve()
             weights_path_crf = weights_path_crf.with_suffix(".pth.tar")
             torch.save({"model_state_dict": self.crf.cpu().state_dict()}, weights_path_crf)
             self.crf.to(self.device)
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/torch_bert/torch_transformers_squad.py` & `deeppavlov-1.2.0/deeppavlov/models/torch_bert/torch_transformers_squad.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
 from logging import getLogger
 from pathlib import Path
 from typing import List, Tuple, Optional, Dict
 
 import numpy as np
 import torch
-from overrides import overrides
 from transformers import AutoModelForQuestionAnswering, AutoConfig
 from transformers.data.processors.utils import InputFeatures
 
 from deeppavlov.core.commands.utils import expand_path
 from deeppavlov.core.common.errors import ConfigError
 from deeppavlov.core.common.registry import register
 from deeppavlov.core.models.torch_model import TorchModel
@@ -260,15 +258,14 @@
             end_pred_batch.append(prediction[max_ind][1])
             logits_batch.append(prediction[max_ind][2])
             scores_batch.append(prediction[max_ind][3])
             ind_batch.append(max_ind)
 
         return start_pred_batch, end_pred_batch, logits_batch, scores_batch, ind_batch
 
-    @overrides
     def load(self, fname=None):
         if fname is not None:
             self.load_path = fname
 
         if self.pretrained_bert:
             logger.debug(f"From pretrained {self.pretrained_bert}.")
             config = AutoConfig.from_pretrained(self.pretrained_bert,
```

### Comparing `deeppavlov-1.1.1/deeppavlov/models/vectorizers/hashing_tfidf_vectorizer.py` & `deeppavlov-1.2.0/deeppavlov/models/vectorizers/hashing_tfidf_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/paramsearch.py` & `deeppavlov-1.2.0/deeppavlov/paramsearch.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/settings.py` & `deeppavlov-1.2.0/deeppavlov/settings.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/utils/connector/dialog_logger.py` & `deeppavlov-1.2.0/deeppavlov/utils/connector/dialog_logger.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/utils/pip_wrapper/pip_wrapper.py` & `deeppavlov-1.2.0/deeppavlov/utils/pip_wrapper/pip_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/utils/server/metrics.py` & `deeppavlov-1.2.0/deeppavlov/utils/server/metrics.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/utils/server/server.py` & `deeppavlov-1.2.0/deeppavlov/utils/server/server.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/utils/settings/log_config.json` & `deeppavlov-1.2.0/deeppavlov/utils/settings/log_config.json`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/utils/socket/socket.py` & `deeppavlov-1.2.0/deeppavlov/utils/socket/socket.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/vocabs/typos.py` & `deeppavlov-1.2.0/deeppavlov/vocabs/typos.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov/vocabs/wiki_sqlite.py` & `deeppavlov-1.2.0/deeppavlov/vocabs/wiki_sqlite.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/deeppavlov.egg-info/PKG-INFO` & `deeppavlov-1.2.0/deeppavlov.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: deeppavlov
-Version: 1.1.1
+Version: 1.2.0
 Summary: An open source library for building end-to-end dialog systems and training chatbots.
 Home-page: https://github.com/deeppavlov/DeepPavlov
-Download-URL: https://github.com/deeppavlov/DeepPavlov/archive/1.1.1.tar.gz
+Download-URL: https://github.com/deeppavlov/DeepPavlov/archive/1.2.0.tar.gz
 Author: Neural Networks and Deep Learning lab, MIPT
 Author-email: info@deeppavlov.ai
 License: Apache License, Version 2.0
 Keywords: NLP,NER,SQUAD,Intents,Chatbot
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
```

### Comparing `deeppavlov-1.1.1/deeppavlov.egg-info/SOURCES.txt` & `deeppavlov-1.2.0/deeppavlov.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 deeppavlov/configs/classifiers/rusentiment_bert.json
 deeppavlov/configs/classifiers/rusentiment_convers_bert.json
 deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_2L.json
 deeppavlov/configs/classifiers/rusentiment_convers_distilrubert_6L.json
 deeppavlov/configs/classifiers/sentiment_sst_conv_bert.json
 deeppavlov/configs/classifiers/sentiment_twitter.json
 deeppavlov/configs/classifiers/topics_distilbert_base_uncased.json
-deeppavlov/configs/classifiers/glue/glue_cola_cased_bert_torch.json
+deeppavlov/configs/classifiers/glue/glue_cola_roberta.json
 deeppavlov/configs/classifiers/glue/glue_mnli_cased_bert_torch.json
 deeppavlov/configs/classifiers/glue/glue_mnli_mm_cased_bert_torch.json
 deeppavlov/configs/classifiers/glue/glue_mnli_roberta.json
-deeppavlov/configs/classifiers/glue/glue_mrpc_cased_bert_torch.json
-deeppavlov/configs/classifiers/glue/glue_qnli_cased_bert_torch.json
-deeppavlov/configs/classifiers/glue/glue_qqp_cased_bert_torch.json
+deeppavlov/configs/classifiers/glue/glue_mrpc_roberta.json
+deeppavlov/configs/classifiers/glue/glue_qnli_roberta.json
+deeppavlov/configs/classifiers/glue/glue_qqp_roberta.json
 deeppavlov/configs/classifiers/glue/glue_rte_cased_bert_torch.json
 deeppavlov/configs/classifiers/glue/glue_rte_roberta_mnli.json
-deeppavlov/configs/classifiers/glue/glue_sst2_cased_bert_torch.json
-deeppavlov/configs/classifiers/glue/glue_stsb_cased_bert_torch.json
+deeppavlov/configs/classifiers/glue/glue_sst2_roberta.json
+deeppavlov/configs/classifiers/glue/glue_stsb_roberta.json
 deeppavlov/configs/classifiers/glue/glue_wnli_roberta.json
 deeppavlov/configs/classifiers/superglue/superglue_boolq_roberta_mnli.json
 deeppavlov/configs/classifiers/superglue/superglue_copa_roberta.json
 deeppavlov/configs/classifiers/superglue/superglue_record_roberta.json
 deeppavlov/configs/doc_retrieval/en_ranker_pop_enwiki20180211.json
 deeppavlov/configs/doc_retrieval/en_ranker_tfidf_wiki.json
 deeppavlov/configs/doc_retrieval/ru_ranker_tfidf_wiki.json
@@ -70,17 +70,18 @@
 deeppavlov/configs/ner/ner_rus_bert_probas.json
 deeppavlov/configs/ner/ner_rus_convers_distilrubert_2L.json
 deeppavlov/configs/ner/ner_rus_convers_distilrubert_6L.json
 deeppavlov/configs/odqa/en_odqa_infer_wiki.json
 deeppavlov/configs/odqa/en_odqa_pop_infer_enwiki20180211.json
 deeppavlov/configs/odqa/ru_odqa_infer_wiki.json
 deeppavlov/configs/odqa/ru_odqa_infer_wiki_retr_noans.json
+deeppavlov/configs/ranking/path_ranking_nll_roberta_en.json
 deeppavlov/configs/ranking/ranking_ubuntu_v2_torch_bert_uncased.json
-deeppavlov/configs/ranking/rel_ranking_bert_en.json
-deeppavlov/configs/ranking/rel_ranking_bert_ru.json
+deeppavlov/configs/ranking/rel_ranking_nll_bert_ru.json
+deeppavlov/configs/ranking/rel_ranking_roberta_en.json
 deeppavlov/configs/regressors/translation_ranker.json
 deeppavlov/configs/relation_extraction/re_docred.json
 deeppavlov/configs/relation_extraction/re_rured.json
 deeppavlov/configs/russian_super_glue/russian_superglue_danetqa_rubert.json
 deeppavlov/configs/russian_super_glue/russian_superglue_lidirus_rubert.json
 deeppavlov/configs/russian_super_glue/russian_superglue_muserc_rubert.json
 deeppavlov/configs/russian_super_glue/russian_superglue_parus_rubert.json
@@ -198,19 +199,21 @@
 deeppavlov/models/embedders/abstract_embedder.py
 deeppavlov/models/embedders/fasttext_embedder.py
 deeppavlov/models/embedders/tfidf_weighted_embedder.py
 deeppavlov/models/embedders/transformers_embedder.py
 deeppavlov/models/entity_extraction/__init__.py
 deeppavlov/models/entity_extraction/entity_detection_parser.py
 deeppavlov/models/entity_extraction/entity_linking.py
+deeppavlov/models/entity_extraction/find_word.py
 deeppavlov/models/entity_extraction/ner_chunker.py
 deeppavlov/models/kbqa/__init__.py
 deeppavlov/models/kbqa/query_generator.py
 deeppavlov/models/kbqa/query_generator_base.py
 deeppavlov/models/kbqa/rel_ranking_infer.py
+deeppavlov/models/kbqa/ru_adj_to_noun.py
 deeppavlov/models/kbqa/sentence_answer.py
 deeppavlov/models/kbqa/template_matcher.py
 deeppavlov/models/kbqa/tree_to_sparql.py
 deeppavlov/models/kbqa/type_define.py
 deeppavlov/models/kbqa/utils.py
 deeppavlov/models/kbqa/wiki_parser.py
 deeppavlov/models/preprocessors/__init__.py
@@ -256,40 +259,38 @@
 deeppavlov/models/torch_bert/__init__.py
 deeppavlov/models/torch_bert/crf.py
 deeppavlov/models/torch_bert/multitask_transformer.py
 deeppavlov/models/torch_bert/torch_bert_ranker.py
 deeppavlov/models/torch_bert/torch_transformers_classifier.py
 deeppavlov/models/torch_bert/torch_transformers_el_ranker.py
 deeppavlov/models/torch_bert/torch_transformers_multiplechoice.py
+deeppavlov/models/torch_bert/torch_transformers_nll_ranking.py
 deeppavlov/models/torch_bert/torch_transformers_sequence_tagger.py
 deeppavlov/models/torch_bert/torch_transformers_squad.py
 deeppavlov/models/vectorizers/__init__.py
 deeppavlov/models/vectorizers/hashing_tfidf_vectorizer.py
 deeppavlov/requirements/datasets.txt
 deeppavlov/requirements/en_core_web_sm.txt
 deeppavlov/requirements/fasttext.txt
 deeppavlov/requirements/hdt.txt
 deeppavlov/requirements/kenlm.txt
 deeppavlov/requirements/lxml.txt
 deeppavlov/requirements/opt_einsum.txt
 deeppavlov/requirements/pytorch.txt
 deeppavlov/requirements/rapidfuzz.txt
+deeppavlov/requirements/razdel.txt
 deeppavlov/requirements/ru_core_news_sm.txt
 deeppavlov/requirements/sacremoses.txt
 deeppavlov/requirements/slovnet.txt
 deeppavlov/requirements/sortedcontainers.txt
 deeppavlov/requirements/torchcrf.txt
 deeppavlov/requirements/transformers.txt
 deeppavlov/requirements/udapi.txt
 deeppavlov/requirements/whapi.txt
 deeppavlov/utils/__init__.py
-deeppavlov/utils/agent/__init__.py
-deeppavlov/utils/agent/messages.py
-deeppavlov/utils/agent/rabbitmq.py
-deeppavlov/utils/agent/server.py
 deeppavlov/utils/connector/__init__.py
 deeppavlov/utils/connector/dialog_logger.py
 deeppavlov/utils/pip_wrapper/__init__.py
 deeppavlov/utils/pip_wrapper/pip_wrapper.py
 deeppavlov/utils/server/__init__.py
 deeppavlov/utils/server/metrics.py
 deeppavlov/utils/server/server.py
```

### Comparing `deeppavlov-1.1.1/deeppavlov.egg-info/requires.txt` & `deeppavlov-1.2.0/deeppavlov.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-aio-pika<6.9.0,>=3.2.2
-fastapi<0.78.0,>=0.47.0
+fastapi<=0.89.1,>=0.47.0
 filelock<3.10.0,>=3.0.0
-nltk<3.10.0,>=3.2.5
+nltk<3.10.0,>=3.2.4
 numpy<1.24
-overrides==4.1.2
 pandas<1.6.0,>=1.0.0
-prometheus-client<0.15.0,>=0.13.0
+prometheus-client<=1.16.0,>=0.13.0
 pydantic
-pybind11==2.2.4
+pybind11==2.10.3
 requests<3.0.0,>=2.19.0
 scikit-learn<1.1.0,>=0.24
 scipy<1.10.0
 tqdm<4.65.0,>=4.42.0
 uvicorn<0.19.0,>=0.13.0
 
 [docs]
 sphinx_rtd_theme==0.5.2
+docutils<0.17,>=0.12
 nbsphinx==0.8.4
 ipykernel==5.5.4
 jinja2<=3.0.3
 sphinx-copybutton==0.5.0
-pandoc==2.2
+pandoc==2.3
 ipython_genutils==0.2.0
 
 [docs:python_version < "3.10"]
 sphinx==3.5.4
 
 [docs:python_version >= "3.10"]
 sphinx==4.5.0
```

### Comparing `deeppavlov-1.1.1/setup.py` & `deeppavlov-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,19 +67,20 @@
                 'pytest-instafail',
                 'pexpect'
             ],
             'docs': [
                 'sphinx==3.5.4;python_version<"3.10"',
                 'sphinx==4.5.0;python_version>="3.10"',
                 'sphinx_rtd_theme==0.5.2',
+                'docutils<0.17,>=0.12',
                 'nbsphinx==0.8.4',
                 'ipykernel==5.5.4',
                 'jinja2<=3.0.3',
                 'sphinx-copybutton==0.5.0',
-                'pandoc==2.2',
+                'pandoc==2.3',
                 'ipython_genutils==0.2.0'
             ],
             's3': [
                 'boto3'
             ]
         },
         **read_requirements()
```

### Comparing `deeppavlov-1.1.1/tests/test_quick_start.py` & `deeppavlov-1.2.0/tests/test_quick_start.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,16 +103,16 @@
     },
     "classifiers": {
         ("classifiers/paraphraser_rubert.json", "classifiers", ('IP', 'TI')): [TWO_ARGUMENTS_INFER_CHECK],
         ("classifiers/insults_kaggle_bert.json", "classifiers", ('IP', 'TI')): [ONE_ARGUMENT_INFER_CHECK],
         ("classifiers/rusentiment_bert.json", "classifiers", ('IP',)): [ONE_ARGUMENT_INFER_CHECK],
         ("classifiers/sentiment_twitter.json", "classifiers", ALL_MODES): [ONE_ARGUMENT_INFER_CHECK],
         ("classifiers/sentiment_sst_conv_bert.json", "classifiers", ('IP',)): [ONE_ARGUMENT_INFER_CHECK],
-        ("classifiers/glue/glue_mrpc_cased_bert_torch.json", "classifiers", ('TI',)): [TWO_ARGUMENTS_INFER_CHECK],
-        ("classifiers/glue/glue_stsb_cased_bert_torch.json", "classifiers", ('TI',)): [TWO_ARGUMENTS_INFER_CHECK],
+        ("classifiers/glue/glue_mrpc_roberta.json", "classifiers", ('TI',)): [TWO_ARGUMENTS_INFER_CHECK],
+        ("classifiers/glue/glue_stsb_roberta.json", "classifiers", ('TI',)): [TWO_ARGUMENTS_INFER_CHECK],
         ("classifiers/glue/glue_mnli_roberta.json", "classifiers", ('TI',)): [TWO_ARGUMENTS_INFER_CHECK],
         ("classifiers/glue/glue_rte_roberta_mnli.json", "classifiers", ('TI',)): [TWO_ARGUMENTS_INFER_CHECK],
         ("classifiers/superglue/superglue_copa_roberta.json", "classifiers", ('TI',)): [LIST_ARGUMENTS_INFER_CHECK],
         ("classifiers/superglue/superglue_boolq_roberta_mnli.json", "classifiers", ('TI',)): [TWO_ARGUMENTS_INFER_CHECK],
         ("classifiers/superglue/superglue_record_roberta.json", "classifiers", ('TI',)): [RECORD_ARGUMENTS_INFER_CHECK],
         ("classifiers/topics_distilbert_base_uncased.json", "classifiers", ('TI',)): [ONE_ARGUMENT_INFER_CHECK]
     },
@@ -134,14 +134,20 @@
         ("russian_super_glue/russian_superglue_rcb_rubert.json", "russian_super_glue", ('IP',)): [TWO_ARGUMENTS_INFER_CHECK],
         ("russian_super_glue/russian_superglue_russe_rubert.json", "russian_super_glue", ('IP',)): [TWO_ARGUMENTS_INFER_CHECK],
         ("russian_super_glue/russian_superglue_rwsd_rubert.json", "russian_super_glue", ('IP',)): [TWO_ARGUMENTS_INFER_CHECK],
         ("russian_super_glue/russian_superglue_muserc_rubert.json", "russian_super_glue", ('IP',)): [TWO_ARGUMENTS_INFER_CHECK],
         ("russian_super_glue/russian_superglue_parus_rubert.json", "russian_super_glue", ('IP',)): [LIST_ARGUMENTS_INFER_CHECK],
         ("russian_super_glue/russian_superglue_rucos_rubert.json", "russian_super_glue", ('IP',)): [RECORD_ARGUMENTS_INFER_CHECK]
     },
+    "multitask":{
+        ("multitask/multitask_example.json", "multitask", ALL_MODES): [
+            ('Dummy text',) + (('Dummy text', 'Dummy text'),) * 3 + ('Dummy text',) + (None,)],
+        ("multitask/mt_glue.json", "multitask", ALL_MODES): [
+            ('Dummy text',) * 2 + (('Dummy text', 'Dummy text'),) * 6 + (None,)]
+    },
     "entity_extraction": {
         ("entity_extraction/entity_detection_en.json", "entity_extraction", ('IP',)):
             [
                 ("Forrest Gump is a comedy-drama film directed by Robert Zemeckis and written by Eric Roth.",
                  (['forrest gump', 'robert zemeckis', 'eric roth'],
                   [(0, 12), (48, 63), (79, 88)],
                   [[0, 1], [10, 11], [15, 16]],
@@ -157,80 +163,52 @@
                   [(0, 6), (17, 23), (31, 63), (72, 90)],
                   [[0], [3], [6, 7, 8], [11, 12]],
                   ['CITY', 'COUNTRY', 'LOC', 'LOC'],
                   [(0, 91)],
                   ['Москва — столица России, центр Центрального федерального округа и центр Московской области.'],
                   [0.8359, 0.938, 0.9917, 0.9803]))
             ],
-        ("entity_extraction/entity_linking_en.json", "entity_extraction", ('IP',)):
-            [
-                (['forrest gump', 'robert zemeckis', 'eric roth'],
-                 ['WORK_OF_ART', 'PERSON', 'PERSON'],
-                 ['Forrest Gump is a comedy-drama film directed by Robert Zemeckis and written by Eric Roth.'],
-                 [(0, 12), (48, 63), (79, 88)],
-                 [(0, 89)],
-                 ([['Q134773', 'Q552213', 'Q12016774'], ['Q187364', 'Q36951156'], ['Q942932', 'Q89320386', 'Q89909683']],
-                  [[(1.0, 110, 1.0), (1.0, 13, 0.73), (1.0, 8, 0.04)],
-                   [(1.0, 73, 1.0), (0.5, 52, 0.29)],
-                   [(1.0, 37, 0.95), (1.0, 2, 0.35), (0.67, 2, 0.35)]],
-                  [['Forrest Gump', 'Forrest Gump (novel)', ''],
-                   ['Robert Zemeckis', 'Welcome to Marwen'], ['Eric Roth', '', '']]))
-            ],
-        ("entity_extraction/entity_linking_ru.json", "entity_extraction", ('IP',)):
-            [
-                (['москва', 'россии', 'центрального федерального округа', 'московской области'],
-                 ['CITY', 'COUNTRY', 'LOC', 'LOC'],
-                 ['Москва — столица России, центр Центрального федерального округа и центр Московской области.'],
-                 [(0, 6), (17, 23), (31, 63), (72, 90)],
-                 [(0, 91)],
-                 ([['Q649', 'Q1023006', 'Q2380475'], ['Q159', 'Q2184', 'Q139319'],
-                   ['Q190778', 'Q484215', 'Q21104009'], ['Q1697', 'Q4303932', 'Q24565285']],
-                  [[(1.0, 134, 1.0), (1.0, 20, 0.0), (1.0, 18, 0.0)],
-                   [(1.0, 203, 1.0), (1.0, 58, 1.0), (1.0, 29, 0.93)],
-                   [(1.0, 24, 0.28), (0.67, 11, 0.5), (0.67, 8, 0.4)],
-                   [(0.9, 30, 1.0), (0.9, 6, 0.83), (0.61, 8, 0.03)]],
-                  [['Москва', 'Москоу (Канзас)', 'Москоу (Теннесси)'],
-                   ['Россия', 'Российская Советская Федеративная Социалистическая Республика',
-                    'Российская республика'],
-                   ['Центральный федеральный округ', 'Федеральные округа Российской Федерации',
-                    'Центральный административный округ (Назрань)'],
-                   ['Московская область', 'Московская область (1917—1918)',
-                    'Мостовский (Волгоградская область)']]))
-            ],
         ("entity_extraction/entity_extraction_en.json", "entity_extraction", ('IP',)):
             [
                 ("Forrest Gump is a comedy-drama film directed by Robert Zemeckis and written by Eric Roth.",
                  (['forrest gump', 'robert zemeckis', 'eric roth'],
                   ['WORK_OF_ART', 'PERSON', 'PERSON'],
                   [(0, 12), (48, 63), (79, 88)],
                   [['Q134773', 'Q552213', 'Q12016774'], ['Q187364', 'Q36951156'],
                    ['Q942932', 'Q89320386', 'Q89909683']],
-                  [[(1.0, 110, 1.0), (1.0, 13, 0.73), (1.0, 8, 0.04)], [(1.0, 73, 1.0), (0.5, 52, 0.29)],
-                   [(1.0, 37, 0.95), (1.0, 2, 0.35), (0.67, 2, 0.35)]],
+                  [[[1.1, 110, 1.0], [1.1, 13, 0.73], [1.1, 8, 0.04]], [[1.1, 73, 1.0], [0.5, 52, 0.29]],
+                   [[1.1, 37, 0.95], [1.1, 2, 0.35], [0.67, 2, 0.35]]],
                   [['Forrest Gump', 'Forrest Gump (novel)', ''], ['Robert Zemeckis', 'Welcome to Marwen'],
-                   ['Eric Roth', '', '']]))
+                   ['Eric Roth', '', '']],
+                  [['Forrest Gump', 'Forrest Gump', 'Forrest Gump'], ['Robert Zemeckis', 'Welcome to Marwen'],
+                   ['Eric Roth', 'Eric Roth', 'Eric W Roth']]))
             ],
         ("entity_extraction/entity_extraction_ru.json", "entity_extraction", ('IP',)):
             [
                 ("Москва — столица России, центр Центрального федерального округа и центр Московской области.",
                  (['москва', 'россии', 'центрального федерального округа', 'московской области'],
                   ['CITY', 'COUNTRY', 'LOC', 'LOC'],
                   [(0, 6), (17, 23), (31, 63), (72, 90)],
-                  [['Q649', 'Q1023006', 'Q2380475'], ['Q159', 'Q2184', 'Q139319'],
-                   ['Q190778', 'Q484215', 'Q21104009'], ['Q1697', 'Q4303932', 'Q24565285']],
-                  [[(1.0, 134, 1.0), (1.0, 20, 0.0), (1.0, 18, 0.0)],
-                   [(1.0, 203, 1.0), (1.0, 58, 1.0), (1.0, 29, 0.93)],
-                   [(1.0, 24, 0.28), (0.67, 11, 0.5), (0.67, 8, 0.4)],
-                   [(0.9, 30, 1.0), (0.9, 6, 0.83), (0.61, 8, 0.03)]],
+                  [['Q649', 'Q1023006', 'Q2380475'], ['Q159', 'Q2184', 'Q139319'], ['Q190778', 'Q4504288', 'Q27557290'],
+                   ['Q1697', 'Q4303932', 'Q24565285']],
+                  [[[1.1, 200, 1.0], [1.0, 20, 0.0], [1.0, 18, 0.0]],
+                   [[1.1, 200, 1.0], [1.0, 58, 1.0], [1.0, 29, 0.85]],
+                   [[1.1, 200, 1.0], [0.67, 3, 0.92], [0.67, 3, 0.89]],
+                   [[0.9, 200, 1.0], [0.9, 6, 0.83], [0.61, 8, 0.03]]],
                   [['Москва', 'Москоу (Канзас)', 'Москоу (Теннесси)'],
                    ['Россия', 'Российская Советская Федеративная Социалистическая Республика',
                     'Российская республика'],
-                   ['Центральный федеральный округ', 'Федеральные округа Российской Федерации',
-                    'Центральный административный округ (Назрань)'],
-                   ['Московская область', 'Московская область (1917—1918)', 'Мостовский (Волгоградская область)']]))
+                   ['Центральный федеральный округ', 'Центральный округ (Краснодар)', ''],
+                   ['Московская область', 'Московская область (1917—1918)',
+                    'Мостовский (Волгоградская область)']],
+                  [['Москва', 'Москоу', 'Москоу'],
+                   ['Россия', 'Российская Советская Федеративная Социалистическая Республика',
+                    'Российская республика'],
+                   ['Центральный федеральный округ', 'Центральный округ (Краснодар)', 'Центральный округ (Братск)'],
+                   ['Московская область', 'Московская область', 'Мостовский']]))
             ]
     },
     "ner": {
         ("ner/ner_conll2003_bert.json", "ner_conll2003_bert", ('IP', 'TI')): [ONE_ARGUMENT_INFER_CHECK],
         ("ner/ner_ontonotes_bert.json", "ner_ontonotes_bert", ('IP', 'TI')): [ONE_ARGUMENT_INFER_CHECK],
         ("ner/ner_ontonotes_bert_mult.json", "ner_ontonotes_bert_mult", ('IP', 'TI')): [ONE_ARGUMENT_INFER_CHECK],
         ("ner/ner_rus_bert.json", "ner_rus_bert", ('IP', 'TI')): [ONE_ARGUMENT_INFER_CHECK],
@@ -239,24 +217,30 @@
     "sentence_segmentation": {
         ("sentence_segmentation/sentseg_dailydialog_bert.json", "sentseg_dailydialog_bert", ('IP', 'TI')): [
             (["hey", "alexa", "how", "are", "you"], None)]
     },
     "kbqa": {
         ("kbqa/kbqa_cq_en.json", "kbqa", ('IP',)):
             [
-                ("What is the currency of Sweden?", ("Swedish krona",)),
-                ("Where was Napoleon Bonaparte born?", ("Ajaccio",)),
-                ("When did the Korean War end?", ("27 July 1953",)),
-                ("   ", ("Not Found",))
-            ],
+                ("What is the currency of Sweden?",
+                 ("Swedish krona", ["Q122922"], ["SELECT ?answer WHERE { wd:Q34 wdt:P38 ?answer. }"])),
+                ("Where was Napoleon Bonaparte born?",
+                 ("Ajaccio", ["Q40104"], ["SELECT ?answer WHERE { wd:Q517 wdt:P19 ?answer. }"])),
+                ("When did the Korean War end?",
+                 ("27 July 1953", ["+1953-07-27^^T"], ["SELECT ?answer WHERE { wd:Q8663 wdt:P582 ?answer. }"])),
+                ("   ", ("Not Found", [], []))
+            ],            
         ("kbqa/kbqa_cq_ru.json", "kbqa", ('IP',)):
             [
-                ("Кто такой Оксимирон?", ("российский рэп-исполнитель",)),
-                ("Кто написал «Евгений Онегин»?", ("Александр Сергеевич Пушкин",)),
-                ("абв", ("Not Found",))
+                ("Кто такой Оксимирон?",
+                 ("российский рэп-исполнитель", ['российский рэп-исполнитель"@ru'],
+                  ["SELECT ?answer WHERE { wd:Q4046107 wdt:P0 ?answer. }"])),
+                ("Кто написал «Евгений Онегин»?",
+                 ("Александр Сергеевич Пушкин", ["Q7200"], ["SELECT ?answer WHERE { wd:Q50948 wdt:P50 ?answer. }"])),
+                ("абв", ("Not Found", [], []))
             ]
     },
     "ranking": {
         ("ranking/ranking_ubuntu_v2_torch_bert_uncased.json", "ranking", ('TI',)): [ONE_ARGUMENT_INFER_CHECK]
     },
     "doc_retrieval": {
         ("doc_retrieval/en_ranker_tfidf_wiki_test.json", "doc_retrieval", ('TI',)): [ONE_ARGUMENT_INFER_CHECK],
@@ -395,15 +379,16 @@
             errors = ';'.join([f'expected `{expected}` got `{output}`'
                                for output, expected in zip(outputs, expected_outputs)
                                if expected is not None and expected != output])
             if errors:
                 raise RuntimeError(f'Unexpected results for {config_path}: {errors}')
 
     @staticmethod
-    def infer_api(config_path):
+    def infer_api(config_path, qr_list):
+        *inputs, expected_outputs = zip(*qr_list)
         server_params = get_server_params(config_path)
 
         url_base = 'http://{}:{}'.format(server_params['host'], api_port or server_params['port'])
         url = urljoin(url_base.replace('http://0.0.0.0:', 'http://127.0.0.1:'), server_params['model_endpoint'])
 
         post_headers = {'Accept': 'application/json'}
 
@@ -418,22 +403,18 @@
 
             get_url = urljoin(url_base.replace('http://0.0.0.0:', 'http://127.0.0.1:'), '/api')
             get_response = requests.get(get_url)
             response_code = get_response.status_code
             assert response_code == 200, f"GET /api request returned error code {response_code} with {config_path}"
 
             model_args_names = get_response.json()['in']
-            post_payload = dict()
-            for arg_name in model_args_names:
-                arg_value = ' '.join(['qwerty'] * 10)
-                post_payload[arg_name] = [arg_value]
+            post_payload = dict(zip(model_args_names, inputs))
             # TODO: remove this if from here and socket
-            if 'parus' in str(config_path):
-                post_payload = {k: [v] for k, v in post_payload.items()}
-
+            if 'docred' in str(config_path) or 'rured' in str(config_path):
+                post_payload = {k: v[0] for k, v in post_payload.items()}
             post_response = requests.post(url, json=post_payload, headers=post_headers)
             response_code = post_response.status_code
             assert response_code == 200, f"POST request returned error code {response_code} with {config_path}"
 
         except pexpect.exceptions.EOF:
             raise RuntimeError('Got unexpected EOF: \n{}'.format(logfile.getvalue().decode()))
 
@@ -515,15 +496,15 @@
 
             self.infer(test_configs_path / conf_file, PARAMS[model][(conf_file, model_dir, mode)])
         else:
             pytest.skip("Unsupported mode: {}".format(mode))
 
     def test_inferring_pretrained_model_api(self, model, conf_file, model_dir, mode):
         if 'IP' in mode:
-            self.infer_api(test_configs_path / conf_file)
+            self.infer_api(test_configs_path / conf_file, PARAMS[model][(conf_file, model_dir, mode)])
         else:
             pytest.skip("Unsupported mode: {}".format(mode))
 
     def test_inferring_pretrained_model_socket(self, model, conf_file, model_dir, mode):
         pytest.skip(f"Disabled")
         if 'IP' in mode:
             self.infer_socket(test_configs_path / conf_file, 'TCP')
```

### Comparing `deeppavlov-1.1.1/utils/prepare/hashes.py` & `deeppavlov-1.2.0/utils/prepare/hashes.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/utils/prepare/registry.py` & `deeppavlov-1.2.0/utils/prepare/registry.py`

 * *Files identical despite different names*

### Comparing `deeppavlov-1.1.1/utils/prepare/upload.py` & `deeppavlov-1.2.0/utils/prepare/upload.py`

 * *Files identical despite different names*

