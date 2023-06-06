# Comparing `tmp/pyBigKinds-1.0.0-py3-none-any.whl.zip` & `tmp/pyBigKinds-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6750 bytes, number of entries: 11
+Zip file size: 7143 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      753 b- defN 23-Jun-03 07:43 pyBigKinds/__init__.py
--rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-01 11:08 pyBigKinds/_version.py
--rw-rw-rw-  2.0 fat     1298 b- defN 23-Jun-03 01:08 pyBigKinds/base.py
--rw-rw-rw-  2.0 fat     3242 b- defN 23-Jun-03 07:43 pyBigKinds/preprocessing.py
--rw-rw-rw-  2.0 fat      461 b- defN 23-Jun-03 07:43 pyBigKinds/representation.py
--rw-rw-rw-  2.0 fat     1984 b- defN 23-Jun-03 07:43 pyBigKinds/visualization.py
--rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-03 14:00 pyBigKinds-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1600 b- defN 23-Jun-03 14:00 pyBigKinds-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 14:00 pyBigKinds-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-03 14:00 pyBigKinds-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      883 b- defN 23-Jun-03 14:00 pyBigKinds-1.0.0.dist-info/RECORD
-11 files, 11416 bytes uncompressed, 5256 bytes compressed:  54.0%
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-06 07:37 pyBigKinds/_version.py
+-rw-rw-rw-  2.0 fat     2475 b- defN 23-Jun-06 07:38 pyBigKinds/base.py
+-rw-rw-rw-  2.0 fat     4744 b- defN 23-Jun-06 07:38 pyBigKinds/preprocessing.py
+-rw-rw-rw-  2.0 fat      720 b- defN 23-Jun-06 07:38 pyBigKinds/representation.py
+-rw-rw-rw-  2.0 fat     2374 b- defN 23-Jun-06 07:38 pyBigKinds/visualization.py
+-rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-06 07:44 pyBigKinds-1.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1600 b- defN 23-Jun-06 07:44 pyBigKinds-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 07:44 pyBigKinds-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-06 07:44 pyBigKinds-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      883 b- defN 23-Jun-06 07:44 pyBigKinds-1.0.5.dist-info/RECORD
+11 files, 14744 bytes uncompressed, 5649 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pyBigKinds/representation.py
 Comment: 
 
 Filename: pyBigKinds/visualization.py
 Comment: 
 
-Filename: pyBigKinds-1.0.0.dist-info/LICENSE
+Filename: pyBigKinds-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: pyBigKinds-1.0.0.dist-info/METADATA
+Filename: pyBigKinds-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: pyBigKinds-1.0.0.dist-info/WHEEL
+Filename: pyBigKinds-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: pyBigKinds-1.0.0.dist-info/top_level.txt
+Filename: pyBigKinds-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pyBigKinds-1.0.0.dist-info/RECORD
+Filename: pyBigKinds-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyBigKinds/_version.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.0"
+__version__ = "1.0.5"
```

## pyBigKinds/base.py

```diff
@@ -1,52 +1,80 @@
 import pandas as pd
 
 
 def header_remover(df):
     """[]로 표시된 헤더 삭제"""
-    ans = df["제목"].str.replace("\[[^)]*\]", "")
+    if isinstance(df, pd.DataFrame):
+        ans = df["제목"].str.replace("\[[^)]*\]", "")
+    elif isinstance(df, list):
+        ans = df.str.replace("\[[^)]*\]", "")
+    else:
+        raise TypeError("input value is to be have to list or DataFrame")
     return ans
 
 
 def keyword_list(df):
     """키워드를 list로 변환"""
-    return df["키워드"].values.tolist()
+    if isinstance(df, pd.DataFrame):
+        return df["키워드"].values.tolist()
+    elif isinstance(df, list):
+        return df.values.tolist()
+    else:
+        raise TypeError("input value is to be have to list or DataFrame")
 
 
 def keyword_parser(text_list):
     """키워드 파싱"""
