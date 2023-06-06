# Comparing `tmp/lexikos-0.0.1rc2.tar.gz` & `tmp/lexikos-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikos-0.0.1rc2.tar", last modified: Mon May 22 09:51:57 2023, max compression
+gzip compressed data, was "lexikos-0.0.1rc3.tar", last modified: Tue Jun  6 02:46:30 2023, max compression
```

## Comparing `lexikos-0.0.1rc2.tar` & `lexikos-0.0.1rc3.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.430474 lexikos-0.0.1rc2/
--rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc2/LICENSE
--rw-r--r--   0 mac        (502) staff       (20)       16 2023-04-21 13:04:42.000000 lexikos-0.0.1rc2/MANIFEST.in
--rw-r--r--   0 mac        (502) staff       (20)    27905 2023-05-22 09:51:57.430731 lexikos-0.0.1rc2/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)    14181 2023-05-22 09:48:54.000000 lexikos-0.0.1rc2/README.md
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.365913 lexikos-0.0.1rc2/lexikos/
--rw-r--r--   0 mac        (502) staff       (20)       77 2023-05-22 09:37:26.000000 lexikos-0.0.1rc2/lexikos/__init__.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.363481 lexikos-0.0.1rc2/lexikos/dict/
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.375674 lexikos-0.0.1rc2/lexikos/dict/cmudict-ipa/
--rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc2/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
--rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc2/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.390810 lexikos-0.0.1rc2/lexikos/dict/synthetic/
--rw-r--r--   0 mac        (502) staff       (20)      406 2023-05-19 10:04:44.000000 lexikos-0.0.1rc2/lexikos/dict/synthetic/austalk_en_au.tsv
--rw-r--r--   0 mac        (502) staff       (20)     2618 2023-05-19 10:05:54.000000 lexikos-0.0.1rc2/lexikos/dict/synthetic/sc_cw_en_au.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.429491 lexikos-0.0.1rc2/lexikos/dict/wikipron/
--rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_au_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_in_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_us_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)     2911 2023-05-09 09:56:54.000000 lexikos-0.0.1rc2/lexikos/lexicon.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-05-22 09:51:57.367453 lexikos-0.0.1rc2/lexikos.egg-info/
--rw-r--r--   0 mac        (502) staff       (20)    27905 2023-05-22 09:51:57.000000 lexikos-0.0.1rc2/lexikos.egg-info/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)     1003 2023-05-22 09:51:57.000000 lexikos-0.0.1rc2/lexikos.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (502) staff       (20)        1 2023-05-22 09:51:57.000000 lexikos-0.0.1rc2/lexikos.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (502) staff       (20)        8 2023-05-22 09:51:57.000000 lexikos-0.0.1rc2/lexikos.egg-info/top_level.txt
--rw-r--r--   0 mac        (502) staff       (20)      821 2023-05-22 09:37:31.000000 lexikos-0.0.1rc2/pyproject.toml
--rw-r--r--   0 mac        (502) staff       (20)      113 2023-05-22 09:51:57.431175 lexikos-0.0.1rc2/setup.cfg
--rw-r--r--   0 mac        (502) staff       (20)      964 2023-04-21 13:31:07.000000 lexikos-0.0.1rc2/setup.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.744902 lexikos-0.0.1rc3/
+-rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc3/LICENSE
+-rw-r--r--   0 mac        (502) staff       (20)       16 2023-04-21 13:04:42.000000 lexikos-0.0.1rc3/MANIFEST.in
+-rw-r--r--   0 mac        (502) staff       (20)    29266 2023-06-06 02:46:30.745171 lexikos-0.0.1rc3/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)    15542 2023-06-05 11:09:13.000000 lexikos-0.0.1rc3/README.md
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.672441 lexikos-0.0.1rc3/lexikos/
+-rw-r--r--   0 mac        (502) staff       (20)      105 2023-06-05 09:31:30.000000 lexikos-0.0.1rc3/lexikos/__init__.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.667372 lexikos-0.0.1rc3/lexikos/dict/
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.681853 lexikos-0.0.1rc3/lexikos/dict/cmudict-ipa/
+-rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc3/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc3/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.694037 lexikos-0.0.1rc3/lexikos/dict/synthetic/
+-rw-r--r--   0 mac        (502) staff       (20)      406 2023-05-19 10:04:44.000000 lexikos-0.0.1rc3/lexikos/dict/synthetic/austalk_en_au.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     2618 2023-05-19 10:05:54.000000 lexikos-0.0.1rc3/lexikos/dict/synthetic/sc_cw_en_au.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.743727 lexikos-0.0.1rc3/lexikos/dict/wikipron/
+-rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_au_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_in_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_us_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     5360 2023-06-06 02:44:11.000000 lexikos-0.0.1rc3/lexikos/g2p.py
+-rw-r--r--   0 mac        (502) staff       (20)     2911 2023-05-09 09:56:54.000000 lexikos-0.0.1rc3/lexikos/lexicon.py
+-rw-r--r--   0 mac        (502) staff       (20)     3360 2023-06-05 09:31:30.000000 lexikos-0.0.1rc3/lexikos/normalizer.py
+-rw-r--r--   0 mac        (502) staff       (20)     1354 2023-06-06 02:44:11.000000 lexikos-0.0.1rc3/lexikos/t5.py
+-rw-r--r--   0 mac        (502) staff       (20)      722 2023-06-06 02:44:11.000000 lexikos-0.0.1rc3/lexikos/utils.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.673702 lexikos-0.0.1rc3/lexikos.egg-info/
+-rw-r--r--   0 mac        (502) staff       (20)    29266 2023-06-06 02:46:30.000000 lexikos-0.0.1rc3/lexikos.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)     1071 2023-06-06 02:46:30.000000 lexikos-0.0.1rc3/lexikos.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (502) staff       (20)        1 2023-06-06 02:46:30.000000 lexikos-0.0.1rc3/lexikos.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (502) staff       (20)        8 2023-06-06 02:46:30.000000 lexikos-0.0.1rc3/lexikos.egg-info/top_level.txt
+-rw-r--r--   0 mac        (502) staff       (20)      821 2023-06-05 09:31:30.000000 lexikos-0.0.1rc3/pyproject.toml
+-rw-r--r--   0 mac        (502) staff       (20)      113 2023-06-06 02:46:30.745820 lexikos-0.0.1rc3/setup.cfg
+-rw-r--r--   0 mac        (502) staff       (20)      964 2023-04-21 13:31:07.000000 lexikos-0.0.1rc3/setup.py
```

### Comparing `lexikos-0.0.1rc2/LICENSE` & `lexikos-0.0.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/PKG-INFO` & `lexikos-0.0.1rc3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -267,24 +267,21 @@
 >>> print(lexicon["water"])
 {'w o ɾ ə', 'w ɔ t ə', 'ʋ ɔ ʈ ə r', 'w a ʈ ə r ɯ', 'w ɔ t ə ɹ', 'ʋ a ʈ ə r ɯ', 'w ɑ ɾ ɚ', 'w o t ə', 'w ɔ t ɝ', 'w ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ'}
 ```
 
 ### Phonemization
 
 ```py
