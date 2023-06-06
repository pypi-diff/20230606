# Comparing `tmp/html_parsing_tools-0.8.0.tar.gz` & `tmp/html_parsing_tools-0.9.0.tar.gz`

## Comparing `html_parsing_tools-0.8.0.tar` & `html_parsing_tools-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 html_parsing_tools-0.8.0/Cargo.toml
--rwxr-xr-x   0     1001      121      242 2022-09-08 14:48:19.000000 html_parsing_tools-0.8.0/.github/workflows/build-wheels.sh
--rw-r--r--   0     1001      121     2780 2022-09-08 14:48:19.000000 html_parsing_tools-0.8.0/.github/workflows/build.yml
--rw-r--r--   0     1001      121      685 2022-09-08 14:48:19.000000 html_parsing_tools-0.8.0/.gitignore
--rw-r--r--   0     1001      121       21 2022-09-08 14:48:19.000000 html_parsing_tools-0.8.0/README.md
--rw-r--r--   0     1001      121      326 2022-09-08 14:48:19.000000 html_parsing_tools-0.8.0/pyproject.toml
--rw-r--r--   0     1001      121   282572 2022-09-08 14:48:19.000000 html_parsing_tools-0.8.0/run.py
--rw-r--r--   0     1001      121     7746 2022-09-08 14:48:19.000000 html_parsing_tools-0.8.0/src/lib.rs
--rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 html_parsing_tools-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 html_parsing_tools-0.9.0/Cargo.toml
+-rwxr-xr-x   0     1001      121      242 2022-09-12 07:44:14.000000 html_parsing_tools-0.9.0/.github/workflows/build-wheels.sh
+-rw-r--r--   0     1001      121     2780 2022-09-12 07:44:14.000000 html_parsing_tools-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0     1001      121      685 2022-09-12 07:44:14.000000 html_parsing_tools-0.9.0/.gitignore
+-rw-r--r--   0     1001      121       21 2022-09-12 07:44:14.000000 html_parsing_tools-0.9.0/README.md
+-rw-r--r--   0     1001      121      326 2022-09-12 07:44:14.000000 html_parsing_tools-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      121   396014 2022-09-12 07:44:14.000000 html_parsing_tools-0.9.0/run.py
+-rw-r--r--   0     1001      121     6870 2022-09-12 07:44:14.000000 html_parsing_tools-0.9.0/src/lib.rs
+-rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 html_parsing_tools-0.9.0/PKG-INFO
```

### Comparing `html_parsing_tools-0.8.0/.github/workflows/build.yml` & `html_parsing_tools-0.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `html_parsing_tools-0.8.0/.gitignore` & `html_parsing_tools-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `html_parsing_tools-0.8.0/src/lib.rs` & `html_parsing_tools-0.9.0/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use kuchiki::{traits::TendrilSink, NodeRef};
-use pyo3::{descr, prelude::*};
+use pyo3::prelude::*;
+use regex::RegexBuilder;
 
 const REMOVE_TAGS: [&'static str; 27] = [
     // scripts/styles
     "script",
     "style",
     "noscript",
     // COOKIE BANNERS
@@ -33,27 +34,19 @@
     ".testimonial-text",
     ".pwr-testimonial__quote", // hubspot
 ];
 
 const PICK_TAGS: [&'static str; 6] = ["h1", "h2", "h3", "h4", "h5", "h6"];
 
 #[pyfunction]
-fn parse_html(html: String) -> PyResult<String> {
+fn parse_html(html: String, stop_word: String) -> PyResult<String> {
     let mut result: Vec<String> = vec![];
 
     let document = kuchiki::parse_html().one(html);
 
-    // let mut text: Vec<String> = get_text_and_remove(&document, "li")
-    //     .iter()
-    //     .take(30)
-    //     .cloned()
-    //     .collect();
-
-    // result.append(&mut text);
-
     for tag in REMOVE_TAGS {
         remove_tag(&document, tag);
     }
 
     if true {
         remove_tag(&document, "header");
         remove_tag(&document, "nav");
@@ -91,76 +84,58 @@
         .flatten()
         .map(|x| x.to_string())
         .filter(|x| count_words(x.as_str()) < 128)
         .take(30)
         .collect();
 
     result.append(&mut paragraphs);
-    //     let mut text: Vec<String> = get_text_and_remove(&document, "div")
-    //         .iter()
-    //         .take(30)
-    //         .cloned()
-    //         .collect();
-
-    //     for i in text {
-    //         println!("------");
-    //         println!("{}", i);
-    //     }
-    //     // let mut extra = document
-    //     //     .text_contents()
-    //     //     .split("\n")
-    //     //     // .map(|n| n.replace("\t", "").trim().to_string())
-    //     //     // .filter(|n| !n.is_empty() && count_words(n) > 3)
-    //     //     // .map(|n| trim_punctuation(&n))
-    //     //     // .take(10)
-    //     //     .collect::<Vec<String>>();
-
-    //     // result.append(&mut extra);
-    //     // println!("{:?}", text)
-    // }
 
-    // result.sort_by(|a, b| count_words(b).cmp(&count_words(a)));
     result.sort();
     result.dedup();
-    // Ok(result.join("\n"))
 
-    // Description
+    let stop_word_regex = RegexBuilder::new(stop_word.as_str())
+        .case_insensitive(true)
+        .build()
+        .expect("Invalid Regex");
+
+    result = result
+        .iter()
+        .map(|n| {
+            stop_word_regex
+                .replace_all(&n, "")
+                .to_string()
+                .trim()
+                .to_string()
+        })
+        .filter(|n| !n.to_lowercase().contains("cookie") && !n.contains("©") && count_words(n) > 0)
+        .collect();
+
     let description = get_description(&document);
     if description.is_some() {
         result.push(description.clone().unwrap());
     }
-    if result.len() < 30 {
+    if result.len() < 25 {
         if description.is_some() {
             let description = description.unwrap();
             let description = description.as_str();
             let mut i = result.len();
-            while i < 20 {
+            while i < 25 {
                 result.push(description.to_string());
                 i = i + 1;
             }
         }
     }
 
     // Keywords
     let keywords = get_keywords(&document);
     if keywords.is_some() {
         result.push(keywords.unwrap().to_string());
-        // for keyword in keywords.unwrap().split(", ") {
-        //     result.push(keyword.to_string());
-        //     println!("PUSHING KEYWORD: {}", keyword);
-        // }
-        // println!("{:?}")
     }
 
-    Ok(result
-        .iter()
-        .filter(|n| !n.to_lowercase().contains("cookie"))
-        .cloned()
-        .collect::<Vec<String>>()
-        .join("\n"))
+    Ok(result.join("\n"))
 }
 
 fn get_description(document: &NodeRef) -> Option<String> {
     let tag_nodes = document.select("meta").unwrap();
     for tag_node in tag_nodes.collect::<Vec<_>>() {
         let attributes = tag_node.attributes.borrow();
         let name_attribute = attributes.get("name").unwrap_or("");
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