-    news_key = []
-    for word in text_list:
-        word = word.split(",")
-        news_key.append(word)
-    return news_key
+    if isinstance(text_list, list):
+        news_key = []
+        for word in text_list:
+            if isinstance(word, str):
+                word = word.split(",")
+                news_key.append(word)
+            else:
+                raise ValueError("input list is not valid format")
+        return news_key
+    else:
+        raise TypeError("input type is to be have to list")
 
 
 def duplication_remover(news_key):
     """중복 값 제거"""
-    news_value = []
-    for j in news_key:
-        j = list(set(j))
-        news_value.append(j)
-    return news_value
+    if isinstance(news_key, list):
+        news_value = []
+        for j in news_key:
+            if isinstance(j, list):
+                j = list(set(j))
+                news_value.append(j)
+            else:
+                raise ValueError("input list is not valid format")
+        return news_value
+    else:
+        raise TypeError("input type is to be have to list")
 
 
 def word_counter(news_value):
     """단어 갯수 카운트"""
-    key_words = {}
-    for k in range(len(news_value)):
-        for i in news_value[k]:
-            if i not in key_words:
-                key_words[i] = 1
-            elif i in key_words:
-                key_words[i] += 1
-    return key_words
+    if isinstance(news_value, list):
+        key_words = {}
+        for k in range(len(news_value)):
+            for i in news_value[k]:
+                if i not in key_words:
+                    key_words[i] = 1
+                elif i in key_words:
+                    key_words[i] += 1
+        return key_words
+    else:
+        raise TypeError("input type is to be have to list")
 
 
 def counter_to_dataframe(key_words):
     """counter dict --> dataframe"""
