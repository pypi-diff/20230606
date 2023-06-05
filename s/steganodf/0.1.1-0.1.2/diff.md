# Comparing `tmp/steganodf-0.1.1.tar.gz` & `tmp/steganodf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steganodf-0.1.1.tar", max compression
+gzip compressed data, was "steganodf-0.1.2.tar", max compression
```

## Comparing `steganodf-0.1.1.tar` & `steganodf-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      837 2023-05-29 22:52:55.771268 steganodf-0.1.1/README.md
--rw-r--r--   0        0        0      388 2023-05-30 21:34:22.834802 steganodf-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5298 2023-05-30 21:31:04.708137 steganodf-0.1.1/steganodf/__init__.py
--rw-r--r--   0        0        0       20 2023-05-29 22:48:26.964604 steganodf-0.1.1/steganodf/__main__.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 steganodf-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      837 2023-05-29 22:52:55.771268 steganodf-0.1.2/README.md
+-rw-r--r--   0        0        0      388 2023-06-05 22:34:29.974145 steganodf-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5967 2023-06-05 22:30:27.037481 steganodf-0.1.2/steganodf/__init__.py
+-rw-r--r--   0        0        0       20 2023-05-29 22:48:26.964604 steganodf-0.1.2/steganodf/__main__.py
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 steganodf-0.1.2/PKG-INFO
```

### Comparing `steganodf-0.1.1/README.md` & `steganodf-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `steganodf-0.1.1/steganodf/__init__.py` & `steganodf-0.1.2/steganodf/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import more_itertools as more
 from numpy import remainder
 import pandas as pd
 import hashlib
 import hmac
 
 
-class WatermarkingError(Exception):
+class PayloadError(Exception):
     pass
 
 
 def _is_duplicated(indexes: list) -> bool:
     """Check is there are duplicated elements"""
     return len(indexes) != len(set(indexes))
 
@@ -38,46 +38,46 @@
         hash_function = lambda x: hmac.new(
             password.encode(), msg=str(x).encode(), digestmod=hash_algorithm
         ).hexdigest()
 
     return hash_function
 
 
-def encode_index(indexes: list, message: str) -> list:
-    """Encode a message by permutation
+def encode_index(indexes: list, payload: str) -> list:
+    """Encode a payload by permutation
 
     This function read the list in block of 6 lines.
     With 6 items, you have 6!=720 possible permutation which is enough to store
     1 byte = 256 first permutations.
-    For each block of 6, it encode the message as a bytearray.
+    For each block of 6, it encode the payload as a bytearray.
 
     Todo :
         Add blocksize as argument
 
     Args:
         indexes(list): a list of unique index
-        message(str): the message to store
+        payload(str): the payload to store
     Return:
-        A new indexes with message encoded
+        A new indexes with payload encoded
     """
 
     if _is_duplicated(indexes):
         raise IndexError("No duplicated elements are allowed")
 
     size = len(list(indexes))
-    msg = message.encode()
+    msg = payload.encode()
 
     block_size = 6
     msg_index = 0
     output_list = []
 
     n_block = size // block_size
 
     if len(msg) > n_block:
-        raise WatermarkingError(f"Cannot store a message more than {n_block} bytes ")
+        raise PayloadError(f"Cannot store a payload more than {n_block} bytes ")
 
     i = 0
     for i in range(0, size // block_size * block_size, block_size):
         block = indexes[i : i + block_size]
 
         if msg_index < len(msg):
             a_bytes = msg[msg_index]
@@ -100,69 +100,86 @@
     Differential decoding by comparing indexes and sorted indexes
 
     Args:
         indexes(list): a list of unique index values
         sort_indexes(list): Same list with a different order
 
     Return:
-        The watermark message
+        The watermark payload
     """
     if sort_indexes is None:
         sort_indexes = sorted(indexes)
 
     size = len(indexes)
     block_size = 6
-    message = ""
+    payload = ""
 
     for i in range(0, size // block_size * block_size, block_size):
         u_block = indexes[i : i + block_size]
         s_block = sort_indexes[i : i + block_size]
         a_byte = more.permutation_index(u_block, s_block)
 
         if a_byte != 0:
-            message += chr(a_byte)
+            payload += chr(a_byte)
 
-    return message
+    return payload
 
 
 def encode_pandas(
     df: pd.DataFrame,
-    message: str,
+    payload: str,
     password: str | None = None,
     hash_algorithm: str = "sha256",
 ) -> pd.DataFrame:
     """
-    Store a secret message in dataframe by row permutation.
+    Store a secret payload in dataframe by row permutation.
 
-    This function use encode_index to store a message in a dataframe.
+    This function use encode_index to store a payload in a dataframe.
     The dataframe is sorted by hash value of each row with a user defined algorithm.
     Then it uses this sorted dataframe as reference and computed a new sorted
-    dataframe with the message encoded inside.
+    dataframe with the payload encoded inside.
 
     Args:
         df(pd.DataFrame): dataframe to watermark
-        message: message to encode
+        payload: payload to encode
         password(str): If defined, use a HMAC hash function.
         hash_algorithm(str): Algorithm name supported by hashlib
     Return:
         watermarked dataframe
 
     """
 
+    # Create hash function
     hash_function = _create_hash_fct(hash_algorithm, password)
-    hash_df = df.copy()
-    hash_df["hash"] = hash_df.applymap(str).sum(axis=1).apply(hash_function)
-    hash_df = hash_df.sort_values("hash").reset_index(drop=True)
-
-    h = hash_df[hash_df["hash"].duplicated()]["hash"].squeeze()
-
-    new_index = encode_index(hash_df.index.to_list(), message)
-
-    hash_df.iloc[new_index].to_csv("/tmp/test.csv")
-    return hash_df.iloc[new_index].drop("hash", axis=1).reset_index(drop=True)
+   
+    # Do not edit original 
+    source_df = df.copy()
+    
+    # Remove duplicated rows and keep it for later  
+    duplicated_df = source_df[source_df.duplicated()]
+
+    # Keep only unique rows 
+    source_df = source_df[~source_df.duplicated()]
+    
+    # compute hash 
+    source_df["hash"] =  source_df.applymap(str).sum(axis=1).apply(hash_function)
+    
+    # Sort by hash 
+    source_df = source_df.sort_values("hash").reset_index(drop=True)
+
+    # Get new encoded index 
+    new_index = encode_index(source_df.index.to_list(),payload)
+
+    # Get encoded dataframe  
+    new_df = source_df.iloc[new_index].drop("hash", axis=1)
+    
+    # Concat encoded dataframe with the remaining duplicates
+    new_df = pd.concat((new_df, duplicated_df)).reset_index(drop=True)
+    
+    return new_df
 
 
 def decode_pandas(
     df: pd.DataFrame, hash_algorithm: str = "sha256", password=None
 ) -> str:
     """
     Extract watermark from a dataframe
@@ -171,24 +188,39 @@
         df(pd.DataFrame): DataFrame with a watermark
         hash_algorithm(str): hashlib algorithm name
         password(str): hmac password if required
 
     Raise:
         NoWatermarkFound
     Return:
-        The watermark message
+        The watermark payload
 
 
     """
+    
+    # Compute hash function 
     hash_function = _create_hash_fct(hash_algorithm, password)
-    hash_df = df.copy()
-    hash_df["hash"] = hash_df.applymap(str).sum(axis=1).apply(hash_function)
-    hash_df = hash_df.sort_values("hash").reset_index(names="origin_index")
 
+    # keep a copy 
+    encoded_df = df.copy()
+    
+    # remove duplicated rows 
+    new_df = encoded_df[~encoded_df.duplicated()]
+
+    # Reset index and keep as a new column named 'old'
+    new_df = new_df.reset_index(names="old")
+    
+    # Compute hash 
+    new_df["hash"]=new_df.iloc[:, 1:].applymap(str).sum(axis=1).apply(hash_function)
+    
+    # Sort values by hash 
+    new_df = new_df.sort_values("hash").reset_index()
+    
+    # Extract payload 
     try:
-        message = decode_index(
-            hash_df.index.to_list(), hash_df["origin_index"].to_list()
-        )
+        payload = decode_index(new_df.index.to_list(), new_df["old"].to_list())
+    
     except:
-        raise WatermarkingError("Cannot find a watermark")
+        raise PayloadError("Cannot extract a payload")
+
+    return payload
 
-    return message
```

### Comparing `steganodf-0.1.1/PKG-INFO` & `steganodf-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steganodf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Functions to add steganographic message to a dataframe with row permutation
 Author: Sacha Schutz
 Author-email: sacha@labsquare.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

