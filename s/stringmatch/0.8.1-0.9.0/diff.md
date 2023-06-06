# Comparing `tmp/stringmatch-0.8.1-py3-none-any.whl.zip` & `tmp/stringmatch-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 12912 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat      184 b- defN 22-May-01 09:24 stringmatch/__init__.py
+Zip file size: 14313 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat      205 b- defN 22-May-01 18:11 stringmatch/__init__.py
+-rw-rw-rw-  2.0 fat      325 b- defN 22-May-01 17:15 stringmatch/args.py
 -rw-rw-rw-  2.0 fat     1270 b- defN 22-Apr-30 20:04 stringmatch/distance.py
--rw-rw-rw-  2.0 fat    12262 b- defN 22-May-01 09:01 stringmatch/match.py
--rw-rw-rw-  2.0 fat     4005 b- defN 22-May-01 09:00 stringmatch/ratio.py
+-rw-rw-rw-  2.0 fat    13372 b- defN 22-May-01 17:38 stringmatch/match.py
+-rw-rw-rw-  2.0 fat     7413 b- defN 22-May-01 18:06 stringmatch/ratio.py
 -rw-rw-rw-  2.0 fat      797 b- defN 22-May-01 09:11 stringmatch/scorer.py
--rw-rw-rw-  2.0 fat     2060 b- defN 22-Apr-25 09:12 stringmatch/strings.py
+-rw-rw-rw-  2.0 fat     2103 b- defN 22-May-01 17:01 stringmatch/strings.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Apr-04 20:46 tests/__init__.py
 -rw-rw-rw-  2.0 fat      599 b- defN 22-Apr-27 23:12 tests/test_distance.py
--rw-rw-rw-  2.0 fat     3816 b- defN 22-May-01 09:01 tests/test_match.py
--rw-rw-rw-  2.0 fat     2037 b- defN 22-May-01 09:01 tests/test_ratio.py
+-rw-rw-rw-  2.0 fat     4525 b- defN 22-May-01 18:05 tests/test_match.py
+-rw-rw-rw-  2.0 fat     2699 b- defN 22-May-01 18:19 tests/test_ratio.py
 -rw-rw-rw-  2.0 fat      799 b- defN 22-Apr-29 15:15 tests/test_strings.py
--rw-rw-rw-  2.0 fat     1089 b- defN 22-May-01 09:24 stringmatch-0.8.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    10613 b- defN 22-May-01 09:24 stringmatch-0.8.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-May-01 09:24 stringmatch-0.8.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 22-May-01 09:24 stringmatch-0.8.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1255 b- defN 22-May-01 09:24 stringmatch-0.8.1.dist-info/RECORD
-16 files, 40896 bytes uncompressed, 10862 bytes compressed:  73.4%
+-rw-rw-rw-  2.0 fat     1089 b- defN 22-May-01 18:20 stringmatch-0.9.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11410 b- defN 22-May-01 18:20 stringmatch-0.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-May-01 18:20 stringmatch-0.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 22-May-01 18:20 stringmatch-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1330 b- defN 22-May-01 18:20 stringmatch-0.9.0.dist-info/RECORD
+17 files, 48046 bytes uncompressed, 12149 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: stringmatch/__init__.py
 Comment: 
 
+Filename: stringmatch/args.py
+Comment: 
+
 Filename: stringmatch/distance.py
 Comment: 
 
 Filename: stringmatch/match.py
 Comment: 
 
 Filename: stringmatch/ratio.py
@@ -27,23 +30,23 @@
 
 Filename: tests/test_ratio.py
 Comment: 
 
 Filename: tests/test_strings.py
 Comment: 
 
-Filename: stringmatch-0.8.1.dist-info/LICENSE
+Filename: stringmatch-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: stringmatch-0.8.1.dist-info/METADATA
+Filename: stringmatch-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: stringmatch-0.8.1.dist-info/WHEEL
+Filename: stringmatch-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: stringmatch-0.8.1.dist-info/top_level.txt
+Filename: stringmatch-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: stringmatch-0.8.1.dist-info/RECORD
+Filename: stringmatch-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stringmatch/__init__.py

```diff
@@ -1,9 +1,10 @@
 # flake8: noqa
+from .args import *
 from .distance import *
 from .match import *
 from .ratio import *
 from .scorer import *
 from .strings import *
 
 __title__ = "stringmatch"
-__version__ = "0.8.1"
+__version__ = "0.9.0"
```

