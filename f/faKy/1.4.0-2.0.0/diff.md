# Comparing `tmp/faKy-1.4.0.tar.gz` & `tmp/faKy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faKy-1.4.0.tar", last modified: Tue Jun  6 13:22:33 2023, max compression
+gzip compressed data, was "faKy-2.0.0.tar", last modified: Tue Jun  6 14:06:52 2023, max compression
```

## Comparing `faKy-1.4.0.tar` & `faKy-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:22:33.438114 faKy-1.4.0/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4508 2023-06-06 13:22:33.437829 faKy-1.4.0/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4295 2023-06-06 12:37:50.000000 faKy-1.4.0/README.md
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:22:33.427464 faKy-1.4.0/faKy/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.4.0/faKy/__init__.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:22:33.435375 faKy-1.4.0/faKy/en_core_web_md-2.3.1/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       17 2023-06-06 11:41:49.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/MANIFEST.in
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      362 2023-06-06 11:41:49.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/PKG-INFO
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:22:33.436802 faKy-1.4.0/faKy/en_core_web_md-2.3.1/en_core_web_md/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      291 2023-06-06 11:41:49.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/en_core_web_md/__init__.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/meta.json
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:41:50.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1753 2023-06-06 11:41:50.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/setup.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8177 2023-06-06 13:21:51.000000 faKy-1.4.0/faKy/faKy.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:22:33.429649 faKy-1.4.0/faKy.egg-info/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4508 2023-06-06 13:22:33.000000 faKy-1.4.0/faKy.egg-info/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      471 2023-06-06 13:22:33.000000 faKy-1.4.0/faKy.egg-info/SOURCES.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 13:22:33.000000 faKy-1.4.0/faKy.egg-info/dependency_links.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      122 2023-06-06 13:22:33.000000 faKy-1.4.0/faKy.egg-info/requires.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 13:22:33.000000 faKy-1.4.0/faKy.egg-info/top_level.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 13:22:33.438224 faKy-1.4.0/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      813 2023-06-06 13:22:13.000000 faKy-1.4.0/setup.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:06:52.332484 faKy-2.0.0/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4486 2023-06-06 14:06:52.332142 faKy-2.0.0/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4273 2023-06-06 13:52:24.000000 faKy-2.0.0/README.md
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:06:52.324863 faKy-2.0.0/faKy/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-2.0.0/faKy/__init__.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:06:52.329909 faKy-2.0.0/faKy/en_core_web_md-2.3.1/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       17 2023-06-06 11:41:49.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/MANIFEST.in
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      362 2023-06-06 11:41:49.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/PKG-INFO
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:06:52.330993 faKy-2.0.0/faKy/en_core_web_md-2.3.1/en_core_web_md/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      291 2023-06-06 11:41:49.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/en_core_web_md/__init__.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:41:50.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1753 2023-06-06 11:41:50.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/setup.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8256 2023-06-06 14:05:57.000000 faKy-2.0.0/faKy/faKy.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:06:52.326760 faKy-2.0.0/faKy.egg-info/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4486 2023-06-06 14:06:52.000000 faKy-2.0.0/faKy.egg-info/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      471 2023-06-06 14:06:52.000000 faKy-2.0.0/faKy.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 14:06:52.000000 faKy-2.0.0/faKy.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      122 2023-06-06 14:06:52.000000 faKy-2.0.0/faKy.egg-info/requires.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 14:06:52.000000 faKy-2.0.0/faKy.egg-info/top_level.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 14:06:52.332648 faKy-2.0.0/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      759 2023-06-06 14:06:13.000000 faKy-2.0.0/setup.py
```

### Comparing `faKy-1.4.0/PKG-INFO` & `faKy-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,23 @@
-Metadata-Version: 2.1
-Name: faKy
-Version: 1.4.0
-Summary: Your library description
-Author: Sandro Barres Hamers
-Author-email: sbarreshamers@gmail.com
-Description-Content-Type: text/markdown
-Provides-Extra: vader
-
 # faKy
 We introduce faKy, a feature extraction library in the scope of fake news. It includes functions for calculating the readability scores, Information complexity, sentiment analysis using VADER,  Named Entities, and part-of-speech tags. With these functions, relevant features for fake news detection can be computed. Furthermore, we provide a Dunn test function which can be used to test the significance between multiple independent variables. 
 
 With the development of faKy, we hope to contribute to more sophisticated and interpretable ML models and better comprehend the phenomenon of fake news by understanding these objects’ underlying different linguistic features.
 
 ## Installation
 FaKy can be installed through pip install faKy; the NLTK and spaCy's web_core_web_md are automatically installed within the faKy library
 
 ## faKy 101
 The use case of faKy is the computation of features based on text objects; the faKy library can be used to compute the features for all the text objects in the data frame. See the example code block.
 
 Import the faky library and the corresponding function:
-```python
-from faKy.faKy import process_text_readability 
-```
+    from faKy.faKy import process_text_readability
 
 Apply process_text_readability to the data frame
-```python
-dummy_df['readability'] = dummy_df['text-object'].apply(process_text_readability) 
-```
+    dummy_df['readability'] = dummy_df['text-object'].apply(process_text_readability)
 
 # faKy functionality
 | Function Name             | Usage                                                                                                                                                            |
 |---------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | readability_computation   | Computes the Flesch-Kincaid Reading Ease score for a spaCy document using the Readability class. Returns the original document object.                           |
 | process_text_readability  | Takes a text string as input, processes it with spaCy's NLP pipeline, and computes the Flesch-Kincaid Reading Ease score. Returns the score.                       |
 | compress_doc              | Compresses the serialized form of a spaCy Doc object using gzip, calculates the compressed size, and sets the compressed size to the custom "compressed_size" attribute of the Doc object. Returns the Doc object. |
@@ -40,8 +27,8 @@
 | count_named_entities      | Takes a text input, identifies named entities using spaCy, and returns the count of named entities in the text.                                                 |
 | count_ner_labels          | Takes a text input, identifies named entities using spaCy, and returns a dictionary of named entity label counts.                                               |
 | create_input_vector_NER   | Takes a dictionary of named entity recognition (NER) label counts and creates an input vector with the count for each NER label. Returns the input vector.         |
 | count_pos                 | Counts the number of parts of speech (POS) in a given text. Returns a dictionary with the count of each POS.                                                    |
 | create_input_vector_pos   | Takes a dictionary of POS tag counts and creates an input vector of zeros. Returns the input vector.                                                             |
 | values_by_label           | Takes a DataFrame, a feature, a list of labels, and a label column name. Returns a list of lists containing the values of the feature for each label.             |
 | dunn_table                | Takes a DataFrame of Dunn's test results and creates a new DataFrame with pairwise comparisons between groups. Returns the new DataFrame.                           |
-    
+
```

### Comparing `faKy-1.4.0/README.md` & `faKy-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+Metadata-Version: 2.1
+Name: faKy
+Version: 2.0.0
+Summary: Your library description
+Author: Sandro Barres Hamers
+Author-email: sbarreshamers@gmail.com
+Description-Content-Type: text/markdown
+Provides-Extra: vader
+
 # faKy
 We introduce faKy, a feature extraction library in the scope of fake news. It includes functions for calculating the readability scores, Information complexity, sentiment analysis using VADER,  Named Entities, and part-of-speech tags. With these functions, relevant features for fake news detection can be computed. Furthermore, we provide a Dunn test function which can be used to test the significance between multiple independent variables. 
 
 With the development of faKy, we hope to contribute to more sophisticated and interpretable ML models and better comprehend the phenomenon of fake news by understanding these objects’ underlying different linguistic features.
 
 ## Installation
 FaKy can be installed through pip install faKy; the NLTK and spaCy's web_core_web_md are automatically installed within the faKy library
 
 ## faKy 101
 The use case of faKy is the computation of features based on text objects; the faKy library can be used to compute the features for all the text objects in the data frame. See the example code block.
 
 Import the faky library and the corresponding function:
-```python
-from faKy.faKy import process_text_readability 
-```
+    from faKy.faKy import process_text_readability
 
 Apply process_text_readability to the data frame
-```python
-dummy_df['readability'] = dummy_df['text-object'].apply(process_text_readability) 
-```
+    dummy_df['readability'] = dummy_df['text-object'].apply(process_text_readability)
 
 # faKy functionality
 | Function Name             | Usage                                                                                                                                                            |
 |---------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | readability_computation   | Computes the Flesch-Kincaid Reading Ease score for a spaCy document using the Readability class. Returns the original document object.                           |
 | process_text_readability  | Takes a text string as input, processes it with spaCy's NLP pipeline, and computes the Flesch-Kincaid Reading Ease score. Returns the score.                       |
 | compress_doc              | Compresses the serialized form of a spaCy Doc object using gzip, calculates the compressed size, and sets the compressed size to the custom "compressed_size" attribute of the Doc object. Returns the Doc object. |