-    word_df = pd.DataFrame(key_words.items())
-    word_df.columns = ["단어", "빈도"]
-    word_df = word_df.sort_values(["빈도"], ascending=False).reset_index(
-        drop=True,
-    )  # 내림차순 정렬
-    return word_df
+    if isinstance(key_words, dict):
+        word_df = pd.DataFrame(key_words.items())
+        word_df.columns = ["단어", "빈도"]
+        word_df = word_df.sort_values(["빈도"], ascending=False).reset_index(
+            drop=True,
+        )
+        return word_df
+    else:
+        raise TypeError("input type is to be have to dict")
```

## pyBigKinds/preprocessing.py

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import pandas as pd
 from sklearn.decomposition import NMF, PCA, TruncatedSVD
 from sklearn.feature_extraction.text import CountVectorizer, TfidfTransformer, TfidfVectorizer
 from sklearn.manifold import TSNE
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import Normalizer
 
@@ -12,116 +13,145 @@
     keyword_parser,
     word_counter,
 )
 
 
 def day_range(df):
     """날짜 범위 파악"""
-    print("first day: ", df["일자"].min(), "\n", "last day: ", df["일자"].max())
+    if isinstance(df, pd.DataFrame):
+        print("first day: ", df["일자"].min(), "\n", "last day: ", df["일자"].max())
+    else:
+        raise TypeError("input type is to be have to DataFrame")
 
 
 def press_counter(df):
     """언론사 별 보도 빈도"""
-    freq = df["언론사"].value_counts()
-    brod_df = pd.DataFrame(freq).reset_index()
-    brod_df.rename(columns={"index": "언론사", "언론사": "기사"}, inplace=True)
-    return brod_df
+    if isinstance(df, pd.DataFrame):
+        freq = df["언론사"].value_counts()
+        brod_df = pd.DataFrame(freq).reset_index()
+        brod_df.rename(columns={"index": "언론사", "언론사": "기사"}, inplace=True)
+        return brod_df
+    else:
+        raise TypeError("input type is to be have to DataFrame")
 
 
 def keyword_dataframe(df):
     """키워드 단어 빈도"""
-    lis = keyword_list(df)
-    keywords = keyword_parser(lis)
-    counter = word_counter(keywords)
-    df = counter_to_dataframe(counter)
-    return df
+    if isinstance(df, pd.DataFrame):
+        lis = keyword_list(df)
+        keywords = keyword_parser(lis)
+        counter = word_counter(keywords)
+        df = counter_to_dataframe(counter)
+        return df
+    else:
+        raise TypeError("input type is to be have to DataFrame")
 
 
 def keyword_dataframe_no_duplicated(df):
     """키워드 중복 제거 단어 빈도"""
-    lis = keyword_list(df)
-    keywords = keyword_parser(lis)
-    keywords_set = duplication_remover(keywords)
-    counter = word_counter(keywords_set)
-    df = counter_to_dataframe(counter)
-    return df
+    if isinstance(df, pd.DataFrame):
+        lis = keyword_list(df)
+        keywords = keyword_parser(lis)
+        keywords_set = duplication_remover(keywords)
+        counter = word_counter(keywords_set)
+        df = counter_to_dataframe(counter)
+        return df
+    else:
+        raise TypeError("input type is to be have to DataFrame")
 
 
-def tfidf(df, *press: str):
+def tfidf(df, *press):
     """키워드 상대 빈도"""
-    if press:
-        df = df[press]
-    lis = keyword_list(df)
-
-    tfidfv = TfidfVectorizer()
-    tdm = tfidfv.fit_transform(lis)
-
-    word_count = (
-        pd.DataFrame(
-            {
-                "단어": tfidfv.get_feature_names_out(),
-                "빈도": tdm.sum(axis=0).flat,
-            },
+    if isinstance(df, pd.DataFrame):
+        if isinstance(press, str):
+            df = df[press]
+        lis = keyword_list(df)
+
+        tfidfv = TfidfVectorizer()
+        tdm = tfidfv.fit_transform(lis)
+
+        word_count = (
+            pd.DataFrame(
+                {
+                    "단어": tfidfv.get_feature_names_out(),
+                    "빈도": tdm.sum(axis=0).flat,
+                },
+            )
+            .sort_values("빈도", ascending=False)
+            .reset_index(drop=True)
         )
-        .sort_values("빈도", ascending=False)
-        .reset_index(drop=True)
-    )
-    return word_count
+        return word_count
+    else:
+        raise TypeError("input type is to be have to DataFrame")
 
 
 def tfidf_vector(df):
     """tfidf vector"""
-    lis = keyword_list(df)
-    pipeline = Pipeline(
-        [
-            ("vect", CountVectorizer()),
-            ("tfidf", TfidfTransformer()),
-        ],
-    )
-    vec = pipeline.fit_transform(lis).toarray()
-    return vec
+    if isinstance(df, pd.DataFrame):
+        lis = keyword_list(df)
+        pipeline = Pipeline(
+            [
+                ("vect", CountVectorizer()),
+                ("tfidf", TfidfTransformer()),
+            ],
+        )
+        vec = pipeline.fit_transform(lis).toarray()
+        return vec
+    else:
+        raise TypeError("input type is to be have to DataFrame")
 
 
 def normalize_vector(vec):
     """normalize vector"""
-    vec_nor = Normalizer().fit_transform(vec)
-    return vec_nor
+    if isinstance(vec, np.ndarray):
+        vec_nor = Normalizer().fit_transform(vec)
+        return vec_nor
+    else:
+        raise TypeError("input type is to be have to ndarray")
 
 
 def pca(vec, Random_State=123):
     """PCA"""
+    if isinstance(vec, np.ndarray):
+        pca_df = PCA(n_components=2, random_state=Random_State, copy=False).fit_transform(
+            vec,
+        )
+        pca_df = pd.DataFrame(pca_df, columns=["component 0", "component 1"])
 
-    pca_df = PCA(n_components=2, random_state=Random_State, copy=False).fit_transform(
-        vec,
-    )
-    pca_df = pd.DataFrame(pca_df, columns=["component 0", "component 1"])
-
-    return pca_df
+        return pca_df
+    else:
+        raise TypeError("input type is to be have to ndarray")
 
 
 def nmf(vec, Random_State=123):
     """NMF"""
-
-    nmf_df = NMF(
-        n_components=2, random_state=Random_State, init="random",
-    ).fit_transform(vec)
-    nmf_df = pd.DataFrame(nmf_df, columns=["component 0", "component 1"])
-
-    return nmf_df
+    if isinstance(vec, np.ndarray):
+        nmf_df = NMF(
+            n_components=2, random_state=Random_State, init="random",
+        ).fit_transform(vec)
+        nmf_df = pd.DataFrame(nmf_df, columns=["component 0", "component 1"])
+
+        return nmf_df
+    else:
+        raise TypeError("input type is to be have to ndarray")
 
 
 def t_sne(vec, learn_Rate=100):
     """t-sne"""
-
-    tsne = TSNE(n_components=2, learning_rate=learn_Rate).fit_transform(vec)
-    tsne_df = pd.DataFrame(tsne, columns=["component 0", "component 1"])
+    if isinstance(vec, np.ndarray):
+        tsne = TSNE(n_components=2, learning_rate=learn_Rate).fit_transform(vec)
+        tsne_df = pd.DataFrame(tsne, columns=["component 0", "component 1"])
+    else:
+        raise TypeError("input type is to be have to ndarray")
 
     return tsne_df
 
 
 def lsa(vec):
     """LSA"""
-
-    svd = TruncatedSVD(n_components=2).fit_transform(vec)
-    svd_df = pd.DataFrame(data=svd, columns=["component 0", "component 1"])
+    if isinstance(vec, np.ndarray):
+        svd = TruncatedSVD(n_components=2).fit_transform(vec)
+        svd_df = pd.DataFrame(data=svd, columns=["component 0", "component 1"])
+    else:
+        raise TypeError("input type is to be have to ndarray")
 
     return svd_df
```

