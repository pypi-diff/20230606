# Comparing `tmp/text2phonemesequence-0.1.3.tar.gz` & `tmp/text2phonemesequence-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/text2phonemesequence-0.1.3.tar", last modified: Sun Jun  4 06:34:35 2023, max compression
+gzip compressed data, was "dist/text2phonemesequence-0.1.4.tar", last modified: Tue Jun  6 02:27:01 2023, max compression
```

## Comparing `text2phonemesequence-0.1.3.tar` & `text2phonemesequence-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2838 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1975 2023-06-04 05:13:39.000000 text2phonemesequence-0.1.3/README.md
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/setup.cfg
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.1.3/setup.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-06-04 06:34:11.000000 text2phonemesequence-0.1.3/text2phonemesequence/__init__.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     8114 2023-06-04 05:13:39.000000 text2phonemesequence-0.1.3/text2phonemesequence/text2phonemesequence.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2838 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/SOURCES.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/dependency_links.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/requires.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/top_level.txt
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-06 02:27:01.000000 text2phonemesequence-0.1.4/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2838 2023-06-06 02:27:01.000000 text2phonemesequence-0.1.4/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1975 2023-06-04 05:13:39.000000 text2phonemesequence-0.1.4/README.md
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-06-06 02:27:01.000000 text2phonemesequence-0.1.4/setup.cfg
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.1.4/setup.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-06 02:27:01.000000 text2phonemesequence-0.1.4/text2phonemesequence/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-06-06 02:26:42.000000 text2phonemesequence-0.1.4/text2phonemesequence/__init__.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     8133 2023-06-06 02:23:53.000000 text2phonemesequence-0.1.4/text2phonemesequence/text2phonemesequence.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-06 02:27:01.000000 text2phonemesequence-0.1.4/text2phonemesequence.egg-info/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2838 2023-06-06 02:27:01.000000 text2phonemesequence-0.1.4/text2phonemesequence.egg-info/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-06-06 02:27:01.000000 text2phonemesequence-0.1.4/text2phonemesequence.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-06-06 02:27:01.000000 text2phonemesequence-0.1.4/text2phonemesequence.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-06-06 02:27:01.000000 text2phonemesequence-0.1.4/text2phonemesequence.egg-info/requires.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-06-06 02:27:01.000000 text2phonemesequence-0.1.4/text2phonemesequence.egg-info/top_level.txt
```

### Comparing `text2phonemesequence-0.1.3/PKG-INFO` & `text2phonemesequence-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
```

### Comparing `text2phonemesequence-0.1.3/README.md` & `text2phonemesequence-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.1.3/setup.py` & `text2phonemesequence-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.1.3/text2phonemesequence/text2phonemesequence.py` & `text2phonemesequence-0.1.4/text2phonemesequence/text2phonemesequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.segment_tool = Tokenizer()
         self.language = language
         self.phoneme_length = {'msa.tsv': 27, 'amh.tsv': 28, 'urd.tsv': 152, 'mri.tsv': 30, 'glg.tsv': 22, 'swa.tsv': 28, 'est.tsv': 47, 'hbs-latn.tsv': 31, 'spa.tsv': 28, 'pol.tsv': 38, 'spa-latin.tsv': 24, 'fra.tsv': 43, 'uig.tsv': 33, 'aze.tsv': 34, 'nob.tsv': 52, 'swe.tsv': 36, 'por-bz.tsv': 28, 'arg.tsv': 30, 'yue.tsv': 227, 'sqi.tsv': 42, 'cat.tsv': 27, 'hbs-cyrl.tsv': 31, 'grc.tsv': 39, 'bak.tsv': 44, 'hun.tsv': 67, 'lat-clas.tsv': 61, 'ita.tsv': 37, 'san.tsv': 38, 'arm-w.tsv': 41, 'afr.tsv': 81, 'ind.tsv': 87, 'sme.tsv': 31, 'egy.tsv': 22, 'rus.tsv': 62, 'ady.tsv': 29, 'epo.tsv': 43, 'srp.tsv': 42, 'zho-t.tsv': 135, 'tha.tsv': 295, 'vie-c.tsv': 184, 'kur.tsv': 37, 'ice.tsv': 37, 'geo.tsv': 75, 'cze.tsv': 43, 'ara.tsv': 370, 'tgl.tsv': 27, 'nan.tsv': 175, 'por-po.tsv': 35, 'bos.tsv': 52, 'enm.tsv': 24, 'ltz.tsv': 55, 'ina.tsv': 26, 'ukr.tsv': 39, 'mac.tsv': 44, 'kaz.tsv': 44, 'slk.tsv': 73, 'ang.tsv': 33, 'khm.tsv': 47, 'syc.tsv': 24, 'eus.tsv': 35, 'spa-me.tsv': 28, 'tts.tsv': 26, 'gle.tsv': 36, 'slv.tsv': 35, 'ido.tsv': 23, 'zho-s.tsv': 135, 'vie-n.tsv': 174, 'gre.tsv': 20, 'eng-us.tsv': 119, 'fin.tsv': 44, 'pap.tsv': 26, 'tuk.tsv': 49, 'jpn.tsv': 174, 'bel.tsv': 58, 'uzb.tsv': 36, 'dan.tsv': 42, 'ori.tsv': 45, 'ron.tsv': 30, 'bul.tsv': 40, 'bur.tsv': 52, 'lit.tsv': 87, 'dut.tsv': 48, 'fra-qu.tsv': 255, 'eng-uk.tsv': 129, 'hin.tsv': 110, 'isl.tsv': 41, 'arm-e.tsv': 38, 'kor.tsv': 175, 'tur.tsv': 54, 'fas.tsv': 70, 'ger.tsv': 56, 'tam.tsv': 38, 'wel-sw.tsv': 44, 'vie-s.tsv': 172, 'mlt.tsv': 47, 'wel-nw.tsv': 49, 'slo.tsv': 27, 'lat-eccl.tsv': 43, 'snd.tsv': 60, 'tat.tsv': 103, 'alb.tsv': 40, 'hau.tsv': 45, 'pus.tsv': 34, 'tib.tsv': 61, 'sga.tsv': 47, 'heb.tsv': 39, 'hrx.tsv': 27, 'fao.tsv': 42, 'dsb.tsv': 29}
         self.phone_dict = {}
         if not os.path.exists('./' + language + ".tsv"):
             os.system("wget https://raw.githubusercontent.com/lingjzhu/CharsiuG2P/main/dicts/" + language + ".tsv")
         if os.path.exists('./' + language + ".tsv"):
-            f = open("./" + language + ".tsv", "r")
+            f = open("./" + language + ".tsv", "r", encoding="utf-8")
             list_words = f.read().strip().split("\n")
             f.close()
             for word_phone in list_words:
                 w_p = word_phone.split("\t")
                 assert len(w_p) == 2
                 if "," not in w_p[1]:
                     self.phone_dict[w_p[0]] = [w_p[1]]
@@ -121,8 +121,8 @@
             list_phones[i] = segmented_phone
         return " ▁ ".join(list_phones)
 
 
 if __name__ == '__main__':
     a = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
     print(a.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read ."))
-    a.infer_dataset(input_file="input.txt", output_file="output.txt")
+    a.infer_dataset(input_file="input.txt", output_file="output.txt")
```

### Comparing `text2phonemesequence-0.1.3/text2phonemesequence.egg-info/PKG-INFO` & `text2phonemesequence-0.1.4/text2phonemesequence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
```