## stringmatch/match.py

```diff
@@ -1,22 +1,14 @@
-from typing import Optional, TypedDict
+from typing import Optional
 
+from stringmatch.args import KeywordArguments
 from stringmatch.ratio import Ratio
 from stringmatch.scorer import LevenshteinScorer, _Scorer
 
 
-class KeywordArguments(TypedDict, total=False):
-    score: int
-    limit: Optional[int]
-    latinise: bool
-    ignore_case: bool
-    remove_punctuation: bool
-    only_letters: bool
-
-
 class Match:
     """Contains methods for comparing and matching strings."""
 
     def __init__(self, scorer: type[_Scorer] = LevenshteinScorer) -> None:
         """Initialise the Match class with the correct scoring algorithm,
         to be passed along to the Ratio class.
 
@@ -34,14 +26,15 @@
         string2: str,
         *,
         score: int = 70,
         latinise: bool = False,
         ignore_case: bool = False,
         remove_punctuation: bool = False,
         only_letters: bool = False,
+        include_partial: bool = False,
         **_kwargs,
     ) -> bool:
         """Matches two strings, returns True if they are similar enough.
 
         Parameters
         ----------
         string1 : str
@@ -54,39 +47,43 @@
             If special unicode characters should be removed from the strings, by default False.
         ignore_case : bool, optional
             If the strings should be compared ignoring case, by default False.
         remove_punctuation : bool, optional
             If punctuation should be removed from the strings, by default False.
         only_letters : bool, optional
             If the strings should only be compared by their latin letters, by default False.
+        include_partial : bool, optional
+            If partial substring matches should be included, by default False.
 
         Returns
         -------
         bool
             If the strings are similar enough.
         """
         kwargs: KeywordArguments = {
             "latinise": latinise,
             "ignore_case": ignore_case,
             "remove_punctuation": remove_punctuation,
             "only_letters": only_letters,
+            "include_partial": include_partial,
         }
 
         return Ratio(scorer=self.scorer).ratio(string1, string2, **kwargs) >= score
 
     def match_with_ratio(
         self,
         string1: str,
         string2: str,
         *,
         score: int = 70,
         latinise: bool = False,
         ignore_case: bool = False,
         remove_punctuation: bool = False,
         only_letters: bool = False,
+        include_partial: bool = False,
     ) -> tuple[bool, int]:
         """Same as match, but returns the boolean in a tuple, together with the score.
 
         Parameters
         ----------
         string1 : str
             The first string to compare.
@@ -98,26 +95,29 @@
             If special unicode characters should be removed from the strings, by default False.
         ignore_case : bool, optional
             If the strings should be compared ignoring case, by default False.
         remove_punctuation : bool, optional
             If punctuation should be removed from the strings, by default False.
         only_letters : bool, optional
             If the strings should only be compared by their latin letters, by default False.
+        include_partial : bool, optional
+            If partial substring matches should be included, by default False.
 
         Returns
         -------
         tuple[bool, int]
             If the strings are similar and their score.
         """
         kwargs: KeywordArguments = {
             "score": score,
             "latinise": latinise,
             "ignore_case": ignore_case,
             "remove_punctuation": remove_punctuation,
             "only_letters": only_letters,
+            "include_partial": include_partial,
         }
 
         return (
             self.match(string1, string2, **kwargs),
             Ratio(scorer=self.scorer).ratio(string1, string2, **kwargs),
         )
 
@@ -127,14 +127,15 @@
         string_list: list[str],
         *,
         score: int = 70,
         latinise: bool = False,
         ignore_case: bool = False,
         remove_punctuation: bool = False,
         only_letters: bool = False,
+        include_partial: bool = False,
         **_kwargs,
     ) -> Optional[str]:
         """Returns the best match from a list of strings.
 
         Parameters
         ----------
         string : str
@@ -147,26 +148,29 @@
             If special unicode characters should be removed from the strings, by default False.
         ignore_case : bool, optional
             If the strings should be compared ignoring case, by default False.
         remove_punctuation : bool, optional
             If punctuation should be removed from the strings, by default False.
         only_letters : bool, optional
             If the strings should only be compared by their latin letters, by default False.
+        include_partial : bool, optional
+            If partial substring matches should be included, by default False.
 
         Returns
         -------
         Optional[str]
             The best string found, or None if no good match was found.
         """
         kwargs: KeywordArguments = {
             "score": score,
             "latinise": latinise,
             "remove_punctuation": remove_punctuation,
             "ignore_case": ignore_case,
             "only_letters": only_letters,
+            "include_partial": include_partial,
         }
 
         return (
             max(
                 string_list,
                 key=lambda s: Ratio(scorer=self.scorer).ratio(string, s, **kwargs),
             )
@@ -180,14 +184,15 @@
         string_list: list[str],
         *,
         score: int = 70,
         latinise: bool = False,
         ignore_case: bool = False,
         remove_punctuation: bool = False,
         only_letters: bool = False,
+        include_partial: bool = False,
     ) -> Optional[tuple[str, int]]:
         """Same as get_best_match, but returns a tuple with the best match and its score.
 
         Parameters
         ----------
         string : str
             The string to compare.
@@ -199,27 +204,30 @@
             If special unicode characters should be removed from the strings, by default False.
         ignore_case : bool, optional
             If the strings should be compared ignoring case, by default False.
         remove_punctuation : bool, optional
             If punctuation should be removed from the strings, by default False.
         only_letters : bool, optional
             If the strings should only be compared by their latin letters, by default False.
+        include_partial : bool, optional
+            If partial substring matches should be included, by default False.
 
         Returns
         -------
         Optional[tuple[str, int]]
             The best string and its score found, or None if no good match was found.
         """
 
         kwargs: KeywordArguments = {
             "score": score,
             "latinise": latinise,
             "remove_punctuation": remove_punctuation,
             "ignore_case": ignore_case,
             "only_letters": only_letters,
+            "include_partial": include_partial,
         }
 
         match = self.get_best_match(string, string_list, **kwargs)
 
         return (
             (match, Ratio(scorer=self.scorer).ratio(string, match, **kwargs))
             if match
@@ -233,14 +241,15 @@
         *,
         score: int = 70,
         limit: Optional[int] = 5,
         latinise: bool = False,
         ignore_case: bool = False,
         remove_punctuation: bool = False,
         only_letters: bool = False,
+        include_partial: bool = False,
     ) -> list[str]:
         """Matches a string to a list of strings, returns the strings found that are similar.
         If there are more than `limit` matches,
         only the `limit` best matches are returned, sorted by score.
         If no matches are found, returns an empty list.
 
         Parameters
@@ -258,14 +267,16 @@
             If special unicode characters should be removed from the strings, by default False.
         ignore_case : bool, optional
             If the strings should be compared ignoring case, by default False.
         remove_punctuation : bool, optional
             If punctuation should be removed from the strings, by default False.
         only_letters : bool, optional
             If the strings should only be compared by their latin letters, by default False.
+        include_partial : bool, optional
+            If partial substring matches should be included, by default False.
 
         Returns
         -------
         list[str]
             All of the matches found.
         """
         # we return every match found if the limit is 0 or less
@@ -274,14 +285,15 @@
 
         kwargs: KeywordArguments = {
             "score": score,
             "latinise": latinise,
             "remove_punctuation": remove_punctuation,
             "ignore_case": ignore_case,
             "only_letters": only_letters,
+            "include_partial": include_partial,
         }
 
         return sorted(
             [s for s in string_list if self.match(string, s, **kwargs)],
             key=lambda s: Ratio(scorer=self.scorer).ratio(string, s, **kwargs),
             # by default this would sort the list from lowest to highest.
             reverse=True,
@@ -294,14 +306,15 @@
         *,
         score: int = 70,
         limit: Optional[int] = 5,
         latinise: bool = False,
         ignore_case: bool = False,
         remove_punctuation: bool = False,
         only_letters: bool = False,
+        include_partial: bool = False,
     ) -> list[tuple[str, int]]:
         """Same as get_best_matches, but returns a list of tuples with the best matches and their score.
 
         Parameters
         ----------
         string : str
             The string to compare.
@@ -316,27 +329,30 @@
             If special unicode characters should be removed from the strings, by default False.
         ignore_case : bool, optional
             If the strings should be compared ignoring case, by default False.
         remove_punctuation : bool, optional
             If punctuation should be removed from the strings, by default False.
         only_letters : bool, optional
             If the strings should only be compared by their latin letters, by default False.
+        include_partial : bool, optional
+            If partial substring matches should be included, by default False.
 
         Returns
         -------
         list[tuple[str, int]]
             All of the matches found.
         """
         kwargs: KeywordArguments = {
             "score": score,
             "limit": limit,
             "latinise": latinise,
             "remove_punctuation": remove_punctuation,
             "ignore_case": ignore_case,
             "only_letters": only_letters,
+            "include_partial": include_partial,
         }
 
         matches = self.get_best_matches(string, string_list, **kwargs)
 
         return [
             (match, Ratio(scorer=self.scorer).ratio(string, match, **kwargs))
             for match in matches
```