->>> from transformers import pipeline
->>> import torch
->>> g2p = pipeline(
-...     model="bookbot/byt5-small-wikipron-eng-latn-us-broad",
-...     device=0 if torch.cuda.is_available() else -1,
-... )
->>> g2p("phonemizing", max_length=200)[0]['generated_text']
-'f o ʊ n ə m a ɪ z ɪ ŋ'
->>> g2p("imposimpable", max_length=200)[0]['generated_text']
-'ɪ m p ə z ɪ m p ə b ə l'
+>>> from lexikos import G2p
+>>> g2p = G2p(lang="en-us")
+>>> g2p("Hello there! $100 is not a lot of money in 2023.")
+['h ɛ l o ʊ', 'ð ɛ ə ɹ', 'w ʌ n', 'h ʌ n d ɹ ɪ d', 'd ɑ l ɚ z', 'ɪ z', 'n ɒ t', 'ə', 'l ɑ t', 'ʌ v', 'm ʌ n i', 'ɪ n', 't w ɛ n t i', 't w ɛ n t i', 'θ ɹ iː']
+>>> g2p = G2p(lang="en-au")
+>>> g2p("Hi there mate! Have a g'day!")
+['h a ɪ', 'θ ɛ ə ɹ', 'm e ɪ t', 'h e ɪ v', 'ə', 'ɡ ə ˈd æ ɪ']
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
 | Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
