# Comparing `tmp/coreferee-1.4.0.tar.gz` & `tmp/coreferee-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coreferee-1.4.0.tar", last modified: Mon Jan 30 16:56:31 2023, max compression
+gzip compressed data, was "coreferee-1.4.1.tar", last modified: Tue Jun  6 08:36:48 2023, max compression
```

## Comparing `coreferee-1.4.0.tar` & `coreferee-1.4.1.tar`

### file list

```diff
@@ -1,147 +1,98 @@
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.483307 coreferee-1.4.0/
--rw-rw-r--   0 richard   (1001) richard   (1001)     1134 2023-01-30 16:45:50.000000 coreferee-1.4.0/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)       88 2023-01-30 11:37:52.000000 coreferee-1.4.0/MANIFEST.in
--rw-rw-r--   0 richard   (1001) richard   (1001)     2364 2023-01-30 16:56:31.483307 coreferee-1.4.0/PKG-INFO
--rw-rw-r--   0 richard   (1001) richard   (1001)    51348 2023-01-30 16:49:21.000000 coreferee-1.4.0/README.md
--rw-rw-r--   0 richard   (1001) richard   (1001)      875 2023-01-30 16:54:23.000000 coreferee-1.4.0/SHORTREADME.md
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.471306 coreferee-1.4.0/coreferee/
--rw-rw-r--   0 richard   (1001) richard   (1001)      225 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     4322 2023-01-30 16:45:50.000000 coreferee-1.4.0/coreferee/__main__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    20377 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/annotation.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    10525 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/data_model.py
--rw-rw-r--   0 richard   (1001) richard   (1001)      491 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/errors.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.475307 coreferee-1.4.0/coreferee/lang/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/__init__.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.475307 coreferee-1.4.0/coreferee/lang/common/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/common/__init__.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.475307 coreferee-1.4.0/coreferee/lang/common/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)      795 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/common/data/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/common/data/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    31749 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/common/data/female_names.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    30043 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/common/data/male_names.dat
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.475307 coreferee-1.4.0/coreferee/lang/de/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/de/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)      308 2023-01-30 16:45:50.000000 coreferee-1.4.0/coreferee/lang/de/config.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.475307 coreferee-1.4.0/coreferee/lang/de/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)      344 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/de/data/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/de/data/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)       34 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/de/data/avalent_verb_stems.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)      135 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/de/data/blacklisted_phrases.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       44 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/de/data/neuter_female_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       10 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/de/data/neuter_male_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       47 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/de/data/neuter_person_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       95 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/de/data/verbs_with_personal_subject.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    20611 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/de/language_specific_rules.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.475307 coreferee-1.4.0/coreferee/lang/en/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     1180 2023-01-30 16:45:50.000000 coreferee-1.4.0/coreferee/lang/en/config.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.475307 coreferee-1.4.0/coreferee/lang/en/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)     2292 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/data/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/data/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    23262 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/data/animal_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       29 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/data/avalent_verbs.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       60 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/data/blacklisted_phrases.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)     1429 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/data/exclusively_female_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)      877 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/data/exclusively_male_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    57421 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/data/exclusively_person_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    71725 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/data/person_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    17231 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/en/language_specific_rules.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/coreferee/lang/fr/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)      417 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/config.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/coreferee/lang/fr/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)      501 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/data/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/data/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    13953 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/data/animal_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)      229 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/data/avalent_verbs.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)     1897 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/data/blacklisted_nouns.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)      179 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/data/blacklisted_phrases.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)     1195 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/data/mixed_gender_person_roles.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    38731 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/data/person_roles.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)     4435 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/data/plural_toponyms.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)     1282 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/data/verbs_with_personal_subject.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    48660 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/fr/language_specific_rules.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/coreferee/lang/pl/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/pl/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)      277 2023-01-30 16:45:50.000000 coreferee-1.4.0/coreferee/lang/pl/config.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/coreferee/lang/pl/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)      290 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/pl/data/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/pl/data/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)       72 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/pl/data/blacklisted_phrases.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       95 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/lang/pl/data/verbs_with_personal_subject.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    27762 2023-01-30 13:25:17.000000 coreferee-1.4.0/coreferee/lang/pl/language_specific_rules.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     8423 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/manager.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    28223 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/rules.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    32633 2023-01-30 15:33:06.000000 coreferee-1.4.0/coreferee/tendencies.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     2661 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/test_utils.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/coreferee/training/
--rw-rw-r--   0 richard   (1001) richard   (1001)        0 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/training/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    27195 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/training/loaders.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    22937 2023-01-30 11:37:52.000000 coreferee-1.4.0/coreferee/training/train.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.475307 coreferee-1.4.0/coreferee.egg-info/
--rw-rw-r--   0 richard   (1001) richard   (1001)     2364 2023-01-30 16:56:31.000000 coreferee-1.4.0/coreferee.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1001) richard   (1001)     4364 2023-01-30 16:56:31.000000 coreferee-1.4.0/coreferee.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)        1 2023-01-30 16:56:31.000000 coreferee-1.4.0/coreferee.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)       64 2023-01-30 16:56:31.000000 coreferee-1.4.0/coreferee.egg-info/entry_points.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)       20 2023-01-30 16:56:31.000000 coreferee-1.4.0/coreferee.egg-info/requires.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)       10 2023-01-30 16:56:31.000000 coreferee-1.4.0/coreferee.egg-info/top_level.txt
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.471306 coreferee-1.4.0/models/
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/models/de/
--rw-rw-r--   0 richard   (1001) richard   (1001)      162 2023-01-30 11:37:52.000000 coreferee-1.4.0/models/de/setup.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/models/en/
--rw-rw-r--   0 richard   (1001) richard   (1001)      162 2023-01-30 11:37:53.000000 coreferee-1.4.0/models/en/setup.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/models/fr/
--rw-rw-r--   0 richard   (1001) richard   (1001)      162 2023-01-30 11:37:53.000000 coreferee-1.4.0/models/fr/setup.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/models/pl/
--rw-rw-r--   0 richard   (1001) richard   (1001)      162 2023-01-30 11:37:53.000000 coreferee-1.4.0/models/pl/setup.cfg
--rw-rw-r--   0 richard   (1001) richard   (1001)      100 2023-01-30 11:37:53.000000 coreferee-1.4.0/pyproject.toml
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.471306 coreferee-1.4.0/qcktest/
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.471306 coreferee-1.4.0/qcktest/coreferee/
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.471306 coreferee-1.4.0/qcktest/coreferee/lang/
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.471306 coreferee-1.4.0/qcktest/coreferee/lang/common/
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/qcktest/coreferee/lang/common/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)      795 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/common/data/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)    31749 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/common/data/female_names.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    30043 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/common/data/male_names.dat
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/qcktest/coreferee/lang/de/
--rw-rw-r--   0 richard   (1001) richard   (1001)      308 2023-01-30 15:45:50.000000 coreferee-1.4.0/qcktest/coreferee/lang/de/config.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.483307 coreferee-1.4.0/qcktest/coreferee/lang/de/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)      344 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/de/data/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)       34 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/de/data/avalent_verb_stems.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)      135 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/de/data/blacklisted_phrases.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       44 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/de/data/neuter_female_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       10 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/de/data/neuter_male_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       47 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/de/data/neuter_person_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       95 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/de/data/verbs_with_personal_subject.dat
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.483307 coreferee-1.4.0/qcktest/coreferee/lang/en/
--rw-rw-r--   0 richard   (1001) richard   (1001)     1180 2023-01-30 15:45:50.000000 coreferee-1.4.0/qcktest/coreferee/lang/en/config.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.483307 coreferee-1.4.0/qcktest/coreferee/lang/en/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)     2292 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/en/data/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)    23262 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/en/data/animal_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       29 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/en/data/avalent_verbs.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       60 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/en/data/blacklisted_phrases.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)     1429 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/en/data/exclusively_female_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)      877 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/en/data/exclusively_male_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    57421 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/en/data/exclusively_person_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    71725 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/en/data/person_words.dat
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.483307 coreferee-1.4.0/qcktest/coreferee/lang/fr/
--rw-rw-r--   0 richard   (1001) richard   (1001)      417 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/fr/config.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.483307 coreferee-1.4.0/qcktest/coreferee/lang/fr/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)      501 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/fr/data/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)    13953 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/fr/data/animal_words.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)      229 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/fr/data/avalent_verbs.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)     1897 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/fr/data/blacklisted_nouns.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)      179 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/fr/data/blacklisted_phrases.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)     1195 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/fr/data/mixed_gender_person_roles.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)    38731 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/fr/data/person_roles.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)     4435 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/fr/data/plural_toponyms.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)     1282 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/fr/data/verbs_with_personal_subject.dat
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.483307 coreferee-1.4.0/qcktest/coreferee/lang/pl/
--rw-rw-r--   0 richard   (1001) richard   (1001)      277 2023-01-30 15:45:50.000000 coreferee-1.4.0/qcktest/coreferee/lang/pl/config.cfg
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.483307 coreferee-1.4.0/qcktest/coreferee/lang/pl/data/
--rw-rw-r--   0 richard   (1001) richard   (1001)      290 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/pl/data/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)       72 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/pl/data/blacklisted_phrases.dat
--rw-rw-r--   0 richard   (1001) richard   (1001)       95 2023-01-30 10:37:52.000000 coreferee-1.4.0/qcktest/coreferee/lang/pl/data/verbs_with_personal_subject.dat
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-01-30 16:56:31.479307 coreferee-1.4.0/qcktest/coreferee-1.4.0.dist-info/
--rw-rw-r--   0 richard   (1001) richard   (1001)     1134 2023-01-30 15:49:44.000000 coreferee-1.4.0/qcktest/coreferee-1.4.0.dist-info/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)     1588 2023-01-30 16:56:31.483307 coreferee-1.4.0/setup.cfg
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.466167 coreferee-1.4.1/
+-rw-r--r--   0 richard    (501) staff       (20)     1134 2023-06-05 13:21:56.000000 coreferee-1.4.1/LICENSE
+-rw-r--r--   0 richard    (501) staff       (20)       88 2023-06-05 13:21:56.000000 coreferee-1.4.1/MANIFEST.in
+-rw-r--r--   0 richard    (501) staff       (20)     2415 2023-06-06 08:36:48.466267 coreferee-1.4.1/PKG-INFO
+-rw-r--r--   0 richard    (501) staff       (20)    51476 2023-06-05 13:25:28.000000 coreferee-1.4.1/README.md
+-rw-r--r--   0 richard    (501) staff       (20)      875 2023-06-05 13:24:15.000000 coreferee-1.4.1/SHORTREADME.md
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.456160 coreferee-1.4.1/coreferee/
+-rw-r--r--   0 richard    (501) staff       (20)      225 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)     4322 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/__main__.py
+-rw-r--r--   0 richard    (501) staff       (20)    20377 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/annotation.py
+-rw-r--r--   0 richard    (501) staff       (20)    10525 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/data_model.py
+-rw-r--r--   0 richard    (501) staff       (20)      491 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/errors.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.456930 coreferee-1.4.1/coreferee/lang/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/__init__.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.457016 coreferee-1.4.1/coreferee/lang/common/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/common/__init__.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.457494 coreferee-1.4.1/coreferee/lang/common/data/
+-rw-r--r--   0 richard    (501) staff       (20)      795 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/common/data/LICENSE
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/common/data/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)    31749 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/common/data/female_names.dat
+-rw-r--r--   0 richard    (501) staff       (20)    30043 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/common/data/male_names.dat
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.458073 coreferee-1.4.1/coreferee/lang/de/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)      308 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/config.cfg
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.459488 coreferee-1.4.1/coreferee/lang/de/data/
+-rw-r--r--   0 richard    (501) staff       (20)      344 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/data/LICENSE
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/data/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)       34 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/data/avalent_verb_stems.dat
+-rw-r--r--   0 richard    (501) staff       (20)      135 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/data/blacklisted_phrases.dat
+-rw-r--r--   0 richard    (501) staff       (20)       44 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/data/neuter_female_words.dat
+-rw-r--r--   0 richard    (501) staff       (20)       10 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/data/neuter_male_words.dat
+-rw-r--r--   0 richard    (501) staff       (20)       47 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/data/neuter_person_words.dat
+-rw-r--r--   0 richard    (501) staff       (20)       95 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/data/verbs_with_personal_subject.dat
+-rw-r--r--   0 richard    (501) staff       (20)    20611 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/de/language_specific_rules.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.459812 coreferee-1.4.1/coreferee/lang/en/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)     1180 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/config.cfg
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.461058 coreferee-1.4.1/coreferee/lang/en/data/
+-rw-r--r--   0 richard    (501) staff       (20)     2292 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/data/LICENSE
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/data/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)    23262 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/data/animal_words.dat
+-rw-r--r--   0 richard    (501) staff       (20)       29 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/data/avalent_verbs.dat
+-rw-r--r--   0 richard    (501) staff       (20)       60 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/data/blacklisted_phrases.dat
+-rw-r--r--   0 richard    (501) staff       (20)     1429 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/data/exclusively_female_words.dat
+-rw-r--r--   0 richard    (501) staff       (20)      877 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/data/exclusively_male_words.dat
+-rw-r--r--   0 richard    (501) staff       (20)    57421 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/data/exclusively_person_words.dat
+-rw-r--r--   0 richard    (501) staff       (20)    71725 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/data/person_words.dat
+-rw-r--r--   0 richard    (501) staff       (20)    17231 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/en/language_specific_rules.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.461488 coreferee-1.4.1/coreferee/lang/fr/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)      417 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/config.cfg
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.463573 coreferee-1.4.1/coreferee/lang/fr/data/
+-rw-r--r--   0 richard    (501) staff       (20)      501 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/data/LICENSE
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/data/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)    13953 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/data/animal_words.dat
+-rw-r--r--   0 richard    (501) staff       (20)      229 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/data/avalent_verbs.dat
+-rw-r--r--   0 richard    (501) staff       (20)     1897 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/data/blacklisted_nouns.dat
+-rw-r--r--   0 richard    (501) staff       (20)      179 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/data/blacklisted_phrases.dat
+-rw-r--r--   0 richard    (501) staff       (20)     1195 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/data/mixed_gender_person_roles.dat
+-rw-r--r--   0 richard    (501) staff       (20)    38731 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/data/person_roles.dat
+-rw-r--r--   0 richard    (501) staff       (20)     4435 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/data/plural_toponyms.dat
+-rw-r--r--   0 richard    (501) staff       (20)     1282 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/data/verbs_with_personal_subject.dat
+-rw-r--r--   0 richard    (501) staff       (20)    48660 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/fr/language_specific_rules.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.463941 coreferee-1.4.1/coreferee/lang/pl/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/pl/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)      277 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/pl/config.cfg
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.464468 coreferee-1.4.1/coreferee/lang/pl/data/
+-rw-r--r--   0 richard    (501) staff       (20)      290 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/pl/data/LICENSE
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/pl/data/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)       72 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/pl/data/blacklisted_phrases.dat
+-rw-r--r--   0 richard    (501) staff       (20)       95 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/pl/data/verbs_with_personal_subject.dat
+-rw-r--r--   0 richard    (501) staff       (20)    27762 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/lang/pl/language_specific_rules.py
+-rw-r--r--   0 richard    (501) staff       (20)     8423 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/manager.py
+-rw-r--r--   0 richard    (501) staff       (20)    28223 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/rules.py
+-rw-r--r--   0 richard    (501) staff       (20)    32633 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/tendencies.py
+-rw-r--r--   0 richard    (501) staff       (20)     2661 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/test_utils.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.464855 coreferee-1.4.1/coreferee/training/
+-rw-r--r--   0 richard    (501) staff       (20)        0 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/training/__init__.py
+-rw-r--r--   0 richard    (501) staff       (20)    27195 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/training/loaders.py
+-rw-r--r--   0 richard    (501) staff       (20)    22937 2023-06-05 13:21:56.000000 coreferee-1.4.1/coreferee/training/train.py
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.456825 coreferee-1.4.1/coreferee.egg-info/
+-rw-r--r--   0 richard    (501) staff       (20)     2415 2023-06-06 08:36:48.000000 coreferee-1.4.1/coreferee.egg-info/PKG-INFO
+-rw-r--r--   0 richard    (501) staff       (20)     2614 2023-06-06 08:36:48.000000 coreferee-1.4.1/coreferee.egg-info/SOURCES.txt
+-rw-r--r--   0 richard    (501) staff       (20)        1 2023-06-06 08:36:48.000000 coreferee-1.4.1/coreferee.egg-info/dependency_links.txt
+-rw-r--r--   0 richard    (501) staff       (20)       64 2023-06-06 08:36:48.000000 coreferee-1.4.1/coreferee.egg-info/entry_points.txt
+-rw-r--r--   0 richard    (501) staff       (20)       20 2023-06-06 08:36:48.000000 coreferee-1.4.1/coreferee.egg-info/requires.txt
+-rw-r--r--   0 richard    (501) staff       (20)       10 2023-06-06 08:36:48.000000 coreferee-1.4.1/coreferee.egg-info/top_level.txt
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.452518 coreferee-1.4.1/models/
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.465007 coreferee-1.4.1/models/de/
+-rw-r--r--   0 richard    (501) staff       (20)      162 2023-06-05 13:21:57.000000 coreferee-1.4.1/models/de/setup.cfg
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.465366 coreferee-1.4.1/models/en/
+-rw-r--r--   0 richard    (501) staff       (20)      162 2023-06-05 13:21:57.000000 coreferee-1.4.1/models/en/setup.cfg
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.465586 coreferee-1.4.1/models/fr/
+-rw-r--r--   0 richard    (501) staff       (20)      162 2023-06-05 13:21:57.000000 coreferee-1.4.1/models/fr/setup.cfg
+drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-06-06 08:36:48.465886 coreferee-1.4.1/models/pl/
+-rw-r--r--   0 richard    (501) staff       (20)      162 2023-06-05 13:21:57.000000 coreferee-1.4.1/models/pl/setup.cfg
+-rw-r--r--   0 richard    (501) staff       (20)      100 2023-06-05 13:21:57.000000 coreferee-1.4.1/pyproject.toml
+-rw-r--r--   0 richard    (501) staff       (20)     1628 2023-06-06 08:36:48.466669 coreferee-1.4.1/setup.cfg
```

### Comparing `coreferee-1.4.0/LICENSE` & `coreferee-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/PKG-INFO` & `coreferee-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coreferee
-Version: 1.4.0
+Version: 1.4.1
 Summary: Coreference resolution for English, French, German and Polish, optimised for limited training data and easily extensible for further languages
 Home-page: https://github.com/richardpaulhudson/coreferee
 Author: Richard Paul Hudson
 Author-email: hudsonrichardpaul@gmail.com
 License: MIT
 Keywords: nlp,spacy,spacy-extension,python,machine-learning,coreference,anaphora,coreference-resolution,anaphora-resolution
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,20 +20,21 @@
 Classifier: Natural Language :: Polish
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: <3.11,>=3.6
+Requires-Python: <3.12,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Coreferences are situations where two or more words within a text refer to the same entity, e.g. _**John** went home because **he** was tired_. Resolving coreferences is an important general task within the natural language processing field.
 