@@ -31,8 +36,8 @@
 | count_named_entities      | Takes a text input, identifies named entities using spaCy, and returns the count of named entities in the text.                                                 |
 | count_ner_labels          | Takes a text input, identifies named entities using spaCy, and returns a dictionary of named entity label counts.                                               |
 | create_input_vector_NER   | Takes a dictionary of named entity recognition (NER) label counts and creates an input vector with the count for each NER label. Returns the input vector.         |
 | count_pos                 | Counts the number of parts of speech (POS) in a given text. Returns a dictionary with the count of each POS.                                                    |
 | create_input_vector_pos   | Takes a dictionary of POS tag counts and creates an input vector of zeros. Returns the input vector.                                                             |
 | values_by_label           | Takes a DataFrame, a feature, a list of labels, and a label column name. Returns a list of lists containing the values of the feature for each label.             |
 | dunn_table                | Takes a DataFrame of Dunn's test results and creates a new DataFrame with pairwise comparisons between groups. Returns the new DataFrame.                           |
-    
+
```

### Comparing `faKy-1.4.0/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json` & `faKy-2.0.0/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json`

 * *Files identical despite different names*

### Comparing `faKy-1.4.0/faKy/en_core_web_md-2.3.1/meta.json` & `faKy-2.0.0/faKy/en_core_web_md-2.3.1/meta.json`

 * *Files identical despite different names*

### Comparing `faKy-1.4.0/faKy/en_core_web_md-2.3.1/setup.py` & `faKy-2.0.0/faKy/en_core_web_md-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `faKy-1.4.0/faKy/faKy.py` & `faKy-2.0.0/faKy/faKy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+import spacy.util
+
+# Load the 'en_core_web_md' model
+try:
+    nlp = spacy.load('en_core_web_md')
+except OSError:
+    # Download the model if it's not found
+    spacy.util.download('en_core_web_md')
+    nlp = spacy.load('en_core_web_md')
+
 import pandas as pd 
 import numpy as np
 import sys
 import gzip
 import spacy
-import os
 from spacy.tokens import Doc
 from spacy_readability import Readability
 import nltk
 from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer
 
 
 
 nltk.download('vader_lexicon')
-current_dir = os.path.dirname(os.path.abspath(__file__))
-model_path = os.path.join(current_dir, 'en_core_web_md-2.3.1')
-nlp = spacy.load(model_path)
 
 
 '''
  The function readability_computation computes the Flesch-Kincaid Reading Ease score for a spaCy document using the Readability class. 
  It returns the original document object. 
  It is added to the spaCy pipeline using nlp.add_pipe with last=True.
 '''
```

### Comparing `faKy-1.4.0/faKy.egg-info/PKG-INFO` & `faKy-2.0.0/faKy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.4.0
+Version: 2.0.0
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 
 # faKy
@@ -15,22 +15,18 @@
 ## Installation
 FaKy can be installed through pip install faKy; the NLTK and spaCy's web_core_web_md are automatically installed within the faKy library
 
 ## faKy 101
 The use case of faKy is the computation of features based on text objects; the faKy library can be used to compute the features for all the text objects in the data frame. See the example code block.
 
 Import the faky library and the corresponding function:
-```python
-from faKy.faKy import process_text_readability 
-```
+    from faKy.faKy import process_text_readability
 
 Apply process_text_readability to the data frame
-```python
-dummy_df['readability'] = dummy_df['text-object'].apply(process_text_readability) 
-```
+    dummy_df['readability'] = dummy_df['text-object'].apply(process_text_readability)
 
 # faKy functionality
 | Function Name             | Usage                                                                                                                                                            |
 |---------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | readability_computation   | Computes the Flesch-Kincaid Reading Ease score for a spaCy document using the Readability class. Returns the original document object.                           |
 | process_text_readability  | Takes a text string as input, processes it with spaCy's NLP pipeline, and computes the Flesch-Kincaid Reading Ease score. Returns the score.                       |
 | compress_doc              | Compresses the serialized form of a spaCy Doc object using gzip, calculates the compressed size, and sets the compressed size to the custom "compressed_size" attribute of the Doc object. Returns the Doc object. |
```

### Comparing `faKy-1.4.0/setup.py` & `faKy-2.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='faKy',
-    version='1.4.0',
+    version='2.0.0',
     description='Your library description',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Sandro Barres Hamers',
     author_email='sbarreshamers@gmail.com',
     packages=['faKy'],
     install_requires=[
@@ -19,12 +19,11 @@
         'spacy-readability==1.4.1',
         'nltk==3.7',
         'vaderSentiment==3.3.2',
     ],
     extras_require={
         'vader': ['vaderSentiment'],
     },
-package_data={
-    'faKy': ['en_core_web_md-2.3.1/*', 'en_core_web_md-2.3.1/en_core_web_md/*', 'en_core_web_md-2.3.1/en_core_web_md-2.3.1.egg-info/*'],
-},
-
+    package_data={
+    'faKy': ['en_core_web_md-2.3.1/*', 'en_core_web_md-2.3.1/en_core_web_md/*'],
+}
 )
```