## pyBigKinds/representation.py

```diff
@@ -1,15 +1,22 @@
 # pylint: disable=E0601,W0612
 
+import numpy as np
 from sklearn.cluster import DBSCAN, KMeans
 
 
-def kmeans(vec, k, random_state=None):
+def kmeans(vec, k, random_state=123):
     """K-Means"""
-    kmeans_model = KMeans(n_clusters=k, max_iter=1000, random_state=random_state)
-    return kmeans_model.fit_predict(vec)
+    if isinstance(vec, np.ndarray):
+        kmeans_model = KMeans(n_clusters=k, max_iter=1000, random_state=random_state)
+        return kmeans_model.fit_predict(vec)
+    else:
+        raise TypeError("input type is to be have to ndarray")
 
 
 def dbscan(vec, eps, min_samples, metric="euclidean"):
     """DBSCAN"""
-    dbscan_model = DBSCAN(eps=eps, min_samples=min_samples, metric=metric)
-    return dbscan_model.fit_predict(vec)
+    if isinstance(vec, np.ndarray):
+        dbscan_model = DBSCAN(eps=eps, min_samples=min_samples, metric=metric)
+        return dbscan_model.fit_predict(vec)
+    else:
+        raise TypeError("input type is to be have to ndarray")
```

## pyBigKinds/visualization.py