## stringmatch/ratio.py

```diff
@@ -1,7 +1,10 @@
+import Levenshtein  # type: ignore
+
+from stringmatch.args import KeywordArguments
 from stringmatch.scorer import LevenshteinScorer, _Scorer
 from stringmatch.strings import Strings
 
 
 class Ratio:
     """Contains functions for calculating the ratio of similarity between two strings."""
 
@@ -21,14 +24,15 @@
         string1: str,
         string2: str,
         *,
         latinise: bool = False,
         ignore_case: bool = False,
         remove_punctuation: bool = False,
         only_letters: bool = False,
+        include_partial: bool = False,
         **kwargs,
     ) -> int:
         """Returns the similarity score between two strings.
 
         Parameters
         ----------
         string1 : str
@@ -64,14 +68,21 @@
 
         if only_letters:
             string1, string2 = Strings().only_letters(string1), Strings().only_letters(
                 string2
             )
 
         # if either string is empty we wanna return 0
+        if include_partial:
+            return (
+                self.partial_ratio(string1, string2, **kwargs)
+                if string1 and string2
+                else 0
+            )
+
         return (
             round(self.scorer().score(string1, string2) * 100)
             if string1 and string2
             else 0
         )
 
     def ratio_list(
@@ -102,15 +113,97 @@
             If the strings should only be compared by their latin letters, by default False.
 
         Returns
         -------
         list[int]
             The scores between 0 and 100.
         """
-        kwargs = {
+        kwargs: KeywordArguments = {
             "latinise": latinise,
             "ignore_case": ignore_case,
             "remove_punctuation": remove_punctuation,
             "only_letters": only_letters,
         }
 
         return [self.ratio(string, s, **kwargs) for s in string_list]
+
+    def partial_ratio(
+        self,
+        string1: str,
+        string2: str,
+        *,
+        latinise: bool = False,
+        ignore_case: bool = False,
+        remove_punctuation: bool = False,
+        only_letters: bool = False,
+        **_kwargs,
+    ) -> int:
+        """Returns the similarity score between subsections of strings.
+
+        Parameters
+        ----------
+        string1 : str
+            The first string to compare.
+        string2 : str
+            The second string to compare.
+        latinise : bool, optional
+            If special unicode characters should be removed from the strings, by default False.
+        ignore_case : bool, optional
+            If the strings should be compared ignoring case, by default False.
+        remove_punctuation : bool, optional
+            If punctuation should be removed from the strings, by default False.
+        only_letters : bool, optional
+            If the strings should only be compared by their latin letters, by default False.
+
+        Returns
+        -------
+        int
+            The score between 0 and 100.
+        """
+        kwargs: KeywordArguments = {
+            "latinise": latinise,
+            "ignore_case": ignore_case,
+            "remove_punctuation": remove_punctuation,
+            "only_letters": only_letters,
+        }
+
+        scores = []
+
+        if len(string1) >= len(string2):
+            longer_string, shorter_string = string1, string2
+        else:
+            longer_string, shorter_string = string2, string1
+
+        def partialise_score(long_string: str, short_string: str, score: int):
+            """If the two strings are really far away in length, we adjust the similarity score."""
+            if len(long_string) - len(short_string) >= 10:
+                # The default score threshold is 70,
+                # so if the strings are more than 10 characters apart,
+                # this will not show up by default.
+                return round(score * 0.6)
+            elif len(long_string) - len(short_string) >= 5:
+                return round(score * 0.8)
+            return score
+
+        editops = Levenshtein.editops(longer_string, shorter_string)
+
+        blocks = Levenshtein.matching_blocks(editops, longer_string, shorter_string)
+
+        for block in blocks:
+            longer_string_start = max(block[1] - block[0], 0)
+            longer_string_end = longer_string_start + len(shorter_string)
+            longer_string_substring = longer_string[
+                longer_string_start:longer_string_end
+            ]
+
+            scores.append(
+                partialise_score(
+                    longer_string,
+                    shorter_string,
+                    self.ratio(longer_string_substring, shorter_string, **kwargs),
+                )
+            )
+
+        max_partial = max(scores, default=0)
+
+        # we will return the higher of the two scores, just in case
+        return max(max_partial, self.ratio(string1, string2, **kwargs))
```

