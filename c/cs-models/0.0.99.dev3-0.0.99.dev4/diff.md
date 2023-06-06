# Comparing `tmp/cs-models-0.0.99.dev3.tar.gz` & `tmp/cs-models-0.0.99.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cs-models-0.0.99.dev3.tar", last modified: Wed May 20 21:45:49 2020, max compression
+gzip compressed data, was "dist/cs-models-0.0.99.dev4.tar", last modified: Wed May 20 22:01:23 2020, max compression
```

## Comparing `cs-models-0.0.99.dev3.tar` & `cs-models-0.0.99.dev4.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/
--rw-r--r--   0 sverma     (501) staff       (20)      317 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/PKG-INFO
--rw-r--r--   0 sverma     (501) staff       (20)     1040 2020-05-20 21:45:33.000000 cs-models-0.0.99.dev3/setup.py
--rw-r--r--   0 sverma     (501) staff       (20)       59 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/setup.cfg
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models.egg-info/
--rw-r--r--   0 sverma     (501) staff       (20)      317 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models.egg-info/PKG-INFO
--rw-r--r--   0 sverma     (501) staff       (20)    10029 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models.egg-info/SOURCES.txt
--rw-r--r--   0 sverma     (501) staff       (20)      226 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models.egg-info/requires.txt
--rw-r--r--   0 sverma     (501) staff       (20)       10 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models.egg-info/top_level.txt
--rw-r--r--   0 sverma     (501) staff       (20)        1 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models.egg-info/dependency_links.txt
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_mongo/
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_mongo/DocumentTree/
--rw-r--r--   0 sverma     (501) staff       (20)     4308 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources_mongo/DocumentTree/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      416 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources_mongo/DocumentTree/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources_mongo/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/database/
--rw-r--r--   0 sverma     (501) staff       (20)     3064 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev3/src/cs_models/database/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CompanySEC/
--rw-r--r--   0 sverma     (501) staff       (20)     3197 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CompanySEC/test_company_sec.py
--rw-r--r--   0 sverma     (501) staff       (20)      596 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CompanySEC/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     2995 2019-10-27 22:48:20.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CompanySEC/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      416 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CompanySEC/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PriorArtRefRelation/
--rw-r--r--   0 sverma     (501) staff       (20)     1028 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PriorArtRefRelation/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     3843 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PriorArtRefRelation/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     1081 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PriorArtRefRelation/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     8538 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PriorArtRefRelation/test_prior_art_ref_relation.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Document/
--rw-r--r--   0 sverma     (501) staff       (20)     2084 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Document/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5916 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Document/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     3349 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Document/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)    11558 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Document/test_ptab2_document.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/RelatedMatter/
--rw-r--r--   0 sverma     (501) staff       (20)      927 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/RelatedMatter/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     3699 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/RelatedMatter/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     1175 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/RelatedMatter/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     8858 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/RelatedMatter/test_related_matter.py
--rw-r--r--   0 sverma     (501) staff       (20)     1926 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/all_models.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/DocumentReference/
--rw-r--r--   0 sverma     (501) staff       (20)      947 2020-03-30 21:11:18.000000 cs-models-0.0.99.dev3/src/cs_models/resources/DocumentReference/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     8926 2020-02-27 22:37:25.000000 cs-models-0.0.99.dev3/src/cs_models/resources/DocumentReference/test_document_reference.py
--rw-r--r--   0 sverma     (501) staff       (20)     5353 2020-02-27 22:35:04.000000 cs-models-0.0.99.dev3/src/cs_models/resources/DocumentReference/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     1390 2020-02-27 22:35:04.000000 cs-models-0.0.99.dev3/src/cs_models/resources/DocumentReference/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/File/
--rw-r--r--   0 sverma     (501) staff       (20)      603 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/File/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     6143 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/File/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     1116 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/File/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     6285 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/File/test_file.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/InstitutionProbability/
--rw-r--r--   0 sverma     (501) staff       (20)      782 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/InstitutionProbability/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     4126 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/InstitutionProbability/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      816 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/InstitutionProbability/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     4412 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/InstitutionProbability/test_institution_probability.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PriorArt/
--rw-r--r--   0 sverma     (501) staff       (20)      584 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PriorArt/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     4001 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PriorArt/test_prior_art.py
--rw-r--r--   0 sverma     (501) staff       (20)     6210 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PriorArt/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      976 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PriorArt/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/NDC/
--rw-r--r--   0 sverma     (501) staff       (20)     1184 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev3/src/cs_models/resources/NDC/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     4717 2020-05-05 01:17:30.000000 cs-models-0.0.99.dev3/src/cs_models/resources/NDC/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     6377 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev3/src/cs_models/resources/NDC/test_ndc.py
--rw-r--r--   0 sverma     (501) staff       (20)     1850 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev3/src/cs_models/resources/NDC/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookPatent/
--rw-r--r--   0 sverma     (501) staff       (20)      782 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookPatent/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5336 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookPatent/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     2688 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookPatent/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     9596 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookPatent/test_orange_book_patent.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PacerCase/
--rw-r--r--   0 sverma     (501) staff       (20)     7412 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PacerCase/test_pacer_case.py
--rw-r--r--   0 sverma     (501) staff       (20)     1074 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PacerCase/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5605 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PacerCase/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     1866 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PacerCase/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ClaimChallenged/
--rw-r--r--   0 sverma     (501) staff       (20)     1036 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ClaimChallenged/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     4585 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ClaimChallenged/test_claim_challenged.py
--rw-r--r--   0 sverma     (501) staff       (20)     5443 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ClaimChallenged/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      795 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ClaimChallenged/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Pharmacologic/
--rw-r--r--   0 sverma     (501) staff       (20)      789 2020-05-20 13:50:16.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Pharmacologic/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     4457 2020-05-20 20:24:43.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Pharmacologic/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     3381 2020-05-20 15:46:00.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Pharmacologic/test_pharmacologic.py
--rw-r--r--   0 sverma     (501) staff       (20)     1347 2020-05-20 13:50:16.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Pharmacologic/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Patent/
--rw-r--r--   0 sverma     (501) staff       (20)     1476 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Patent/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5648 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Patent/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     3627 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Patent/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     7754 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Patent/test_patent.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Newswire/
--rw-r--r--   0 sverma     (501) staff       (20)      725 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Newswire/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5189 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Newswire/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     2187 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Newswire/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     7838 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Newswire/test_newswire.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CrossRef/
--rw-r--r--   0 sverma     (501) staff       (20)      866 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CrossRef/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     4291 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CrossRef/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     6048 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CrossRef/test_crossref.py
--rw-r--r--   0 sverma     (501) staff       (20)     1032 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CrossRef/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Proceeding/
--rw-r--r--   0 sverma     (501) staff       (20)     2123 2019-12-04 00:37:20.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Proceeding/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5257 2019-12-04 00:37:20.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Proceeding/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)    12889 2019-12-04 00:37:20.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Proceeding/test_ptabv2_proceeding.py
--rw-r--r--   0 sverma     (501) staff       (20)     2948 2019-12-04 00:37:20.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Proceeding/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/SubsidiarySponsorMapping/
--rw-r--r--   0 sverma     (501) staff       (20)      746 2020-04-10 20:08:05.000000 cs-models-0.0.99.dev3/src/cs_models/resources/SubsidiarySponsorMapping/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5977 2020-04-10 20:08:05.000000 cs-models-0.0.99.dev3/src/cs_models/resources/SubsidiarySponsorMapping/test_subsidiary_sponsor_mapping.py
--rw-r--r--   0 sverma     (501) staff       (20)     4293 2020-04-10 20:08:05.000000 cs-models-0.0.99.dev3/src/cs_models/resources/SubsidiarySponsorMapping/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      727 2020-04-10 20:08:05.000000 cs-models-0.0.99.dev3/src/cs_models/resources/SubsidiarySponsorMapping/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CompanyOUS/
--rw-r--r--   0 sverma     (501) staff       (20)     3642 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CompanyOUS/test_company_ous.py
--rw-r--r--   0 sverma     (501) staff       (20)      568 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CompanyOUS/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     3726 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CompanyOUS/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      652 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev3/src/cs_models/resources/CompanyOUS/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/SetIDPharmacologicCross/
--rw-r--r--   0 sverma     (501) staff       (20)     2482 2020-05-20 20:27:30.000000 cs-models-0.0.99.dev3/src/cs_models/resources/SetIDPharmacologicCross/test_set_id_pharmacologic_cross.py
--rw-r--r--   0 sverma     (501) staff       (20)      398 2020-05-20 21:44:34.000000 cs-models-0.0.99.dev3/src/cs_models/resources/SetIDPharmacologicCross/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     2960 2020-05-20 20:31:14.000000 cs-models-0.0.99.dev3/src/cs_models/resources/SetIDPharmacologicCross/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      514 2020-05-20 20:24:43.000000 cs-models-0.0.99.dev3/src/cs_models/resources/SetIDPharmacologicCross/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/FederalCaseRef/
--rw-r--r--   0 sverma     (501) staff       (20)      918 2020-04-06 05:08:56.000000 cs-models-0.0.99.dev3/src/cs_models/resources/FederalCaseRef/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     3170 2020-04-06 05:08:56.000000 cs-models-0.0.99.dev3/src/cs_models/resources/FederalCaseRef/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      590 2020-04-06 05:08:56.000000 cs-models-0.0.99.dev3/src/cs_models/resources/FederalCaseRef/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     4664 2020-04-06 05:08:56.000000 cs-models-0.0.99.dev3/src/cs_models/resources/FederalCaseRef/test_federal_case_ref.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/TrialStat/
--rw-r--r--   0 sverma     (501) staff       (20)      662 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/TrialStat/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     3806 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/TrialStat/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     4549 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/TrialStat/test_trial_stat.py
--rw-r--r--   0 sverma     (501) staff       (20)      716 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/TrialStat/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentIdentifierSynonym/
--rw-r--r--   0 sverma     (501) staff       (20)      539 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentIdentifierSynonym/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     3471 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentIdentifierSynonym/test_patent_identifier_synonym.py
--rw-r--r--   0 sverma     (501) staff       (20)     3005 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentIdentifierSynonym/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      612 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentIdentifierSynonym/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/UserSearchHistoryItem/
--rw-r--r--   0 sverma     (501) staff       (20)      532 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/UserSearchHistoryItem/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     2972 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/UserSearchHistoryItem/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      747 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/UserSearchHistoryItem/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     2904 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/UserSearchHistoryItem/test_user_search_history_item.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/AbstractText/
--rw-r--r--   0 sverma     (501) staff       (20)      461 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/AbstractText/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     4992 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/AbstractText/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      508 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/AbstractText/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     2546 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/AbstractText/test_abstract_text.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Decision/
--rw-r--r--   0 sverma     (501) staff       (20)     1863 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Decision/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     4533 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Decision/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     2944 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Decision/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     9114 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Decision/test_ptabv2_decision.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/NDCSetIDCross/
--rw-r--r--   0 sverma     (501) staff       (20)     2451 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev3/src/cs_models/resources/NDCSetIDCross/test_ndc_setid_cross.py
--rw-r--r--   0 sverma     (501) staff       (20)      434 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev3/src/cs_models/resources/NDCSetIDCross/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     2769 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev3/src/cs_models/resources/NDCSetIDCross/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      626 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev3/src/cs_models/resources/NDCSetIDCross/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentApplication/
--rw-r--r--   0 sverma     (501) staff       (20)      759 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentApplication/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5009 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentApplication/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      928 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentApplication/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     4604 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentApplication/test_patent_application.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/DrugIndication/
--rw-r--r--   0 sverma     (501) staff       (20)     3824 2020-05-16 20:57:18.000000 cs-models-0.0.99.dev3/src/cs_models/resources/DrugIndication/test_indication.py
--rw-r--r--   0 sverma     (501) staff       (20)      586 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev3/src/cs_models/resources/DrugIndication/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5259 2020-05-16 20:57:18.000000 cs-models-0.0.99.dev3/src/cs_models/resources/DrugIndication/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     1040 2020-05-16 20:57:18.000000 cs-models-0.0.99.dev3/src/cs_models/resources/DrugIndication/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ProceedingStage/
--rw-r--r--   0 sverma     (501) staff       (20)      786 2019-10-24 16:04:45.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ProceedingStage/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     2450 2019-11-03 04:31:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ProceedingStage/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      534 2019-10-24 16:04:45.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ProceedingStage/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     4901 2019-11-03 04:31:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ProceedingStage/test_proceeding_stage.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Subsidiary/
--rw-r--r--   0 sverma     (501) staff       (20)      695 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Subsidiary/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     3574 2020-03-30 21:19:46.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Subsidiary/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     5408 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Subsidiary/test_subsidiary.py
--rw-r--r--   0 sverma     (501) staff       (20)     1236 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Subsidiary/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookExclusivity/
--rw-r--r--   0 sverma     (501) staff       (20)      768 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookExclusivity/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     6958 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookExclusivity/test_orange_book_exclusivity.py
--rw-r--r--   0 sverma     (501) staff       (20)     4538 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookExclusivity/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     1146 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookExclusivity/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ClaimDependency/
--rw-r--r--   0 sverma     (501) staff       (20)     2077 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ClaimDependency/test_claim_dependency.py
--rw-r--r--   0 sverma     (501) staff       (20)      496 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ClaimDependency/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     3422 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ClaimDependency/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      418 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/ClaimDependency/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Claim/
--rw-r--r--   0 sverma     (501) staff       (20)     6199 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Claim/test_claim.py
--rw-r--r--   0 sverma     (501) staff       (20)      848 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Claim/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     3529 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Claim/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     1374 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Claim/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Company/
--rw-r--r--   0 sverma     (501) staff       (20)     5056 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Company/test_company.py
--rw-r--r--   0 sverma     (501) staff       (20)      697 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Company/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     3810 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Company/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      791 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev3/src/cs_models/resources/Company/schemas.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookProduct/
--rw-r--r--   0 sverma     (501) staff       (20)     1134 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookProduct/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5227 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookProduct/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     2645 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookProduct/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)    14284 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookProduct/test_orange_book_product.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentCompound/
--rw-r--r--   0 sverma     (501) staff       (20)      851 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentCompound/models.py
--rw-r--r--   0 sverma     (501) staff       (20)     5287 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentCompound/test_patent_compound.py
--rw-r--r--   0 sverma     (501) staff       (20)     3038 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentCompound/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      967 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/resources/PatentCompound/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)       20 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/utils/
--rw-r--r--   0 sverma     (501) staff       (20)     1598 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/utils/alchemy.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/utils/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)     3664 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/utils/utils.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/utils/profiling/
--rw-r--r--   0 sverma     (501) staff       (20)      569 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev3/src/cs_models/utils/profiling/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/aact_database/
--rw-r--r--   0 sverma     (501) staff       (20)     1274 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/aact_database/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Intervention/
--rw-r--r--   0 sverma     (501) staff       (20)      714 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Intervention/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Intervention/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Study/
--rw-r--r--   0 sverma     (501) staff       (20)     3352 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Study/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Study/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/InterventionOtherNames/
--rw-r--r--   0 sverma     (501) staff       (20)      768 2020-04-07 02:12:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/InterventionOtherNames/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2020-04-06 05:08:48.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/InterventionOtherNames/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/DetailedDescription/
--rw-r--r--   0 sverma     (501) staff       (20)      637 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/DetailedDescription/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/DetailedDescription/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/BrowseCondition/
--rw-r--r--   0 sverma     (501) staff       (20)      669 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/BrowseCondition/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/BrowseCondition/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/BrowseIntervention/
--rw-r--r--   0 sverma     (501) staff       (20)      678 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/BrowseIntervention/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/BrowseIntervention/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/StudyReference/
--rw-r--r--   0 sverma     (501) staff       (20)      713 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/StudyReference/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/StudyReference/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Condition/
--rw-r--r--   0 sverma     (501) staff       (20)      630 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Condition/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Condition/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Link/
--rw-r--r--   0 sverma     (501) staff       (20)      636 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Link/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Link/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/BriefSummary/
--rw-r--r--   0 sverma     (501) staff       (20)      597 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/BriefSummary/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/BriefSummary/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Sponsor/
--rw-r--r--   0 sverma     (501) staff       (20)      872 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Sponsor/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Sponsor/__init__.py
--rw-r--r--   0 sverma     (501) staff       (20)      514 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Sponsor/schemas.py
--rw-r--r--   0 sverma     (501) staff       (20)     1561 2019-11-25 03:10:56.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/something.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/MeshTerm/
--rw-r--r--   0 sverma     (501) staff       (20)      773 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/MeshTerm/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/MeshTerm/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Keyword/
--rw-r--r--   0 sverma     (501) staff       (20)      645 2020-04-07 02:12:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Keyword/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2020-04-07 02:12:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/Keyword/__init__.py
-drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 21:45:49.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/MeshHeading/
--rw-r--r--   0 sverma     (501) staff       (20)      592 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/MeshHeading/models.py
--rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev3/src/cs_models/resources_aact/MeshHeading/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/
+-rw-r--r--   0 sverma     (501) staff       (20)      317 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/PKG-INFO
+-rw-r--r--   0 sverma     (501) staff       (20)     1040 2020-05-20 21:59:27.000000 cs-models-0.0.99.dev4/setup.py
+-rw-r--r--   0 sverma     (501) staff       (20)       59 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/setup.cfg
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models.egg-info/
+-rw-r--r--   0 sverma     (501) staff       (20)      317 2020-05-20 22:01:22.000000 cs-models-0.0.99.dev4/src/cs_models.egg-info/PKG-INFO
+-rw-r--r--   0 sverma     (501) staff       (20)    10029 2020-05-20 22:01:22.000000 cs-models-0.0.99.dev4/src/cs_models.egg-info/SOURCES.txt
+-rw-r--r--   0 sverma     (501) staff       (20)      226 2020-05-20 22:01:22.000000 cs-models-0.0.99.dev4/src/cs_models.egg-info/requires.txt
+-rw-r--r--   0 sverma     (501) staff       (20)       10 2020-05-20 22:01:22.000000 cs-models-0.0.99.dev4/src/cs_models.egg-info/top_level.txt
+-rw-r--r--   0 sverma     (501) staff       (20)        1 2020-05-20 22:01:22.000000 cs-models-0.0.99.dev4/src/cs_models.egg-info/dependency_links.txt
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_mongo/
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_mongo/DocumentTree/
+-rw-r--r--   0 sverma     (501) staff       (20)     4308 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources_mongo/DocumentTree/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      416 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources_mongo/DocumentTree/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources_mongo/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/database/
+-rw-r--r--   0 sverma     (501) staff       (20)     3064 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev4/src/cs_models/database/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CompanySEC/
+-rw-r--r--   0 sverma     (501) staff       (20)     3197 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CompanySEC/test_company_sec.py
+-rw-r--r--   0 sverma     (501) staff       (20)      596 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CompanySEC/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2995 2019-10-27 22:48:20.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CompanySEC/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      416 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CompanySEC/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PriorArtRefRelation/
+-rw-r--r--   0 sverma     (501) staff       (20)     1028 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PriorArtRefRelation/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3843 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PriorArtRefRelation/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1081 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PriorArtRefRelation/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     8538 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PriorArtRefRelation/test_prior_art_ref_relation.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Document/
+-rw-r--r--   0 sverma     (501) staff       (20)     2084 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Document/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5916 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Document/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3349 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Document/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)    11558 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Document/test_ptab2_document.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/RelatedMatter/
+-rw-r--r--   0 sverma     (501) staff       (20)      927 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/RelatedMatter/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3699 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/RelatedMatter/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1175 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/RelatedMatter/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     8858 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/RelatedMatter/test_related_matter.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1926 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/all_models.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/DocumentReference/
+-rw-r--r--   0 sverma     (501) staff       (20)      947 2020-03-30 21:11:18.000000 cs-models-0.0.99.dev4/src/cs_models/resources/DocumentReference/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     8926 2020-02-27 22:37:25.000000 cs-models-0.0.99.dev4/src/cs_models/resources/DocumentReference/test_document_reference.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5353 2020-02-27 22:35:04.000000 cs-models-0.0.99.dev4/src/cs_models/resources/DocumentReference/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1390 2020-02-27 22:35:04.000000 cs-models-0.0.99.dev4/src/cs_models/resources/DocumentReference/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/File/
+-rw-r--r--   0 sverma     (501) staff       (20)      603 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/File/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     6143 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/File/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1116 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/File/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     6285 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/File/test_file.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/InstitutionProbability/
+-rw-r--r--   0 sverma     (501) staff       (20)      782 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/InstitutionProbability/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4126 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/InstitutionProbability/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      816 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/InstitutionProbability/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4412 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/InstitutionProbability/test_institution_probability.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PriorArt/
+-rw-r--r--   0 sverma     (501) staff       (20)      584 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PriorArt/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4001 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PriorArt/test_prior_art.py
+-rw-r--r--   0 sverma     (501) staff       (20)     6210 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PriorArt/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      976 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PriorArt/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/NDC/
+-rw-r--r--   0 sverma     (501) staff       (20)     1184 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev4/src/cs_models/resources/NDC/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4717 2020-05-05 01:17:30.000000 cs-models-0.0.99.dev4/src/cs_models/resources/NDC/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     6377 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev4/src/cs_models/resources/NDC/test_ndc.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1850 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev4/src/cs_models/resources/NDC/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookPatent/
+-rw-r--r--   0 sverma     (501) staff       (20)      782 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookPatent/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5336 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookPatent/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2688 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookPatent/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     9596 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookPatent/test_orange_book_patent.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PacerCase/
+-rw-r--r--   0 sverma     (501) staff       (20)     7412 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PacerCase/test_pacer_case.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1074 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PacerCase/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5605 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PacerCase/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1866 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PacerCase/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ClaimChallenged/
+-rw-r--r--   0 sverma     (501) staff       (20)     1036 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ClaimChallenged/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4585 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ClaimChallenged/test_claim_challenged.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5443 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ClaimChallenged/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      795 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ClaimChallenged/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Pharmacologic/
+-rw-r--r--   0 sverma     (501) staff       (20)      789 2020-05-20 13:50:16.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Pharmacologic/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4457 2020-05-20 20:24:43.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Pharmacologic/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3381 2020-05-20 15:46:00.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Pharmacologic/test_pharmacologic.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1347 2020-05-20 13:50:16.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Pharmacologic/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Patent/
+-rw-r--r--   0 sverma     (501) staff       (20)     1476 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Patent/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5648 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Patent/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3627 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Patent/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     7754 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Patent/test_patent.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Newswire/
+-rw-r--r--   0 sverma     (501) staff       (20)      725 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Newswire/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5189 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Newswire/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2187 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Newswire/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     7838 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Newswire/test_newswire.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CrossRef/
+-rw-r--r--   0 sverma     (501) staff       (20)      866 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CrossRef/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4291 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CrossRef/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     6048 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CrossRef/test_crossref.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1032 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CrossRef/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Proceeding/
+-rw-r--r--   0 sverma     (501) staff       (20)     2123 2019-12-04 00:37:20.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Proceeding/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5257 2019-12-04 00:37:20.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Proceeding/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)    12889 2019-12-04 00:37:20.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Proceeding/test_ptabv2_proceeding.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2948 2019-12-04 00:37:20.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Proceeding/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/SubsidiarySponsorMapping/
+-rw-r--r--   0 sverma     (501) staff       (20)      746 2020-04-10 20:08:05.000000 cs-models-0.0.99.dev4/src/cs_models/resources/SubsidiarySponsorMapping/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5977 2020-04-10 20:08:05.000000 cs-models-0.0.99.dev4/src/cs_models/resources/SubsidiarySponsorMapping/test_subsidiary_sponsor_mapping.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4293 2020-04-10 20:08:05.000000 cs-models-0.0.99.dev4/src/cs_models/resources/SubsidiarySponsorMapping/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      727 2020-04-10 20:08:05.000000 cs-models-0.0.99.dev4/src/cs_models/resources/SubsidiarySponsorMapping/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CompanyOUS/
+-rw-r--r--   0 sverma     (501) staff       (20)     3642 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CompanyOUS/test_company_ous.py
+-rw-r--r--   0 sverma     (501) staff       (20)      568 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CompanyOUS/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3726 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CompanyOUS/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      652 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev4/src/cs_models/resources/CompanyOUS/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/SetIDPharmacologicCross/
+-rw-r--r--   0 sverma     (501) staff       (20)     2482 2020-05-20 20:27:30.000000 cs-models-0.0.99.dev4/src/cs_models/resources/SetIDPharmacologicCross/test_set_id_pharmacologic_cross.py
+-rw-r--r--   0 sverma     (501) staff       (20)      404 2020-05-20 21:53:19.000000 cs-models-0.0.99.dev4/src/cs_models/resources/SetIDPharmacologicCross/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2960 2020-05-20 20:31:14.000000 cs-models-0.0.99.dev4/src/cs_models/resources/SetIDPharmacologicCross/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      514 2020-05-20 20:24:43.000000 cs-models-0.0.99.dev4/src/cs_models/resources/SetIDPharmacologicCross/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/FederalCaseRef/
+-rw-r--r--   0 sverma     (501) staff       (20)      918 2020-04-06 05:08:56.000000 cs-models-0.0.99.dev4/src/cs_models/resources/FederalCaseRef/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3170 2020-04-06 05:08:56.000000 cs-models-0.0.99.dev4/src/cs_models/resources/FederalCaseRef/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      590 2020-04-06 05:08:56.000000 cs-models-0.0.99.dev4/src/cs_models/resources/FederalCaseRef/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4664 2020-04-06 05:08:56.000000 cs-models-0.0.99.dev4/src/cs_models/resources/FederalCaseRef/test_federal_case_ref.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/TrialStat/
+-rw-r--r--   0 sverma     (501) staff       (20)      662 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/TrialStat/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3806 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/TrialStat/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4549 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/TrialStat/test_trial_stat.py
+-rw-r--r--   0 sverma     (501) staff       (20)      716 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/TrialStat/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentIdentifierSynonym/
+-rw-r--r--   0 sverma     (501) staff       (20)      539 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentIdentifierSynonym/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3471 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentIdentifierSynonym/test_patent_identifier_synonym.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3005 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentIdentifierSynonym/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      612 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentIdentifierSynonym/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/UserSearchHistoryItem/
+-rw-r--r--   0 sverma     (501) staff       (20)      532 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/UserSearchHistoryItem/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2972 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/UserSearchHistoryItem/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      747 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/UserSearchHistoryItem/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2904 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/UserSearchHistoryItem/test_user_search_history_item.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/AbstractText/
+-rw-r--r--   0 sverma     (501) staff       (20)      461 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/AbstractText/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4992 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/AbstractText/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      508 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/AbstractText/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2546 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/AbstractText/test_abstract_text.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Decision/
+-rw-r--r--   0 sverma     (501) staff       (20)     1863 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Decision/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4533 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Decision/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2944 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Decision/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     9114 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Decision/test_ptabv2_decision.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/NDCSetIDCross/
+-rw-r--r--   0 sverma     (501) staff       (20)     2451 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev4/src/cs_models/resources/NDCSetIDCross/test_ndc_setid_cross.py
+-rw-r--r--   0 sverma     (501) staff       (20)      434 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev4/src/cs_models/resources/NDCSetIDCross/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2769 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev4/src/cs_models/resources/NDCSetIDCross/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      626 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev4/src/cs_models/resources/NDCSetIDCross/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentApplication/
+-rw-r--r--   0 sverma     (501) staff       (20)      759 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentApplication/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5009 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentApplication/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      928 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentApplication/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4604 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentApplication/test_patent_application.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/DrugIndication/
+-rw-r--r--   0 sverma     (501) staff       (20)     3824 2020-05-16 20:57:18.000000 cs-models-0.0.99.dev4/src/cs_models/resources/DrugIndication/test_indication.py
+-rw-r--r--   0 sverma     (501) staff       (20)      586 2020-05-19 14:44:08.000000 cs-models-0.0.99.dev4/src/cs_models/resources/DrugIndication/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5259 2020-05-16 20:57:18.000000 cs-models-0.0.99.dev4/src/cs_models/resources/DrugIndication/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1040 2020-05-16 20:57:18.000000 cs-models-0.0.99.dev4/src/cs_models/resources/DrugIndication/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ProceedingStage/
+-rw-r--r--   0 sverma     (501) staff       (20)      786 2019-10-24 16:04:45.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ProceedingStage/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2450 2019-11-03 04:31:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ProceedingStage/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      534 2019-10-24 16:04:45.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ProceedingStage/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4901 2019-11-03 04:31:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ProceedingStage/test_proceeding_stage.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Subsidiary/
+-rw-r--r--   0 sverma     (501) staff       (20)      695 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Subsidiary/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3574 2020-03-30 21:19:46.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Subsidiary/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5408 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Subsidiary/test_subsidiary.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1236 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Subsidiary/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookExclusivity/
+-rw-r--r--   0 sverma     (501) staff       (20)      768 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookExclusivity/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     6958 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookExclusivity/test_orange_book_exclusivity.py
+-rw-r--r--   0 sverma     (501) staff       (20)     4538 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookExclusivity/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1146 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookExclusivity/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ClaimDependency/
+-rw-r--r--   0 sverma     (501) staff       (20)     2077 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ClaimDependency/test_claim_dependency.py
+-rw-r--r--   0 sverma     (501) staff       (20)      496 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ClaimDependency/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3422 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ClaimDependency/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      418 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/ClaimDependency/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Claim/
+-rw-r--r--   0 sverma     (501) staff       (20)     6199 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Claim/test_claim.py
+-rw-r--r--   0 sverma     (501) staff       (20)      848 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Claim/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3529 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Claim/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1374 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Claim/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Company/
+-rw-r--r--   0 sverma     (501) staff       (20)     5056 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Company/test_company.py
+-rw-r--r--   0 sverma     (501) staff       (20)      697 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Company/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3810 2019-11-19 14:13:48.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Company/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      791 2019-10-28 04:40:52.000000 cs-models-0.0.99.dev4/src/cs_models/resources/Company/schemas.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookProduct/
+-rw-r--r--   0 sverma     (501) staff       (20)     1134 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookProduct/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5227 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookProduct/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     2645 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookProduct/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)    14284 2020-04-21 15:10:01.000000 cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookProduct/test_orange_book_product.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentCompound/
+-rw-r--r--   0 sverma     (501) staff       (20)      851 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentCompound/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)     5287 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentCompound/test_patent_compound.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3038 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentCompound/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      967 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/resources/PatentCompound/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)       20 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/utils/
+-rw-r--r--   0 sverma     (501) staff       (20)     1598 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/utils/alchemy.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/utils/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)     3664 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/utils/utils.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/utils/profiling/
+-rw-r--r--   0 sverma     (501) staff       (20)      569 2019-10-24 15:06:10.000000 cs-models-0.0.99.dev4/src/cs_models/utils/profiling/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/aact_database/
+-rw-r--r--   0 sverma     (501) staff       (20)     1274 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/aact_database/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Intervention/
+-rw-r--r--   0 sverma     (501) staff       (20)      714 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Intervention/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Intervention/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Study/
+-rw-r--r--   0 sverma     (501) staff       (20)     3352 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Study/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Study/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/InterventionOtherNames/
+-rw-r--r--   0 sverma     (501) staff       (20)      768 2020-04-07 02:12:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/InterventionOtherNames/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2020-04-06 05:08:48.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/InterventionOtherNames/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/DetailedDescription/
+-rw-r--r--   0 sverma     (501) staff       (20)      637 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/DetailedDescription/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/DetailedDescription/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/BrowseCondition/
+-rw-r--r--   0 sverma     (501) staff       (20)      669 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/BrowseCondition/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/BrowseCondition/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/BrowseIntervention/
+-rw-r--r--   0 sverma     (501) staff       (20)      678 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/BrowseIntervention/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/BrowseIntervention/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/StudyReference/
+-rw-r--r--   0 sverma     (501) staff       (20)      713 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/StudyReference/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/StudyReference/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Condition/
+-rw-r--r--   0 sverma     (501) staff       (20)      630 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Condition/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Condition/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Link/
+-rw-r--r--   0 sverma     (501) staff       (20)      636 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Link/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Link/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/BriefSummary/
+-rw-r--r--   0 sverma     (501) staff       (20)      597 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/BriefSummary/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/BriefSummary/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Sponsor/
+-rw-r--r--   0 sverma     (501) staff       (20)      872 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Sponsor/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Sponsor/__init__.py
+-rw-r--r--   0 sverma     (501) staff       (20)      514 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Sponsor/schemas.py
+-rw-r--r--   0 sverma     (501) staff       (20)     1561 2019-11-25 03:10:56.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/something.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/MeshTerm/
+-rw-r--r--   0 sverma     (501) staff       (20)      773 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/MeshTerm/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/MeshTerm/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Keyword/
+-rw-r--r--   0 sverma     (501) staff       (20)      645 2020-04-07 02:12:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Keyword/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2020-04-07 02:12:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/Keyword/__init__.py
+drwxr-xr-x   0 sverma     (501) staff       (20)        0 2020-05-20 22:01:23.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/MeshHeading/
+-rw-r--r--   0 sverma     (501) staff       (20)      592 2019-11-10 20:18:50.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/MeshHeading/models.py
+-rw-r--r--   0 sverma     (501) staff       (20)        0 2019-11-10 20:04:33.000000 cs-models-0.0.99.dev4/src/cs_models/resources_aact/MeshHeading/__init__.py
```

### Comparing `cs-models-0.0.99.dev3/setup.py` & `cs-models-0.0.99.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "pymongo==3.8.0",
     "psycopg2-binary==2.8.4",
 ]
 
 if __name__ == "__main__":
     setuptools.setup(
         name="cs-models",
-        version="0.0.99-dev3",
+        version="0.0.99-dev4",
         author="Harsh Verma",
         author_email="harsh@capitolscience.com",
         description="MySQL db models",
         # long_description=long_description,
         # long_description_content_type='text/markdown',
         url="https://github.com/ezpz76/cs-models",
         packages=setuptools.find_packages(where="src"),
```

### Comparing `cs-models-0.0.99.dev3/src/cs_models.egg-info/SOURCES.txt` & `cs-models-0.0.99.dev4/src/cs_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_mongo/DocumentTree/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_mongo/DocumentTree/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/database/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/database/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CompanySEC/test_company_sec.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CompanySEC/test_company_sec.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CompanySEC/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CompanySEC/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CompanySEC/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CompanySEC/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PriorArtRefRelation/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PriorArtRefRelation/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PriorArtRefRelation/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PriorArtRefRelation/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PriorArtRefRelation/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PriorArtRefRelation/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PriorArtRefRelation/test_prior_art_ref_relation.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PriorArtRefRelation/test_prior_art_ref_relation.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Document/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Document/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Document/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Document/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Document/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Document/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Document/test_ptab2_document.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Document/test_ptab2_document.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/RelatedMatter/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/RelatedMatter/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/RelatedMatter/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/RelatedMatter/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/RelatedMatter/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/RelatedMatter/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/RelatedMatter/test_related_matter.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/RelatedMatter/test_related_matter.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/all_models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/all_models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/DocumentReference/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/DocumentReference/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/DocumentReference/test_document_reference.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/DocumentReference/test_document_reference.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/DocumentReference/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/DocumentReference/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/DocumentReference/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/DocumentReference/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/File/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/File/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/File/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/File/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/File/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/File/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/File/test_file.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/File/test_file.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/InstitutionProbability/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/InstitutionProbability/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/InstitutionProbability/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/InstitutionProbability/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/InstitutionProbability/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/InstitutionProbability/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/InstitutionProbability/test_institution_probability.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/InstitutionProbability/test_institution_probability.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PriorArt/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PriorArt/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PriorArt/test_prior_art.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PriorArt/test_prior_art.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PriorArt/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PriorArt/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PriorArt/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PriorArt/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/NDC/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/NDC/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/NDC/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/NDC/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/NDC/test_ndc.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/NDC/test_ndc.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/NDC/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/NDC/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookPatent/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookPatent/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookPatent/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookPatent/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookPatent/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookPatent/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookPatent/test_orange_book_patent.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookPatent/test_orange_book_patent.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PacerCase/test_pacer_case.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PacerCase/test_pacer_case.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PacerCase/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PacerCase/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PacerCase/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PacerCase/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PacerCase/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PacerCase/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/ClaimChallenged/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/ClaimChallenged/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/ClaimChallenged/test_claim_challenged.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/ClaimChallenged/test_claim_challenged.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/ClaimChallenged/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/ClaimChallenged/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/ClaimChallenged/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/ClaimChallenged/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Pharmacologic/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Pharmacologic/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Pharmacologic/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Pharmacologic/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Pharmacologic/test_pharmacologic.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Pharmacologic/test_pharmacologic.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Pharmacologic/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Pharmacologic/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Patent/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Patent/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Patent/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Patent/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Patent/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Patent/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Patent/test_patent.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Patent/test_patent.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Newswire/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Newswire/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Newswire/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Newswire/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Newswire/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Newswire/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Newswire/test_newswire.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Newswire/test_newswire.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CrossRef/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CrossRef/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CrossRef/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CrossRef/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CrossRef/test_crossref.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CrossRef/test_crossref.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CrossRef/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CrossRef/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Proceeding/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Proceeding/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Proceeding/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Proceeding/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Proceeding/test_ptabv2_proceeding.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Proceeding/test_ptabv2_proceeding.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Proceeding/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Proceeding/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/SubsidiarySponsorMapping/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/SubsidiarySponsorMapping/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/SubsidiarySponsorMapping/test_subsidiary_sponsor_mapping.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/SubsidiarySponsorMapping/test_subsidiary_sponsor_mapping.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/SubsidiarySponsorMapping/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/SubsidiarySponsorMapping/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/SubsidiarySponsorMapping/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/SubsidiarySponsorMapping/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CompanyOUS/test_company_ous.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CompanyOUS/test_company_ous.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CompanyOUS/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CompanyOUS/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CompanyOUS/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CompanyOUS/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/CompanyOUS/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/CompanyOUS/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/SetIDPharmacologicCross/test_set_id_pharmacologic_cross.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/SetIDPharmacologicCross/test_set_id_pharmacologic_cross.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/SetIDPharmacologicCross/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/SetIDPharmacologicCross/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/SetIDPharmacologicCross/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/SetIDPharmacologicCross/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/FederalCaseRef/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/FederalCaseRef/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/FederalCaseRef/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/FederalCaseRef/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/FederalCaseRef/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/FederalCaseRef/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/FederalCaseRef/test_federal_case_ref.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/FederalCaseRef/test_federal_case_ref.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/TrialStat/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/TrialStat/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/TrialStat/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/TrialStat/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/TrialStat/test_trial_stat.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/TrialStat/test_trial_stat.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/TrialStat/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/TrialStat/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentIdentifierSynonym/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentIdentifierSynonym/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentIdentifierSynonym/test_patent_identifier_synonym.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentIdentifierSynonym/test_patent_identifier_synonym.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentIdentifierSynonym/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentIdentifierSynonym/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentIdentifierSynonym/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentIdentifierSynonym/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/UserSearchHistoryItem/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/UserSearchHistoryItem/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/UserSearchHistoryItem/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/UserSearchHistoryItem/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/UserSearchHistoryItem/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/UserSearchHistoryItem/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/UserSearchHistoryItem/test_user_search_history_item.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/UserSearchHistoryItem/test_user_search_history_item.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/AbstractText/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/AbstractText/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/AbstractText/test_abstract_text.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/AbstractText/test_abstract_text.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Decision/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Decision/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Decision/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Decision/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Decision/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Decision/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PTAB2Decision/test_ptabv2_decision.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PTAB2Decision/test_ptabv2_decision.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/NDCSetIDCross/test_ndc_setid_cross.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/NDCSetIDCross/test_ndc_setid_cross.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/NDCSetIDCross/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/NDCSetIDCross/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/NDCSetIDCross/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/NDCSetIDCross/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentApplication/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentApplication/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentApplication/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentApplication/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentApplication/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentApplication/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentApplication/test_patent_application.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentApplication/test_patent_application.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/DrugIndication/test_indication.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/DrugIndication/test_indication.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/DrugIndication/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/DrugIndication/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/DrugIndication/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/DrugIndication/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/DrugIndication/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/DrugIndication/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/ProceedingStage/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/ProceedingStage/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/ProceedingStage/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/ProceedingStage/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/ProceedingStage/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/ProceedingStage/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/ProceedingStage/test_proceeding_stage.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/ProceedingStage/test_proceeding_stage.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Subsidiary/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Subsidiary/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Subsidiary/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Subsidiary/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Subsidiary/test_subsidiary.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Subsidiary/test_subsidiary.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Subsidiary/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Subsidiary/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookExclusivity/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookExclusivity/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookExclusivity/test_orange_book_exclusivity.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookExclusivity/test_orange_book_exclusivity.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookExclusivity/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookExclusivity/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookExclusivity/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookExclusivity/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/ClaimDependency/test_claim_dependency.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/ClaimDependency/test_claim_dependency.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/ClaimDependency/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/ClaimDependency/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Claim/test_claim.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Claim/test_claim.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Claim/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Claim/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Claim/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Claim/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Claim/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Claim/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Company/test_company.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Company/test_company.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Company/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Company/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Company/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Company/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/Company/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/Company/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookProduct/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookProduct/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookProduct/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookProduct/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookProduct/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookProduct/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/OrangeBookProduct/test_orange_book_product.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/OrangeBookProduct/test_orange_book_product.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentCompound/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentCompound/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentCompound/test_patent_compound.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentCompound/test_patent_compound.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentCompound/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentCompound/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources/PatentCompound/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources/PatentCompound/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/utils/alchemy.py` & `cs-models-0.0.99.dev4/src/cs_models/utils/alchemy.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/utils/utils.py` & `cs-models-0.0.99.dev4/src/cs_models/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/utils/profiling/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/utils/profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/aact_database/__init__.py` & `cs-models-0.0.99.dev4/src/cs_models/aact_database/__init__.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/Intervention/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/Intervention/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/Study/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/Study/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/InterventionOtherNames/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/InterventionOtherNames/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/DetailedDescription/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/DetailedDescription/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/BrowseCondition/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/BrowseCondition/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/BrowseIntervention/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/BrowseIntervention/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/StudyReference/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/StudyReference/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/Condition/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/Condition/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/Link/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/Link/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/BriefSummary/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/BriefSummary/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/Sponsor/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/Sponsor/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/Sponsor/schemas.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/Sponsor/schemas.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/something.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/something.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/MeshTerm/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/MeshTerm/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/Keyword/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/Keyword/models.py`

 * *Files identical despite different names*

### Comparing `cs-models-0.0.99.dev3/src/cs_models/resources_aact/MeshHeading/models.py` & `cs-models-0.0.99.dev4/src/cs_models/resources_aact/MeshHeading/models.py`

 * *Files identical despite different names*