@@ -317,32 +314,32 @@
 | en-AU (Broad)  | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
 | en-AU (Narrow) | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
 | en-AU          | AusTalk (§) | IPA       | [Link](./lexikos/dict/synthetic/austalk_en_au.tsv)     |                                                                                                                       |
 | en-AU          | SC-CW (§)   | IPA       | [Link](./lexikos/dict/synthetic/sc_cw_en_au.tsv)       |                                                                                                                       |
 
 ### English `(en-CA)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
-| en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  |           |
-| en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |           |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-ca-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-ca-broad) |
+| en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-NZ)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
-| en-NZ (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_broad.tsv)  |           |
-| en-NZ (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_narrow.tsv) |           |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-NZ (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-nz-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-nz-broad) |
+| en-NZ (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-IN)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
-| en-IN (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_broad.tsv)  |           |
-| en-IN (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_narrow.tsv) |           |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-IN (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-in-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-in-broad) |
+| en-IN (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_narrow.tsv) |                                                                                                                       |
 
 
 ## Training G2P Model
 
 We modified the sequence-to-sequence training script of [🤗 HuggingFace](https://github.com/huggingface/transformers/blob/main/examples/pytorch/translation/run_translation.py) for the purpose of training G2P models. Refer to their [installation requirements](https://github.com/huggingface/transformers/tree/main/examples/pytorch/translation) for more details.
 
 Training a new G2P model generally follow this recipe:
@@ -438,19 +435,19 @@
 | Language Family        | Code                              | Region                                                | Corpus | G2P Model |
 | ---------------------- | --------------------------------- | ----------------------------------------------------- | :----: | :-------: |
 | African English        | en-ZA                             | South Africa                                          |        |           |
 | Australian English     | en-AU                             | Australia                                             |   ✅    |     ✅     |
 | East Asian English     | en-CN, en-HK, en-JP, en-KR, en-TW | China, Hong Kong, Japan, South Korea, Taiwan          |        |           |
 | European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |   🚧    |     🚧     |
 | Mexican English        | en-MX                             | Mexico                                                |        |           |
-| New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |           |
-| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |     🚧     |
+| New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |     ✅     |
+| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |     ✅     |
 | Middle Eastern English | en-EG, en-IL                      | Egypt, Israel                                         |        |           |
 | Southeast Asian        | en-TH, en-ID, en-MY, en-PH, en-SG | Thailand, Indonesia, Malaysia, Philippines, Singapore |        |           |
-| South Asian English    | en-IN                             | India                                                 |   ✅    |           |
+| South Asian English    | en-IN                             | India                                                 |   ✅    |     ✅     |
   
 ## Resources
 
 - [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P)
 - [Microsoft CNTK](https://github.com/microsoft/CNTK/tree/master)
 - [CMU Pronouncing Dictionary - IPA](https://github.com/menelik3/cmudict-ipa)
 - [Wikipron](https://github.com/CUNY-CL/wikipron/tree/master)
```

### Comparing `lexikos-0.0.1rc2/README.md` & `lexikos-0.0.1rc3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -48,24 +48,21 @@
 >>> print(lexicon["water"])
 {'w o ɾ ə', 'w ɔ t ə', 'ʋ ɔ ʈ ə r', 'w a ʈ ə r ɯ', 'w ɔ t ə ɹ', 'ʋ a ʈ ə r ɯ', 'w ɑ ɾ ɚ', 'w o t ə', 'w ɔ t ɝ', 'w ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ'}
 ```
 
 ### Phonemization
 
 ```py
->>> from transformers import pipeline
->>> import torch
->>> g2p = pipeline(
-...     model="bookbot/byt5-small-wikipron-eng-latn-us-broad",
-...     device=0 if torch.cuda.is_available() else -1,
-... )
->>> g2p("phonemizing", max_length=200)[0]['generated_text']
-'f o ʊ n ə m a ɪ z ɪ ŋ'
->>> g2p("imposimpable", max_length=200)[0]['generated_text']
-'ɪ m p ə z ɪ m p ə b ə l'
+>>> from lexikos import G2p
+>>> g2p = G2p(lang="en-us")
+>>> g2p("Hello there! $100 is not a lot of money in 2023.")
+['h ɛ l o ʊ', 'ð ɛ ə ɹ', 'w ʌ n', 'h ʌ n d ɹ ɪ d', 'd ɑ l ɚ z', 'ɪ z', 'n ɒ t', 'ə', 'l ɑ t', 'ʌ v', 'm ʌ n i', 'ɪ n', 't w ɛ n t i', 't w ɛ n t i', 'θ ɹ iː']
+>>> g2p = G2p(lang="en-au")
+>>> g2p("Hi there mate! Have a g'day!")
+['h a ɪ', 'θ ɛ ə ɹ', 'm e ɪ t', 'h e ɪ v', 'ə', 'ɡ ə ˈd æ ɪ']
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
 | Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
@@ -98,32 +95,32 @@
 | en-AU (Broad)  | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
 | en-AU (Narrow) | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
 | en-AU          | AusTalk (§) | IPA       | [Link](./lexikos/dict/synthetic/austalk_en_au.tsv)     |                                                                                                                       |
 | en-AU          | SC-CW (§)   | IPA       | [Link](./lexikos/dict/synthetic/sc_cw_en_au.tsv)       |                                                                                                                       |
 
 ### English `(en-CA)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
-| en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  |           |
-| en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |           |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-ca-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-ca-broad) |
+| en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-NZ)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
-| en-NZ (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_broad.tsv)  |           |
-| en-NZ (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_narrow.tsv) |           |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-NZ (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-nz-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-nz-broad) |
+| en-NZ (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-IN)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
-| en-IN (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_broad.tsv)  |           |
-| en-IN (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_narrow.tsv) |           |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-IN (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-in-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-in-broad) |
+| en-IN (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_narrow.tsv) |                                                                                                                       |
 
 
 ## Training G2P Model
 
 We modified the sequence-to-sequence training script of [🤗 HuggingFace](https://github.com/huggingface/transformers/blob/main/examples/pytorch/translation/run_translation.py) for the purpose of training G2P models. Refer to their [installation requirements](https://github.com/huggingface/transformers/tree/main/examples/pytorch/translation) for more details.
 
 Training a new G2P model generally follow this recipe:
@@ -219,19 +216,19 @@
 | Language Family        | Code                              | Region                                                | Corpus | G2P Model |
 | ---------------------- | --------------------------------- | ----------------------------------------------------- | :----: | :-------: |
 | African English        | en-ZA                             | South Africa                                          |        |           |
 | Australian English     | en-AU                             | Australia                                             |   ✅    |     ✅     |
 | East Asian English     | en-CN, en-HK, en-JP, en-KR, en-TW | China, Hong Kong, Japan, South Korea, Taiwan          |        |           |
 | European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |   🚧    |     🚧     |
 | Mexican English        | en-MX                             | Mexico                                                |        |           |
-| New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |           |
-| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |     🚧     |
+| New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |     ✅     |
+| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |     ✅     |
 | Middle Eastern English | en-EG, en-IL                      | Egypt, Israel                                         |        |           |
 | Southeast Asian        | en-TH, en-ID, en-MY, en-PH, en-SG | Thailand, Indonesia, Malaysia, Philippines, Singapore |        |           |
-| South Asian English    | en-IN                             | India                                                 |   ✅    |           |
+| South Asian English    | en-IN                             | India                                                 |   ✅    |     ✅     |
   
 ## Resources
 
 - [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P)
 - [Microsoft CNTK](https://github.com/microsoft/CNTK/tree/master)
 - [CMU Pronouncing Dictionary - IPA](https://github.com/menelik3/cmudict-ipa)
 - [Wikipron](https://github.com/CUNY-CL/wikipron/tree/master)
```

### Comparing `lexikos-0.0.1rc2/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv` & `lexikos-0.0.1rc3/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv` & `lexikos-0.0.1rc3/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/synthetic/sc_cw_en_au.tsv` & `lexikos-0.0.1rc3/lexikos/dict/synthetic/sc_cw_en_au.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_au_broad.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_au_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_au_narrow.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_au_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_ca_broad.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_ca_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_in_broad.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_in_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_in_narrow.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_in_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_nz_broad.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_nz_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_uk_broad.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_uk_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_us_broad.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_us_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/dict/wikipron/eng_latn_us_narrow.tsv` & `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_us_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos/lexicon.py` & `lexikos-0.0.1rc3/lexikos/lexicon.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc2/lexikos.egg-info/PKG-INFO` & `lexikos-0.0.1rc3/lexikos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -267,24 +267,21 @@
 >>> print(lexicon["water"])
 {'w o ɾ ə', 'w ɔ t ə', 'ʋ ɔ ʈ ə r', 'w a ʈ ə r ɯ', 'w ɔ t ə ɹ', 'ʋ a ʈ ə r ɯ', 'w ɑ ɾ ɚ', 'w o t ə', 'w ɔ t ɝ', 'w ɔ ʈ ə r', 'w ɔ ɾ ɚ', 'w ɑ t ə ɹ'}
 ```
 
 ### Phonemization
 
 ```py
->>> from transformers import pipeline
->>> import torch
->>> g2p = pipeline(
-...     model="bookbot/byt5-small-wikipron-eng-latn-us-broad",
-...     device=0 if torch.cuda.is_available() else -1,
-... )
->>> g2p("phonemizing", max_length=200)[0]['generated_text']
-'f o ʊ n ə m a ɪ z ɪ ŋ'
->>> g2p("imposimpable", max_length=200)[0]['generated_text']
-'ɪ m p ə z ɪ m p ə b ə l'
+>>> from lexikos import G2p
+>>> g2p = G2p(lang="en-us")
+>>> g2p("Hello there! $100 is not a lot of money in 2023.")
+['h ɛ l o ʊ', 'ð ɛ ə ɹ', 'w ʌ n', 'h ʌ n d ɹ ɪ d', 'd ɑ l ɚ z', 'ɪ z', 'n ɒ t', 'ə', 'l ɑ t', 'ʌ v', 'm ʌ n i', 'ɪ n', 't w ɛ n t i', 't w ɛ n t i', 'θ ɹ iː']
+>>> g2p = G2p(lang="en-au")
+>>> g2p("Hi there mate! Have a g'day!")
+['h a ɪ', 'θ ɛ ə ɹ', 'm e ɪ t', 'h e ɪ v', 'ə', 'ɡ ə ˈd æ ɪ']
 ```
 
 ## Dictionaries & Models
 
 ### English `(en)`
 
 | Language | Dictionary | Phone Set | Corpus                                       | G2P Model |
@@ -317,32 +314,32 @@
 | en-AU (Broad)  | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-au-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-au-broad) |
 | en-AU (Narrow) | Wikipron    | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_au_narrow.tsv) |                                                                                                                       |
 | en-AU          | AusTalk (§) | IPA       | [Link](./lexikos/dict/synthetic/austalk_en_au.tsv)     |                                                                                                                       |
 | en-AU          | SC-CW (§)   | IPA       | [Link](./lexikos/dict/synthetic/sc_cw_en_au.tsv)       |                                                                                                                       |
 
 ### English `(en-CA)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
-| en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  |           |
-| en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |           |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-CA (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-ca-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-ca-broad) |
+| en-CA (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_ca_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-NZ)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
-| en-NZ (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_broad.tsv)  |           |
-| en-NZ (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_narrow.tsv) |           |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-NZ (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-nz-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-nz-broad) |
+| en-NZ (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_nz_narrow.tsv) |                                                                                                                       |
 
 ### English `(en-IN)`
 
-| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model |
-| -------------- | ---------- | --------- | ------------------------------------------------------ | --------- |
-| en-IN (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_broad.tsv)  |           |
-| en-IN (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_narrow.tsv) |           |
+| Language       | Dictionary | Phone Set | Corpus                                                 | G2P Model                                                                                                             |
+| -------------- | ---------- | --------- | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
+| en-IN (Broad)  | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_broad.tsv)  | [bookbot/byt5-small-wikipron-eng-latn-in-broad](https://huggingface.co/bookbot/byt5-small-wikipron-eng-latn-in-broad) |
+| en-IN (Narrow) | Wikipron   | IPA       | [Link](./lexikos/dict/wikipron/eng_latn_in_narrow.tsv) |                                                                                                                       |
 
 
 ## Training G2P Model
 
 We modified the sequence-to-sequence training script of [🤗 HuggingFace](https://github.com/huggingface/transformers/blob/main/examples/pytorch/translation/run_translation.py) for the purpose of training G2P models. Refer to their [installation requirements](https://github.com/huggingface/transformers/tree/main/examples/pytorch/translation) for more details.
 
 Training a new G2P model generally follow this recipe:
@@ -438,19 +435,19 @@
 | Language Family        | Code                              | Region                                                | Corpus | G2P Model |
 | ---------------------- | --------------------------------- | ----------------------------------------------------- | :----: | :-------: |
 | African English        | en-ZA                             | South Africa                                          |        |           |
 | Australian English     | en-AU                             | Australia                                             |   ✅    |     ✅     |
 | East Asian English     | en-CN, en-HK, en-JP, en-KR, en-TW | China, Hong Kong, Japan, South Korea, Taiwan          |        |           |
 | European English       | en-UK, en-HU, en-IE               | United Kingdom, Hungary, Ireland                      |   🚧    |     🚧     |
 | Mexican English        | en-MX                             | Mexico                                                |        |           |
-| New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |           |
-| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |     🚧     |
+| New Zealand English    | en-NZ                             | New Zealand                                           |   ✅    |     ✅     |
+| North American         | en-CA, en-US                      | Canada, United States                                 |   ✅    |     ✅     |
 | Middle Eastern English | en-EG, en-IL                      | Egypt, Israel                                         |        |           |
 | Southeast Asian        | en-TH, en-ID, en-MY, en-PH, en-SG | Thailand, Indonesia, Malaysia, Philippines, Singapore |        |           |
-| South Asian English    | en-IN                             | India                                                 |   ✅    |           |
+| South Asian English    | en-IN                             | India                                                 |   ✅    |     ✅     |
   
 ## Resources
 
 - [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P)
 - [Microsoft CNTK](https://github.com/microsoft/CNTK/tree/master)
 - [CMU Pronouncing Dictionary - IPA](https://github.com/menelik3/cmudict-ipa)
 - [Wikipron](https://github.com/CUNY-CL/wikipron/tree/master)
```

### Comparing `lexikos-0.0.1rc2/lexikos.egg-info/SOURCES.txt` & `lexikos-0.0.1rc3/lexikos.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 lexikos/__init__.py
+lexikos/g2p.py
 lexikos/lexicon.py
+lexikos/normalizer.py
+lexikos/t5.py
+lexikos/utils.py
 lexikos.egg-info/PKG-INFO
 lexikos.egg-info/SOURCES.txt
 lexikos.egg-info/dependency_links.txt
 lexikos.egg-info/top_level.txt
 lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
 lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
 lexikos/dict/synthetic/austalk_en_au.tsv
```

### Comparing `lexikos-0.0.1rc2/pyproject.toml` & `lexikos-0.0.1rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexikos"
-version = "0.0.1rc2"
+version = "0.0.1rc3"
 description = "A collection of pronunciation dictionaries and neural grapheme-to-phoneme models."
 readme = "README.md"
 authors = [{ name="w11wo", email="wilson@bookbotkids.com" }, { name="anantoj", email="gg.ananto@gmail.com" }, { name="DavidSamuell", email="davidsamuel.7878@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
```

### Comparing `lexikos-0.0.1rc2/setup.py` & `lexikos-0.0.1rc3/setup.py`

 * *Files identical despite different names*

