# Comparing `tmp/streamlit-code-editor-0.1.1.tar.gz` & `tmp/streamlit-code-editor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-code-editor-0.1.1.tar", last modified: Mon May 29 07:12:15 2023, max compression
+gzip compressed data, was "streamlit-code-editor-0.1.2.tar", last modified: Tue Jun  6 03:44:12 2023, max compression
```

## Comparing `streamlit-code-editor-0.1.1.tar` & `streamlit-code-editor-0.1.2.tar`

### file list

```diff
@@ -1,474 +1,474 @@
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-29 07:12:15.446534 streamlit-code-editor-0.1.1/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1063 2023-03-06 21:07:31.000000 streamlit-code-editor-0.1.1/LICENSE
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       46 2023-03-06 21:07:31.000000 streamlit-code-editor-0.1.1/MANIFEST.in
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      473 2023-05-29 07:12:15.446534 streamlit-code-editor-0.1.1/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1999 2023-05-23 07:31:47.000000 streamlit-code-editor-0.1.1/README.md
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-29 07:12:15.156534 streamlit-code-editor-0.1.1/code_editor/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10233 2023-05-29 07:09:57.000000 streamlit-code-editor-0.1.1/code_editor/__init__.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-29 07:12:15.156534 streamlit-code-editor-0.1.1/code_editor/frontend/
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-29 07:12:15.396534 streamlit-code-editor-0.1.1/code_editor/frontend/build/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10000 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/01843025c65367159319c38263f48d04.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    63816 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0194846970eda6e0cefa23b927f08c6e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2043 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/03325b4ae8405296dacf9ae05e26531f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/03b6f5ed432b1096271448f530f79c3a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3735 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/03c56ebda61883932ac977566b95f407.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      133 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/051172af4df2228c8acf8d04d449ab1d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2387 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0553db997944b413b1a043e8c1ad88f4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3655 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/056489c8a2f20e6c0711dc94adb524a2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8334 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/05ef8a2098a3256a1257757fb8ffb3c2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      136 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/05f2b6d27716f95c75421370d5ee9029.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5477 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/064d4fd688937e22a9cdd76464ecb878.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/07011752aeaa58913a688453ba034167.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/07de343f3a3a86b4c67e887239399197.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3258 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/097741808204e197094057c1344756ca.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3115 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/097d09db97ec6a45524ce80e638c797c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    68713 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/09a310c4ea520a0f5ca740bb2016928b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    14003 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0a08b8e098108d065c74d35d6a9c0cc1.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3540 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0a3f85997947fcc989b003237e68e745.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0a4438ad4f6617ec42fb006d2c3da2ad.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0a84849cb72c84fb6a9b4d831df64ffa.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5162 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0acd14d54fc38bf54dadf85820714821.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0bbdfc82acc2ea66ba14ad4c65193773.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0c14e3f2bbdb026c7dbdecf587f1df62.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0c93349d05810059db73cafb8956afd5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2825 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0cfd541bb9ee002abe8b6e4ab9b86b14.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7107 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0d00ea50a328567db544fad75070d9b8.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0d23aba2dc82c8a5b2c908efb76d1b53.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    63535 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0dd2ab985d396bccde7f956625b7a7a1.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2954 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0e999c67bec4b090ae7d8c251c09c28f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      636 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0ef970d469f39672562d807d8dddc6d4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3962 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0f027df2077c334d2de9666c9b8e9a91.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      124 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/0ffb18fb70c87335edee31a479f58a43.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1046b30afca9b1942dd448bcafff2a95.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6398 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/105ae586c1f6e683a679a348391435bb.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7077 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/10da42883a34b8be117d14de1843a954.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1261ef2b1ed112b8f15686ce9b968b0f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10527 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/12c633400db331c2418b99ce7e315433.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      135 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/144e38358d6dddaaa6bc2602bf312b6a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/14de4e2d134ba188b7779aec466c329e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      602 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/15c1702980a2c8f97c7fd788e1cbd647.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      970 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/15c91c2f86e19c549b22d8334997123a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    12675 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1625a99070bb2f4044b331a709ee1706.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2336 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/167d8367dd297e6ee1f577ac7081a29e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60085 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1779c08ccc8bc6bc9315767f70affd26.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    62625 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/18f127ef6adaaa44a6e2fb644b93b799.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2905 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/195752809a26f7856c92650764084402.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4821 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/19653e310aad2482567d0db1251f8182.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    22341 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/19d85c7ccd7e65ba43dcdaca01957f1c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1abe08b3249335736c0f016631f03702.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    61980 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1ae81db67c5f8d029d08ff85a015fc16.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      135 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1b7b64ca98b308253619de9983f137da.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      136 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1bfb62a79fa8c12cd02be55ec9646ea4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2312 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1ce8e9b4ee3517650a9f68eacb0a4982.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1d48b3a38a76bfc80d5718a91fd4c252.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2604 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1e8926b91c7905dd025d84afe3467eec.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    26727 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1f4a7aa6367d628bc4b7eaa5a1b3ef2a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    22922 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/1f6bd82343ef4bf4958a54bd5d6a6a34.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2011976f347dff043a461b1fbb850994.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4798 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/216872dc6f3f50bb160fec86ff2933bd.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5359 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/21bf585ac7ffbc66eaa5e3a50fa3372a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2307 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/22f9d8d605f141aa5819155ea80239ad.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    63734 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/234717c34d74ef2a6260356e5985f9e0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/23e579d49d8f8206607964d627b336b7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6694 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2426b2433bfd1f69da1242bcb507bd0e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3185 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/24f3bc3586adabc0f36d87606c6f0ddf.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20569 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2596d709aa44f538d4116bc6c3706b06.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2396 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/25e15b02a9d0fb4530fcd4702c869755.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11171 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/266944eca1ef829d6921c984fc9f11cf.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5007 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/26bd9db40544eaf30fbd346a9a52615c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25004 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/26e11038d41222231a867fc86a868df8.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8499 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/277ab522cc834bbc55d4d9b569e1cf94.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    77284 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2942996c35be4edbe85dfe7d53332097.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5893 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2965e68764d57c2f7e3059b1d99286fe.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1234 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2987c57a184004a1f172eef983a30806.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/299f60eb59b60b0f2478f771104213e3.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/29dd0fe96b9fb6bfee8eca138f01394d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19664 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2babf28f53dee57bae31bfcf1e19ea2d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6938 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2c3161ab5238bbc74841c24d33a784a0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    39955 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2cd3c714d326cea24080567e0416aa37.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6706 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2d77b3b44059c1ab560055e72e0e0e3e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10412 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2df3932e0b73558fa3f5e1370ace1bc7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2539 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2e7bea0f731853287ae3d3f88b663ad0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/2f70915bee5cd7267e53e5b969d8eb9a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3020c220cfcf7a97372ed572fae92ec8.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      133 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3068bb1a1d1e69644accc2f3945707f5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   233340 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/30ec25d81ca9193fc10d7e2bdbd08b5d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15639 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3107792026d1bf99e9d93e4c81734de9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    31685 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3151bdbe5041d568fcead4b15f0b9bf0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/31a7c73e2e24faf8299472bf33a95f9f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/31b457d1e9dfba8bffe535ec22ae0d8e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2507 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/31f4c6f3cbf93398c67c2224c9ed624f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/329fd36cc40af8cb92bd6aadc8e719f1.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/32ad89f1eb8d218e23f74b7524372b75.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    63693 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/32fe96b5bb58c52172373da60009c5c5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/330b0c4e3c2fb85009ef6daf099b607b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5526 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/34d9a659619737faf20d7512fe90e81c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5197 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/34ff37a57fce940aba08c378205545e8.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5310 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/351e6fa1b5d88a440eeaed3a31ee3d6f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3072 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/35266861294967f36d3c93156c830447.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3092 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/35a8886ea7469abc2ba058e2ea8e5b95.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/38b2b13102a2cedd38c531675909a2e1.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2960 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/38f0712774de696a14932e7d2b2c0f12.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4375 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/392fc1e7db2be8ae886b8a174ed5f1fb.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    51203 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/39e6e227e4250c67bdc5b753c465915f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    12806 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3a824037bf9d331361ce1d0fb3001a43.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25025 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3ad292ed08ee2cd9c5b12f1a82e7e9bc.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3b0327da890a2fc2c6b1b3b9534306f3.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3b7aa4bec85f22922900b661299b0167.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8996 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3bdbffe97b0f785a7713d2dbdd64801a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2313 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3c2581bce25c91393b40e940c0ddee68.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   510872 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3c9439fce81cf3226f62896ca463e8ca.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      136 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3cbef9c27a8f652b5f90bdb7f50f489f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64673 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3d92e27f401fcf12b5ce2be1171184d9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3db61c65b05bc0206e606f60bfdfbe8d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7944 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3dfcb4e35c8d48b01a2137610d3b3d4f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3235 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/3f17e5dd2b36b8c0285196e1ce2b52e0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      141 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/40064f074583135ca817d3240c2ed429.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3009 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4043efc94814bf9f434f88868211848a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1247 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/405b6974c5f5b32cd98b3c2ad8b032d2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8900 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/40d800cfc16788b79c4c02dd9f72f5f3.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10684 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/40dd2e80df3c9d5f34d5aa05957c5eff.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/416ed2107351fd987a35ec4cb508e7ba.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4288 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/418fe57f4c98d83a556beb0831a2a40d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    45235 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4241093bc1c5f092aa5fb1196ace91ba.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4373 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/425e23055811e88085525e71b2ba6bb2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      733 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4277f1534f71e1c32776b169b57db211.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2386 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4290b269910f9aaf0969012ff1feb13a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      554 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/44b045e0cca5628c408353e416d5e5a4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      631 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/467cd6ba827f7342fb4e2324d342c385.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/46db3c1bd8fd10cf01f4e91271fe51a2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4781f85ddf971e4685e26b481b2d0879.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      451 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/47d6c28f186a0a30422e3122be9eb0a6.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    65165 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/480e0affe9d760337876fd24b22d5809.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/49db9cf6f30a219cf140f7846d87a418.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4ba67801fa5b8763a193b659cdaa39f2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    77308 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4c04cb74c12bf337e225aed9c0521659.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    68592 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4c08c7944ffc5f364e2d3aad643d15d2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4ceef1d773c3bc407cb32a2a9d7a0fb7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4d3535459dc8829878c59eec84dd7d50.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      135 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4d5a5bf22332df156f82d6b223f87e93.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4d60660cfabdb7fe2ffbf84c1b6b61ec.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    41728 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4ecc354d3e5be846f698c09b5f7bd16d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4991 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4f46cd6ed5421a8f2ad7ff1bb804a960.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7864 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4f54ff83938f1add6990f965486bd5e7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4f602915a313027d036689b04e8c264e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2974 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/4f752c49db3b3f0058f3d1ce3c92e25a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1757 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/505ebb9da3344a8eba700ee31f25c4d2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   109964 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/50c2574eba3c27efdab147e2d120b613.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5187c57f286362152187a6e9b5619599.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5215a383dc75b5d5808f4e9dcabc4798.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7271 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/523dd7a7d453c67ba612864b4d5ee8dd.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   230721 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5245243ee21ee7690967ff575a3583e4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8456 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/52cda852c190dfd8f4ad750a60743ef2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    36487 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/53192a5baa72c24e67bcc111e66f1500.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    24095 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/541a90d8c2fddf14455d5e9b20093952.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4239 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/54f19494323aa0dd45457484e4fcac1a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11665 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/552986fe7c45c3d988eb1fd669dc805e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      500 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/55ccafd461c6f27fa9f080361348474a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5659bda221c28b734675cd7b003936cf.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      677 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5791ea1a612a644934c54c26aa18504f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7647 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5a05020fca553a804f36ec3617dc21e7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6058 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5a119ce4c514656cda20e4becc644201.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5b1d2b627fc4ab262f046c3d4df39896.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3749 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5c5a3d84b5476f0d498f272a19da47ab.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5113 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5c6e5f40bd93b386350a1ad4f8fd10fc.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    14603 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5d50defd988518e2183b19ca9f3e055d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6641 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5e134468d8ec013bb90da0cb213db59b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5e299868db8f582a38bfd49191c66452.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/5eb3eb988b6e830c0223e6c98cda5fae.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/601bafbdee8c23b55126c5e1964a3f8e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/60954fd51b67276a98ee24a999c39174.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7772 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/614e7176508881ee3cc61ebf431a5e7e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3124 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/61afad92d1f60d84915d4641b8cac704.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7481 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/61dc75e78fd07c5ae408b57e0d6eff5d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6247279dbb9c17a5fe8670679c2efa79.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6261136900e4499d1bdbe6cfa5d77018.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20109 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/626b9c443d579b4f96ebd7d94856c202.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    48903 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/633c938619cd4e7ffcd0610bf9faa396.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      410 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/637430ad29735bff7f1c612af9eeb1f8.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4492 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/63ec95a52b6af5f003b7d6954380e700.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      997 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/669d075dd410684e566a1bed44c89be7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      133 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/671983dc71a4a790345e0d886a5d552d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5427 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/67ff608d411e5ca5841e431e0b42b181.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3754 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6825f199e6a2631be783316321a0664e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/68fe89dbba54111bf19429b0216a9b5a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    80122 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/69005ce9040e1b234ff47bc0f7f480ff.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4308 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6984ea1ce8669c75833670198d4ac4fa.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4732 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6a3084a2f3fb3ef289d8b7e67acaa791.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    13443 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6ae82b343f9707b605dde454ba106b77.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6b0e6ef64d1b67ffdd756f3756f67a8d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3442 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6b205a0e029cd2e276d40cb484cc1c6c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6b935ecf051eedddc3e5866ad9bc2407.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   320537 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6bb4cdd15a7c12c2c43ebe29f9a2fd79.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    22001 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6c3dee46596728df5294b9d982a67116.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    24474 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6c6d5003d33b3b63f9d02a86896c369d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4586 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6c7757283a3093c691a07f06e54d2dee.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    12766 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6e035acfae5b616647e697164a3c9e13.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    29841 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6e840dd7704b077d11fe8dc11532bbe9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6e8c0ebd5905c7de447cc22128fd5799.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7525 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6f069b25a76dd8bf8d09422bcd193b71.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/6fa983289e62f70d40916e28ac753995.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      846 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/70469d2308d951ebeb703dce5d00e5f8.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    29118 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7109ca6386e492fdf9fce2139e8eb0e3.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    21817 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/716cca9d5723b3b43bfaf1276d5a5af4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    74583 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7262ef4d9dd563dca4ced20a02ca6d38.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5997 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7375ae622e3ad1870b3d1c37e4c50bee.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16643 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/751a9a93854b218b7c75912bf98ff77e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/75b9b4dd40e8e36ea8dd3aaa410a1edd.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/76673952d5d955ad3d06c57fc2ceb1bc.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2927 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/76b477377d31d3d072ab87bed05d66e9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6393 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/77579027d58465f78a596283cdb8014e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5099 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7758bc38709f0c93f37afaa76005849f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/778b4110847987fbfc51b84b0e235e1d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15893 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/77aa2f870c827152a612e4dd01afe6f5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/77be0eaf4d31d3a1e6e16e9905ca80bc.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/77c544b2ce5f734e61e3c3d63ea7f827.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     9172 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7841a6f4b151f35e50e2d24a905f8e13.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8695 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/78e82d00c9656481b608ad6eb38386e7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/78f57b4c6c98f3226c710b994071e12b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   504984 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7c0dcc2eb746acd1fcca7b6c011bc74a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3169 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7cf54dc1ccacfc8c023d864bedc450ec.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    13336 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7d93830b8b6505afe21e3cd9687cf110.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3977 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7dbadd192db68dc1487c0a15e5555288.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2257 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7de52009bba59e6c56e7fe6e8d095c95.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7dee8bceaa3c2e167aa6bbd97badf4d9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7630 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7fd520db96d00e94afd6958a39c9b2d5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1443 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/7fea20b47393446521d73d06ca1a3739.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3094 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8014561b9e8e9468f7016b7eb77be35e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8203 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/804134556c8616a87fb2af9d5d6a2045.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      133 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/809aad7340c184c76c4bf229a697df28.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3963 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/81006885152a3ae4437c23949be6eeb3.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3317 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8145075193478e6eb02630b64ab22fcb.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    23836 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/814f84920751835b4879eb7223d39c13.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3660 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8191766455b80a3708beaaf628e99537.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8205e4c3776c3cd9e6a9268b983342dc.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5018 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/82f57eab37cd8616b4cb20464b521c28.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1355 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/83ba9ea36ef32382d02c70ec66ce5054.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/83d96a9f8c82b870aa08a2a01b667cdc.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3997 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/84ed885d43d5b6ff63adf0d2148fc717.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8555c9e84b1a7796821635d4418bc10b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/85ada81b8ae00c5c02f3e7d78c1c7bab.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/86261f3873c6c41cd7b202869eda8711.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4770 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/86f41b7d629fa664717c13bc0b15f858.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8414 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/877fd48e980be7b27a5be8709dfb4137.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8adc477823e6d755e4bb908723108013.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4181 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8aef2165cf82917e5b7ab3de1078c38c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8b1930520e20f14d59f03846b26ee631.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8b2f56ada6f4e413d1f786360ca56a7a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    38694 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8bba3f3e4551f6f2df07a63ed918832b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    73847 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8da76f935ba41b969ccfa86ffb0204e7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7673 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8dd471b7a7961537ab2f12c396abac0c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      133 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8f7b2f5e6a1fbe5447eb6b48b1b706f0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5775 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/8fe48c25228bc4338703865e3f274c21.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3719 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/90f1cdb42141f0c68a111b2654b8a963.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9118d85d3fc7d5e18701a6fa9abaf7bf.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9157540a213078aaca3efb693fe0431b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      639 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/91ad327423f4967e4f6fd57069a0f2fc.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1590035 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/91f49599a810af1ed0c1a351f14ac99e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/92193223f1119a6d4dc3e4e598cb52cc.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1377 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9283cc89e2d71979a143de94a99c9b25.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16175 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/93dff17e993be4a78aea4e3c17d0916d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1658 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/94bee8dbbe41187a879f001f1816fece.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1234 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/95352557a17c5b8f35836c54bdda82cc.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/95feaecc61642afa67a5da13324b01ba.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    61447 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/964c20018a0ed8d9df087e1e2b7ff42d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3131 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/997640c55a6ded9da7e02f7f9d5a6999.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4213 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/99bdbd9ffac9d3f82203c940cd516275.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7586 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9ad3134af3a1c0fe5ea962734f299608.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4261 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9ad97362888f6a84140fbf080f891fb9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9b0ee69b55e67d310e8165850d26b516.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4105 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9c6191709aeeb06c154b663c97f29c4f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5386 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9cb6191837a0ec577c55784ac62b3a95.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5552 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9cdc503727ada0c759eee4fc85f65b85.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2486 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9e088492749dd72c420b9ea14be309a4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4182 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9e0dd4c9ca60aa42d546eb9af778e61d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   149171 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9e4cd56d3ac46d41b26f9438a9f1f702.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6599 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/9e8b8a51838fdf51d67ede9266370774.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7189 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a01032f2e14eb1760897a74a0e91d8ae.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5151 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a125cc5185ce9a2f8a5473da5389f8fd.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a1883a50fa7e229ceeb72b409367a1b1.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a188d4f92371f4cd2ff24618bfd9cbd1.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    14548 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a18ed57495d8cbc2106ce69d0851c7c4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4219 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a1903a62b39d6a82986555ba4274acf9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    54807 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a2ab4c99a92a2bae95882a1b9299abf4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a2bdeadee19fc235201177a881aa36d3.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1916 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a2cf3aa294c3363984aaedf2ca5b6836.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2074 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a2dcd9175eea1e0d9495592be74f1771.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4185 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a32acfcd6d04e5e4518733feb8bbc3eb.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2832 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a3418e0832b9830794d2882246090e8a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7417 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a3a1f677a611b1f72cdea0893dc26b40.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1033 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a41198acaea59c7a948e4bbcbb27bcc7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1582 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a45002b33f6c20a7aafbc7fe0bda75ac.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a46b2436ca8aefa702a802793beb6284.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a4e596382ff74ce76300b0d13854ee60.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5840 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a4e75a90086b7aa62994a3f43a2d8880.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64849 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a60f2f71ae2b4878222a37fb1c989af1.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    63559 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a798df9c8e782a2529e03b75c6ae5d69.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11612 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a7bf3fc7983a5201967101144ed1af6d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/a88efc791c64200677603e2742bb31cb.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7200 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/aa2062a974236db91d207b6f872a3d42.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/acc1f9afdf512f62de124cd64fc414ec.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    61109 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/ad1b9015520f163ed0bf785c97b7f901.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4143 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/af4259f92460394617ab4beae656cf69.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    28117 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/asset-manifest.json
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3959 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b07b9f998c402374d5ae61f8a5f90834.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16699 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b0860bdbd6a010f08ac65facbc751ec5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b0e6205a0e4e8e8bc47ea70edb1b438a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    32752 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b0f580aa76da5ecb8b8539dfafccaa74.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3568 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b2bfbd167e10a2f1499b6b7173521a32.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3786 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b2ed29ed03abbb90d4e6460f78cc49e6.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b2fbe444b88a758f45f7a1c4beb686d9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b322f95f1e5bebb4a5b18f9f2b458273.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3012 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b34e7646857d3e4810190d77cdd47c72.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2333 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b3c15b07ee65a11d3a4dc03a3fd4f520.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b3c8fac34d63a9fe758b737a2560c911.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2715 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b3d2e28a5c9c6eca4522120beaa8bd1b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7032 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b41a93a0b42dca8629be07ee243f9444.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      841 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b46dcbc460a77e0a225a0d717b2c5c44.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b53b20cabeea14ae8ad8a4d19f8da928.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b543f2132fa98d7f3fbb4cc21b85798d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3822 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b5bddfc3bcf40896e10bcf747f168e3d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b6bbe63b8bee85fdb29d83a7d6eb6b13.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b727aec9e66a495d4d5b3ad745bc4aa5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2406 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b76c4ef3ef560839cc53abdc90dc0635.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b7fd910a3ae745f5f74c065a25cbd640.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4203 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b7fe810ac8ab02489be6d2a267e335f3.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3673 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b93a7e92b54afaf7df25ce1f71abde96.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/b9bded89e6e24aabbc3352ed5af3706d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4185 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/bab5d1e072fae9427c7a92aa03c6c994.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3832 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/bd82757a59fac35f7323d8c129dd177f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    80457 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/bee967a08d8144813e1eca995e850db7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/bf24eb9b91f882cafcfa6a7e8e3c56b1.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2043 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/bf5dc4fb83ec42e1506dd557a39d8b51.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   197459 2023-05-29 07:11:00.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/bootstrap.min.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3296 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c0155133f8b91c3fd72585e1bbd0663f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      137 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c0eebaec55db3f9dfe8e8e6f1eeef982.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6976 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c2a9533633141e25796248a15b084f4f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15787 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c3d4155a442737116676e355d101e60b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c3ec73ec5450fb4cac984fc867dd54eb.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    46420 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c4e1812b01dcf14f11e8b553051eb7e3.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6680 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c5981946a499b7a8e118460de13b2a3c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      760 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c62509c4188fb5f0ac84cb18db4953a9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    34092 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c6ab877a9e42f3dd8f1ae60490334b0d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2383 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c6bf611b1170b31a97c85c46bc02edc5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20656 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c72d5cb0802acdf0c3cf889feb4cf08f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      803 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c79bebdedaeeb0e84627cfb705eba4c0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c7a7a718c85bba6144b2a580a717ff0e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4124 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c7b1c44013938dc49548d0e944959160.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c8465177ba476b68337fa2cf3743db20.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    28553 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c897e5b4c4aab18a0b0b92b21af4995d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15961 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c9328914dfba7d21d76188d3f7b1b2c0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      125 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/c98e74fc97b04fe8bf43dcdff549afcf.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/caa320a365f2d3616ca721bcc981f1a4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    12869 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/cae868cec072275a187aecc552b58c3b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   500428 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/cbfc81eb8025b48dbb4d584913f9424a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/cce112a2a78f215dbf8026fccd277412.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    22938 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/cd3f176a354e18ffa533a7db5a995db6.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60782 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d008fa7e4114f9d35c2d38675944fc5a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1008 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d02def03076d1780451dac3f58ffdde5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20500 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d2013da8217d405f944a65fe2a0d978d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2040 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d2b376303879422f058fe3b5dc9efdf2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    22649 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d2f1ec1eaa573f91172c62b58a0b0925.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d313df4eab72b5bcdd6d64098167a8c0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3898 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d3a04193dbcd949adc1a9333911c8601.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8316 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d4fbb5d2bcf90560d95e04ec9183b645.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4620 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d529068f6631dc56ed25b229d6256c61.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7963 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d5a37181e369dece490ec467a51b874c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6722 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d72af7d954398c5d9d9697968cdbf4c0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5981 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d7cf2ff2cfce5a8766c462d361b9bf8b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1566 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d8d2a50e7d00d6926a59e7f0c605dd94.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d9081202d161fd0a700316a8cb076f31.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d917b953089af88146c9d372fae04338.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17516 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/d92b3534728e5aa0fc51e894cf7b2d71.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/daa5b3009f7d0a190395dbe21d9ff89b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16089 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/db0489d6a9164cb0e09fc2b1a9c7f35b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/db1f36e971cc752e709cc9ccf3e78970.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6601 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/db500c5379116eafe008d7d7b66a4220.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6266 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/db988bf23763dc4b5bf25c93368bfcd3.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    71747 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/dce67fe447e34f4ffe4578c95206e567.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    23611 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/dd843e6eabf91ddb48f8417ed259cabf.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     9007 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/deccaca19352980d272cc86040fad45d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/defb40a0b82472531a9639d25cfdf1b6.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      135 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e003d9c6f76f9b2bcad8bbe72f5aaf4b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2431 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e028d3d2b9861b82f6820743b8189e16.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4948 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e049c3b6ea982f67acd227871680de7a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e1f3357b2b8d16b4875692dfbdded291.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   206288 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e204504ae663c061f07092b2b2cdf870.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17687 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e28ada780a72301df4bafb9c8b1d1ae6.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8212 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e29701a1f6ad24a12a2fbd8ad82a3cb7.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3263 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e2b840449781aa7657b2c797d410f894.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3368 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e30f8c7030c064f949e786be09f3095b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e3dcf6e782f47a8ae315d506571e57bf.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    47515 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e43fb8d8bc1621bccce93b7f7600df07.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    39905 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e463a1cf5e818c9a3c704b57999a27d5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2582 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e48b7b3ffe6b1614919441fb9c25dd4c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3253 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e4bd34571302089306a2275b73ccabc9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20682 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e5a091ce9f3db02f839cb36dd4cb83ed.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     9506 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e5f086d57eaffac1bf402e308c87b0a8.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    21510 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e6e5c919b2f511e045d3d259a8f12b6c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7585 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e856077b2667951810c754aa5696ffbb.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8170 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e88b7914c8a46336d80ee6870837aed0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4038 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e8e531b8b51d386a66e3881b36ee0add.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3331 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e8fa0688c54573296b67b7caec859462.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4560 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/e94ac678b756a9a3190694b95a9430a5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2937 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/ea2db5427faaf15731c301cbc942d8fa.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/eab387dee57def86c245a3d71365a614.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1373 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/eb041468daa482e56a0b8a48c3f40f7b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6015 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/eb5e0358db5309c4df6f1b0480690e31.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10019 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/ebb3dae889b7e4d6240c4941bc4e177b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2986 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/ec1870c6f2f5cb02a22ae24aa56f2d2d.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2479 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/ed2e5b8cfcf5dc3e279f34f7b6122525.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/ed467b0f1e10c0e98c4c75fa0b449b4a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    43646 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/edbd54e9b9231be01dfe502d6155a746.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4907 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/edc0ebd7ed759f2ed2082fe0d236dc0e.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/ef68d1d2222a45a86eb6065b77b0368c.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20687 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/ef8e937a4924aa7a7ec3f1c1856f68a3.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/ef939a6546ba280ff6df495187b1fea9.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/efae0fc6f092182099e02328bc39980f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8775 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f178b8178993c239247db2175a0f5292.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f20880859755c71283bcb010ad3c71ef.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f340f898873d57bbfffeb51bdab50f49.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1587 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f38fddaec7640c79658fc641e6ff3bb0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4725 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f3ae2ab1bc71db88c5afcd7c90916489.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3020 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f42a62d762c34d1ca7c418ea25726655.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3566 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f4ba3bed98e8325a3a723ec3f40069e2.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f4dfd0c9ebf076ba045b2e2b3c5490c8.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f542ac16a923e0535afa0f2e0949d36a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    24273 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f56295fa3830defe6dff72219c94f323.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    66975 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f5634886f504b67a4fb52ba3eda0bb91.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f56d32e1f2b28367fb9708336457c4a6.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f574c6ed6a178b4374b7c570ab2fce5f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3326 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f621ec46ae2b56dbbfc7208b961baeec.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8171 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f6bb72adbd9c04c120ec80cfe244cea0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f76ee9c8abfdd96fb9d70116d40435d5.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f7f74eec10f0f40d32b9a3c4283f92e0.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   111566 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f93f5974d7b6905236730a2b4567fb80.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11292 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f9a561c620224bfab5a21efecbfbe15b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2863 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f9bf7dc81acb8807eaf82f4e307266d4.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20419 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/f9e12872a8aca64e07a75735e4404d2f.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8440 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/fae5d14d159a50986dc91ba7623cdfef.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17530 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/fafe7b33e520b9ab327172152fcbeac1.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    62759 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/fc2c1d48fae7bb55b997e42e6186360b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4859 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/fcbe79021ef2b8e24eeac38f2ebd1e6b.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19734 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/fe0c814b919ab5701ce9e9adce6c1a5a.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15540 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/fe10bf958ca84418c6af95259c7b4260.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1080 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/fe64d890e7fa0c0beae6f2e7a96a7ede.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/ff8b71b1bce6feb81065d8340e07dfeb.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2095 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/index.html
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-29 07:12:15.156534 streamlit-code-editor-0.1.1/code_editor/frontend/build/static/
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-29 07:12:15.446534 streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1543458 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4045 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js.LICENSE.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  5081405 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18526 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/main.571a6b52.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    56863 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/main.571a6b52.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1590 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/runtime-main.ad47a231.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8369 2023-05-29 07:11:32.000000 streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/runtime-main.ad47a231.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-05-29 07:12:15.446534 streamlit-code-editor-0.1.1/setup.cfg
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      844 2023-05-29 07:09:44.000000 streamlit-code-editor-0.1.1/setup.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-05-29 07:12:15.446534 streamlit-code-editor-0.1.1/streamlit_code_editor.egg-info/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      473 2023-05-29 07:12:15.000000 streamlit-code-editor-0.1.1/streamlit_code_editor.egg-info/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    28890 2023-05-29 07:12:15.000000 streamlit-code-editor-0.1.1/streamlit_code_editor.egg-info/SOURCES.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-05-29 07:12:15.000000 streamlit-code-editor-0.1.1/streamlit_code_editor.egg-info/dependency_links.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-05-29 07:12:15.000000 streamlit-code-editor-0.1.1/streamlit_code_editor.egg-info/requires.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       12 2023-05-29 07:12:15.000000 streamlit-code-editor-0.1.1/streamlit_code_editor.egg-info/top_level.txt
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-06 03:44:12.841729 streamlit-code-editor-0.1.2/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1063 2023-03-06 21:07:31.000000 streamlit-code-editor-0.1.2/LICENSE
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       46 2023-03-06 21:07:31.000000 streamlit-code-editor-0.1.2/MANIFEST.in
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      473 2023-06-06 03:44:12.841729 streamlit-code-editor-0.1.2/PKG-INFO
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1999 2023-05-23 07:31:47.000000 streamlit-code-editor-0.1.2/README.md
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-06 03:44:12.681729 streamlit-code-editor-0.1.2/code_editor/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10233 2023-05-29 07:09:57.000000 streamlit-code-editor-0.1.2/code_editor/__init__.py
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-06 03:44:12.671728 streamlit-code-editor-0.1.2/code_editor/frontend/
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-06 03:44:12.811729 streamlit-code-editor-0.1.2/code_editor/frontend/build/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10000 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/01843025c65367159319c38263f48d04.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    63816 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0194846970eda6e0cefa23b927f08c6e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2043 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/03325b4ae8405296dacf9ae05e26531f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/03b6f5ed432b1096271448f530f79c3a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3735 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/03c56ebda61883932ac977566b95f407.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      133 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/051172af4df2228c8acf8d04d449ab1d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2387 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0553db997944b413b1a043e8c1ad88f4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3655 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/056489c8a2f20e6c0711dc94adb524a2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8334 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/05ef8a2098a3256a1257757fb8ffb3c2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      136 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/05f2b6d27716f95c75421370d5ee9029.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5477 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/064d4fd688937e22a9cdd76464ecb878.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/07011752aeaa58913a688453ba034167.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/07de343f3a3a86b4c67e887239399197.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3258 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/097741808204e197094057c1344756ca.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3115 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/097d09db97ec6a45524ce80e638c797c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    68713 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/09a310c4ea520a0f5ca740bb2016928b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    14003 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0a08b8e098108d065c74d35d6a9c0cc1.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3540 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0a3f85997947fcc989b003237e68e745.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0a4438ad4f6617ec42fb006d2c3da2ad.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0a84849cb72c84fb6a9b4d831df64ffa.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5162 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0acd14d54fc38bf54dadf85820714821.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0bbdfc82acc2ea66ba14ad4c65193773.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0c14e3f2bbdb026c7dbdecf587f1df62.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0c93349d05810059db73cafb8956afd5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2825 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0cfd541bb9ee002abe8b6e4ab9b86b14.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7107 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0d00ea50a328567db544fad75070d9b8.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0d23aba2dc82c8a5b2c908efb76d1b53.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    63535 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0dd2ab985d396bccde7f956625b7a7a1.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2954 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0e999c67bec4b090ae7d8c251c09c28f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      636 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0ef970d469f39672562d807d8dddc6d4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3962 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0f027df2077c334d2de9666c9b8e9a91.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      124 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/0ffb18fb70c87335edee31a479f58a43.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1046b30afca9b1942dd448bcafff2a95.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6398 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/105ae586c1f6e683a679a348391435bb.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7077 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/10da42883a34b8be117d14de1843a954.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1261ef2b1ed112b8f15686ce9b968b0f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10527 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/12c633400db331c2418b99ce7e315433.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      135 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/144e38358d6dddaaa6bc2602bf312b6a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/14de4e2d134ba188b7779aec466c329e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      602 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/15c1702980a2c8f97c7fd788e1cbd647.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      970 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/15c91c2f86e19c549b22d8334997123a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    12675 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1625a99070bb2f4044b331a709ee1706.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2336 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/167d8367dd297e6ee1f577ac7081a29e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60085 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1779c08ccc8bc6bc9315767f70affd26.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    62625 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/18f127ef6adaaa44a6e2fb644b93b799.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2905 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/195752809a26f7856c92650764084402.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4821 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/19653e310aad2482567d0db1251f8182.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    22341 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/19d85c7ccd7e65ba43dcdaca01957f1c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1abe08b3249335736c0f016631f03702.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    61980 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1ae81db67c5f8d029d08ff85a015fc16.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      135 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1b7b64ca98b308253619de9983f137da.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      136 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1bfb62a79fa8c12cd02be55ec9646ea4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2312 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1ce8e9b4ee3517650a9f68eacb0a4982.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1d48b3a38a76bfc80d5718a91fd4c252.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2604 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1e8926b91c7905dd025d84afe3467eec.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    26727 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1f4a7aa6367d628bc4b7eaa5a1b3ef2a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    22922 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/1f6bd82343ef4bf4958a54bd5d6a6a34.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2011976f347dff043a461b1fbb850994.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4798 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/216872dc6f3f50bb160fec86ff2933bd.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5359 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/21bf585ac7ffbc66eaa5e3a50fa3372a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2307 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/22f9d8d605f141aa5819155ea80239ad.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    63734 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/234717c34d74ef2a6260356e5985f9e0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/23e579d49d8f8206607964d627b336b7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6694 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2426b2433bfd1f69da1242bcb507bd0e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3185 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/24f3bc3586adabc0f36d87606c6f0ddf.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20569 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2596d709aa44f538d4116bc6c3706b06.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2396 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/25e15b02a9d0fb4530fcd4702c869755.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11171 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/266944eca1ef829d6921c984fc9f11cf.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5007 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/26bd9db40544eaf30fbd346a9a52615c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25004 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/26e11038d41222231a867fc86a868df8.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8499 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/277ab522cc834bbc55d4d9b569e1cf94.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    77284 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2942996c35be4edbe85dfe7d53332097.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5893 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2965e68764d57c2f7e3059b1d99286fe.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1234 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2987c57a184004a1f172eef983a30806.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/299f60eb59b60b0f2478f771104213e3.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/29dd0fe96b9fb6bfee8eca138f01394d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19664 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2babf28f53dee57bae31bfcf1e19ea2d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6938 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2c3161ab5238bbc74841c24d33a784a0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    39955 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2cd3c714d326cea24080567e0416aa37.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6706 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2d77b3b44059c1ab560055e72e0e0e3e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10412 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2df3932e0b73558fa3f5e1370ace1bc7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2539 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2e7bea0f731853287ae3d3f88b663ad0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/2f70915bee5cd7267e53e5b969d8eb9a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3020c220cfcf7a97372ed572fae92ec8.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      133 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3068bb1a1d1e69644accc2f3945707f5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   233340 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/30ec25d81ca9193fc10d7e2bdbd08b5d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15639 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3107792026d1bf99e9d93e4c81734de9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    31685 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3151bdbe5041d568fcead4b15f0b9bf0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/31a7c73e2e24faf8299472bf33a95f9f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/31b457d1e9dfba8bffe535ec22ae0d8e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2507 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/31f4c6f3cbf93398c67c2224c9ed624f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/329fd36cc40af8cb92bd6aadc8e719f1.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/32ad89f1eb8d218e23f74b7524372b75.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    63693 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/32fe96b5bb58c52172373da60009c5c5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/330b0c4e3c2fb85009ef6daf099b607b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5526 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/34d9a659619737faf20d7512fe90e81c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5197 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/34ff37a57fce940aba08c378205545e8.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5310 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/351e6fa1b5d88a440eeaed3a31ee3d6f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3072 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/35266861294967f36d3c93156c830447.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3092 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/35a8886ea7469abc2ba058e2ea8e5b95.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/38b2b13102a2cedd38c531675909a2e1.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2960 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/38f0712774de696a14932e7d2b2c0f12.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4375 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/392fc1e7db2be8ae886b8a174ed5f1fb.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    51203 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/39e6e227e4250c67bdc5b753c465915f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    12806 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3a824037bf9d331361ce1d0fb3001a43.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25025 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3ad292ed08ee2cd9c5b12f1a82e7e9bc.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3b0327da890a2fc2c6b1b3b9534306f3.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3b7aa4bec85f22922900b661299b0167.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8996 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3bdbffe97b0f785a7713d2dbdd64801a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2313 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3c2581bce25c91393b40e940c0ddee68.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   510872 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3c9439fce81cf3226f62896ca463e8ca.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      136 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3cbef9c27a8f652b5f90bdb7f50f489f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64673 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3d92e27f401fcf12b5ce2be1171184d9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3db61c65b05bc0206e606f60bfdfbe8d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7944 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3dfcb4e35c8d48b01a2137610d3b3d4f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3235 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/3f17e5dd2b36b8c0285196e1ce2b52e0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      141 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/40064f074583135ca817d3240c2ed429.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3009 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4043efc94814bf9f434f88868211848a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1247 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/405b6974c5f5b32cd98b3c2ad8b032d2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8900 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/40d800cfc16788b79c4c02dd9f72f5f3.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10684 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/40dd2e80df3c9d5f34d5aa05957c5eff.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/416ed2107351fd987a35ec4cb508e7ba.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4288 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/418fe57f4c98d83a556beb0831a2a40d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    45235 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4241093bc1c5f092aa5fb1196ace91ba.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4373 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/425e23055811e88085525e71b2ba6bb2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      733 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4277f1534f71e1c32776b169b57db211.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2386 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4290b269910f9aaf0969012ff1feb13a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      554 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/44b045e0cca5628c408353e416d5e5a4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      631 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/467cd6ba827f7342fb4e2324d342c385.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/46db3c1bd8fd10cf01f4e91271fe51a2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4781f85ddf971e4685e26b481b2d0879.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      451 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/47d6c28f186a0a30422e3122be9eb0a6.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    65165 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/480e0affe9d760337876fd24b22d5809.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/49db9cf6f30a219cf140f7846d87a418.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4ba67801fa5b8763a193b659cdaa39f2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    77308 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4c04cb74c12bf337e225aed9c0521659.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    68592 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4c08c7944ffc5f364e2d3aad643d15d2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4ceef1d773c3bc407cb32a2a9d7a0fb7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4d3535459dc8829878c59eec84dd7d50.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      135 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4d5a5bf22332df156f82d6b223f87e93.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4d60660cfabdb7fe2ffbf84c1b6b61ec.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    41728 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4ecc354d3e5be846f698c09b5f7bd16d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4991 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4f46cd6ed5421a8f2ad7ff1bb804a960.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7864 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4f54ff83938f1add6990f965486bd5e7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4f602915a313027d036689b04e8c264e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2974 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/4f752c49db3b3f0058f3d1ce3c92e25a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1757 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/505ebb9da3344a8eba700ee31f25c4d2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   109964 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/50c2574eba3c27efdab147e2d120b613.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5187c57f286362152187a6e9b5619599.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5215a383dc75b5d5808f4e9dcabc4798.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7271 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/523dd7a7d453c67ba612864b4d5ee8dd.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   230721 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5245243ee21ee7690967ff575a3583e4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8456 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/52cda852c190dfd8f4ad750a60743ef2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    36487 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/53192a5baa72c24e67bcc111e66f1500.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    24095 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/541a90d8c2fddf14455d5e9b20093952.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4239 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/54f19494323aa0dd45457484e4fcac1a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11665 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/552986fe7c45c3d988eb1fd669dc805e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      500 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/55ccafd461c6f27fa9f080361348474a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5659bda221c28b734675cd7b003936cf.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      677 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5791ea1a612a644934c54c26aa18504f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7647 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5a05020fca553a804f36ec3617dc21e7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6058 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5a119ce4c514656cda20e4becc644201.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5b1d2b627fc4ab262f046c3d4df39896.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3749 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5c5a3d84b5476f0d498f272a19da47ab.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5113 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5c6e5f40bd93b386350a1ad4f8fd10fc.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    14603 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5d50defd988518e2183b19ca9f3e055d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6641 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5e134468d8ec013bb90da0cb213db59b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5e299868db8f582a38bfd49191c66452.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/5eb3eb988b6e830c0223e6c98cda5fae.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/601bafbdee8c23b55126c5e1964a3f8e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/60954fd51b67276a98ee24a999c39174.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7772 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/614e7176508881ee3cc61ebf431a5e7e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3124 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/61afad92d1f60d84915d4641b8cac704.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7481 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/61dc75e78fd07c5ae408b57e0d6eff5d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6247279dbb9c17a5fe8670679c2efa79.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6261136900e4499d1bdbe6cfa5d77018.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20109 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/626b9c443d579b4f96ebd7d94856c202.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    48903 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/633c938619cd4e7ffcd0610bf9faa396.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      410 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/637430ad29735bff7f1c612af9eeb1f8.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4492 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/63ec95a52b6af5f003b7d6954380e700.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      997 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/669d075dd410684e566a1bed44c89be7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      133 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/671983dc71a4a790345e0d886a5d552d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5427 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/67ff608d411e5ca5841e431e0b42b181.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3754 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6825f199e6a2631be783316321a0664e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/68fe89dbba54111bf19429b0216a9b5a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    80122 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/69005ce9040e1b234ff47bc0f7f480ff.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4308 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6984ea1ce8669c75833670198d4ac4fa.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4732 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6a3084a2f3fb3ef289d8b7e67acaa791.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    13443 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6ae82b343f9707b605dde454ba106b77.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6b0e6ef64d1b67ffdd756f3756f67a8d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3442 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6b205a0e029cd2e276d40cb484cc1c6c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6b935ecf051eedddc3e5866ad9bc2407.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   320537 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6bb4cdd15a7c12c2c43ebe29f9a2fd79.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    22001 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6c3dee46596728df5294b9d982a67116.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    24474 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6c6d5003d33b3b63f9d02a86896c369d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4586 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6c7757283a3093c691a07f06e54d2dee.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    12766 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6e035acfae5b616647e697164a3c9e13.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    29841 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6e840dd7704b077d11fe8dc11532bbe9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6e8c0ebd5905c7de447cc22128fd5799.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7525 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6f069b25a76dd8bf8d09422bcd193b71.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/6fa983289e62f70d40916e28ac753995.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      846 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/70469d2308d951ebeb703dce5d00e5f8.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    29118 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7109ca6386e492fdf9fce2139e8eb0e3.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    21817 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/716cca9d5723b3b43bfaf1276d5a5af4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    74583 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7262ef4d9dd563dca4ced20a02ca6d38.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5997 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7375ae622e3ad1870b3d1c37e4c50bee.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16643 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/751a9a93854b218b7c75912bf98ff77e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/75b9b4dd40e8e36ea8dd3aaa410a1edd.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/76673952d5d955ad3d06c57fc2ceb1bc.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2927 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/76b477377d31d3d072ab87bed05d66e9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6393 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/77579027d58465f78a596283cdb8014e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5099 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7758bc38709f0c93f37afaa76005849f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/778b4110847987fbfc51b84b0e235e1d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15893 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/77aa2f870c827152a612e4dd01afe6f5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/77be0eaf4d31d3a1e6e16e9905ca80bc.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/77c544b2ce5f734e61e3c3d63ea7f827.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     9172 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7841a6f4b151f35e50e2d24a905f8e13.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8695 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/78e82d00c9656481b608ad6eb38386e7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/78f57b4c6c98f3226c710b994071e12b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   504984 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7c0dcc2eb746acd1fcca7b6c011bc74a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3169 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7cf54dc1ccacfc8c023d864bedc450ec.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    13336 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7d93830b8b6505afe21e3cd9687cf110.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3977 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7dbadd192db68dc1487c0a15e5555288.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2257 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7de52009bba59e6c56e7fe6e8d095c95.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7dee8bceaa3c2e167aa6bbd97badf4d9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7630 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7fd520db96d00e94afd6958a39c9b2d5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1443 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/7fea20b47393446521d73d06ca1a3739.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3094 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8014561b9e8e9468f7016b7eb77be35e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8203 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/804134556c8616a87fb2af9d5d6a2045.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      133 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/809aad7340c184c76c4bf229a697df28.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3963 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/81006885152a3ae4437c23949be6eeb3.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3317 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8145075193478e6eb02630b64ab22fcb.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    23836 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/814f84920751835b4879eb7223d39c13.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3660 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8191766455b80a3708beaaf628e99537.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8205e4c3776c3cd9e6a9268b983342dc.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5018 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/82f57eab37cd8616b4cb20464b521c28.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1355 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/83ba9ea36ef32382d02c70ec66ce5054.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/83d96a9f8c82b870aa08a2a01b667cdc.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3997 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/84ed885d43d5b6ff63adf0d2148fc717.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8555c9e84b1a7796821635d4418bc10b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/85ada81b8ae00c5c02f3e7d78c1c7bab.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/86261f3873c6c41cd7b202869eda8711.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4770 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/86f41b7d629fa664717c13bc0b15f858.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8414 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/877fd48e980be7b27a5be8709dfb4137.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8adc477823e6d755e4bb908723108013.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4181 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8aef2165cf82917e5b7ab3de1078c38c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8b1930520e20f14d59f03846b26ee631.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8b2f56ada6f4e413d1f786360ca56a7a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    38694 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8bba3f3e4551f6f2df07a63ed918832b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    73847 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8da76f935ba41b969ccfa86ffb0204e7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7673 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8dd471b7a7961537ab2f12c396abac0c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      133 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8f7b2f5e6a1fbe5447eb6b48b1b706f0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5775 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/8fe48c25228bc4338703865e3f274c21.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3719 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/90f1cdb42141f0c68a111b2654b8a963.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9118d85d3fc7d5e18701a6fa9abaf7bf.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9157540a213078aaca3efb693fe0431b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      639 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/91ad327423f4967e4f6fd57069a0f2fc.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1590035 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/91f49599a810af1ed0c1a351f14ac99e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/92193223f1119a6d4dc3e4e598cb52cc.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1377 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9283cc89e2d71979a143de94a99c9b25.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16175 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/93dff17e993be4a78aea4e3c17d0916d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1658 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/94bee8dbbe41187a879f001f1816fece.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1234 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/95352557a17c5b8f35836c54bdda82cc.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/95feaecc61642afa67a5da13324b01ba.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    61447 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/964c20018a0ed8d9df087e1e2b7ff42d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3131 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/997640c55a6ded9da7e02f7f9d5a6999.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4213 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/99bdbd9ffac9d3f82203c940cd516275.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7586 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9ad3134af3a1c0fe5ea962734f299608.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4261 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9ad97362888f6a84140fbf080f891fb9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9b0ee69b55e67d310e8165850d26b516.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4105 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9c6191709aeeb06c154b663c97f29c4f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5386 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9cb6191837a0ec577c55784ac62b3a95.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5552 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9cdc503727ada0c759eee4fc85f65b85.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2486 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9e088492749dd72c420b9ea14be309a4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4182 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9e0dd4c9ca60aa42d546eb9af778e61d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   149171 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9e4cd56d3ac46d41b26f9438a9f1f702.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6599 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/9e8b8a51838fdf51d67ede9266370774.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7189 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a01032f2e14eb1760897a74a0e91d8ae.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5151 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a125cc5185ce9a2f8a5473da5389f8fd.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a1883a50fa7e229ceeb72b409367a1b1.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a188d4f92371f4cd2ff24618bfd9cbd1.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    14548 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a18ed57495d8cbc2106ce69d0851c7c4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4219 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a1903a62b39d6a82986555ba4274acf9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    54807 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a2ab4c99a92a2bae95882a1b9299abf4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a2bdeadee19fc235201177a881aa36d3.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1916 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a2cf3aa294c3363984aaedf2ca5b6836.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2074 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a2dcd9175eea1e0d9495592be74f1771.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4185 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a32acfcd6d04e5e4518733feb8bbc3eb.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2832 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a3418e0832b9830794d2882246090e8a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7417 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a3a1f677a611b1f72cdea0893dc26b40.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1033 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a41198acaea59c7a948e4bbcbb27bcc7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1582 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a45002b33f6c20a7aafbc7fe0bda75ac.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a46b2436ca8aefa702a802793beb6284.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a4e596382ff74ce76300b0d13854ee60.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5840 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a4e75a90086b7aa62994a3f43a2d8880.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64849 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a60f2f71ae2b4878222a37fb1c989af1.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    63559 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a798df9c8e782a2529e03b75c6ae5d69.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11612 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a7bf3fc7983a5201967101144ed1af6d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/a88efc791c64200677603e2742bb31cb.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7200 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/aa2062a974236db91d207b6f872a3d42.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/acc1f9afdf512f62de124cd64fc414ec.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    61109 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/ad1b9015520f163ed0bf785c97b7f901.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4143 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/af4259f92460394617ab4beae656cf69.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    28117 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/asset-manifest.json
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3959 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b07b9f998c402374d5ae61f8a5f90834.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16699 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b0860bdbd6a010f08ac65facbc751ec5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b0e6205a0e4e8e8bc47ea70edb1b438a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    32752 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b0f580aa76da5ecb8b8539dfafccaa74.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3568 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b2bfbd167e10a2f1499b6b7173521a32.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3786 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b2ed29ed03abbb90d4e6460f78cc49e6.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b2fbe444b88a758f45f7a1c4beb686d9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b322f95f1e5bebb4a5b18f9f2b458273.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3012 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b34e7646857d3e4810190d77cdd47c72.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2333 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b3c15b07ee65a11d3a4dc03a3fd4f520.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b3c8fac34d63a9fe758b737a2560c911.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2715 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b3d2e28a5c9c6eca4522120beaa8bd1b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7032 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b41a93a0b42dca8629be07ee243f9444.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      841 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b46dcbc460a77e0a225a0d717b2c5c44.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b53b20cabeea14ae8ad8a4d19f8da928.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b543f2132fa98d7f3fbb4cc21b85798d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3822 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b5bddfc3bcf40896e10bcf747f168e3d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b6bbe63b8bee85fdb29d83a7d6eb6b13.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b727aec9e66a495d4d5b3ad745bc4aa5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2406 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b76c4ef3ef560839cc53abdc90dc0635.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b7fd910a3ae745f5f74c065a25cbd640.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4203 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b7fe810ac8ab02489be6d2a267e335f3.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3673 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b93a7e92b54afaf7df25ce1f71abde96.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/b9bded89e6e24aabbc3352ed5af3706d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4185 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/bab5d1e072fae9427c7a92aa03c6c994.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3832 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/bd82757a59fac35f7323d8c129dd177f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    80457 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/bee967a08d8144813e1eca995e850db7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/bf24eb9b91f882cafcfa6a7e8e3c56b1.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2043 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/bf5dc4fb83ec42e1506dd557a39d8b51.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   197459 2023-06-06 03:43:10.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/bootstrap.min.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3296 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c0155133f8b91c3fd72585e1bbd0663f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      137 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c0eebaec55db3f9dfe8e8e6f1eeef982.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6976 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c2a9533633141e25796248a15b084f4f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15787 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c3d4155a442737116676e355d101e60b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c3ec73ec5450fb4cac984fc867dd54eb.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    46420 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c4e1812b01dcf14f11e8b553051eb7e3.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6680 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c5981946a499b7a8e118460de13b2a3c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      760 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c62509c4188fb5f0ac84cb18db4953a9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    34092 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c6ab877a9e42f3dd8f1ae60490334b0d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2383 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c6bf611b1170b31a97c85c46bc02edc5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20656 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c72d5cb0802acdf0c3cf889feb4cf08f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      803 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c79bebdedaeeb0e84627cfb705eba4c0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c7a7a718c85bba6144b2a580a717ff0e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4124 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c7b1c44013938dc49548d0e944959160.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c8465177ba476b68337fa2cf3743db20.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    28553 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c897e5b4c4aab18a0b0b92b21af4995d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15961 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c9328914dfba7d21d76188d3f7b1b2c0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      125 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/c98e74fc97b04fe8bf43dcdff549afcf.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/caa320a365f2d3616ca721bcc981f1a4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    12869 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/cae868cec072275a187aecc552b58c3b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   500428 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/cbfc81eb8025b48dbb4d584913f9424a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/cce112a2a78f215dbf8026fccd277412.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    22938 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/cd3f176a354e18ffa533a7db5a995db6.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60782 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d008fa7e4114f9d35c2d38675944fc5a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1008 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d02def03076d1780451dac3f58ffdde5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20500 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d2013da8217d405f944a65fe2a0d978d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2040 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d2b376303879422f058fe3b5dc9efdf2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    22649 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d2f1ec1eaa573f91172c62b58a0b0925.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d313df4eab72b5bcdd6d64098167a8c0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3898 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d3a04193dbcd949adc1a9333911c8601.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8316 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d4fbb5d2bcf90560d95e04ec9183b645.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4620 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d529068f6631dc56ed25b229d6256c61.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7963 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d5a37181e369dece490ec467a51b874c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6722 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d72af7d954398c5d9d9697968cdbf4c0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5981 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d7cf2ff2cfce5a8766c462d361b9bf8b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1566 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d8d2a50e7d00d6926a59e7f0c605dd94.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d9081202d161fd0a700316a8cb076f31.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d917b953089af88146c9d372fae04338.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17516 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/d92b3534728e5aa0fc51e894cf7b2d71.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/daa5b3009f7d0a190395dbe21d9ff89b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16089 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/db0489d6a9164cb0e09fc2b1a9c7f35b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/db1f36e971cc752e709cc9ccf3e78970.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6601 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/db500c5379116eafe008d7d7b66a4220.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6266 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/db988bf23763dc4b5bf25c93368bfcd3.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    71747 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/dce67fe447e34f4ffe4578c95206e567.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    23611 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/dd843e6eabf91ddb48f8417ed259cabf.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     9007 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/deccaca19352980d272cc86040fad45d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      134 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/defb40a0b82472531a9639d25cfdf1b6.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      135 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e003d9c6f76f9b2bcad8bbe72f5aaf4b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2431 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e028d3d2b9861b82f6820743b8189e16.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4948 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e049c3b6ea982f67acd227871680de7a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e1f3357b2b8d16b4875692dfbdded291.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   206288 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e204504ae663c061f07092b2b2cdf870.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17687 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e28ada780a72301df4bafb9c8b1d1ae6.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8212 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e29701a1f6ad24a12a2fbd8ad82a3cb7.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3263 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e2b840449781aa7657b2c797d410f894.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3368 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e30f8c7030c064f949e786be09f3095b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e3dcf6e782f47a8ae315d506571e57bf.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    47515 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e43fb8d8bc1621bccce93b7f7600df07.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    39905 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e463a1cf5e818c9a3c704b57999a27d5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2582 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e48b7b3ffe6b1614919441fb9c25dd4c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3253 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e4bd34571302089306a2275b73ccabc9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20682 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e5a091ce9f3db02f839cb36dd4cb83ed.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     9506 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e5f086d57eaffac1bf402e308c87b0a8.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    21510 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e6e5c919b2f511e045d3d259a8f12b6c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7585 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e856077b2667951810c754aa5696ffbb.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8170 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e88b7914c8a46336d80ee6870837aed0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4038 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e8e531b8b51d386a66e3881b36ee0add.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3331 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e8fa0688c54573296b67b7caec859462.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4560 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/e94ac678b756a9a3190694b95a9430a5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2937 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/ea2db5427faaf15731c301cbc942d8fa.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/eab387dee57def86c245a3d71365a614.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1373 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/eb041468daa482e56a0b8a48c3f40f7b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6015 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/eb5e0358db5309c4df6f1b0480690e31.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10019 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/ebb3dae889b7e4d6240c4941bc4e177b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2986 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/ec1870c6f2f5cb02a22ae24aa56f2d2d.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2479 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/ed2e5b8cfcf5dc3e279f34f7b6122525.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/ed467b0f1e10c0e98c4c75fa0b449b4a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    43646 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/edbd54e9b9231be01dfe502d6155a746.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4907 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/edc0ebd7ed759f2ed2082fe0d236dc0e.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/ef68d1d2222a45a86eb6065b77b0368c.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20687 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/ef8e937a4924aa7a7ec3f1c1856f68a3.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/ef939a6546ba280ff6df495187b1fea9.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      130 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/efae0fc6f092182099e02328bc39980f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8775 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f178b8178993c239247db2175a0f5292.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f20880859755c71283bcb010ad3c71ef.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f340f898873d57bbfffeb51bdab50f49.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1587 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f38fddaec7640c79658fc641e6ff3bb0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4725 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f3ae2ab1bc71db88c5afcd7c90916489.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3020 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f42a62d762c34d1ca7c418ea25726655.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3566 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f4ba3bed98e8325a3a723ec3f40069e2.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f4dfd0c9ebf076ba045b2e2b3c5490c8.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      128 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f542ac16a923e0535afa0f2e0949d36a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    24273 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f56295fa3830defe6dff72219c94f323.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    66975 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f5634886f504b67a4fb52ba3eda0bb91.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      132 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f56d32e1f2b28367fb9708336457c4a6.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f574c6ed6a178b4374b7c570ab2fce5f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3326 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f621ec46ae2b56dbbfc7208b961baeec.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8171 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f6bb72adbd9c04c120ec80cfe244cea0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      127 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f76ee9c8abfdd96fb9d70116d40435d5.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      129 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f7f74eec10f0f40d32b9a3c4283f92e0.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   111566 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f93f5974d7b6905236730a2b4567fb80.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11292 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f9a561c620224bfab5a21efecbfbe15b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2863 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f9bf7dc81acb8807eaf82f4e307266d4.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20419 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/f9e12872a8aca64e07a75735e4404d2f.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8440 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/fae5d14d159a50986dc91ba7623cdfef.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17530 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/fafe7b33e520b9ab327172152fcbeac1.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    62759 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/fc2c1d48fae7bb55b997e42e6186360b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4859 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/fcbe79021ef2b8e24eeac38f2ebd1e6b.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19734 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/fe0c814b919ab5701ce9e9adce6c1a5a.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15540 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/fe10bf958ca84418c6af95259c7b4260.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1080 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/fe64d890e7fa0c0beae6f2e7a96a7ede.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      131 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/ff8b71b1bce6feb81065d8340e07dfeb.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2095 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/index.html
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-06 03:44:12.671728 streamlit-code-editor-0.1.2/code_editor/frontend/build/static/
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-06 03:44:12.831729 streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1543458 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4045 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js.LICENSE.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  5081405 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18537 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/main.028f53cc.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    56882 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/main.028f53cc.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1590 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/runtime-main.ad47a231.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     8369 2023-06-06 03:43:37.000000 streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/runtime-main.ad47a231.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-06-06 03:44:12.841729 streamlit-code-editor-0.1.2/setup.cfg
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      844 2023-06-06 03:42:55.000000 streamlit-code-editor-0.1.2/setup.py
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-06 03:44:12.841729 streamlit-code-editor-0.1.2/streamlit_code_editor.egg-info/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      473 2023-06-06 03:44:12.000000 streamlit-code-editor-0.1.2/streamlit_code_editor.egg-info/PKG-INFO
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    28890 2023-06-06 03:44:12.000000 streamlit-code-editor-0.1.2/streamlit_code_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-06-06 03:44:12.000000 streamlit-code-editor-0.1.2/streamlit_code_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-06-06 03:44:12.000000 streamlit-code-editor-0.1.2/streamlit_code_editor.egg-info/requires.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       12 2023-06-06 03:44:12.000000 streamlit-code-editor-0.1.2/streamlit_code_editor.egg-info/top_level.txt
```

### Comparing `streamlit-code-editor-0.1.1/LICENSE` & `streamlit-code-editor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/README.md` & `streamlit-code-editor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/__init__.py` & `streamlit-code-editor-0.1.2/code_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/01843025c65367159319c38263f48d04.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/01843025c65367159319c38263f48d04.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0194846970eda6e0cefa23b927f08c6e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0194846970eda6e0cefa23b927f08c6e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/03325b4ae8405296dacf9ae05e26531f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/03325b4ae8405296dacf9ae05e26531f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/03c56ebda61883932ac977566b95f407.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/03c56ebda61883932ac977566b95f407.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0553db997944b413b1a043e8c1ad88f4.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0553db997944b413b1a043e8c1ad88f4.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/056489c8a2f20e6c0711dc94adb524a2.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/056489c8a2f20e6c0711dc94adb524a2.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/05ef8a2098a3256a1257757fb8ffb3c2.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/05ef8a2098a3256a1257757fb8ffb3c2.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/064d4fd688937e22a9cdd76464ecb878.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/064d4fd688937e22a9cdd76464ecb878.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/097741808204e197094057c1344756ca.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/097741808204e197094057c1344756ca.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/097d09db97ec6a45524ce80e638c797c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/097d09db97ec6a45524ce80e638c797c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/09a310c4ea520a0f5ca740bb2016928b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/09a310c4ea520a0f5ca740bb2016928b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0a08b8e098108d065c74d35d6a9c0cc1.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0a08b8e098108d065c74d35d6a9c0cc1.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0a3f85997947fcc989b003237e68e745.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0a3f85997947fcc989b003237e68e745.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0acd14d54fc38bf54dadf85820714821.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0acd14d54fc38bf54dadf85820714821.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0cfd541bb9ee002abe8b6e4ab9b86b14.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0cfd541bb9ee002abe8b6e4ab9b86b14.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0d00ea50a328567db544fad75070d9b8.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0d00ea50a328567db544fad75070d9b8.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0dd2ab985d396bccde7f956625b7a7a1.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0dd2ab985d396bccde7f956625b7a7a1.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0e999c67bec4b090ae7d8c251c09c28f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0e999c67bec4b090ae7d8c251c09c28f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0ef970d469f39672562d807d8dddc6d4.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0ef970d469f39672562d807d8dddc6d4.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/0f027df2077c334d2de9666c9b8e9a91.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/0f027df2077c334d2de9666c9b8e9a91.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/105ae586c1f6e683a679a348391435bb.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/105ae586c1f6e683a679a348391435bb.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/10da42883a34b8be117d14de1843a954.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/10da42883a34b8be117d14de1843a954.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/12c633400db331c2418b99ce7e315433.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/12c633400db331c2418b99ce7e315433.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/15c1702980a2c8f97c7fd788e1cbd647.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/15c1702980a2c8f97c7fd788e1cbd647.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/15c91c2f86e19c549b22d8334997123a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/15c91c2f86e19c549b22d8334997123a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/1625a99070bb2f4044b331a709ee1706.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/1625a99070bb2f4044b331a709ee1706.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/167d8367dd297e6ee1f577ac7081a29e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/167d8367dd297e6ee1f577ac7081a29e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/1779c08ccc8bc6bc9315767f70affd26.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/1779c08ccc8bc6bc9315767f70affd26.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/18f127ef6adaaa44a6e2fb644b93b799.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/18f127ef6adaaa44a6e2fb644b93b799.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/195752809a26f7856c92650764084402.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/195752809a26f7856c92650764084402.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/19653e310aad2482567d0db1251f8182.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/19653e310aad2482567d0db1251f8182.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/19d85c7ccd7e65ba43dcdaca01957f1c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/19d85c7ccd7e65ba43dcdaca01957f1c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/1ae81db67c5f8d029d08ff85a015fc16.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/1ae81db67c5f8d029d08ff85a015fc16.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/1ce8e9b4ee3517650a9f68eacb0a4982.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/1ce8e9b4ee3517650a9f68eacb0a4982.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/1e8926b91c7905dd025d84afe3467eec.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/1e8926b91c7905dd025d84afe3467eec.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/1f4a7aa6367d628bc4b7eaa5a1b3ef2a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/1f4a7aa6367d628bc4b7eaa5a1b3ef2a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/1f6bd82343ef4bf4958a54bd5d6a6a34.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/1f6bd82343ef4bf4958a54bd5d6a6a34.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/216872dc6f3f50bb160fec86ff2933bd.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/216872dc6f3f50bb160fec86ff2933bd.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/21bf585ac7ffbc66eaa5e3a50fa3372a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/21bf585ac7ffbc66eaa5e3a50fa3372a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/22f9d8d605f141aa5819155ea80239ad.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/22f9d8d605f141aa5819155ea80239ad.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/234717c34d74ef2a6260356e5985f9e0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/234717c34d74ef2a6260356e5985f9e0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2426b2433bfd1f69da1242bcb507bd0e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2426b2433bfd1f69da1242bcb507bd0e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/24f3bc3586adabc0f36d87606c6f0ddf.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/24f3bc3586adabc0f36d87606c6f0ddf.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2596d709aa44f538d4116bc6c3706b06.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2596d709aa44f538d4116bc6c3706b06.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/25e15b02a9d0fb4530fcd4702c869755.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/25e15b02a9d0fb4530fcd4702c869755.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/266944eca1ef829d6921c984fc9f11cf.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/266944eca1ef829d6921c984fc9f11cf.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/26bd9db40544eaf30fbd346a9a52615c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/26bd9db40544eaf30fbd346a9a52615c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/26e11038d41222231a867fc86a868df8.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/26e11038d41222231a867fc86a868df8.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/277ab522cc834bbc55d4d9b569e1cf94.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/277ab522cc834bbc55d4d9b569e1cf94.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2942996c35be4edbe85dfe7d53332097.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2942996c35be4edbe85dfe7d53332097.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2965e68764d57c2f7e3059b1d99286fe.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2965e68764d57c2f7e3059b1d99286fe.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2987c57a184004a1f172eef983a30806.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2987c57a184004a1f172eef983a30806.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2babf28f53dee57bae31bfcf1e19ea2d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2babf28f53dee57bae31bfcf1e19ea2d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2c3161ab5238bbc74841c24d33a784a0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2c3161ab5238bbc74841c24d33a784a0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2cd3c714d326cea24080567e0416aa37.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2cd3c714d326cea24080567e0416aa37.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2d77b3b44059c1ab560055e72e0e0e3e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2d77b3b44059c1ab560055e72e0e0e3e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2df3932e0b73558fa3f5e1370ace1bc7.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2df3932e0b73558fa3f5e1370ace1bc7.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/2e7bea0f731853287ae3d3f88b663ad0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/2e7bea0f731853287ae3d3f88b663ad0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/30ec25d81ca9193fc10d7e2bdbd08b5d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/30ec25d81ca9193fc10d7e2bdbd08b5d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/3107792026d1bf99e9d93e4c81734de9.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/3107792026d1bf99e9d93e4c81734de9.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/3151bdbe5041d568fcead4b15f0b9bf0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/3151bdbe5041d568fcead4b15f0b9bf0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/31f4c6f3cbf93398c67c2224c9ed624f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/31f4c6f3cbf93398c67c2224c9ed624f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/32fe96b5bb58c52172373da60009c5c5.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/32fe96b5bb58c52172373da60009c5c5.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/34d9a659619737faf20d7512fe90e81c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/34d9a659619737faf20d7512fe90e81c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/34ff37a57fce940aba08c378205545e8.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/34ff37a57fce940aba08c378205545e8.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/351e6fa1b5d88a440eeaed3a31ee3d6f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/351e6fa1b5d88a440eeaed3a31ee3d6f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/35266861294967f36d3c93156c830447.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/35266861294967f36d3c93156c830447.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/35a8886ea7469abc2ba058e2ea8e5b95.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/35a8886ea7469abc2ba058e2ea8e5b95.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/38f0712774de696a14932e7d2b2c0f12.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/38f0712774de696a14932e7d2b2c0f12.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/392fc1e7db2be8ae886b8a174ed5f1fb.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/392fc1e7db2be8ae886b8a174ed5f1fb.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/39e6e227e4250c67bdc5b753c465915f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/39e6e227e4250c67bdc5b753c465915f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/3a824037bf9d331361ce1d0fb3001a43.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/3a824037bf9d331361ce1d0fb3001a43.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/3ad292ed08ee2cd9c5b12f1a82e7e9bc.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/3ad292ed08ee2cd9c5b12f1a82e7e9bc.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/3bdbffe97b0f785a7713d2dbdd64801a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/3bdbffe97b0f785a7713d2dbdd64801a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/3c2581bce25c91393b40e940c0ddee68.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/3c2581bce25c91393b40e940c0ddee68.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/3c9439fce81cf3226f62896ca463e8ca.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/3c9439fce81cf3226f62896ca463e8ca.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/3d92e27f401fcf12b5ce2be1171184d9.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/3d92e27f401fcf12b5ce2be1171184d9.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/3dfcb4e35c8d48b01a2137610d3b3d4f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/3dfcb4e35c8d48b01a2137610d3b3d4f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/3f17e5dd2b36b8c0285196e1ce2b52e0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/3f17e5dd2b36b8c0285196e1ce2b52e0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/4043efc94814bf9f434f88868211848a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/4043efc94814bf9f434f88868211848a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/405b6974c5f5b32cd98b3c2ad8b032d2.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/405b6974c5f5b32cd98b3c2ad8b032d2.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/40d800cfc16788b79c4c02dd9f72f5f3.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/40d800cfc16788b79c4c02dd9f72f5f3.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/40dd2e80df3c9d5f34d5aa05957c5eff.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/40dd2e80df3c9d5f34d5aa05957c5eff.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/418fe57f4c98d83a556beb0831a2a40d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/418fe57f4c98d83a556beb0831a2a40d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/4241093bc1c5f092aa5fb1196ace91ba.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/4241093bc1c5f092aa5fb1196ace91ba.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/425e23055811e88085525e71b2ba6bb2.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/425e23055811e88085525e71b2ba6bb2.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/4277f1534f71e1c32776b169b57db211.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/4277f1534f71e1c32776b169b57db211.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/4290b269910f9aaf0969012ff1feb13a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/4290b269910f9aaf0969012ff1feb13a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/44b045e0cca5628c408353e416d5e5a4.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/44b045e0cca5628c408353e416d5e5a4.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/467cd6ba827f7342fb4e2324d342c385.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/467cd6ba827f7342fb4e2324d342c385.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/480e0affe9d760337876fd24b22d5809.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/480e0affe9d760337876fd24b22d5809.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/4c04cb74c12bf337e225aed9c0521659.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/4c04cb74c12bf337e225aed9c0521659.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/4c08c7944ffc5f364e2d3aad643d15d2.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/4c08c7944ffc5f364e2d3aad643d15d2.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/4ecc354d3e5be846f698c09b5f7bd16d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/4ecc354d3e5be846f698c09b5f7bd16d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/4f46cd6ed5421a8f2ad7ff1bb804a960.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/4f46cd6ed5421a8f2ad7ff1bb804a960.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/4f54ff83938f1add6990f965486bd5e7.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/4f54ff83938f1add6990f965486bd5e7.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/4f752c49db3b3f0058f3d1ce3c92e25a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/4f752c49db3b3f0058f3d1ce3c92e25a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/505ebb9da3344a8eba700ee31f25c4d2.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/505ebb9da3344a8eba700ee31f25c4d2.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/50c2574eba3c27efdab147e2d120b613.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/50c2574eba3c27efdab147e2d120b613.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/523dd7a7d453c67ba612864b4d5ee8dd.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/523dd7a7d453c67ba612864b4d5ee8dd.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/5245243ee21ee7690967ff575a3583e4.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/5245243ee21ee7690967ff575a3583e4.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/52cda852c190dfd8f4ad750a60743ef2.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/52cda852c190dfd8f4ad750a60743ef2.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/53192a5baa72c24e67bcc111e66f1500.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/53192a5baa72c24e67bcc111e66f1500.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/541a90d8c2fddf14455d5e9b20093952.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/541a90d8c2fddf14455d5e9b20093952.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/54f19494323aa0dd45457484e4fcac1a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/54f19494323aa0dd45457484e4fcac1a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/552986fe7c45c3d988eb1fd669dc805e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/552986fe7c45c3d988eb1fd669dc805e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/5791ea1a612a644934c54c26aa18504f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/5791ea1a612a644934c54c26aa18504f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/5a05020fca553a804f36ec3617dc21e7.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/5a05020fca553a804f36ec3617dc21e7.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/5a119ce4c514656cda20e4becc644201.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/5a119ce4c514656cda20e4becc644201.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/5c5a3d84b5476f0d498f272a19da47ab.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/5c5a3d84b5476f0d498f272a19da47ab.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/5c6e5f40bd93b386350a1ad4f8fd10fc.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/5c6e5f40bd93b386350a1ad4f8fd10fc.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/5d50defd988518e2183b19ca9f3e055d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/5d50defd988518e2183b19ca9f3e055d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/5e134468d8ec013bb90da0cb213db59b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/5e134468d8ec013bb90da0cb213db59b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/614e7176508881ee3cc61ebf431a5e7e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/614e7176508881ee3cc61ebf431a5e7e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/61afad92d1f60d84915d4641b8cac704.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/61afad92d1f60d84915d4641b8cac704.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/61dc75e78fd07c5ae408b57e0d6eff5d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/61dc75e78fd07c5ae408b57e0d6eff5d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/626b9c443d579b4f96ebd7d94856c202.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/626b9c443d579b4f96ebd7d94856c202.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/633c938619cd4e7ffcd0610bf9faa396.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/633c938619cd4e7ffcd0610bf9faa396.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/63ec95a52b6af5f003b7d6954380e700.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/63ec95a52b6af5f003b7d6954380e700.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/669d075dd410684e566a1bed44c89be7.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/669d075dd410684e566a1bed44c89be7.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/67ff608d411e5ca5841e431e0b42b181.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/67ff608d411e5ca5841e431e0b42b181.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6825f199e6a2631be783316321a0664e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6825f199e6a2631be783316321a0664e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/69005ce9040e1b234ff47bc0f7f480ff.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/69005ce9040e1b234ff47bc0f7f480ff.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6984ea1ce8669c75833670198d4ac4fa.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6984ea1ce8669c75833670198d4ac4fa.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6a3084a2f3fb3ef289d8b7e67acaa791.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6a3084a2f3fb3ef289d8b7e67acaa791.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6ae82b343f9707b605dde454ba106b77.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6ae82b343f9707b605dde454ba106b77.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6b205a0e029cd2e276d40cb484cc1c6c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6b205a0e029cd2e276d40cb484cc1c6c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6bb4cdd15a7c12c2c43ebe29f9a2fd79.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6bb4cdd15a7c12c2c43ebe29f9a2fd79.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6c3dee46596728df5294b9d982a67116.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6c3dee46596728df5294b9d982a67116.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6c6d5003d33b3b63f9d02a86896c369d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6c6d5003d33b3b63f9d02a86896c369d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6c7757283a3093c691a07f06e54d2dee.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6c7757283a3093c691a07f06e54d2dee.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6e035acfae5b616647e697164a3c9e13.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6e035acfae5b616647e697164a3c9e13.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6e840dd7704b077d11fe8dc11532bbe9.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6e840dd7704b077d11fe8dc11532bbe9.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/6f069b25a76dd8bf8d09422bcd193b71.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/6f069b25a76dd8bf8d09422bcd193b71.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/70469d2308d951ebeb703dce5d00e5f8.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/70469d2308d951ebeb703dce5d00e5f8.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7109ca6386e492fdf9fce2139e8eb0e3.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7109ca6386e492fdf9fce2139e8eb0e3.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/716cca9d5723b3b43bfaf1276d5a5af4.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/716cca9d5723b3b43bfaf1276d5a5af4.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7262ef4d9dd563dca4ced20a02ca6d38.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7262ef4d9dd563dca4ced20a02ca6d38.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7375ae622e3ad1870b3d1c37e4c50bee.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7375ae622e3ad1870b3d1c37e4c50bee.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/751a9a93854b218b7c75912bf98ff77e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/751a9a93854b218b7c75912bf98ff77e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/76b477377d31d3d072ab87bed05d66e9.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/76b477377d31d3d072ab87bed05d66e9.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/77579027d58465f78a596283cdb8014e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/77579027d58465f78a596283cdb8014e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7758bc38709f0c93f37afaa76005849f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7758bc38709f0c93f37afaa76005849f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/77aa2f870c827152a612e4dd01afe6f5.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/77aa2f870c827152a612e4dd01afe6f5.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7841a6f4b151f35e50e2d24a905f8e13.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7841a6f4b151f35e50e2d24a905f8e13.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/78e82d00c9656481b608ad6eb38386e7.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/78e82d00c9656481b608ad6eb38386e7.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7c0dcc2eb746acd1fcca7b6c011bc74a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7c0dcc2eb746acd1fcca7b6c011bc74a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7cf54dc1ccacfc8c023d864bedc450ec.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7cf54dc1ccacfc8c023d864bedc450ec.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7d93830b8b6505afe21e3cd9687cf110.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7d93830b8b6505afe21e3cd9687cf110.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7dbadd192db68dc1487c0a15e5555288.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7dbadd192db68dc1487c0a15e5555288.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7de52009bba59e6c56e7fe6e8d095c95.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7de52009bba59e6c56e7fe6e8d095c95.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7fd520db96d00e94afd6958a39c9b2d5.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7fd520db96d00e94afd6958a39c9b2d5.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/7fea20b47393446521d73d06ca1a3739.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/7fea20b47393446521d73d06ca1a3739.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/8014561b9e8e9468f7016b7eb77be35e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/8014561b9e8e9468f7016b7eb77be35e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/804134556c8616a87fb2af9d5d6a2045.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/804134556c8616a87fb2af9d5d6a2045.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/81006885152a3ae4437c23949be6eeb3.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/81006885152a3ae4437c23949be6eeb3.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/8145075193478e6eb02630b64ab22fcb.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/8145075193478e6eb02630b64ab22fcb.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/814f84920751835b4879eb7223d39c13.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/814f84920751835b4879eb7223d39c13.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/8191766455b80a3708beaaf628e99537.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/8191766455b80a3708beaaf628e99537.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/82f57eab37cd8616b4cb20464b521c28.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/82f57eab37cd8616b4cb20464b521c28.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/83ba9ea36ef32382d02c70ec66ce5054.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/83ba9ea36ef32382d02c70ec66ce5054.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/84ed885d43d5b6ff63adf0d2148fc717.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/84ed885d43d5b6ff63adf0d2148fc717.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/86f41b7d629fa664717c13bc0b15f858.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/86f41b7d629fa664717c13bc0b15f858.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/877fd48e980be7b27a5be8709dfb4137.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/877fd48e980be7b27a5be8709dfb4137.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/8aef2165cf82917e5b7ab3de1078c38c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/8aef2165cf82917e5b7ab3de1078c38c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/8bba3f3e4551f6f2df07a63ed918832b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/8bba3f3e4551f6f2df07a63ed918832b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/8da76f935ba41b969ccfa86ffb0204e7.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/8da76f935ba41b969ccfa86ffb0204e7.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/8dd471b7a7961537ab2f12c396abac0c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/8dd471b7a7961537ab2f12c396abac0c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/8fe48c25228bc4338703865e3f274c21.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/8fe48c25228bc4338703865e3f274c21.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/90f1cdb42141f0c68a111b2654b8a963.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/90f1cdb42141f0c68a111b2654b8a963.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/91ad327423f4967e4f6fd57069a0f2fc.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/91ad327423f4967e4f6fd57069a0f2fc.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/91f49599a810af1ed0c1a351f14ac99e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/91f49599a810af1ed0c1a351f14ac99e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/9283cc89e2d71979a143de94a99c9b25.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/9283cc89e2d71979a143de94a99c9b25.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/93dff17e993be4a78aea4e3c17d0916d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/93dff17e993be4a78aea4e3c17d0916d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/94bee8dbbe41187a879f001f1816fece.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/94bee8dbbe41187a879f001f1816fece.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/95352557a17c5b8f35836c54bdda82cc.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/95352557a17c5b8f35836c54bdda82cc.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/964c20018a0ed8d9df087e1e2b7ff42d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/964c20018a0ed8d9df087e1e2b7ff42d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/997640c55a6ded9da7e02f7f9d5a6999.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/997640c55a6ded9da7e02f7f9d5a6999.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/99bdbd9ffac9d3f82203c940cd516275.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/99bdbd9ffac9d3f82203c940cd516275.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/9ad3134af3a1c0fe5ea962734f299608.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/9ad3134af3a1c0fe5ea962734f299608.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/9ad97362888f6a84140fbf080f891fb9.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/9ad97362888f6a84140fbf080f891fb9.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/9c6191709aeeb06c154b663c97f29c4f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/9c6191709aeeb06c154b663c97f29c4f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/9cb6191837a0ec577c55784ac62b3a95.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/9cb6191837a0ec577c55784ac62b3a95.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/9cdc503727ada0c759eee4fc85f65b85.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/9cdc503727ada0c759eee4fc85f65b85.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/9e088492749dd72c420b9ea14be309a4.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/9e088492749dd72c420b9ea14be309a4.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/9e0dd4c9ca60aa42d546eb9af778e61d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/9e0dd4c9ca60aa42d546eb9af778e61d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/9e4cd56d3ac46d41b26f9438a9f1f702.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/9e4cd56d3ac46d41b26f9438a9f1f702.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/9e8b8a51838fdf51d67ede9266370774.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/9e8b8a51838fdf51d67ede9266370774.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a01032f2e14eb1760897a74a0e91d8ae.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a01032f2e14eb1760897a74a0e91d8ae.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a125cc5185ce9a2f8a5473da5389f8fd.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a125cc5185ce9a2f8a5473da5389f8fd.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a18ed57495d8cbc2106ce69d0851c7c4.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a18ed57495d8cbc2106ce69d0851c7c4.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a1903a62b39d6a82986555ba4274acf9.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a1903a62b39d6a82986555ba4274acf9.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a2ab4c99a92a2bae95882a1b9299abf4.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a2ab4c99a92a2bae95882a1b9299abf4.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a2cf3aa294c3363984aaedf2ca5b6836.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a2cf3aa294c3363984aaedf2ca5b6836.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a2dcd9175eea1e0d9495592be74f1771.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a2dcd9175eea1e0d9495592be74f1771.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a32acfcd6d04e5e4518733feb8bbc3eb.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a32acfcd6d04e5e4518733feb8bbc3eb.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a3418e0832b9830794d2882246090e8a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a3418e0832b9830794d2882246090e8a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a3a1f677a611b1f72cdea0893dc26b40.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a3a1f677a611b1f72cdea0893dc26b40.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a41198acaea59c7a948e4bbcbb27bcc7.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a41198acaea59c7a948e4bbcbb27bcc7.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a45002b33f6c20a7aafbc7fe0bda75ac.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a45002b33f6c20a7aafbc7fe0bda75ac.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a4e75a90086b7aa62994a3f43a2d8880.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a4e75a90086b7aa62994a3f43a2d8880.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a60f2f71ae2b4878222a37fb1c989af1.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a60f2f71ae2b4878222a37fb1c989af1.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a798df9c8e782a2529e03b75c6ae5d69.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a798df9c8e782a2529e03b75c6ae5d69.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/a7bf3fc7983a5201967101144ed1af6d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/a7bf3fc7983a5201967101144ed1af6d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/aa2062a974236db91d207b6f872a3d42.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/aa2062a974236db91d207b6f872a3d42.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/ad1b9015520f163ed0bf785c97b7f901.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/ad1b9015520f163ed0bf785c97b7f901.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/af4259f92460394617ab4beae656cf69.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/af4259f92460394617ab4beae656cf69.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/asset-manifest.json` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/asset-manifest.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.874448123620309%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.028f53cc.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.028f53cc.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.028f53cc.chunk.js.map'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "entrypoints": [
         "static/js/runtime-main.ad47a231.js",
         "static/js/2.2eaf9c7f.chunk.js",
-        "static/js/main.571a6b52.chunk.js"
+        "static/js/main.028f53cc.chunk.js"
     ],
     "files": {
         "abap.js": "./cce112a2a78f215dbf8026fccd277412.js",
         "abc.js": "./2987c57a184004a1f172eef983a30806.js",
         "actionscript.js": "./0a3f85997947fcc989b003237e68e745.js",
         "ada.js": "./330b0c4e3c2fb85009ef6daf099b607b.js",
         "alda.js": "./29dd0fe96b9fb6bfee8eca138f01394d.js",
@@ -121,16 +121,16 @@
         "livescript.js": "./75b9b4dd40e8e36ea8dd3aaa410a1edd.js",
         "logiql.js": "./b2fbe444b88a758f45f7a1c4beb686d9.js",
         "logtalk.js": "./b53b20cabeea14ae8ad8a4d19f8da928.js",
         "lsl.js": "./53192a5baa72c24e67bcc111e66f1500.js",
         "lua.js": "./c79bebdedaeeb0e84627cfb705eba4c0.js",
         "luapage.js": "./3020c220cfcf7a97372ed572fae92ec8.js",
         "lucene.js": "./0c14e3f2bbdb026c7dbdecf587f1df62.js",
-        "main.js": "./static/js/main.571a6b52.chunk.js",
-        "main.js.map": "./static/js/main.571a6b52.chunk.js.map",
+        "main.js": "./static/js/main.028f53cc.chunk.js",
+        "main.js.map": "./static/js/main.028f53cc.chunk.js.map",
         "makefile.js": "./55ccafd461c6f27fa9f080361348474a.js",
         "markdown.js": "./3c2581bce25c91393b40e940c0ddee68.js",
         "mask.js": "./6fa983289e62f70d40916e28ac753995.js",
         "matlab.js": "./03b6f5ed432b1096271448f530f79c3a.js",
         "maze.js": "./44b045e0cca5628c408353e416d5e5a4.js",
         "mediawiki.js": "./809aad7340c184c76c4bf229a697df28.js",
         "mel.js": "./0a84849cb72c84fb6a9b4d831df64ffa.js",
```

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b07b9f998c402374d5ae61f8a5f90834.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b07b9f998c402374d5ae61f8a5f90834.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b0860bdbd6a010f08ac65facbc751ec5.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b0860bdbd6a010f08ac65facbc751ec5.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b0f580aa76da5ecb8b8539dfafccaa74.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b0f580aa76da5ecb8b8539dfafccaa74.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b2bfbd167e10a2f1499b6b7173521a32.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b2bfbd167e10a2f1499b6b7173521a32.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b2ed29ed03abbb90d4e6460f78cc49e6.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b2ed29ed03abbb90d4e6460f78cc49e6.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b34e7646857d3e4810190d77cdd47c72.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b34e7646857d3e4810190d77cdd47c72.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b3c15b07ee65a11d3a4dc03a3fd4f520.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b3c15b07ee65a11d3a4dc03a3fd4f520.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b3d2e28a5c9c6eca4522120beaa8bd1b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b3d2e28a5c9c6eca4522120beaa8bd1b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b41a93a0b42dca8629be07ee243f9444.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b41a93a0b42dca8629be07ee243f9444.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b46dcbc460a77e0a225a0d717b2c5c44.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b46dcbc460a77e0a225a0d717b2c5c44.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b5bddfc3bcf40896e10bcf747f168e3d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b5bddfc3bcf40896e10bcf747f168e3d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b76c4ef3ef560839cc53abdc90dc0635.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b76c4ef3ef560839cc53abdc90dc0635.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b7fe810ac8ab02489be6d2a267e335f3.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b7fe810ac8ab02489be6d2a267e335f3.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/b93a7e92b54afaf7df25ce1f71abde96.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/b93a7e92b54afaf7df25ce1f71abde96.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/bab5d1e072fae9427c7a92aa03c6c994.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/bab5d1e072fae9427c7a92aa03c6c994.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/bd82757a59fac35f7323d8c129dd177f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/bd82757a59fac35f7323d8c129dd177f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/bee967a08d8144813e1eca995e850db7.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/bee967a08d8144813e1eca995e850db7.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/bf5dc4fb83ec42e1506dd557a39d8b51.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/bf5dc4fb83ec42e1506dd557a39d8b51.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/bootstrap.min.css` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c0155133f8b91c3fd72585e1bbd0663f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c0155133f8b91c3fd72585e1bbd0663f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c2a9533633141e25796248a15b084f4f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c2a9533633141e25796248a15b084f4f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c3d4155a442737116676e355d101e60b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c3d4155a442737116676e355d101e60b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c4e1812b01dcf14f11e8b553051eb7e3.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c4e1812b01dcf14f11e8b553051eb7e3.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c5981946a499b7a8e118460de13b2a3c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c5981946a499b7a8e118460de13b2a3c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c62509c4188fb5f0ac84cb18db4953a9.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c62509c4188fb5f0ac84cb18db4953a9.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c6ab877a9e42f3dd8f1ae60490334b0d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c6ab877a9e42f3dd8f1ae60490334b0d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c6bf611b1170b31a97c85c46bc02edc5.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c6bf611b1170b31a97c85c46bc02edc5.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c72d5cb0802acdf0c3cf889feb4cf08f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c72d5cb0802acdf0c3cf889feb4cf08f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c79bebdedaeeb0e84627cfb705eba4c0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c79bebdedaeeb0e84627cfb705eba4c0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c7b1c44013938dc49548d0e944959160.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c7b1c44013938dc49548d0e944959160.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c897e5b4c4aab18a0b0b92b21af4995d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c897e5b4c4aab18a0b0b92b21af4995d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/c9328914dfba7d21d76188d3f7b1b2c0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/c9328914dfba7d21d76188d3f7b1b2c0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/cae868cec072275a187aecc552b58c3b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/cae868cec072275a187aecc552b58c3b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/cbfc81eb8025b48dbb4d584913f9424a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/cbfc81eb8025b48dbb4d584913f9424a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/cd3f176a354e18ffa533a7db5a995db6.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/cd3f176a354e18ffa533a7db5a995db6.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d008fa7e4114f9d35c2d38675944fc5a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d008fa7e4114f9d35c2d38675944fc5a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d02def03076d1780451dac3f58ffdde5.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d02def03076d1780451dac3f58ffdde5.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d2013da8217d405f944a65fe2a0d978d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d2013da8217d405f944a65fe2a0d978d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d2b376303879422f058fe3b5dc9efdf2.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d2b376303879422f058fe3b5dc9efdf2.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d2f1ec1eaa573f91172c62b58a0b0925.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d2f1ec1eaa573f91172c62b58a0b0925.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d3a04193dbcd949adc1a9333911c8601.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d3a04193dbcd949adc1a9333911c8601.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d4fbb5d2bcf90560d95e04ec9183b645.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d4fbb5d2bcf90560d95e04ec9183b645.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d529068f6631dc56ed25b229d6256c61.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d529068f6631dc56ed25b229d6256c61.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d5a37181e369dece490ec467a51b874c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d5a37181e369dece490ec467a51b874c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d72af7d954398c5d9d9697968cdbf4c0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d72af7d954398c5d9d9697968cdbf4c0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d7cf2ff2cfce5a8766c462d361b9bf8b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d7cf2ff2cfce5a8766c462d361b9bf8b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d8d2a50e7d00d6926a59e7f0c605dd94.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d8d2a50e7d00d6926a59e7f0c605dd94.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/d92b3534728e5aa0fc51e894cf7b2d71.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/d92b3534728e5aa0fc51e894cf7b2d71.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/db0489d6a9164cb0e09fc2b1a9c7f35b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/db0489d6a9164cb0e09fc2b1a9c7f35b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/db500c5379116eafe008d7d7b66a4220.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/db500c5379116eafe008d7d7b66a4220.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/db988bf23763dc4b5bf25c93368bfcd3.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/db988bf23763dc4b5bf25c93368bfcd3.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/dce67fe447e34f4ffe4578c95206e567.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/dce67fe447e34f4ffe4578c95206e567.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/dd843e6eabf91ddb48f8417ed259cabf.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/dd843e6eabf91ddb48f8417ed259cabf.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/deccaca19352980d272cc86040fad45d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/deccaca19352980d272cc86040fad45d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e028d3d2b9861b82f6820743b8189e16.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e028d3d2b9861b82f6820743b8189e16.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e049c3b6ea982f67acd227871680de7a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e049c3b6ea982f67acd227871680de7a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e1f3357b2b8d16b4875692dfbdded291.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e1f3357b2b8d16b4875692dfbdded291.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e204504ae663c061f07092b2b2cdf870.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e204504ae663c061f07092b2b2cdf870.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e28ada780a72301df4bafb9c8b1d1ae6.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e28ada780a72301df4bafb9c8b1d1ae6.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e29701a1f6ad24a12a2fbd8ad82a3cb7.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e29701a1f6ad24a12a2fbd8ad82a3cb7.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e2b840449781aa7657b2c797d410f894.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e2b840449781aa7657b2c797d410f894.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e30f8c7030c064f949e786be09f3095b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e30f8c7030c064f949e786be09f3095b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e43fb8d8bc1621bccce93b7f7600df07.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e43fb8d8bc1621bccce93b7f7600df07.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e463a1cf5e818c9a3c704b57999a27d5.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e463a1cf5e818c9a3c704b57999a27d5.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e48b7b3ffe6b1614919441fb9c25dd4c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e48b7b3ffe6b1614919441fb9c25dd4c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e4bd34571302089306a2275b73ccabc9.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e4bd34571302089306a2275b73ccabc9.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e5a091ce9f3db02f839cb36dd4cb83ed.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e5a091ce9f3db02f839cb36dd4cb83ed.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e5f086d57eaffac1bf402e308c87b0a8.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e5f086d57eaffac1bf402e308c87b0a8.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e6e5c919b2f511e045d3d259a8f12b6c.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e6e5c919b2f511e045d3d259a8f12b6c.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e856077b2667951810c754aa5696ffbb.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e856077b2667951810c754aa5696ffbb.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e88b7914c8a46336d80ee6870837aed0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e88b7914c8a46336d80ee6870837aed0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e8e531b8b51d386a66e3881b36ee0add.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e8e531b8b51d386a66e3881b36ee0add.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e8fa0688c54573296b67b7caec859462.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e8fa0688c54573296b67b7caec859462.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/e94ac678b756a9a3190694b95a9430a5.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/e94ac678b756a9a3190694b95a9430a5.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/ea2db5427faaf15731c301cbc942d8fa.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/ea2db5427faaf15731c301cbc942d8fa.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/eb041468daa482e56a0b8a48c3f40f7b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/eb041468daa482e56a0b8a48c3f40f7b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/eb5e0358db5309c4df6f1b0480690e31.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/eb5e0358db5309c4df6f1b0480690e31.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/ebb3dae889b7e4d6240c4941bc4e177b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/ebb3dae889b7e4d6240c4941bc4e177b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/ec1870c6f2f5cb02a22ae24aa56f2d2d.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/ec1870c6f2f5cb02a22ae24aa56f2d2d.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/ed2e5b8cfcf5dc3e279f34f7b6122525.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/ed2e5b8cfcf5dc3e279f34f7b6122525.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/edbd54e9b9231be01dfe502d6155a746.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/edbd54e9b9231be01dfe502d6155a746.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/edc0ebd7ed759f2ed2082fe0d236dc0e.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/edc0ebd7ed759f2ed2082fe0d236dc0e.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/ef8e937a4924aa7a7ec3f1c1856f68a3.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/ef8e937a4924aa7a7ec3f1c1856f68a3.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f178b8178993c239247db2175a0f5292.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f178b8178993c239247db2175a0f5292.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f38fddaec7640c79658fc641e6ff3bb0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f38fddaec7640c79658fc641e6ff3bb0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f3ae2ab1bc71db88c5afcd7c90916489.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f3ae2ab1bc71db88c5afcd7c90916489.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f42a62d762c34d1ca7c418ea25726655.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f42a62d762c34d1ca7c418ea25726655.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f4ba3bed98e8325a3a723ec3f40069e2.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f4ba3bed98e8325a3a723ec3f40069e2.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f56295fa3830defe6dff72219c94f323.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f56295fa3830defe6dff72219c94f323.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f5634886f504b67a4fb52ba3eda0bb91.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f5634886f504b67a4fb52ba3eda0bb91.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f621ec46ae2b56dbbfc7208b961baeec.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f621ec46ae2b56dbbfc7208b961baeec.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f6bb72adbd9c04c120ec80cfe244cea0.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f6bb72adbd9c04c120ec80cfe244cea0.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f93f5974d7b6905236730a2b4567fb80.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f93f5974d7b6905236730a2b4567fb80.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f9a561c620224bfab5a21efecbfbe15b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f9a561c620224bfab5a21efecbfbe15b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f9bf7dc81acb8807eaf82f4e307266d4.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f9bf7dc81acb8807eaf82f4e307266d4.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/f9e12872a8aca64e07a75735e4404d2f.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/f9e12872a8aca64e07a75735e4404d2f.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/fae5d14d159a50986dc91ba7623cdfef.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/fae5d14d159a50986dc91ba7623cdfef.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/fafe7b33e520b9ab327172152fcbeac1.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/fafe7b33e520b9ab327172152fcbeac1.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/fc2c1d48fae7bb55b997e42e6186360b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/fc2c1d48fae7bb55b997e42e6186360b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/fcbe79021ef2b8e24eeac38f2ebd1e6b.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/fcbe79021ef2b8e24eeac38f2ebd1e6b.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/fe0c814b919ab5701ce9e9adce6c1a5a.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/fe0c814b919ab5701ce9e9adce6c1a5a.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/fe10bf958ca84418c6af95259c7b4260.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/fe10bf958ca84418c6af95259c7b4260.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/fe64d890e7fa0c0beae6f2e7a96a7ede.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/fe64d890e7fa0c0beae6f2e7a96a7ede.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/index.html` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="./bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,i,l=t[0],a=t[1],f=t[2],p=0,s=[];p<l.length;p++)i=l[p],Object.prototype.hasOwnProperty.call(o,i)&&o[i]&&s.push(o[i][0]),o[i]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(c&&c(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,l=1;l<r.length;l++){var a=r[l];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=i(i.s=r[0]))}return e}var n={},o={1:0},u=[];function i(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,i),r.l=!0,r.exports}i.m=e,i.c=n,i.d=function(e,t,r){i.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},i.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},i.t=function(e,t){if(1&t&&(e=i(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(i.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)i.d(r,n,function(t){return e[t]}.bind(null,n));return r},i.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return i.d(t,"a",t),t},i.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},i.p="./";var l=this["webpackJsonpstreamlit-code-editor"]=this["webpackJsonpstreamlit-code-editor"]||[],a=l.push.bind(l);l.push=t,l=l.slice();for(var f=0;f<l.length;f++)t(l[f]);var c=a;r()}([])</script><script src="./static/js/2.2eaf9c7f.chunk.js"></script><script src="./static/js/main.571a6b52.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="./bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,i,l=t[0],a=t[1],f=t[2],p=0,s=[];p<l.length;p++)i=l[p],Object.prototype.hasOwnProperty.call(o,i)&&o[i]&&s.push(o[i][0]),o[i]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(c&&c(t);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,l=1;l<r.length;l++){var a=r[l];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=i(i.s=r[0]))}return e}var n={},o={1:0},u=[];function i(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,i),r.l=!0,r.exports}i.m=e,i.c=n,i.d=function(e,t,r){i.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},i.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},i.t=function(e,t){if(1&t&&(e=i(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(i.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)i.d(r,n,function(t){return e[t]}.bind(null,n));return r},i.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return i.d(t,"a",t),t},i.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},i.p="./";var l=this["webpackJsonpstreamlit-code-editor"]=this["webpackJsonpstreamlit-code-editor"]||[],a=l.push.bind(l);l.push=t,l=l.slice();for(var f=0;f<l.length;f++)t(l[f]);var c=a;r()}([])</script><script src="./static/js/2.2eaf9c7f.chunk.js"></script><script src="./static/js/main.028f53cc.chunk.js"></script></body></html>
```

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js.LICENSE.txt` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js.map` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/main.571a6b52.chunk.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/main.028f53cc.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -406,15 +406,15 @@
                             }, {
                                 name: "response",
                                 description: "Send custom response",
                                 exec: function(e) {
                                     var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "",
                                         n = e.getSession().$modeId.split("/").pop();
                                     g.a.setComponentValue({
-                                        text: f,
+                                        text: e.getValue(),
                                         type: t,
                                         lang: n
                                     })
                                 }
                             }, {
                                 name: "editSnippets",
                                 description: "Edit snippets",
@@ -726,8 +726,8 @@
             }), document.getElementById("root"))
         }
     },
     [
         [501, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.571a6b52.chunk.js.map
+//# sourceMappingURL=main.028f53cc.chunk.js.map
```

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/main.571a6b52.chunk.js.map` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/main.028f53cc.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8285714285714285%*

 * *Differences: {"'file'": "'static/js/main.028f53cc.chunk.js'",*

 * * "'mappings'": "'0UAoCaA,EAAS,SAAH,GAA+H,IAAzHC,EAAI,EAAJA,KAAMC,EAAK,EAALA,MAAOC,EAAS,EAATA,UAAWC,EAAK,EAALA,MAAOC,EAAa,EAAbA,cAAeC,EAAQ,EAARA,SAAUC,EAAgB,EAAhBA,iBAAkBC,EAAS,EAATA,UAAWC,EAAI,EAAJA,KAAMC,EAAQ,EAARA,SAiDlH,OA/CAC,qBAAU,WACR,GAAGH,EAAUI,QAAQ,CAGnBC,IAAIC,QAAQ,oBAAoBC,aAAaC,IAAIR,EAAUI,QAAQK,QACnE,IAAMC,EAAcC,KAAKC,MAAMb,GAC5BW,EAAYZ,UAAYY,EAAYZ,SAASe,OAAS,GAEvDH,EAAYZ,SAASgB,SAAQ,SAACC,GAC2B,IAAD,EAApD,GAAGA,EAAQC,MAAgC,kBAAjBD,EAAQC,MAC5BL,KA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.571a6b52.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.028f53cc.chunk.js",
+    "mappings": "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",
     "names": [
         "Editor",
         "lang",
         "theme",
         "shortcuts",
         "props",
         "snippetString",
@@ -282,12 +282,12 @@
         "button-menu.tsx",
         "CodeEditor.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "import { useEffect} from \"react\"\nimport AceEditor from \"react-ace\";\nimport ace from \"ace-builds\";\n\nimport \"ace-builds/webpack-resolver\";\nimport \"ace-builds/src-noconflict/mode-python\";\nimport \"ace-builds/src-noconflict/mode-javascript\";\nimport \"ace-builds/src-noconflict/ext-language_tools\";\nimport \"ace-builds/src-noconflict/ext-searchbox\";\nimport \"ace-builds/src-noconflict/ext-prompt\";\nimport \"ace-builds/src-noconflict/ext-modelist\";\nimport \"ace-builds/src-noconflict/ext-keybinding_menu\";\n\nexport interface KeyBinding {\n    bindkey: string | object,\n    name: string\n}\n\nexport interface EditorKeyBindings {\n  commands?: KeyBinding[],\n  completer?: KeyBinding[]\n}\n\nexport type EditorProps = {\n    code: string,\n    lang: string,\n    theme: string,\n    shortcuts: string,\n    props: any,\n    editorRef: any,\n    snippetString: string,\n    commands: object[],\n    keybindingString: string,\n    onChange: (value: string, event?: any) => void \n  }\n  \nexport const Editor = ({ lang, theme, shortcuts, props, snippetString, commands, keybindingString, editorRef, code, onChange }: EditorProps ) => {\n    \n  useEffect(() => {\n    if(editorRef.current){\n\n      // Add/remove keybindings\n      ace.require('ace/autocomplete').Autocomplete.for(editorRef.current.editor);\n      const keybindings = JSON.parse(keybindingString) as EditorKeyBindings;\n      if(keybindings.commands && keybindings.commands.length > 0){\n        // const bindkeySelector = editorRef.current.editor.commands.platform as string;\n        keybindings.commands.forEach((binding) => {\n            if(binding.name && typeof binding.name === \"string\"){\n              if (JSON.stringify(editorRef.current.editor.commands.commands[binding.name].bindKey ?? \"\") !== JSON.stringify(binding.bindkey)) {\n                const newCommand = {...editorRef.current.editor.commands.commands[binding.name]};\n                newCommand.bindKey = binding.bindkey;\n                editorRef.current.editor.commands.addCommand(newCommand);\n                commands= [...commands, newCommand];\n              }\n            }\n   \n        });\n      }\n      if(keybindings.completer && keybindings.completer.length > 0){\n        // const bindkeySelector = editorRef.current.editor.completer.keyboardHandler.platform as string;\n        keybindings.completer.forEach((binding) => {\n            if(binding.name && typeof binding.name === \"string\"){\n              if (JSON.stringify(editorRef.current.editor.completer.keyboardHandler.commands[binding.name].bindKey ?? \"\") !== JSON.stringify(binding.bindkey)) {\n                const newCommand = {...editorRef.current.editor.completer.keyboardHandler.commands[binding.name]};\n                newCommand.bindKey = binding.bindkey;\n                editorRef.current.editor.completer.keyboardHandler.addCommand(newCommand);\n              }\n            }\n        });\n      }\n\n      // Add/remove snippets\n      ace.require(\"ace/ext/keybinding_menu\").init(editorRef.current.editor);\n      const snippetManager = ace.require('ace/snippets').snippetManager;\n      const snippets = JSON.parse(snippetString) as object;\n      for (const [snippetsLang, snippetsAddRemove] of Object.entries(snippets)){\n        if(snippetsAddRemove[0])\n          snippetManager.register(snippetManager.parseSnippetFile(snippetsAddRemove[0], snippetsLang), snippetsLang)\n        \n        if(snippetsAddRemove[1])\n          snippetManager.unregister(snippetManager.parseSnippetFile(snippetsAddRemove[1], snippetsLang), snippetsLang)\n      }\n    }\n  }, [snippetString, keybindingString]);\n\n  return (\n          <AceEditor\n           ref={editorRef}\n           name=\"REACT_ACE_EDITOR\"\n           mode={lang}\n           theme={theme}\n           value={code}\n           keyboardHandler={shortcuts}\n           commands={commands}\n           onChange={onChange}\n           {...props}/>\n  );\n};",
         "// import styled, { ThemeProvider, css } from \"styled-components\"\nimport { useRef, useState } from \"react\"\nimport styled, { ThemeProvider } from 'styled-components/macro'\nimport * as Icons from \"react-feather\"\n\n\nexport interface customInfoText {\n  name: string,\n  class?: string,\n  style?: object,\n  theme?: object\n}\n\nexport interface infoBar {\n  name?: string,\n  css?: string,\n  style?: object,\n  info?: customInfoText[]\n}\n\nexport interface customButton {\n  name: string,\n  feather?: string,\n  iconSize?: number,\n  primary?: boolean,\n  hasText?: boolean,\n  showWithIcon?: boolean,\n  alwaysOn?: boolean,\n  commands?: any[],\n  toggledCommands?: any[],\n  class?: string,\n  style?: object,\n  theme?: object, \n  classToggle?: string,\n}\n\nexport interface buttonGroup {\n  name: string,\n  buttons: customButton[],\n  style?: object,\n  toggleOnlyOne?: boolean,\n}\n\nexport interface menu {\n  style?: object,\n  css?: string,\n  groups?: buttonGroup[]\n}\n\nexport const StyledDiv = styled.div``;\nexport const StyledRegSpan = styled.span``;\n\nexport const StyledSpan = styled.span`\n  height: 2.5rem;\n  line-height: 2.5rem;\n  margin: 0px 0.4rem 0.15rem 0.4rem;\n  opacity: 0;\n  transform: scale(0);\n  transition: opacity 300ms 150ms, transform 300ms 150ms;\n`;\n\nexport const StyledButton = styled.button<{primary?: boolean, themeProp: string, theme: object}>`\n  border: none;\n  border-radius: 5px;\n  background: none;\n  height: 2.5rem;\n  line-height: 0;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  opacity: 0;\n  position: absolute;\n  transform: scale(0);\n  transition: opacity 20ms 300ms, transform 20ms 300ms;\n  z-index: 9994;\n  :focus {\n    outline: none;\n  }\n  span{\n    color: ${props => props.themeProp === \"streamlit_dark\"? \"rgba(250,250,250,0.6)\": \"rgba(0,0,0,0.5)\"};\n    transform: scale(0);\n    transform-origin: right;\n    transition: opacity 300ms 150ms, transform 300ms 150ms;\n  }\n  :hover span {\n    color: ${props => props.primary? props.theme.primaryColor : props.themeProp === \"streamlit_dark\"? \"rgb(250,250,250)\" : \"rgb(49, 51, 63)\"};\n    opacity: 1;\n    transform: scale(1);\n  }\n  svg {\n    stroke: ${props => props.themeProp === \"streamlit_dark\"? \"rgba(250,250,250,0.6)\": \"rgba(0,0,0,0.5)\"};\n    transform: scale(0);\n    transition: opacity 300ms 150ms, transform 300ms 150ms;\n  }\n  :hover svg {\n    stroke: ${props => props.primary? props.theme.primaryColor : props.themeProp === \"streamlit_dark\"? \"rgb(250,250,250)\" : \"rgb(49, 51, 63)\"};\n  }\n`;\n\nexport type iconKey = keyof typeof Icons;\n\nexport const creatIcon = (name: iconKey, size = 16) => {\n  const CustomIcon = Icons[name];\n  return <CustomIcon size={`${size}`} />;\n}\n\nexport type CustomInfoBar = {\n  theme: object,\n  info: infoBar,\n  infoRef: any,\n}\n\nexport const Info = ({info, theme, infoRef}: CustomInfoBar) => {\n\n  return (\n    <ThemeProvider theme={theme}>\n      {(Object.keys(info).length === 0) ? `` : <StyledDiv key=\"info_bar\" className={\"custom_info_bar \" + (info.name? info.name : \"\")} css={info.css} style={info.style}>\n        {<StyledRegSpan ref={infoRef} key=\"code_editor_info_message\" className=\"code_editor-info message\">\n          </StyledRegSpan>}\n        {(info.info || []).map((info: customInfoText)=>(\n          <StyledRegSpan key={\"info_\" + info.name} className={info.class} style={info.style}>\n            {info.name}\n          </StyledRegSpan>\n        ))}\n      </StyledDiv>}\n    </ThemeProvider>);\n}\n  \nexport type CustomButtonType = {\n  button: customButton, \n  theme: object, \n  themeProp: string, \n  executeAll: (ref: React.RefObject<HTMLButtonElement>, commands: any[]) => void\n}\nexport const Button = ({button, theme, themeProp, executeAll}: CustomButtonType) => {\n  const [toggle, setToggle] = useState(false);     //this toggle is currently not being used\n  const ref = useRef<HTMLButtonElement>(null);\n\n  const execute = (commands: any[], toggledCommands?: any[]) => {\n    if(button.classToggle){\n      setToggle(!toggle);\n      if (ref.current){\n        ref.current.classList.toggle(button.classToggle);\n        if(ref.current.classList.contains(button.classToggle))\n          executeAll(ref, commands);\n        else\n          executeAll(ref, toggledCommands ?? commands);\n      }\n      else \n        executeAll(ref, toggle? toggledCommands?? commands : commands);\n    } \n    else \n      executeAll(ref, commands);\n  }\n\n  return (\n    <StyledButton \n      ref={ref}\n      primary={button.primary? button.primary : false} \n      className={(button.class? button.class: \"\" ) + (button.alwaysOn? \" always-on\" : \"\") + (button.showWithIcon? \" with-icon\" : \"\") }\n      themeProp={themeProp}\n      style={button.style} \n      theme={theme}\n      onClick={() => execute(button.commands ?? [], button.toggledCommands)}>\n        {(button.hasText && button.name)? <StyledSpan >{button.name}</StyledSpan> : ``}\n        {button.feather? creatIcon(button.feather as iconKey || \"X\", button.iconSize) : \"\"}\n    </StyledButton>\n  )\n}\n\nexport type CustomButtonSet = \n{\n  theme: object,\n  themeProp: string,\n  buttonGroup: buttonGroup,\n  executeAll: (commands: any[]) => void \n}\n  \nexport const Set = ({buttonGroup, executeAll, theme, themeProp}: CustomButtonSet) => {\n\n  const execute = (buttonRef: React.RefObject<HTMLButtonElement>, commands: any[]) => {\n    // Do things here that depend on which button is clicked using buttonRef.current\n    if(commands)\n      executeAll(commands);\n  }\n\n  return (\n      <ThemeProvider theme={theme}>\n        {buttonGroup.buttons.map( (button) => (\n        <Button \n          key={buttonGroup.name + \"_\" + button.name}\n          button={button}\n          themeProp={themeProp}\n          theme={theme}\n          executeAll={(ref, commands) => execute(ref, commands)}/>\n      ))}\n    </ThemeProvider>\n  )\n}\n  \nexport type CustomMenu = \n{\n  menu : menu,\n  theme: object,\n  themeProp: string,\n  executeAll: (commands: any[]) => void\n}\n  \nexport const Menu = ({menu, executeAll, theme, themeProp}: CustomMenu) => {\n\n  const execute = (buttonRef: React.RefObject<HTMLButtonElement>, commands: any[]) => {\n    // Do things here that depend on which button is clicked using buttonRef.current\n    if(commands)\n      executeAll(commands);\n  }\n  \n  return (\n    <ThemeProvider theme={theme}>\n      {(Object.keys(menu).length === 0 )? \"\" : <StyledDiv key=\"menu_bar\" className=\"custom_menu\" style={menu.style} css={menu.css}>\n        {!menu.groups? `` : menu.groups.map((group: buttonGroup, index) => (\n          <StyledDiv key={\"group_\" + group.name + index} className={\"menu_group \" + group.name} style={group.style} data-one-toggle-only={group.toggleOnlyOne} >\n              {group.buttons.map((button: customButton,)=>(\n                <Button \n                  key={group.name + \"_\" + button.name}\n                  button={button}\n                  themeProp={themeProp}\n                  theme={theme}\n                  executeAll={(ref, commands) => execute(ref, commands)}/>\n              ))}\n          </StyledDiv>\n        ))}\n      </StyledDiv>}\n    </ThemeProvider>\n  )\n}",
-        "import {\n  Streamlit,\n  withStreamlitConnection,\n  ComponentProps,\n  Theme,\n} from \"streamlit-component-lib\"\nimport styled, { createGlobalStyle } from \"styled-components/macro\"\nimport { useState, useRef, useEffect, useMemo } from \"react\"\nimport AceEditor from \"react-ace\";\nimport ace from \"ace-builds\";\nimport { Editor } from './editor';\nimport { Menu as ButtonMenu, Set as ButtonSet, customButton, buttonGroup, Info as InfoBar } from \"./button-menu\"\n\nimport \"ace-builds/webpack-resolver\";\nimport \"ace-builds/src-noconflict/mode-python\";\nimport \"ace-builds/src-noconflict/mode-javascript\";\nimport \"ace-builds/src-noconflict/ext-language_tools\";\nimport \"ace-builds/src-noconflict/ext-searchbox\";\nimport \"ace-builds/src-noconflict/ext-prompt\";\nimport \"ace-builds/src-noconflict/ext-modelist\";\n\ninterface CodeEditorProps extends ComponentProps {\n  args: any\n  width: number\n  disabled: boolean\n  theme?: Theme\n}\n\nconst defaultOptions = {\n  fontFamily: '\"Source Code Pro\", monospace',\n  cursorStyle: \"smooth\",\n  displayIndentGuides: false,\n  wrap: false,\n  highlightActiveLine: true,\n  showPrintMargin: false,\n  showLineNumbers: false,\n  foldStyle: \"markbegin\",\n  autoScrollEditorIntoView: false,\n  animatedScroll: true,\n  fadeFoldWidgets: true,\n}\n\nconst defaultEditorProps = {\n  editorProps: {\n    $blockScrolling: true\n  }\n}\n\nconst defaultProps = {\n  cursorStart: 1,\n  enableBasicAutocompletion: false,\n  enableLiveAutocompletion: true,\n  enableSnippets: true,\n  focus: false,\n  fontSize: 14,\n  highlightActiveLine: true,\n  navigateToFileEnd: true,\n  placeholder: null,\n  readOnly: false,\n  scrollMargin: [15, 15, 0, 0],\n  setOptions: defaultOptions,\n  showGutter: true,\n  showPrintMargin: false,\n  style: {},\n  tabSize: 4,\n  width: \"auto\",\n  debounceChangePeriod: 250,\n}\n\nconst GlobalCSS = createGlobalStyle<{isDisabled?: boolean, inject: string}>`\n  html {\n    opacity: ${props => props.isDisabled? \"0.5\": \"1\"};\n    cursor: ${props => props.isDisabled? \"not-allowed\": \"auto\"};\n    pointer-events: ${props => props.isDisabled? \"none\": \"auto\"};\n  }\n  body {\n    margin: 0;\n    padding: 0;\n  }\n  ${props => props.inject}\n`\nconst StyledCodeEditor = styled.div`\n  width: 100%;\n  border-radius: 8px;\n  overflow: hidden;\n  display: flex;\n  flex-direction: column;\n  :hover button {\n    opacity: 1;\n    transform: scale(1);\n  }\n  button.always-on {\n    opacity: 1;\n    transform: scale(1);\n    transition: none;\n  }\n  :hover button svg {\n        opacity: 1;\n        transform: scale(1);\n  }\n  :hover button.with-icon span {\n    opacity: 1;\n    transform: scale(1);\n  }\n  button.always-on > span {\n    opacity: 1;\n    transform: scale(1);\n    transition: none;\n  }\n  button.always-on > svg {\n    opacity: 1;\n    transform: scale(1);\n    transition: none;\n  }\n  `;\n\nconst CodeEditor = ({ args, width, disabled, theme }: CodeEditorProps) => {\n\n  //sets code to the initial value every time the component is rendered\n  //to set the initial value once, use a function instead of a value.\n  const [code, setCode] = useState(args['code']);\n  // const [keybindingAddRemove, setKeybindingAddRemove] = useState([\"\",\"\"]);\n\n  const aceEditor = useRef<AceEditor>(null);\n  const infoTextRef = useRef<HTMLSpanElement>(null);\n  const baseSession = useRef<ace.Ace.EditSession | null>(null);\n  const keepFocus = useRef<boolean>(false);\n  const reset = useRef<boolean>(false);\n\n  var timeoutId: NodeJS.Timeout;\n\n  /**\n    * This function takes as input either a snippetText string that is expected\n    * to be already formatted like the text in a SnippetFile or a dictionary or \n    * and array of dictionaries. For the first case, it just returns the input.\n    * For the second and third case, a (SnippetFile format) string is constructed\n    * from the dict(s) and returned. Learn more about snippets {@link  here}\n    * @param snippetRaw snippets to be converted to a single snippetText string\n    * @returns {string} snippetText\n    */\n  const createSnippets = (snippetRaw: string | object | [object]): string => {\n    return (typeof snippetRaw === \"string\" ? snippetRaw : (Array.isArray(snippetRaw) ? snippetRaw : [snippetRaw]).map(({ name, code }) =>\n    ([\n      'snippet ' + name,\n      code.split('\\n')\n        .map((c: string) => '\\t' + c)\n        .join('\\n'),\n    ].join('\\n'))\n    ).join('\\n'))\n  }\n  const [snippetAddRemove, setSnippetAddRemove] = useState({[args['lang']] : [createSnippets(args[\"snippets\"][0]), createSnippets(args[\"snippets\"][1])]});\n  const [keybindingAddRemove, setKeybindingAddRemove] = useState(args['keybindings']);\n\n\n  useEffect(() => {\n    return () => {\n      if (timeoutId) {\n        clearTimeout(timeoutId);\n      }\n    }\n  }, []);\n\n  useEffect(() => {\n    if(aceEditor.current && keepFocus.current){\n      aceEditor.current.editor.focus();\n      keepFocus.current = false;\n    }\n  }, [keepFocus.current]);\n\n  // To reasons for the useEffect here: \n  //   1. to set the focus on the editor only when the focus argument has changed to true.\n  //   2. to set the focus on the editor after rendering the component at which point, the \n  //      editor should be ready.\n  useEffect(() => {\n    if(aceEditor.current && args.focus){\n      aceEditor.current.editor.focus();\n    }\n  }, [args.focus]);\n\n  const onChangeHandler = (newCode: string) => {\n    setCode(newCode);\n  }\n\n  // commands is an array of objects containing functions\n  // that the editor can be triggered to call.\n  const commands = { commands: [\n    {\n      name: 'submit', //name for the key binding.\n      description: \"Send 'submit' response\", //description of the command\n      bindKey: { win: 'Ctrl-Enter', mac: 'Command-Enter' }, //key combination used for the command.\n      exec: (editor: any) => {\n        const outgoingMode = editor.getSession().$modeId.split(\"/\").pop();\n        Streamlit.setComponentValue({text: editor.getValue(), type: \"submit\", lang: outgoingMode });\n      }\n    },\n    {\n      name: 'saveState',\n      description: \"Save state\",\n      bindKey: { win: 'Ctrl-Alt-S', mac: 'Command-Alt-S' },\n      exec: (editor: ace.Ace.Editor) => {\n        setCode(editor.getValue());\n      }\n    },\n    {\n      name: 'copyAll',\n      description: \"Copy all text to clipboard\",\n      exec: (editor: ace.Ace.Editor) => {\n        unsecureCopyTextToClipboard(editor.getValue());\n      }\n    },\n    {\n      name: 'reset',\n      exec: () => {\n        resetEditor();\n      }\n    },\n    {\n      name: 'keepFocus',\n      description: \"Return cursor to editor\",\n      exec: () => {\n        keepFocus.current = true;\n      }\n    },\n    {\n      name: \"setMode\",\n      description: \"Set language mode\",\n      exec: (editor: ace.Ace.Editor, lang: string) => {\n          if(lang && typeof lang === \"string\")\n            editor.getSession().setMode(\"ace/mode/\" + lang);\n      },\n      readOnly: true\n    },\n    {\n      name: \"changeShortcuts\",\n      description: \"Switch shortcuts\",\n      exec: (editor: any, shortcuts?: string) => {\n        if(shortcuts && typeof shortcuts === \"string\")\n          editor.setKeyboardHandler(\"ace/keyboard/\" + shortcuts);\n        else {\n          //rotate through the available keyboard handlers\n          const handlers = [\"ace/keyboard/vim\", \"ace/keyboard/emacs\", \"ace/keyboard/sublime\", \"ace/keyboard/vscode\"];\n          const currentHandler = handlers[(handlers.indexOf(editor.$keybindingId) + 1) % 4];\n          editor.setKeyboardHandler(currentHandler);\n        }\n      },\n      readOnly: true\n    },\n    {\n      name: 'toggleKeyboardShortcuts',\n      exec: (editor: ace.Ace.Editor) => {\n        if(!document.getElementById('kbshortcutmenu'))\n          editor.execCommand('showKeyboardShortcuts');\n        else \n          editor.execCommand('simulateKeyPress', {type:\"keydown\", keyCode: 27});\n      }\n    },\n    {\n      name: 'simulateKeyPress',\n      exec: (editor: ace.Ace.Editor, args: {type: string, key?: string, keyCode?: number}) => {\n        if(args.key)\n          document.dispatchEvent(new KeyboardEvent(args.type,{'key': args.key})); \n        else if(args.keyCode)\n          document.dispatchEvent(new KeyboardEvent(args.type,{'keyCode': args.keyCode})); \n      }\n    },\n    {\n      name: 'infoMessage',\n      description: \"Display message in info bar\",\n      exec: (editor: ace.Ace.Editor, args: {text: string, timeout?: number, classToggle?: string, targetQueryString?: string} ) => {\n        if(args.targetQueryString){\n          const target = document.querySelector(args.targetQueryString) as HTMLElement;\n          if(target){\n            target.innerText = args.text;\n            target.classList.add(args.classToggle || \"\")\n            if(args.timeout){\n              timeoutId = setTimeout(() => {\n                target.classList.remove(args.classToggle || \"\");\n              }, args.timeout);\n            }\n          }\n        }\n        else if(infoTextRef.current){\n          infoTextRef.current.innerText = args.text;\n          infoTextRef.current.classList.add(args.classToggle || \"\");\n          if(args.timeout){\n            timeoutId = setTimeout(() => {\n              infoTextRef.current?.classList.remove(args.classToggle || \"\");\n            }, args.timeout);\n          }\n        }\n      }\n    },\n    {\n      name: 'response', //name for the key binding.\n      description: \"Send custom response\", //description of the command\n      exec: (editor: any, responseType = \"\") => {\n        const outgoingMode = editor.getSession().$modeId.split(\"/\").pop();\n        Streamlit.setComponentValue({ text: code, type: responseType, lang: outgoingMode });\n      }\n    },\n    {\n      name: 'editSnippets',\n      description: \"Edit snippets\",\n      bindKey: { win: 'Ctrl-Alt-M', mac: 'Command-Alt-M' },\n      exec: (editor: any) => {\n        const snippetManager = ace.require('ace/snippets').snippetManager;\n        if(baseSession.current){\n          const outgoingMode = editor.getSession().$modeId.split(\"/\").pop();\n          if(outgoingMode === \"snippets\"){\n            const snippetText = editor.getSession().getValue();\n            editor.setSession(baseSession.current);\n            baseSession.current = null;\n            setCode(editor.getSession().getValue());\n            if(outgoingMode === \"snippets\"){}\n            try{\n              const snippetsPlusMinus = snippetText.split(\"###~~~\")[1];\n              const [snippetsPlus, snippetsMinus] = snippetsPlusMinus.split(\"###---\");\n              const snippetsToAdd = snippetsPlus.split(\"###+++\")[1];\n              const snippetsToRemove = snippetsMinus;\n              const langMode = editor.getSession().$modeId.split(\"/\").pop();\n              setSnippetAddRemove({[langMode] : [snippetAddRemove[langMode][0] + snippetsToAdd, snippetAddRemove[langMode][1] + snippetsToRemove]});\n            } catch (error) {\n              editor.execCommand(\"infoMessage\",{text: \"error parsing file, restoring original file\", timeout: 2000, classToggle: \"show\"});\n            }\n          }\n        } else {\n          const langMode = editor.getSession().$modeId.split(\"/\").pop()\n          const snippetConcatText = `\\n###~~~#(DO NOT EDIT THIS LINE)\n# Commented out above are all the snippets that are currently\n# registered for ${args['lang']} mode.\n\\n\\n###+++#(DO NOT EDIT THIS LINE) \\n# Put the snippets you want to add below this line.\\n\\n\\n\\n\n\\n\\n\\n###---#(DO NOT EDIT THIS LINE) \\n# Put the snippets you want to remove below this line.\\n\\n\\n\\n\\n\\n\\n`;\n          const snippetText = \"#\" + createSnippets(snippetManager.snippetMap[langMode].map((snip: any) => ({name: snip.name, code: snip.content}))).replace(/\\n/g, \"\\n#\") + snippetConcatText;\n          // snippetManager.files[editor.getSession().$modeId].snippetText\n          const lineCount = (snippetText.match(/\\n/g) || []).length;\n          baseSession.current = editor.getSession();\n          const snippetsSession = ace.createEditSession(snippetText, \"ace/mode/snippets\");\n          editor.setSession(snippetsSession);\n          const cursorPos = {row: (lineCount - 15)>0? lineCount - 15 : 0, column: 0};\n          editor.moveCursorTo(cursorPos.row, cursorPos.column);\n          editor.renderer.scrollCursorIntoView(cursorPos, 0.5);\n        }\n      }\n    },\n    {\n      name: 'editKeyBindings',\n      description: \"Edit keybindings\",\n      bindKey: { win: 'Ctrl-Alt-B', mac: 'Command-Alt-B' },\n      exec: (editor: any) => {\n        ace.require('ace/autocomplete').Autocomplete.for(editor);\n        if(baseSession.current){\n          const outgoingMode = editor.getSession().$modeId.split(\"/\").pop();\n          if(outgoingMode === \"json\"){\n            const keybindingsJSON = editor.getSession().getValue();\n            editor.setSession(baseSession.current);\n            baseSession.current = null;\n            setCode(editor.getSession().getValue());\n            try{\n              setKeybindingAddRemove(JSON.parse(keybindingsJSON));\n            } catch (error) {\n              editor.execCommand(\"infoMessage\",{text: \"error parsing file, restoring original file\", timeout: 2000, classToggle: \"show\"});\n            }\n          }\n        } else {\n          const keybindings = {commands: {}, completer: {}};\n          if(editor.completer && editor.completer.keyboardHandler.commands){\n            keybindings.completer = Object.keys(editor.completer.keyboardHandler.commands).map((key: any) => ({bindkey: editor.completer.keyboardHandler.commands[key].bindKey ?? \"\", name: editor.completer.keyboardHandler.commands[key].name}));\n          }\n          if(editor.commands.commands){\n            keybindings.commands = Object.keys(editor.commands.commands).map((key: any) => ({bindkey: editor.commands.commands[key].bindKey ?? \"\", name: editor.commands.commands[key].name}));\n          }\n          const keybindingsJSON = JSON.stringify(keybindings, undefined, 2);\n          baseSession.current = editor.getSession();\n          const keybindingsSession = ace.createEditSession(keybindingsJSON, \"ace/mode/json\");\n          editor.setSession(keybindingsSession);\n        }\n      }\n    },\n    {\n      name: 'exitSession', //name for the key binding.\n      bindKey: { win: 'Esc', mac: 'Esc' },\n      description: \"Return to main session (keep changes)\", //description of the command\n      exec: (editor: any) => {\n        if(baseSession.current){\n          const mode = editor.getSession().$modeId.split(\"/\").pop();\n          if (mode === \"snippets\")\n            editor.execCommand(\"editSnippets\");\n          else if (mode === \"json\")\n            editor.execCommand(\"editKeyBindings\");\n        }\n      }\n    },\n    {\n      name: 'abandonSession', //name for the key binding.\n      bindKey: { win: 'Ctrl-Alt-Esc', mac: 'Command-Alt-Esc' },\n      description: \"Return to main session (discard changes)\", //description of the command\n      exec: (editor: any) => {\n        if(baseSession.current){\n          editor.setSession(baseSession.current);\n          baseSession.current = null;\n          setCode(editor.getSession().getValue());\n        }\n      }\n    },\n    {\n      name: 'classART', //name for the key binding.\n      description: \"Add/Remove/Toggle class for element\", //description of the command\n      exec: (editor: any, args: {targetQueryString: string, type: string, class: string}) => {\n        if(args.targetQueryString && args.type && args.class){\n          switch(args.type){\n            case \"add\":\n              document.querySelectorAll(args.targetQueryString)?.forEach((el: any) => el.classList.add(args.class));\n              break;\n            case \"remove\":\n              document.querySelectorAll(args.targetQueryString)?.forEach((el: any) => el.classList.remove(args.class));\n              break;\n            case \"toggle\":\n              document.querySelectorAll(args.targetQueryString)?.forEach((el: any) => el.classList.toggle(args.class));\n              break;\n            default:\n              break;\n          }\n        }\n      }\n    },\n    {\n      name: 'conditionalExecute', //name for the key binding.\n      description: \"Execute command if element exists\", //description of the command\n      exec: (editor: any, args: {targetQueryString: string, command: any[], condition?: boolean}) => {\n        if(args.targetQueryString && args.command && Array.isArray(args.command)){\n          if(!(args.condition ?? true) === !document.querySelector(args.targetQueryString)){\n            typeof args.command[0] === \"string\" ? execute(args.command[0], args.command[1]) : console.warn(\"Editor command - conditionalExecute: improper command format! Command array must contain name of command as first element and arguments as second element.\");\n          }\n        }\n      }\n    }\n  ]};\n\n  const execute = (command: string, args: any = \"\") => {\n    const editor = aceEditor.current?.editor;\n    if (editor) {\n      if (!args) {\n        editor.execCommand(command)\n      }\n      else if (typeof args === \"number\" || typeof args === \"string\") {\n        editor.execCommand(command, args);\n      }\n      else if (typeof args === \"object\" && !Array.isArray(args)) {\n        var containsNumsStr = true;\n        Object.keys(args).forEach((key: any) => {\n          containsNumsStr = typeof args[key] === \"string\" || typeof args[key] === \"number\" || Array.isArray(args[key]);\n        });\n        if (Object.keys(args).length < 4 && containsNumsStr) {\n          editor.execCommand(command, args);\n        }\n      }\n      else {\n        console.warn(`Function - execute: failed to parse/execute \"${command}\" command!`);\n      }\n    }\n  }\n\n  const executeAll = (commands: any[]) => {\n    commands.forEach(singleCommand => {\n      if (Array.isArray(singleCommand)) {\n        typeof singleCommand[0] === \"string\" ? execute(singleCommand[0], singleCommand[1]) : console.warn(\"Function - executeAll: improper command format! Singular commands must contain name of command as first element and arguments as second element.\");\n      } else if (typeof singleCommand === \"string\") {\n        execute(singleCommand);\n      } else {\n        console.warn(\"Function - executeAll: failed to parse/execute command(s)!\");\n      }\n    });\n  }\n\n  const resetEditor = () => {\n    setCode(args['code']);\n  }\n\n  const unsecureCopyTextToClipboard = (text: string) => {\n    const textField = document.createElement('textarea');\n    textField.value = text;\n    document.body.appendChild(textField);\n    textField.select();\n    document.execCommand('copy');\n    textField.remove();\n  }\n\n  /**\n   * resizeObserver observes changes in elements its given to observe and is used here\n   * to communicate to streamlit the height of the component that has changed\n   * so that streamlit can adjust the iframe containing the component accordingly.\n   */\n  const resizeObserver = new ResizeObserver((entries: any) => {\n    // If we know that the body will always fully contain our component (without cutting it off)\n    // then we can use docuemnt.body height instead\n    Streamlit.setFrameHeight((entries[0].contentBoxSize.blockSize ?? entries[0].contentRect.height)); \n  })\n\n  const observe = (divElem: any) => {\n    divElem ? resizeObserver.observe(divElem as HTMLDivElement) : resizeObserver.disconnect();\n  }\n\n  // This useEffect is used to reset the editor when the code argument changes and\n  // the allow_reset argument is true. The allow_reset argument only impacts the\n  // behavior of the component when the component has a fixed key argument because\n  // changing the key argument results in the creation of a new component instance.\n  // Everything would be reset anyways.\n  useEffect(() => {\n    if (args['allow_reset'] === true && args['code'] !== code) {\n      reset.current = !reset.current;\n      resetEditor();\n    }\n  }, [args['code']]);\n\n  /**\n   * This could also be memoized but I don't think it would be necessary because its not expensive.\n   */\n  const themeChoice = () => {\n    const isDarkTheme = theme? theme.base === \"dark\" : true;\n    switch (args['theme']) {\n      case \"contrast\":\n        return isDarkTheme? \"streamlit_light\" : \"streamlit_dark\";\n      case \"light\":\n        return \"streamlit_light\";\n      case \"dark\":\n        return \"streamlit_dark\";\n      case \"default\":\n        return isDarkTheme? \"streamlit_dark\" : \"streamlit_light\";\n      default:\n        return isDarkTheme? \"streamlit_dark\" : \"streamlit_light\";\n    }\n  }\n\n  const themeProp = themeChoice();\n  const componentContainerProps = args[\"component_props\"];\n\n  const {info: infoArg, menu: menuArg, focus: focusArg, code: codeArg, ...rest} = args;\n  const editorArgsString = JSON.stringify(rest);\n  const menuArgsString = JSON.stringify(menuArg);\n  const infoArgsString = JSON.stringify(infoArg);\n  const buttonArgsString = JSON.stringify(args['buttons']);\n  const themeString = JSON.stringify(theme);\n  const snippets = JSON.stringify(snippetAddRemove);\n\n  /**\n   * This section contains the main sub-components (child components). These components are wrapped in useMemos\n   * in order to prevent unnecessary re-rendering of the components. This is listed as one of its use cases in the\n   * React docs ({@link https://beta.reactjs.org/reference/react/useMemo#skipping-re-rendering-of-components Skipping re-rendering of components})\n   *\n   * This component is the editor component that is rendered. It is only re-rendered when\n   * certain properties change. This is important because we should account for the possibility that the editor \n   * is being used at any given moment. Unnecessary and frequent re-rendering of the editor (for outside reasons\n   * especially) can impact user experience and responsiveness.\n   */\n  const editor = useMemo(() => {\n    const keybindings = JSON.stringify(keybindingAddRemove);\n    const revertedArgs = JSON.parse(editorArgsString);\n\n    // Create commands for each button\n    if(revertedArgs['buttons'].length > 0) {\n      revertedArgs['buttons'].forEach((button: any) => {\n          commands.commands = [...commands.commands, {\n            name: (button.name as string).trim().replace(/\\s+/g, '_') + '_button',\n            description: \"Execute '\" + button.name + \"' button command(s)\",\n            exec: () => {\n            executeAll(button.commands);\n          }}];\n      });\n    }\n\n    let heightProps = {};\n    if(typeof revertedArgs['height'] === \"number\") \n      heightProps = {minLines: 1, maxLines: revertedArgs['height']};\n    else if(typeof revertedArgs['height'] === \"string\") \n      heightProps = {height: revertedArgs['height']};\n    else if(Array.isArray(revertedArgs['height']) && revertedArgs['height'].length === 2) \n      heightProps = {minLines: revertedArgs['height'][0], maxLines: revertedArgs['height'][1]};\n\n    const aceEditorProps = { ...defaultEditorProps, ...revertedArgs['editorProps'] };\n    const aceOptions = { ...defaultOptions, ...revertedArgs['options'] };\n    const partProps = { setOptions: aceOptions, editorProps: aceEditorProps };\n    const aceProps = { ...defaultProps, ...partProps,...heightProps, ...revertedArgs['props'] };\n\n    /**\n     * TODO: Remove props from aceProps that we don't want to allow user access to.\n     */\n    return (\n        <Editor\n         editorRef={aceEditor}\n         code={code} \n         lang={revertedArgs['lang']} \n         theme={themeProp} \n         shortcuts={revertedArgs['shortcuts']} \n         snippetString={snippets} \n         commands={commands.commands} \n         keybindingString={keybindings} \n         props={aceProps} \n         onChange={(value) => onChangeHandler(value)} />\n      );\n  }, [editorArgsString, themeProp, snippets, keybindingAddRemove, reset.current]);\n\n  const buttons = useMemo(() => {\n    const revertedButtons = JSON.parse(buttonArgsString);\n    const revertedTheme = JSON.parse(themeString);\n    const customButtonTheme = revertedTheme ?? {};\n    const customButtons = {buttons: (revertedButtons ?? []) as customButton[], name: \"customButtons\"} as buttonGroup;\n    return (\n      < ButtonSet\n       buttonGroup={customButtons} \n       theme={customButtonTheme} \n       themeProp={themeProp} \n       executeAll={(commands) => executeAll(commands)} />\n    );\n  }, [buttonArgsString, themeString, themeProp]);\n\n  const menu = useMemo(() => {\n    const revertedMenu = JSON.parse(menuArgsString);\n    const revertedTheme = JSON.parse(themeString);\n    const menuTheme = revertedTheme ?? {};\n    return (\n      <ButtonMenu\n       menu={revertedMenu} \n       theme={menuTheme} \n       themeProp={themeProp} \n       executeAll={(commands) => executeAll(commands)} />\n    );\n  }, [menuArgsString, themeString, themeProp]);\n\n  const info = useMemo(() => {\n    const revertedInfo = JSON.parse(infoArgsString);\n    const revertedTheme = JSON.parse(themeString);\n    const infoTheme = revertedTheme ?? {};\n    return (\n      <InfoBar\n       infoRef={infoTextRef} \n       info={revertedInfo} \n       theme={infoTheme} />\n    );\n  }, [infoArgsString, themeString]);\n\n  const globalCSS = useMemo(() => {\n    return (\n      <GlobalCSS isDisabled={disabled} inject={componentContainerProps.globalCSS} />\n    );\n  }, [componentContainerProps.globalCSS, disabled]);\n\n  return (\n    <StyledCodeEditor ref={observe} style={componentContainerProps.style} css={componentContainerProps.css} className={\"streamlit_code-editor \" + theme?.base ?? \"\" } >\n      {globalCSS}\n      {editor}\n      {buttons}\n      {menu}\n      {info}\n    </StyledCodeEditor>\n  )\n}\n\nexport default withStreamlitConnection(CodeEditor)",
+        "import {\n  Streamlit,\n  withStreamlitConnection,\n  ComponentProps,\n  Theme,\n} from \"streamlit-component-lib\"\nimport styled, { createGlobalStyle } from \"styled-components/macro\"\nimport { useState, useRef, useEffect, useMemo } from \"react\"\nimport AceEditor from \"react-ace\";\nimport ace from \"ace-builds\";\nimport { Editor } from './editor';\nimport { Menu as ButtonMenu, Set as ButtonSet, customButton, buttonGroup, Info as InfoBar } from \"./button-menu\"\n\nimport \"ace-builds/webpack-resolver\";\nimport \"ace-builds/src-noconflict/mode-python\";\nimport \"ace-builds/src-noconflict/mode-javascript\";\nimport \"ace-builds/src-noconflict/ext-language_tools\";\nimport \"ace-builds/src-noconflict/ext-searchbox\";\nimport \"ace-builds/src-noconflict/ext-prompt\";\nimport \"ace-builds/src-noconflict/ext-modelist\";\n\ninterface CodeEditorProps extends ComponentProps {\n  args: any\n  width: number\n  disabled: boolean\n  theme?: Theme\n}\n\nconst defaultOptions = {\n  fontFamily: '\"Source Code Pro\", monospace',\n  cursorStyle: \"smooth\",\n  displayIndentGuides: false,\n  wrap: false,\n  highlightActiveLine: true,\n  showPrintMargin: false,\n  showLineNumbers: false,\n  foldStyle: \"markbegin\",\n  autoScrollEditorIntoView: false,\n  animatedScroll: true,\n  fadeFoldWidgets: true,\n}\n\nconst defaultEditorProps = {\n  editorProps: {\n    $blockScrolling: true\n  }\n}\n\nconst defaultProps = {\n  cursorStart: 1,\n  enableBasicAutocompletion: false,\n  enableLiveAutocompletion: true,\n  enableSnippets: true,\n  focus: false,\n  fontSize: 14,\n  highlightActiveLine: true,\n  navigateToFileEnd: true,\n  placeholder: null,\n  readOnly: false,\n  scrollMargin: [15, 15, 0, 0],\n  setOptions: defaultOptions,\n  showGutter: true,\n  showPrintMargin: false,\n  style: {},\n  tabSize: 4,\n  width: \"auto\",\n  debounceChangePeriod: 250,\n}\n\nconst GlobalCSS = createGlobalStyle<{isDisabled?: boolean, inject: string}>`\n  html {\n    opacity: ${props => props.isDisabled? \"0.5\": \"1\"};\n    cursor: ${props => props.isDisabled? \"not-allowed\": \"auto\"};\n    pointer-events: ${props => props.isDisabled? \"none\": \"auto\"};\n  }\n  body {\n    margin: 0;\n    padding: 0;\n  }\n  ${props => props.inject}\n`\nconst StyledCodeEditor = styled.div`\n  width: 100%;\n  border-radius: 8px;\n  overflow: hidden;\n  display: flex;\n  flex-direction: column;\n  :hover button {\n    opacity: 1;\n    transform: scale(1);\n  }\n  button.always-on {\n    opacity: 1;\n    transform: scale(1);\n    transition: none;\n  }\n  :hover button svg {\n        opacity: 1;\n        transform: scale(1);\n  }\n  :hover button.with-icon span {\n    opacity: 1;\n    transform: scale(1);\n  }\n  button.always-on > span {\n    opacity: 1;\n    transform: scale(1);\n    transition: none;\n  }\n  button.always-on > svg {\n    opacity: 1;\n    transform: scale(1);\n    transition: none;\n  }\n  `;\n\nconst CodeEditor = ({ args, width, disabled, theme }: CodeEditorProps) => {\n\n  //sets code to the initial value every time the component is rendered\n  //to set the initial value once, use a function instead of a value.\n  const [code, setCode] = useState(args['code']);\n  // const [keybindingAddRemove, setKeybindingAddRemove] = useState([\"\",\"\"]);\n\n  const aceEditor = useRef<AceEditor>(null);\n  const infoTextRef = useRef<HTMLSpanElement>(null);\n  const baseSession = useRef<ace.Ace.EditSession | null>(null);\n  const keepFocus = useRef<boolean>(false);\n  const reset = useRef<boolean>(false);\n\n  var timeoutId: NodeJS.Timeout;\n\n  /**\n    * This function takes as input either a snippetText string that is expected\n    * to be already formatted like the text in a SnippetFile or a dictionary or \n    * and array of dictionaries. For the first case, it just returns the input.\n    * For the second and third case, a (SnippetFile format) string is constructed\n    * from the dict(s) and returned. Learn more about snippets {@link  here}\n    * @param snippetRaw snippets to be converted to a single snippetText string\n    * @returns {string} snippetText\n    */\n  const createSnippets = (snippetRaw: string | object | [object]): string => {\n    return (typeof snippetRaw === \"string\" ? snippetRaw : (Array.isArray(snippetRaw) ? snippetRaw : [snippetRaw]).map(({ name, code }) =>\n    ([\n      'snippet ' + name,\n      code.split('\\n')\n        .map((c: string) => '\\t' + c)\n        .join('\\n'),\n    ].join('\\n'))\n    ).join('\\n'))\n  }\n  const [snippetAddRemove, setSnippetAddRemove] = useState({[args['lang']] : [createSnippets(args[\"snippets\"][0]), createSnippets(args[\"snippets\"][1])]});\n  const [keybindingAddRemove, setKeybindingAddRemove] = useState(args['keybindings']);\n\n\n  useEffect(() => {\n    return () => {\n      if (timeoutId) {\n        clearTimeout(timeoutId);\n      }\n    }\n  }, []);\n\n  useEffect(() => {\n    if(aceEditor.current && keepFocus.current){\n      aceEditor.current.editor.focus();\n      keepFocus.current = false;\n    }\n  }, [keepFocus.current]);\n\n  // To reasons for the useEffect here: \n  //   1. to set the focus on the editor only when the focus argument has changed to true.\n  //   2. to set the focus on the editor after rendering the component at which point, the \n  //      editor should be ready.\n  useEffect(() => {\n    if(aceEditor.current && args.focus){\n      aceEditor.current.editor.focus();\n    }\n  }, [args.focus]);\n\n  const onChangeHandler = (newCode: string) => {\n    setCode(newCode);\n  }\n\n  // commands is an array of objects containing functions\n  // that the editor can be triggered to call.\n  const commands = { commands: [\n    {\n      name: 'submit', //name for the key binding.\n      description: \"Send 'submit' response\", //description of the command\n      bindKey: { win: 'Ctrl-Enter', mac: 'Command-Enter' }, //key combination used for the command.\n      exec: (editor: any) => {\n        const outgoingMode = editor.getSession().$modeId.split(\"/\").pop();\n        Streamlit.setComponentValue({text: editor.getValue(), type: \"submit\", lang: outgoingMode });\n      }\n    },\n    {\n      name: 'saveState',\n      description: \"Save state\",\n      bindKey: { win: 'Ctrl-Alt-S', mac: 'Command-Alt-S' },\n      exec: (editor: ace.Ace.Editor) => {\n        setCode(editor.getValue());\n      }\n    },\n    {\n      name: 'copyAll',\n      description: \"Copy all text to clipboard\",\n      exec: (editor: ace.Ace.Editor) => {\n        unsecureCopyTextToClipboard(editor.getValue());\n      }\n    },\n    {\n      name: 'reset',\n      exec: () => {\n        resetEditor();\n      }\n    },\n    {\n      name: 'keepFocus',\n      description: \"Return cursor to editor\",\n      exec: () => {\n        keepFocus.current = true;\n      }\n    },\n    {\n      name: \"setMode\",\n      description: \"Set language mode\",\n      exec: (editor: ace.Ace.Editor, lang: string) => {\n          if(lang && typeof lang === \"string\")\n            editor.getSession().setMode(\"ace/mode/\" + lang);\n      },\n      readOnly: true\n    },\n    {\n      name: \"changeShortcuts\",\n      description: \"Switch shortcuts\",\n      exec: (editor: any, shortcuts?: string) => {\n        if(shortcuts && typeof shortcuts === \"string\")\n          editor.setKeyboardHandler(\"ace/keyboard/\" + shortcuts);\n        else {\n          //rotate through the available keyboard handlers\n          const handlers = [\"ace/keyboard/vim\", \"ace/keyboard/emacs\", \"ace/keyboard/sublime\", \"ace/keyboard/vscode\"];\n          const currentHandler = handlers[(handlers.indexOf(editor.$keybindingId) + 1) % 4];\n          editor.setKeyboardHandler(currentHandler);\n        }\n      },\n      readOnly: true\n    },\n    {\n      name: 'toggleKeyboardShortcuts',\n      exec: (editor: ace.Ace.Editor) => {\n        if(!document.getElementById('kbshortcutmenu'))\n          editor.execCommand('showKeyboardShortcuts');\n        else \n          editor.execCommand('simulateKeyPress', {type:\"keydown\", keyCode: 27});\n      }\n    },\n    {\n      name: 'simulateKeyPress',\n      exec: (editor: ace.Ace.Editor, args: {type: string, key?: string, keyCode?: number}) => {\n        if(args.key)\n          document.dispatchEvent(new KeyboardEvent(args.type,{'key': args.key})); \n        else if(args.keyCode)\n          document.dispatchEvent(new KeyboardEvent(args.type,{'keyCode': args.keyCode})); \n      }\n    },\n    {\n      name: 'infoMessage',\n      description: \"Display message in info bar\",\n      exec: (editor: ace.Ace.Editor, args: {text: string, timeout?: number, classToggle?: string, targetQueryString?: string} ) => {\n        if(args.targetQueryString){\n          const target = document.querySelector(args.targetQueryString) as HTMLElement;\n          if(target){\n            target.innerText = args.text;\n            target.classList.add(args.classToggle || \"\")\n            if(args.timeout){\n              timeoutId = setTimeout(() => {\n                target.classList.remove(args.classToggle || \"\");\n              }, args.timeout);\n            }\n          }\n        }\n        else if(infoTextRef.current){\n          infoTextRef.current.innerText = args.text;\n          infoTextRef.current.classList.add(args.classToggle || \"\");\n          if(args.timeout){\n            timeoutId = setTimeout(() => {\n              infoTextRef.current?.classList.remove(args.classToggle || \"\");\n            }, args.timeout);\n          }\n        }\n      }\n    },\n    {\n      name: 'response', //name for the key binding.\n      description: \"Send custom response\", //description of the command\n      exec: (editor: any, responseType = \"\") => {\n        const outgoingMode = editor.getSession().$modeId.split(\"/\").pop();\n        Streamlit.setComponentValue({ text: editor.getValue(), type: responseType, lang: outgoingMode });\n      }\n    },\n    {\n      name: 'editSnippets',\n      description: \"Edit snippets\",\n      bindKey: { win: 'Ctrl-Alt-M', mac: 'Command-Alt-M' },\n      exec: (editor: any) => {\n        const snippetManager = ace.require('ace/snippets').snippetManager;\n        if(baseSession.current){\n          const outgoingMode = editor.getSession().$modeId.split(\"/\").pop();\n          if(outgoingMode === \"snippets\"){\n            const snippetText = editor.getSession().getValue();\n            editor.setSession(baseSession.current);\n            baseSession.current = null;\n            setCode(editor.getSession().getValue());\n            if(outgoingMode === \"snippets\"){}\n            try{\n              const snippetsPlusMinus = snippetText.split(\"###~~~\")[1];\n              const [snippetsPlus, snippetsMinus] = snippetsPlusMinus.split(\"###---\");\n              const snippetsToAdd = snippetsPlus.split(\"###+++\")[1];\n              const snippetsToRemove = snippetsMinus;\n              const langMode = editor.getSession().$modeId.split(\"/\").pop();\n              setSnippetAddRemove({[langMode] : [snippetAddRemove[langMode][0] + snippetsToAdd, snippetAddRemove[langMode][1] + snippetsToRemove]});\n            } catch (error) {\n              editor.execCommand(\"infoMessage\",{text: \"error parsing file, restoring original file\", timeout: 2000, classToggle: \"show\"});\n            }\n          }\n        } else {\n          const langMode = editor.getSession().$modeId.split(\"/\").pop()\n          const snippetConcatText = `\\n###~~~#(DO NOT EDIT THIS LINE)\n# Commented out above are all the snippets that are currently\n# registered for ${args['lang']} mode.\n\\n\\n###+++#(DO NOT EDIT THIS LINE) \\n# Put the snippets you want to add below this line.\\n\\n\\n\\n\n\\n\\n\\n###---#(DO NOT EDIT THIS LINE) \\n# Put the snippets you want to remove below this line.\\n\\n\\n\\n\\n\\n\\n`;\n          const snippetText = \"#\" + createSnippets(snippetManager.snippetMap[langMode].map((snip: any) => ({name: snip.name, code: snip.content}))).replace(/\\n/g, \"\\n#\") + snippetConcatText;\n          // snippetManager.files[editor.getSession().$modeId].snippetText\n          const lineCount = (snippetText.match(/\\n/g) || []).length;\n          baseSession.current = editor.getSession();\n          const snippetsSession = ace.createEditSession(snippetText, \"ace/mode/snippets\");\n          editor.setSession(snippetsSession);\n          const cursorPos = {row: (lineCount - 15)>0? lineCount - 15 : 0, column: 0};\n          editor.moveCursorTo(cursorPos.row, cursorPos.column);\n          editor.renderer.scrollCursorIntoView(cursorPos, 0.5);\n        }\n      }\n    },\n    {\n      name: 'editKeyBindings',\n      description: \"Edit keybindings\",\n      bindKey: { win: 'Ctrl-Alt-B', mac: 'Command-Alt-B' },\n      exec: (editor: any) => {\n        ace.require('ace/autocomplete').Autocomplete.for(editor);\n        if(baseSession.current){\n          const outgoingMode = editor.getSession().$modeId.split(\"/\").pop();\n          if(outgoingMode === \"json\"){\n            const keybindingsJSON = editor.getSession().getValue();\n            editor.setSession(baseSession.current);\n            baseSession.current = null;\n            setCode(editor.getSession().getValue());\n            try{\n              setKeybindingAddRemove(JSON.parse(keybindingsJSON));\n            } catch (error) {\n              editor.execCommand(\"infoMessage\",{text: \"error parsing file, restoring original file\", timeout: 2000, classToggle: \"show\"});\n            }\n          }\n        } else {\n          const keybindings = {commands: {}, completer: {}};\n          if(editor.completer && editor.completer.keyboardHandler.commands){\n            keybindings.completer = Object.keys(editor.completer.keyboardHandler.commands).map((key: any) => ({bindkey: editor.completer.keyboardHandler.commands[key].bindKey ?? \"\", name: editor.completer.keyboardHandler.commands[key].name}));\n          }\n          if(editor.commands.commands){\n            keybindings.commands = Object.keys(editor.commands.commands).map((key: any) => ({bindkey: editor.commands.commands[key].bindKey ?? \"\", name: editor.commands.commands[key].name}));\n          }\n          const keybindingsJSON = JSON.stringify(keybindings, undefined, 2);\n          baseSession.current = editor.getSession();\n          const keybindingsSession = ace.createEditSession(keybindingsJSON, \"ace/mode/json\");\n          editor.setSession(keybindingsSession);\n        }\n      }\n    },\n    {\n      name: 'exitSession', //name for the key binding.\n      bindKey: { win: 'Esc', mac: 'Esc' },\n      description: \"Return to main session (keep changes)\", //description of the command\n      exec: (editor: any) => {\n        if(baseSession.current){\n          const mode = editor.getSession().$modeId.split(\"/\").pop();\n          if (mode === \"snippets\")\n            editor.execCommand(\"editSnippets\");\n          else if (mode === \"json\")\n            editor.execCommand(\"editKeyBindings\");\n        }\n      }\n    },\n    {\n      name: 'abandonSession', //name for the key binding.\n      bindKey: { win: 'Ctrl-Alt-Esc', mac: 'Command-Alt-Esc' },\n      description: \"Return to main session (discard changes)\", //description of the command\n      exec: (editor: any) => {\n        if(baseSession.current){\n          editor.setSession(baseSession.current);\n          baseSession.current = null;\n          setCode(editor.getSession().getValue());\n        }\n      }\n    },\n    {\n      name: 'classART', //name for the key binding.\n      description: \"Add/Remove/Toggle class for element\", //description of the command\n      exec: (editor: any, args: {targetQueryString: string, type: string, class: string}) => {\n        if(args.targetQueryString && args.type && args.class){\n          switch(args.type){\n            case \"add\":\n              document.querySelectorAll(args.targetQueryString)?.forEach((el: any) => el.classList.add(args.class));\n              break;\n            case \"remove\":\n              document.querySelectorAll(args.targetQueryString)?.forEach((el: any) => el.classList.remove(args.class));\n              break;\n            case \"toggle\":\n              document.querySelectorAll(args.targetQueryString)?.forEach((el: any) => el.classList.toggle(args.class));\n              break;\n            default:\n              break;\n          }\n        }\n      }\n    },\n    {\n      name: 'conditionalExecute', //name for the key binding.\n      description: \"Execute command if element exists\", //description of the command\n      exec: (editor: any, args: {targetQueryString: string, command: any[], condition?: boolean}) => {\n        if(args.targetQueryString && args.command && Array.isArray(args.command)){\n          if(!(args.condition ?? true) === !document.querySelector(args.targetQueryString)){\n            typeof args.command[0] === \"string\" ? execute(args.command[0], args.command[1]) : console.warn(\"Editor command - conditionalExecute: improper command format! Command array must contain name of command as first element and arguments as second element.\");\n          }\n        }\n      }\n    }\n  ]};\n\n  const execute = (command: string, args: any = \"\") => {\n    const editor = aceEditor.current?.editor;\n    if (editor) {\n      if (!args) {\n        editor.execCommand(command)\n      }\n      else if (typeof args === \"number\" || typeof args === \"string\") {\n        editor.execCommand(command, args);\n      }\n      else if (typeof args === \"object\" && !Array.isArray(args)) {\n        var containsNumsStr = true;\n        Object.keys(args).forEach((key: any) => {\n          containsNumsStr = typeof args[key] === \"string\" || typeof args[key] === \"number\" || Array.isArray(args[key]);\n        });\n        if (Object.keys(args).length < 4 && containsNumsStr) {\n          editor.execCommand(command, args);\n        }\n      }\n      else {\n        console.warn(`Function - execute: failed to parse/execute \"${command}\" command!`);\n      }\n    }\n  }\n\n  const executeAll = (commands: any[]) => {\n    commands.forEach(singleCommand => {\n      if (Array.isArray(singleCommand)) {\n        typeof singleCommand[0] === \"string\" ? execute(singleCommand[0], singleCommand[1]) : console.warn(\"Function - executeAll: improper command format! Singular commands must contain name of command as first element and arguments as second element.\");\n      } else if (typeof singleCommand === \"string\") {\n        execute(singleCommand);\n      } else {\n        console.warn(\"Function - executeAll: failed to parse/execute command(s)!\");\n      }\n    });\n  }\n\n  const resetEditor = () => {\n    setCode(args['code']);\n  }\n\n  const unsecureCopyTextToClipboard = (text: string) => {\n    const textField = document.createElement('textarea');\n    textField.value = text;\n    document.body.appendChild(textField);\n    textField.select();\n    document.execCommand('copy');\n    textField.remove();\n  }\n\n  /**\n   * resizeObserver observes changes in elements its given to observe and is used here\n   * to communicate to streamlit the height of the component that has changed\n   * so that streamlit can adjust the iframe containing the component accordingly.\n   */\n  const resizeObserver = new ResizeObserver((entries: any) => {\n    // If we know that the body will always fully contain our component (without cutting it off)\n    // then we can use docuemnt.body height instead\n    Streamlit.setFrameHeight((entries[0].contentBoxSize.blockSize ?? entries[0].contentRect.height)); \n  })\n\n  const observe = (divElem: any) => {\n    divElem ? resizeObserver.observe(divElem as HTMLDivElement) : resizeObserver.disconnect();\n  }\n\n  // This useEffect is used to reset the editor when the code argument changes and\n  // the allow_reset argument is true. The allow_reset argument only impacts the\n  // behavior of the component when the component has a fixed key argument because\n  // changing the key argument results in the creation of a new component instance.\n  // Everything would be reset anyways.\n  useEffect(() => {\n    if (args['allow_reset'] === true && args['code'] !== code) {\n      reset.current = !reset.current;\n      resetEditor();\n    }\n  }, [args['code']]);\n\n  /**\n   * This could also be memoized but I don't think it would be necessary because its not expensive.\n   */\n  const themeChoice = () => {\n    const isDarkTheme = theme? theme.base === \"dark\" : true;\n    switch (args['theme']) {\n      case \"contrast\":\n        return isDarkTheme? \"streamlit_light\" : \"streamlit_dark\";\n      case \"light\":\n        return \"streamlit_light\";\n      case \"dark\":\n        return \"streamlit_dark\";\n      case \"default\":\n        return isDarkTheme? \"streamlit_dark\" : \"streamlit_light\";\n      default:\n        return isDarkTheme? \"streamlit_dark\" : \"streamlit_light\";\n    }\n  }\n\n  const themeProp = themeChoice();\n  const componentContainerProps = args[\"component_props\"];\n\n  const {info: infoArg, menu: menuArg, focus: focusArg, code: codeArg, ...rest} = args;\n  const editorArgsString = JSON.stringify(rest);\n  const menuArgsString = JSON.stringify(menuArg);\n  const infoArgsString = JSON.stringify(infoArg);\n  const buttonArgsString = JSON.stringify(args['buttons']);\n  const themeString = JSON.stringify(theme);\n  const snippets = JSON.stringify(snippetAddRemove);\n\n  /**\n   * This section contains the main sub-components (child components). These components are wrapped in useMemos\n   * in order to prevent unnecessary re-rendering of the components. This is listed as one of its use cases in the\n   * React docs ({@link https://beta.reactjs.org/reference/react/useMemo#skipping-re-rendering-of-components Skipping re-rendering of components})\n   *\n   * This component is the editor component that is rendered. It is only re-rendered when\n   * certain properties change. This is important because we should account for the possibility that the editor \n   * is being used at any given moment. Unnecessary and frequent re-rendering of the editor (for outside reasons\n   * especially) can impact user experience and responsiveness.\n   */\n  const editor = useMemo(() => {\n    const keybindings = JSON.stringify(keybindingAddRemove);\n    const revertedArgs = JSON.parse(editorArgsString);\n\n    // Create commands for each button\n    if(revertedArgs['buttons'].length > 0) {\n      revertedArgs['buttons'].forEach((button: any) => {\n          commands.commands = [...commands.commands, {\n            name: (button.name as string).trim().replace(/\\s+/g, '_') + '_button',\n            description: \"Execute '\" + button.name + \"' button command(s)\",\n            exec: () => {\n            executeAll(button.commands);\n          }}];\n      });\n    }\n\n    let heightProps = {};\n    if(typeof revertedArgs['height'] === \"number\") \n      heightProps = {minLines: 1, maxLines: revertedArgs['height']};\n    else if(typeof revertedArgs['height'] === \"string\") \n      heightProps = {height: revertedArgs['height']};\n    else if(Array.isArray(revertedArgs['height']) && revertedArgs['height'].length === 2) \n      heightProps = {minLines: revertedArgs['height'][0], maxLines: revertedArgs['height'][1]};\n\n    const aceEditorProps = { ...defaultEditorProps, ...revertedArgs['editorProps'] };\n    const aceOptions = { ...defaultOptions, ...revertedArgs['options'] };\n    const partProps = { setOptions: aceOptions, editorProps: aceEditorProps };\n    const aceProps = { ...defaultProps, ...partProps,...heightProps, ...revertedArgs['props'] };\n\n    /**\n     * TODO: Remove props from aceProps that we don't want to allow user access to.\n     */\n    return (\n        <Editor\n         editorRef={aceEditor}\n         code={code} \n         lang={revertedArgs['lang']} \n         theme={themeProp} \n         shortcuts={revertedArgs['shortcuts']} \n         snippetString={snippets} \n         commands={commands.commands} \n         keybindingString={keybindings} \n         props={aceProps} \n         onChange={(value) => onChangeHandler(value)} />\n      );\n  }, [editorArgsString, themeProp, snippets, keybindingAddRemove, reset.current]);\n\n  const buttons = useMemo(() => {\n    const revertedButtons = JSON.parse(buttonArgsString);\n    const revertedTheme = JSON.parse(themeString);\n    const customButtonTheme = revertedTheme ?? {};\n    const customButtons = {buttons: (revertedButtons ?? []) as customButton[], name: \"customButtons\"} as buttonGroup;\n    return (\n      < ButtonSet\n       buttonGroup={customButtons} \n       theme={customButtonTheme} \n       themeProp={themeProp} \n       executeAll={(commands) => executeAll(commands)} />\n    );\n  }, [buttonArgsString, themeString, themeProp]);\n\n  const menu = useMemo(() => {\n    const revertedMenu = JSON.parse(menuArgsString);\n    const revertedTheme = JSON.parse(themeString);\n    const menuTheme = revertedTheme ?? {};\n    return (\n      <ButtonMenu\n       menu={revertedMenu} \n       theme={menuTheme} \n       themeProp={themeProp} \n       executeAll={(commands) => executeAll(commands)} />\n    );\n  }, [menuArgsString, themeString, themeProp]);\n\n  const info = useMemo(() => {\n    const revertedInfo = JSON.parse(infoArgsString);\n    const revertedTheme = JSON.parse(themeString);\n    const infoTheme = revertedTheme ?? {};\n    return (\n      <InfoBar\n       infoRef={infoTextRef} \n       info={revertedInfo} \n       theme={infoTheme} />\n    );\n  }, [infoArgsString, themeString]);\n\n  const globalCSS = useMemo(() => {\n    return (\n      <GlobalCSS isDisabled={disabled} inject={componentContainerProps.globalCSS} />\n    );\n  }, [componentContainerProps.globalCSS, disabled]);\n\n  return (\n    <StyledCodeEditor ref={observe} style={componentContainerProps.style} css={componentContainerProps.css} className={\"streamlit_code-editor \" + theme?.base ?? \"\" } >\n      {globalCSS}\n      {editor}\n      {buttons}\n      {menu}\n      {info}\n    </StyledCodeEditor>\n  )\n}\n\nexport default withStreamlitConnection(CodeEditor)",
         "// / <reference types=\"styled-components/cssprop\" />\nimport React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport CodeEditor from \"./CodeEditor\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <CodeEditor />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/runtime-main.ad47a231.js` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/runtime-main.ad47a231.js`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/code_editor/frontend/build/static/js/runtime-main.ad47a231.js.map` & `streamlit-code-editor-0.1.2/code_editor/frontend/build/static/js/runtime-main.ad47a231.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-code-editor-0.1.1/setup.py` & `streamlit-code-editor-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-code-editor",
-    version="0.1.1",
+    version="0.1.2",
     author="Anas Bouzid",
     author_email="anasbouzid@gmail.com",
     description="React-ace editor customized for Streamlit",
     long_description="React-ace component with custom themes wrapped with customizable interface elements for better integration as a Streamlit code editor",
     long_description_content_type="text/plain",
     url="https://github.com/bouzidanas/streamlit.io/tree/dev/streamlit-code-editor",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-code-editor-0.1.1/streamlit_code_editor.egg-info/SOURCES.txt` & `streamlit-code-editor-0.1.2/streamlit_code_editor.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -450,16 +450,16 @@
 code_editor/frontend/build/fe10bf958ca84418c6af95259c7b4260.js
 code_editor/frontend/build/fe64d890e7fa0c0beae6f2e7a96a7ede.js
 code_editor/frontend/build/ff8b71b1bce6feb81065d8340e07dfeb.js
 code_editor/frontend/build/index.html
 code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js
 code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js.LICENSE.txt
 code_editor/frontend/build/static/js/2.2eaf9c7f.chunk.js.map
-code_editor/frontend/build/static/js/main.571a6b52.chunk.js
-code_editor/frontend/build/static/js/main.571a6b52.chunk.js.map
+code_editor/frontend/build/static/js/main.028f53cc.chunk.js
+code_editor/frontend/build/static/js/main.028f53cc.chunk.js.map
 code_editor/frontend/build/static/js/runtime-main.ad47a231.js
 code_editor/frontend/build/static/js/runtime-main.ad47a231.js.map
 streamlit_code_editor.egg-info/PKG-INFO
 streamlit_code_editor.egg-info/SOURCES.txt
 streamlit_code_editor.egg-info/dependency_links.txt
 streamlit_code_editor.egg-info/requires.txt
 streamlit_code_editor.egg-info/top_level.txt
```