## stringmatch/strings.py

```diff
@@ -34,27 +34,28 @@
         """
         return "".join(
             c for c in string if c not in "!\"#'()*+,-./:;<=>?[]^_`{|}~’„“»«"
         )
 
     def only_letters(self, string: str) -> str:
         """Removes all non-latin letters from the string.
+        Does also keep numbers.
         A more extreme version of remove_punctuation().
 
         Parameters
         ----------
         string : str
             The string to remove non-latin letters from.
 
         Returns
         -------
         str
             The string with non-latin letters removed.
         """
-        alphabet = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ "
+        alphabet = "1234567890abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ "
         return "".join(c for c in string if c in alphabet)
 
     def ignore_case(self, string: str, lower: bool = True) -> str:
         """Removes case from a string.
 
         Parameters
         ----------
```

## tests/test_match.py

```diff
@@ -25,24 +25,39 @@
 
     assert Match().match("»»ᅳtestᅳ►", "test", only_letters=True) is True
     assert Match().match("»»ᅳtestᅳ►", "test", only_letters=False) is False
 
     assert Match(LevenshteinScorer).match("test", "th test") is True
     assert Match(JaroWinklerScorer).match("test", "th test") is False
 
+    assert Match().match("testbot testmann", "testbot", include_partial=True) is True
+    assert Match().match("testbot testmann", "testbot", include_partial=False) is False
+
 
 def test_match_with_ratio():
     assert Match().match_with_ratio("test", "test") == (True, 100)
     assert Match().match_with_ratio("test", "nope") == (False, 25)
     assert Match().match_with_ratio("searchlib", "srechlib") == (True, 82)
     assert Match(scorer=JaroWinklerScorer).match_with_ratio("test", "th test") == (
         False,
         60,
     )
     assert Match().match_with_ratio("Woosh", "woosh", ignore_case=True) == (True, 100)
+    assert Match().match_with_ratio(
+        "testbot testmann", "testbot", include_partial=True
+    ) == (True, 80)
+    assert Match().match_with_ratio(
+        "testbot testmann", "testbot", include_partial=False
+    ) == (False, 61)
+    assert Match().match_with_ratio(
+        "A string", "A string thats like really really long", include_partial=True
+    ) == (False, 60)
+    assert Match().match_with_ratio(
+        "A string", "A string thats like really really long", include_partial=False
+    ) == (False, 35)
 
 
 def test_get_best_match():
     assert Match().get_best_match("test", ["test", "nope", "tset"]) == "test"
     assert Match().get_best_match("whatever", ["test", "nope", "tset"]) is None
 
     searches = ["stringmat", "strinma", "strings", "mtch", "whatever", "s"]
```

## tests/test_ratio.py

```diff
@@ -44,7 +44,19 @@
     assert Ratio().ratio_list("test", ["th TEST", "hwatever", "*"]) == [18, 33, 0]
     assert Ratio().ratio_list(
         "test", ["th TEST", "hwatever", "*"], ignore_case=True, only_letters=True
     ) == [73, 33, 0]
     assert Ratio(JaroWinklerScorer).ratio_list(
         "test", ["th TEST", "hwatever", "*"], ignore_case=True, only_letters=True
     ) == [60, 58, 0]
+
+
+def test_partial_ratio():
+    assert Ratio().partial_ratio("test124", "93210") == 20
+    assert Ratio().partial_ratio("93210", "test124") == 20
+    assert Ratio().partial_ratio("testbot test", "testbot") == 80
+    assert Ratio().partial_ratio("TESTbot test", "testbot", ignore_case=True) == 80
+    assert Ratio().partial_ratio("TESTbot test", "testbot", ignore_case=False) == 42
+    assert Ratio().partial_ratio("a", "this is a test") == 13
+    assert Ratio().partial_ratio("a test", "this is a test") == 60
+    assert Ratio().partial_ratio("this", "this is a test") == 60
+    assert Ratio().partial_ratio("this is a test", "this this this") == 71
```

## Comparing `stringmatch-0.8.1.dist-info/LICENSE` & `stringmatch-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `stringmatch-0.8.1.dist-info/METADATA` & `stringmatch-0.9.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringmatch
-Version: 0.8.1
+Version: 0.9.0
 Summary: A library to match and compare strings.
 Home-page: https://github.com/atomflunder/stringmatch
 Author: atomflunder
 Author-email: 80397293+atomflunder@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -52,15 +52,15 @@
 
 ## Key Features
 
 This library **matches compares and strings to each other** based mainly on, among others, the [Levenshtein distance](https://en.wikipedia.org/wiki/Levenshtein_distance).  
 What makes stringmatch special compared to other libraries with similar functions:
 
 - 💨 Lightweight, straightforward and easy to use
-- ⚡ Extremely fast, up to 10x faster than comparable libraries
+- ⚡ Very high speed, 2-10x faster while providing better search results
 - 🧰 Allows for highly customisable searches
 - 📚 Lots of utility functions to make your life easier
 - 🌍 Handles special unicode characters, like emojis or characters from other languages, like ジャパニーズ
 
 ## Requirements
 
 - Python 3.9 or later.
@@ -106,21 +106,24 @@
 
 ```python
 from stringmatch import Ratio
 
 ratio = Ratio()
 
 # Getting the ratio between the two strings:
-ratio.ratio("stringmatch", "stringmatch")   # returns 100
-ratio.ratio("stringmatch", "strngmach")     # returns 90
-ratio.ratio("stringmatch", "eh")            # returns 15
+ratio.ratio("stringmatch", "stringmatch")           # returns 100
+ratio.ratio("stringmatch", "strngmach")             # returns 90
+ratio.ratio("stringmatch", "eh")                    # returns 15
 
 # Getting the ratio between the first string and the list of strings at once:
 searches = ["stringmatch", "strngmach", "eh"]
-ratio.ratio_list("stringmatch", searches)   # returns [100, 90, 15]
+ratio.ratio_list("stringmatch", searches)           # returns [100, 90, 15]
+
+# Searching for partial ratios with substrings:
+ratio.partial_ratio("a string", "a string longer")  # returns 80
 ```
 
 ### Matching & Ratios
 
 You can also get both the match and the ratio together in a tuple using these functions:
 
 ```python
@@ -254,25 +257,41 @@
 
 ---
 
 ### `only_letters`
 
 | Type  | Default | Description |
 | ---   | ---     | ---         |
-| Boolean | False | Removes every character that is not in the latin alphabet, a more extreme version of `remove_punctuation`. 
+| Boolean | False | Removes every character that is not a number or in the latin alphabet, a more extreme version of `remove_punctuation`. 
 
 ```python
 # Example:
 
 match("»»ᅳtestᅳ►", "test", only_letters=True)   # returns True
 match("»»ᅳtestᅳ►", "test", only_letters=False)  # returns False
 ```
 
 ---
 
+### `include_partial`
+
+| Type  | Default | Description |
+| ---   | ---     | ---         |
+| Boolean | False | If set to true, also searches for partial substring matches. This may lead to more desirable results but is a bit slower. If the strings are very far apart in length this will return 60% of its value, if they are moderately far apart, 80%.
+
+```python
+# Example:
+
+# returns (True, 60)
+match_with_ratio("A string", "A string thats like really really long", score=60, include_partial=True)
+
+# returns (False, 35)
+match_with_ratio("A string", "A string thats like really really long", score=60, include_partial=False)
+```
+
 ### Scoring Algorithms
 
 You can pass in different scoring algorithms when initializing the `Match()` and `Ratio()` classes.  
 The available options are: [`LevenshteinScorer`](https://en.wikipedia.org/wiki/Levenshtein_distance), [`JaroScorer`](https://en.wikipedia.org/wiki/Jaro–Winkler_distance#Jaro_similarity), [`JaroWinklerScorer`](https://en.wikipedia.org/wiki/Jaro–Winkler_distance#Jaro–Winkler_similarity).   
 
 Click on the links for detailed information about these, but speaking generally the Jaro Scorer will be the fastest, focussing on the characters the strings have in common.  
 The Jaro-Winkler Scorer slightly modified the Jaro Scorer to prioritise characters at the start of the string.
```

## Comparing `stringmatch-0.8.1.dist-info/RECORD` & `stringmatch-0.9.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-stringmatch/__init__.py,sha256=yWyq-k3QofWIzNqRsua4kf8-AkKtUnahHFHcLzuag18,184
+stringmatch/__init__.py,sha256=Ewp9cNKKXUYMet6ODtZyj2AR3qBVu70vVjj1z49byLY,205
+stringmatch/args.py,sha256=qqyY3tUqKBkZjIx6Mq5euB_NA-NMpDlWwvuc3Q-mImQ,325
 stringmatch/distance.py,sha256=8qeNQ_yv1QHhSoQNmmp6VNpqjyx7suS1wgecx9MrDZQ,1270
-stringmatch/match.py,sha256=y4v3oIWUU2lxnn5v7pxIheEgNlkxzwv1-9y1b5Elbdg,12262
-stringmatch/ratio.py,sha256=0-XRM9iqnoR20xmVMIFi8s4Di01uVaX1TT31xYYyQ0E,4005
+stringmatch/match.py,sha256=9lx_Q1A9_Cc-Mkeo-bIPvoOIGeuUv27GvZ1_uDW48bE,13372
+stringmatch/ratio.py,sha256=BUoYGI_4pxGNEepQHZ5fGdl8QqhTWCX41tRdoQxvzLw,7413
 stringmatch/scorer.py,sha256=ccB3INjAa4q44LQ1SwlOmRZYymwwjAKwEjyEAXpG1ew,797
-stringmatch/strings.py,sha256=Dm0Pbq8m1OqPTQw68lPjbeXq-xF6KlIAfy9neYv8GQA,2060
+stringmatch/strings.py,sha256=WDV7CyYBoiyo4DgELW2HCWX5daHh_S2EbIcX52VucCM,2103
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_distance.py,sha256=Er5T16oaOZVqY9vl9PSqKC_hJiztwR6ocDx37s8rY5A,599
-tests/test_match.py,sha256=kqktwL28c6Rpr9fzlWFhQ4iK2RBQVAAqGXwxnnPDpQc,3816
-tests/test_ratio.py,sha256=LTNE5qO0QPPISaBhcJbBrhVX22UIphyS4YOg4dM3Q4g,2037
+tests/test_match.py,sha256=Wn-47HCK6UVy-xhh50U7zupzGTPLfPVOO2YT1il5BfQ,4525
+tests/test_ratio.py,sha256=-m_pCKLlp16Dq0I8zl5x0gA74rmsVrgfFQbFsb1mqww,2699
 tests/test_strings.py,sha256=8SNBfX9lYBvCTnb96qkFTQa3lxVNBC4S0fZuBlBbMkA,799
-stringmatch-0.8.1.dist-info/LICENSE,sha256=_CPd9pTWMQYE3eaG4lzJXaVi7PPeC_-IVdnBZm-szRY,1089
-stringmatch-0.8.1.dist-info/METADATA,sha256=X_So9NuxSQqNshPAD18dppe4mc3v454QxEpEzC4Kftw,10613
-stringmatch-0.8.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-stringmatch-0.8.1.dist-info/top_level.txt,sha256=CWeIhBETOUOEc-oxK3IMrYd7fwwR5MEKY_TxX90_IgU,18
-stringmatch-0.8.1.dist-info/RECORD,,
+stringmatch-0.9.0.dist-info/LICENSE,sha256=_CPd9pTWMQYE3eaG4lzJXaVi7PPeC_-IVdnBZm-szRY,1089
+stringmatch-0.9.0.dist-info/METADATA,sha256=RZw9HQafWh69XMD4OfmzgujP9_PT6s5lqomFOvuo34w,11410
+stringmatch-0.9.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+stringmatch-0.9.0.dist-info/top_level.txt,sha256=CWeIhBETOUOEc-oxK3IMrYd7fwwR5MEKY_TxX90_IgU,18
+stringmatch-0.9.0.dist-info/RECORD,,
```