```diff
@@ -1,76 +1,82 @@
 # pylint: disable=W0612
-
 import platform
 
 import matplotlib.pyplot as plt
+import pandas as pd
 import wordcloud
 
 from .base import (
     counter_to_dataframe,
     duplication_remover,
     keyword_list,
     keyword_parser,
     word_counter,
 )
 
-if platform.system() in ["Windows", "linux"]:
+if platform.system() in ["Windows", "Linux"]:
     plt.rcParams["font.family"] = "Malgun Gothic"
     font_path = "malgun"
 
 elif platform.system() == "Darwin":
     plt.rcParams["font.family"] = "AppleGothic"
     font_path = "AppleGothic"
 
 else:
     print("미지원 os입니다.")
 
 plt.rcParams["axes.unicode_minus"] = False
 
 
-def keywords_wordcloud(df, press: str):
+def keywords_wordcloud(df, press):
     """언론사 별 키워드 워드클라우드 생성"""
-    df_keywords = df[df["언론사"] == press]
-    keywords = keyword_list(df_keywords)
-    news_key = keyword_parser(keywords)
-    news_key = duplication_remover(news_key)
-    key = word_counter(news_key)
-    news_key = counter_to_dataframe(key)
-    wc = wordcloud.WordCloud(
-        font_path=font_path,
-        width=500,
-        height=500,
-        background_color="white",
-    ).generate_from_frequencies(news_key.set_index("단어").to_dict()["빈도"])
-
-    plt.imshow(wc)
-    plt.axis("off")
-    plt.show()
-
-
-def top_words(df, press: str):
-    """언론사 별 사용 단어 빈도 상위 25개"""
-    df_keywords = df[df["언론사"].str.contains(press)]
-    keywords = keyword_list(df_keywords)
-    news_key = keyword_parser(keywords)
-    news_key = duplication_remover(news_key)
-    key = word_counter(news_key)
-    news_key = counter_to_dataframe(key)
-
-    data = news_key.head(25)
-    plt.barh(data["단어"], data["빈도"].sort_values(ascending=True))
-    plt.show()
+    if isinstance(df, pd.DataFrame):
+        df_keywords = df[df[press] == press]
+        keywords = keyword_list(df_keywords)
+        news_key = keyword_parser(keywords)
+        news_key = duplication_remover(news_key)
+        key = word_counter(news_key)
+        news_key = counter_to_dataframe(key)
+        wc = wordcloud.WordCloud(
+            font_path=font_path,
+            width=500,
+            height=500,
+            background_color="white",
+        ).generate_from_frequencies(news_key.set_index("단어").to_dict()["빈도"])
+
+        plt.imshow(wc)
+        plt.axis("off")
+        plt.show()
+    else:
+        raise TypeError("input type is to be have to DataFrame")
+
+
+def top_words(df, press, top_n=25):
+    """언론사 별 사용 단어 빈도 상위 n개"""
+    if isinstance(df, pd.DataFrame):
+        df_keywords = df[df[press].str.contains(press)]
+        keywords = keyword_list(df_keywords)
+        news_key = keyword_parser(keywords)
+        news_key = duplication_remover(news_key)
+        key = word_counter(news_key)
+        news_key = counter_to_dataframe(key)
+
+        data = news_key.head(top_n)
+        plt.barh(data["단어"], data["빈도"].sort_values(ascending=True))
+        plt.show()
+    else:
+        raise TypeError("input type is to be have to DataFrame")
 
 
-def scatterplot(df, label: str):
+def scatterplot(df, label):
     """scatter plot for dimension reduction"""
-    fig, ax = plt.subplots()
-    try:
+    if isinstance(df, pd.DataFrame):
+        fig, ax = plt.subplots()
         groups = df.groupby(label)
-    except:
-        raise ValueError("There's no label")
 
-    for name, points in groups:
-        ax.scatter(points["component 0"], points["component 1"], label=name)
+        for name, points in groups:
+            ax.scatter(points["component 0"], points["component 1"], label=name)
 
-    ax.legend()
-    plt.show()
+        ax.legend()
+        plt.show()
+    else:
+        raise TypeError("input type is to be have to DataFrame")
```

## Comparing `pyBigKinds-1.0.0.dist-info/LICENSE` & `pyBigKinds-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyBigKinds-1.0.0.dist-info/METADATA` & `pyBigKinds-1.0.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBigKinds
-Version: 1.0.0
+Version: 1.0.5
 Summary: BigKinds Data Analysis Toolkit for python
 Home-page: https://github.com/sorrychoe/pyBigKinds
 Author: Sorrychoe
 License: MIT
 Project-URL: Source Code, https://github.com/sorrychoe/pyBigKinds
 Project-URL: Bug Tracker, https://github.com/sorrychoe/pyBigKinds/issues
 Keywords: Journalism,preprocessing-data,BigKinds
```