-Coreferee is a Python 3 library (tested with versions 3.6—3.10) that is used together with [spaCy](https://spacy.io/) (tested with versions 3.0.0—3.5.0) to resolve coreferences within English, French, German and Polish texts. It is designed so that it is easy to add support for new languages. It uses a mixture of neural networks and programmed rules.
+Coreferee is a Python 3 library (tested with versions 3.6—3.11) that is used together with [spaCy](https://spacy.io/) (tested with versions 3.0.0—3.5.0) to resolve coreferences within English, French, German and Polish texts. It is designed so that it is easy to add support for new languages. It uses a mixture of neural networks and programmed rules.
 
 The library was originally developed at [msg systems](https://www.msg.group/en) and was also maintained for a while at [Explosion AI](https://explosion.ai).
 
 For more information, please see the [main documentation on GitHub](https://github.com/richardpaulhudson/coreferee).
```

### Comparing `coreferee-1.4.0/README.md` & `coreferee-1.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,27 +29,28 @@
   - [6.4 Version 1.1.1](#version-111)
   - [6.5 Version 1.1.2](#version-112)
   - [6.6 Version 1.1.3](#version-113)
   - [6.7 Version 1.2.0](#version-120)
   - [6.8 Version 1.3.0](#version-130)
   - [6.9 Version 1.3.1](#version-131)
   - [6.10 Version 1.4.0](#version-140)
+  - [6.11 Version 1.4.1](#version-141)
 - [7. Open issues/requests for assistance](#open-issues)
 
 <a id="introduction"></a>
 
 ### 1. Introduction
 
 <a id="the-basic-idea"></a>
 
 #### 1.1 The basic idea
 
 Coreferences are situations where two or more words within a text refer to the same entity, e.g. _**John** went home because **he** was tired_. Resolving coreferences is an important general task within the natural language processing field.
 
-Coreferee is a Python 3 library (tested with versions 3.6—3.10) that is used together with [spaCy](https://spacy.io/) (tested with versions 3.0.0—3.5.0) to resolve coreferences within English, French, German and Polish texts. It is designed so that it is easy to add support for new languages. It uses a mixture of neural networks and programmed rules.
+Coreferee is a Python 3 library (tested with versions 3.6—3.11) that is used together with [spaCy](https://spacy.io/) (tested with versions 3.0.0—3.5.0) to resolve coreferences within English, French, German and Polish texts. It is designed so that it is easy to add support for new languages. It uses a mixture of neural networks and programmed rules.
 
 The library was originally developed at [msg systems](https://www.msg.group/en) and was also maintained for a while at [Explosion AI](https://explosion.ai).
 
 <a id="getting-started"></a>
 
 #### 1.2 Getting started
 
@@ -637,17 +638,23 @@
 - Added support for the v3.4.1 English models.
 
 <a id="version-140"></a>
 
 ##### 6.10 Version 1.4.0
 
 - Made it possible to package spaCy pipelines containing Coreferee.
-- Add an entry point for Coreferee so it does not need to be imported explicitly alongside spaCy.
+- Added an entry point for Coreferee so it does not need to be imported explicitly alongside spaCy.
 - Added support for spaCy v3.5 for English, German and Polish.
 
+<a id="version-141"></a>
+
+##### 6.11 Version 1.4.1
+
+- Added support for Python v3.11.
+
 <a id="open-issues"></a>
 
 ### 7. Open issues / requests for assistance
 
 1. Because optimising parsing speed was not a priority in the [project within which Coreferee came into being](#background-information), Coreferee is written purely in Python; it would be helpful if somebody could convert relevant parts of it to Cython.
 
 2. It would be useful if somebody could find a way of benchmarking Coreferee against other coreference resolution solutions, especially for English. One problem this would probably present is that using a benchmark necessitates a normative scope where a system aims to find exactly those types of coreference marked within the benchmark corpus, whereas the scope of Coreferee was determined by project requirements.
```

### Comparing `coreferee-1.4.0/SHORTREADME.md` & `coreferee-1.4.1/SHORTREADME.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Coreferences are situations where two or more words within a text refer to the same entity, e.g. _**John** went home because **he** was tired_. Resolving coreferences is an important general task within the natural language processing field.
 
-Coreferee is a Python 3 library (tested with versions 3.6—3.10) that is used together with [spaCy](https://spacy.io/) (tested with versions 3.0.0—3.5.0) to resolve coreferences within English, French, German and Polish texts. It is designed so that it is easy to add support for new languages. It uses a mixture of neural networks and programmed rules.
+Coreferee is a Python 3 library (tested with versions 3.6—3.11) that is used together with [spaCy](https://spacy.io/) (tested with versions 3.0.0—3.5.0) to resolve coreferences within English, French, German and Polish texts. It is designed so that it is easy to add support for new languages. It uses a mixture of neural networks and programmed rules.
 
 The library was originally developed at [msg systems](https://www.msg.group/en) and was also maintained for a while at [Explosion AI](https://explosion.ai).
 
 For more information, please see the [main documentation on GitHub](https://github.com/richardpaulhudson/coreferee).
```

### Comparing `coreferee-1.4.0/coreferee/__main__.py` & `coreferee-1.4.1/coreferee/__main__.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/annotation.py` & `coreferee-1.4.1/coreferee/annotation.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/data_model.py` & `coreferee-1.4.1/coreferee/data_model.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/common/data/LICENSE` & `coreferee-1.4.1/coreferee/lang/common/data/LICENSE`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/common/data/female_names.dat` & `coreferee-1.4.1/coreferee/lang/common/data/female_names.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/common/data/male_names.dat` & `coreferee-1.4.1/coreferee/lang/common/data/male_names.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/de/language_specific_rules.py` & `coreferee-1.4.1/coreferee/lang/de/language_specific_rules.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/en/config.cfg` & `coreferee-1.4.1/coreferee/lang/en/config.cfg`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/en/data/LICENSE` & `coreferee-1.4.1/coreferee/lang/en/data/LICENSE`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/en/data/animal_words.dat` & `coreferee-1.4.1/coreferee/lang/en/data/animal_words.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/en/data/exclusively_female_words.dat` & `coreferee-1.4.1/coreferee/lang/en/data/exclusively_female_words.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/en/data/exclusively_male_words.dat` & `coreferee-1.4.1/coreferee/lang/en/data/exclusively_male_words.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/en/data/exclusively_person_words.dat` & `coreferee-1.4.1/coreferee/lang/en/data/exclusively_person_words.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/en/data/person_words.dat` & `coreferee-1.4.1/coreferee/lang/en/data/person_words.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/en/language_specific_rules.py` & `coreferee-1.4.1/coreferee/lang/en/language_specific_rules.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/fr/data/animal_words.dat` & `coreferee-1.4.1/coreferee/lang/fr/data/animal_words.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/fr/data/blacklisted_nouns.dat` & `coreferee-1.4.1/coreferee/lang/fr/data/blacklisted_nouns.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/fr/data/mixed_gender_person_roles.dat` & `coreferee-1.4.1/coreferee/lang/fr/data/mixed_gender_person_roles.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/fr/data/person_roles.dat` & `coreferee-1.4.1/coreferee/lang/fr/data/person_roles.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/fr/data/plural_toponyms.dat` & `coreferee-1.4.1/coreferee/lang/fr/data/plural_toponyms.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/fr/data/verbs_with_personal_subject.dat` & `coreferee-1.4.1/coreferee/lang/fr/data/verbs_with_personal_subject.dat`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/fr/language_specific_rules.py` & `coreferee-1.4.1/coreferee/lang/fr/language_specific_rules.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/lang/pl/language_specific_rules.py` & `coreferee-1.4.1/coreferee/lang/pl/language_specific_rules.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/manager.py` & `coreferee-1.4.1/coreferee/manager.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/rules.py` & `coreferee-1.4.1/coreferee/rules.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/tendencies.py` & `coreferee-1.4.1/coreferee/tendencies.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/test_utils.py` & `coreferee-1.4.1/coreferee/test_utils.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/training/loaders.py` & `coreferee-1.4.1/coreferee/training/loaders.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee/training/train.py` & `coreferee-1.4.1/coreferee/training/train.py`

 * *Files identical despite different names*

### Comparing `coreferee-1.4.0/coreferee.egg-info/PKG-INFO` & `coreferee-1.4.1/coreferee.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coreferee
-Version: 1.4.0
+Version: 1.4.1
 Summary: Coreference resolution for English, French, German and Polish, optimised for limited training data and easily extensible for further languages
 Home-page: https://github.com/richardpaulhudson/coreferee
 Author: Richard Paul Hudson
 Author-email: hudsonrichardpaul@gmail.com
 License: MIT
 Keywords: nlp,spacy,spacy-extension,python,machine-learning,coreference,anaphora,coreference-resolution,anaphora-resolution
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,20 +20,21 @@
 Classifier: Natural Language :: Polish
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: <3.11,>=3.6
+Requires-Python: <3.12,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Coreferences are situations where two or more words within a text refer to the same entity, e.g. _**John** went home because **he** was tired_. Resolving coreferences is an important general task within the natural language processing field.
 
-Coreferee is a Python 3 library (tested with versions 3.6—3.10) that is used together with [spaCy](https://spacy.io/) (tested with versions 3.0.0—3.5.0) to resolve coreferences within English, French, German and Polish texts. It is designed so that it is easy to add support for new languages. It uses a mixture of neural networks and programmed rules.
+Coreferee is a Python 3 library (tested with versions 3.6—3.11) that is used together with [spaCy](https://spacy.io/) (tested with versions 3.0.0—3.5.0) to resolve coreferences within English, French, German and Polish texts. It is designed so that it is easy to add support for new languages. It uses a mixture of neural networks and programmed rules.
 
 The library was originally developed at [msg systems](https://www.msg.group/en) and was also maintained for a while at [Explosion AI](https://explosion.ai).
 
 For more information, please see the [main documentation on GitHub](https://github.com/richardpaulhudson/coreferee).
```

### Comparing `coreferee-1.4.0/setup.cfg` & `coreferee-1.4.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = coreferee
-version = 1.4.0
+version = 1.4.1
 description = Coreference resolution for English, French, German and Polish, optimised for limited training data and easily extensible for further languages
 long_description = file: SHORTREADME.md
 long_description_content_type = text/markdown
 url = https://github.com/richardpaulhudson/coreferee
 author = Richard Paul Hudson
 author_email = hudsonrichardpaul@gmail.com
 license = MIT
@@ -23,21 +23,22 @@
 	Natural Language :: Polish
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	Topic :: Text Processing :: Linguistic
 
 [options]
 include_package_data = True
 packages = find:
-python_requires = >=3.6,<3.11
+python_requires = >=3.6,<3.12
 install_requires = 
 	spacy>=3.0.0,<3.6.0
 
 [options.entry_points]
 spacy_factories = 
 	coreferee = coreferee.manager:CorefereeBroker
```

