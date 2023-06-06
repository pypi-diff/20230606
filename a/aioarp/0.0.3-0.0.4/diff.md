# Comparing `tmp/aioarp-0.0.3.tar.gz` & `tmp/aioarp-0.0.4.tar.gz`

## Comparing `aioarp-0.0.3.tar` & `aioarp-0.0.4.tar`

### file list

```diff
@@ -1,209 +1,215 @@
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 aioarp-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aioarp-0.0.3/requirements.txt
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aioarp-0.0.3/unasync.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.3/.github/workflows/main.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/120fd5a3e305da5b
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/12101680e8031881
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/16b1a595f0c0b695
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/17946c0e3734f56
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/18bd9323e775c06
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1911b721541a132
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1a43e2fa66cc521
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1bfc7af844c09624
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1c4766f25c290393
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1cf748db3edf4393
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/1d813f87eae436dc
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/20360c87813708ee
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/20b471ae4ae2c716
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/20cf28b4a08829e
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/20e8c6fb6ec65fba
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/22273ee756d2aeab
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/22eb75e2705cd7cb
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/258218bd1af61054
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/259f2d45c9b5e8f8
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/259f7be1f71aae17
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/27380b38303cddd4
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/277c58fd0e92dc6f
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/2894d2afe73e6dee
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/28bfffee8af0f637
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/29a3dfb41b2e153e
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/29ec5304bead68a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/2b17b1ab21ba1879
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/2b74d3f1efd79c7b
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/2f2908e30cbaaf6f
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/3546886ec7b89ca2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/3a9f29e79b12106b
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/3c82c38fdeb726f5
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/3cf42c96bb03e8e
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/40ec6c4657092d14
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/42d47131a22f033d
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/44618acc04af2a98
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/464ea8dcb036f50b
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/48dc01dafed313cb
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4bfeb322489be7b2
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4c18fbd43c6124d9
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4c7aefddb4afaa07
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4ce11f41c925600e
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4d80d8cbd7abb331
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4dcc3bf9688e8634
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/4e4abc9127fe2106
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/522c23633820a258
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/5259c25c40a66c52
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/53480da31b2357be
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/536385ed3a8bbf59
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/53922c565bc4cfdf
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/54ca2556c07eb0e4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/57ee6e97f4833ae1
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/5845e4d7f49b3f6b
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/590fd00a0401d086
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/5e5e4a02dc426617
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/608e0f7e2331dfd0
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6190d891377c8571
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6269535ee79a68b3
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6390cd3a2155b002
--rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/64f9f289e0610564
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6572fa7cae8df134
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/65bac7c6a4c4cb5e
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/65d6dc214750c212
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6857c9063a540073
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/68e278cd0a30d24c
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6aa5b22c44c81236
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6aee26157f3848b9
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6b926a7206e2e0f5
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6ba798af16bd34e5
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6dbcf7ab6c32f876
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6de1f164718890ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/6ec79cb0a99a4ffa
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/70ee6f5e2e8b7d90
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/75d5cb975af2bc07
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/7753615b71d6a36e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/78dc31b63dbd1e69
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/79da2ffd4120460
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/7d0a3cccefcd7db3
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/7f23f9f7d375f4fd
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/80b8f04bc59d958c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/82b9ee56f8fed787
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8362e113a849836
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/841d7ee35702e48e
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/85532fbdb4ec8100
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/859b9d135acd891b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/85a7bda1ebac02be
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/869f865c9f14daf7
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/879246cf978566b8
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/89ad75a37b7215d3
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8af090de0021767
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8ba2e035b666505
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8caa6ea7d00a8ef9
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8e5085aaf38947dd
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/8e9682f1b99c3026
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/93389fd7b221ce32
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/936f955f01285847
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/94a86b805b8c04e2
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/9600ec5b79137dcc
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/967dc6947ad8c113
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/990e2b74e6a14435
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/9db40d9bd33cc32a
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a0edd6b97fbe3e68
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a12cec0addd27620
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a22627f4ad982518
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a41b182cef331aa5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a42de4efa897ae1e
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a5253384caf62eef
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a62236fd623ff7ad
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a64cd85354e281c5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/a7b52a5c13a67fed
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/aabe170d14233a1f
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/aac73f953da24b03
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/ac1d91a6ebb4bed9
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/aced40484cbf3132
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/adb7c2d2342ef983
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/b27cd0e5108544e0
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/b3202a665cec273b
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/b74ab4e72907ed4b
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/b752bc22791212b3
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/b874aac73807837a
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bb3a8375be948e99
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bb98194f279aef4d
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bc9d2b60dadbf05e
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bd0ea26a717d1380
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bd3e6a97ee360bd7
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bdd7c44b4f88bf5b
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/bffaaf1ee55da212
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c0cc1810bd812c85
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c0d92e761aa72a56
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c12c935be2da0714
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c24cf3b955d01f58
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c2e7f8eb8bfe8525
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c370f17718b5228b
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c3b1cc9370bb49b5
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c54b124e74d7c29a
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c64725c588d56756
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c6c7c5bdc9a58d71
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c78c3248c370d9f2
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c7a507ee84d3e2ab
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/c908c9d3ee0eb43c
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/cc374f0497dbc539
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/cc5595ab776e807c
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/cd40078ccedf2012
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/cd84fa1ee95c780c
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/cdc31ad9b3ea9979
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/d08cf74ff5eeb16e
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/d3d46de068ceaf65
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/d4ed3103ad57bd80
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/d8259ee38b03fc0e
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/dc53fc214ceea0dd
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/de93c4dfa993ec19
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e11920c476dc4f59
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e12d636458d129da
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e25cfbd84c59869
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e2a8017124da7733
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e305b1c5b826225
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e512a2b647437caa
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e84bd53ae32ad4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e8f0ea35cc3b448a
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/e9d1ab2b1a8c3cca
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/eb250aff0edc4ecb
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/eee42766c50b6490
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f0ff9ca6cba080b9
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f2ebd390a47aa1cd
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f3ac79af6cdde497
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f3d289f55f0ad6bd
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f45e36470415dca1
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f56e6b11a3d4a68b
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f58c3d661899d706
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/f96d453d0b6b9c85
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/fb10e8087c484390
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/fd508bd27e156044
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aioarp-0.0.3/.ruff_cache/content/ffe7d79671eca8f
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/__about__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/__init__.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_arp.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_async.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_client.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_exceptions.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_mock.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_sync.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_utils.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/defaults.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_backends/__init__.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_backends/_async.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_backends/_base.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_backends/_mock.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 aioarp-0.0.3/aioarp/_backends/_sync.py
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 aioarp-0.0.3/scripts/check
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.3/scripts/lint
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.3/scripts/test
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/test_async.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/test_client.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/test_proto.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/test_sync.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.3/tests/test_utils.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 aioarp-0.0.3/README.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 aioarp-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 aioarp-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aioarp-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aioarp-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aioarp-0.0.4/unasync.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aioarp-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 aioarp-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/120fd5a3e305da5b
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/12101680e8031881
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/16b1a595f0c0b695
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/17946c0e3734f56
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/18bd9323e775c06
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1911b721541a132
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1a43e2fa66cc521
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1bfc7af844c09624
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1c4766f25c290393
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1cf748db3edf4393
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/1d813f87eae436dc
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/20360c87813708ee
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/20b471ae4ae2c716
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/20cf28b4a08829e
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/20e8c6fb6ec65fba
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/22273ee756d2aeab
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/22eb75e2705cd7cb
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/23b5bf7a560a3d85
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/258218bd1af61054
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/259f2d45c9b5e8f8
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/259f7be1f71aae17
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/27380b38303cddd4
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/277c58fd0e92dc6f
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/2894d2afe73e6dee
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/28bfffee8af0f637
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/29459fb899e6be63
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/29a3dfb41b2e153e
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/29ec5304bead68a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/2b17b1ab21ba1879
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/2b74d3f1efd79c7b
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/2f2908e30cbaaf6f
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/3546886ec7b89ca2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/3a9f29e79b12106b
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/3c82c38fdeb726f5
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/3cf42c96bb03e8e
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/40ec6c4657092d14
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/42d47131a22f033d
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/44618acc04af2a98
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/464ea8dcb036f50b
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/48dc01dafed313cb
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4bfeb322489be7b2
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4c18fbd43c6124d9
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4c7aefddb4afaa07
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4ce11f41c925600e
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4d80d8cbd7abb331
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4dcc3bf9688e8634
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/4e4abc9127fe2106
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/522c23633820a258
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/5259c25c40a66c52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/53480da31b2357be
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/536385ed3a8bbf59
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/53922c565bc4cfdf
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/54ca2556c07eb0e4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/57ee6e97f4833ae1
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/5845e4d7f49b3f6b
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/590fd00a0401d086
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/5e5e4a02dc426617
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/608e0f7e2331dfd0
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6190d891377c8571
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6269535ee79a68b3
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6390cd3a2155b002
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/64f9f289e0610564
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6572fa7cae8df134
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/65bac7c6a4c4cb5e
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/65d6dc214750c212
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6857c9063a540073
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/68e278cd0a30d24c
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6aa5b22c44c81236
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6aee26157f3848b9
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6b926a7206e2e0f5
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6ba798af16bd34e5
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6dbcf7ab6c32f876
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6de1f164718890ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/6ec79cb0a99a4ffa
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/70ee6f5e2e8b7d90
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/75d5cb975af2bc07
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/7753615b71d6a36e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/78dc31b63dbd1e69
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/79da2ffd4120460
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/7d0a3cccefcd7db3
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/7f23f9f7d375f4fd
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/80b8f04bc59d958c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/82b9ee56f8fed787
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8362e113a849836
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/837a3e06585749a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/841d7ee35702e48e
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/85532fbdb4ec8100
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/859b9d135acd891b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/85a7bda1ebac02be
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/869f865c9f14daf7
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/879246cf978566b8
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/89ad75a37b7215d3
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8af090de0021767
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8ba2e035b666505
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8caa6ea7d00a8ef9
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8e5085aaf38947dd
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/8e9682f1b99c3026
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/93389fd7b221ce32
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/936f955f01285847
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/94a86b805b8c04e2
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/9600ec5b79137dcc
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/967dc6947ad8c113
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/990e2b74e6a14435
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/9db40d9bd33cc32a
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a0edd6b97fbe3e68
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a12cec0addd27620
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a22627f4ad982518
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a41b182cef331aa5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a42de4efa897ae1e
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a5253384caf62eef
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a62236fd623ff7ad
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a64cd85354e281c5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/a7b52a5c13a67fed
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/aabe170d14233a1f
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/aac73f953da24b03
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/ac1d91a6ebb4bed9
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/ace8365de45531
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/aced40484cbf3132
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/adb7c2d2342ef983
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b1ec491bf059cec3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b27cd0e5108544e0
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b3202a665cec273b
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b74ab4e72907ed4b
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b752bc22791212b3
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/b874aac73807837a
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bb3a8375be948e99
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bb98194f279aef4d
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bc9d2b60dadbf05e
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bd0ea26a717d1380
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bd3e6a97ee360bd7
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bdd7c44b4f88bf5b
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/bffaaf1ee55da212
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c0cc1810bd812c85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c0d92e761aa72a56
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c12c935be2da0714
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c24cf3b955d01f58
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c2e7f8eb8bfe8525
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c370f17718b5228b
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c3b1cc9370bb49b5
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c54b124e74d7c29a
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c64725c588d56756
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c6c7c5bdc9a58d71
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c78c3248c370d9f2
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c7a507ee84d3e2ab
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/c908c9d3ee0eb43c
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/cc374f0497dbc539
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/cc5595ab776e807c
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/cd40078ccedf2012
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/cd84fa1ee95c780c
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/cdc31ad9b3ea9979
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/d08cf74ff5eeb16e
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/d3d46de068ceaf65
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/d4ed3103ad57bd80
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/d8259ee38b03fc0e
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/dc53fc214ceea0dd
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/de93c4dfa993ec19
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e11920c476dc4f59
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e12d636458d129da
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e25cfbd84c59869
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e2a8017124da7733
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e305b1c5b826225
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e512a2b647437caa
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e84bd53ae32ad4a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e8f0ea35cc3b448a
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/e9d1ab2b1a8c3cca
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/eb250aff0edc4ecb
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/eee42766c50b6490
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f0ff9ca6cba080b9
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f2ebd390a47aa1cd
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f3ac79af6cdde497
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f3d289f55f0ad6bd
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f45e36470415dca1
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f56e6b11a3d4a68b
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f58c3d661899d706
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/f96d453d0b6b9c85
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/fb10e8087c484390
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/fd508bd27e156044
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aioarp-0.0.4/.ruff_cache/content/ffe7d79671eca8f
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/__about__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/__init__.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_arp.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_async.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_client.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_exceptions.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_mock.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_sync.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_utils.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/defaults.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_backends/__init__.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_backends/_async.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_backends/_base.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_backends/_mock.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 aioarp-0.0.4/aioarp/_backends/_sync.py
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 aioarp-0.0.4/scripts/check
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.4/scripts/lint
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.4/scripts/test
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/test_async.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/test_client.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/test_proto.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/test_sync.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.4/tests/test_utils.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aioarp-0.0.4/README.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 aioarp-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 aioarp-0.0.4/PKG-INFO
```

### Comparing `aioarp-0.0.3/unasync.py` & `aioarp-0.0.4/unasync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/120fd5a3e305da5b` & `aioarp-0.0.4/.ruff_cache/content/120fd5a3e305da5b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/16b1a595f0c0b695` & `aioarp-0.0.4/.ruff_cache/content/16b1a595f0c0b695`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/18bd9323e775c06` & `aioarp-0.0.4/.ruff_cache/content/18bd9323e775c06`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/1a43e2fa66cc521` & `aioarp-0.0.4/.ruff_cache/content/1a43e2fa66cc521`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/1bfc7af844c09624` & `aioarp-0.0.4/.ruff_cache/content/1bfc7af844c09624`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/1cf748db3edf4393` & `aioarp-0.0.4/.ruff_cache/content/1cf748db3edf4393`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/1d813f87eae436dc` & `aioarp-0.0.4/.ruff_cache/content/1d813f87eae436dc`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/20b471ae4ae2c716` & `aioarp-0.0.4/.ruff_cache/content/20b471ae4ae2c716`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/20cf28b4a08829e` & `aioarp-0.0.4/.ruff_cache/content/20cf28b4a08829e`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/22273ee756d2aeab` & `aioarp-0.0.4/.ruff_cache/content/22273ee756d2aeab`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/259f7be1f71aae17` & `aioarp-0.0.4/.ruff_cache/content/259f7be1f71aae17`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/277c58fd0e92dc6f` & `aioarp-0.0.4/.ruff_cache/content/277c58fd0e92dc6f`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/2894d2afe73e6dee` & `aioarp-0.0.4/.ruff_cache/content/2894d2afe73e6dee`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/28bfffee8af0f637` & `aioarp-0.0.4/.ruff_cache/content/28bfffee8af0f637`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/29a3dfb41b2e153e` & `aioarp-0.0.4/.ruff_cache/content/29a3dfb41b2e153e`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/29ec5304bead68a2` & `aioarp-0.0.4/.ruff_cache/content/29ec5304bead68a2`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/2b74d3f1efd79c7b` & `aioarp-0.0.4/.ruff_cache/content/2b74d3f1efd79c7b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/2f2908e30cbaaf6f` & `aioarp-0.0.4/.ruff_cache/content/2f2908e30cbaaf6f`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/40ec6c4657092d14` & `aioarp-0.0.4/.ruff_cache/content/40ec6c4657092d14`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/44618acc04af2a98` & `aioarp-0.0.4/.ruff_cache/content/44618acc04af2a98`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/464ea8dcb036f50b` & `aioarp-0.0.4/.ruff_cache/content/464ea8dcb036f50b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/48dc01dafed313cb` & `aioarp-0.0.4/.ruff_cache/content/48dc01dafed313cb`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/4c18fbd43c6124d9` & `aioarp-0.0.4/.ruff_cache/content/4c18fbd43c6124d9`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/4c7aefddb4afaa07` & `aioarp-0.0.4/.ruff_cache/content/4c7aefddb4afaa07`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/4ce11f41c925600e` & `aioarp-0.0.4/.ruff_cache/content/4ce11f41c925600e`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/4e4abc9127fe2106` & `aioarp-0.0.4/.ruff_cache/content/4e4abc9127fe2106`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/5259c25c40a66c52` & `aioarp-0.0.4/.ruff_cache/content/5259c25c40a66c52`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/54ca2556c07eb0e4` & `aioarp-0.0.4/.ruff_cache/content/54ca2556c07eb0e4`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/5845e4d7f49b3f6b` & `aioarp-0.0.4/.ruff_cache/content/5845e4d7f49b3f6b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/590fd00a0401d086` & `aioarp-0.0.4/.ruff_cache/content/590fd00a0401d086`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/608e0f7e2331dfd0` & `aioarp-0.0.4/.ruff_cache/content/608e0f7e2331dfd0`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/6190d891377c8571` & `aioarp-0.0.4/.ruff_cache/content/6190d891377c8571`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/6390cd3a2155b002` & `aioarp-0.0.4/.ruff_cache/content/6390cd3a2155b002`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/64f9f289e0610564` & `aioarp-0.0.4/.ruff_cache/content/64f9f289e0610564`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/65d6dc214750c212` & `aioarp-0.0.4/.ruff_cache/content/65d6dc214750c212`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/6aa5b22c44c81236` & `aioarp-0.0.4/.ruff_cache/content/6aa5b22c44c81236`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/6b926a7206e2e0f5` & `aioarp-0.0.4/.ruff_cache/content/6b926a7206e2e0f5`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/6ba798af16bd34e5` & `aioarp-0.0.4/.ruff_cache/content/6ba798af16bd34e5`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/85532fbdb4ec8100` & `aioarp-0.0.4/.ruff_cache/content/85532fbdb4ec8100`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/859b9d135acd891b` & `aioarp-0.0.4/.ruff_cache/content/859b9d135acd891b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/879246cf978566b8` & `aioarp-0.0.4/.ruff_cache/content/879246cf978566b8`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/8af090de0021767` & `aioarp-0.0.4/.ruff_cache/content/8af090de0021767`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/8ba2e035b666505` & `aioarp-0.0.4/.ruff_cache/content/8ba2e035b666505`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/8caa6ea7d00a8ef9` & `aioarp-0.0.4/.ruff_cache/content/8caa6ea7d00a8ef9`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/8e9682f1b99c3026` & `aioarp-0.0.4/.ruff_cache/content/8e9682f1b99c3026`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/93389fd7b221ce32` & `aioarp-0.0.4/.ruff_cache/content/93389fd7b221ce32`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/936f955f01285847` & `aioarp-0.0.4/.ruff_cache/content/936f955f01285847`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/a0edd6b97fbe3e68` & `aioarp-0.0.4/.ruff_cache/content/a0edd6b97fbe3e68`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/a12cec0addd27620` & `aioarp-0.0.4/.ruff_cache/content/a12cec0addd27620`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/a22627f4ad982518` & `aioarp-0.0.4/.ruff_cache/content/a22627f4ad982518`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/aabe170d14233a1f` & `aioarp-0.0.4/.ruff_cache/content/aabe170d14233a1f`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/aac73f953da24b03` & `aioarp-0.0.4/.ruff_cache/content/aac73f953da24b03`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/b74ab4e72907ed4b` & `aioarp-0.0.4/.ruff_cache/content/b74ab4e72907ed4b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/b874aac73807837a` & `aioarp-0.0.4/.ruff_cache/content/b874aac73807837a`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/bb3a8375be948e99` & `aioarp-0.0.4/.ruff_cache/content/bb3a8375be948e99`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/bb98194f279aef4d` & `aioarp-0.0.4/.ruff_cache/content/bb98194f279aef4d`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/bc9d2b60dadbf05e` & `aioarp-0.0.4/.ruff_cache/content/bc9d2b60dadbf05e`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/bd0ea26a717d1380` & `aioarp-0.0.4/.ruff_cache/content/bd0ea26a717d1380`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/bd3e6a97ee360bd7` & `aioarp-0.0.4/.ruff_cache/content/bd3e6a97ee360bd7`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/bdd7c44b4f88bf5b` & `aioarp-0.0.4/.ruff_cache/content/bdd7c44b4f88bf5b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/c12c935be2da0714` & `aioarp-0.0.4/.ruff_cache/content/c12c935be2da0714`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/c6c7c5bdc9a58d71` & `aioarp-0.0.4/.ruff_cache/content/c6c7c5bdc9a58d71`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/c78c3248c370d9f2` & `aioarp-0.0.4/.ruff_cache/content/c78c3248c370d9f2`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/cc374f0497dbc539` & `aioarp-0.0.4/.ruff_cache/content/cc374f0497dbc539`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/cc5595ab776e807c` & `aioarp-0.0.4/.ruff_cache/content/cc5595ab776e807c`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/cdc31ad9b3ea9979` & `aioarp-0.0.4/.ruff_cache/content/cdc31ad9b3ea9979`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/d3d46de068ceaf65` & `aioarp-0.0.4/.ruff_cache/content/d3d46de068ceaf65`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/d4ed3103ad57bd80` & `aioarp-0.0.4/.ruff_cache/content/d4ed3103ad57bd80`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/d8259ee38b03fc0e` & `aioarp-0.0.4/.ruff_cache/content/d8259ee38b03fc0e`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/e12d636458d129da` & `aioarp-0.0.4/.ruff_cache/content/e12d636458d129da`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/e25cfbd84c59869` & `aioarp-0.0.4/.ruff_cache/content/e25cfbd84c59869`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/e2a8017124da7733` & `aioarp-0.0.4/.ruff_cache/content/e2a8017124da7733`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/e84bd53ae32ad4a` & `aioarp-0.0.4/.ruff_cache/content/e84bd53ae32ad4a`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/eee42766c50b6490` & `aioarp-0.0.4/.ruff_cache/content/eee42766c50b6490`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/f45e36470415dca1` & `aioarp-0.0.4/.ruff_cache/content/f45e36470415dca1`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/f56e6b11a3d4a68b` & `aioarp-0.0.4/.ruff_cache/content/f56e6b11a3d4a68b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/f58c3d661899d706` & `aioarp-0.0.4/.ruff_cache/content/f58c3d661899d706`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.ruff_cache/content/fd508bd27e156044` & `aioarp-0.0.4/.ruff_cache/content/fd508bd27e156044`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/aioarp/_arp.py` & `aioarp-0.0.4/aioarp/_arp.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/aioarp/_async.py` & `aioarp-0.0.4/aioarp/_async.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/aioarp/_client.py` & `aioarp-0.0.4/aioarp/_client.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/aioarp/_sync.py` & `aioarp-0.0.4/aioarp/_sync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/aioarp/_utils.py` & `aioarp-0.0.4/aioarp/_utils.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/aioarp/_backends/_async.py` & `aioarp-0.0.4/aioarp/_backends/_async.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/aioarp/_backends/_mock.py` & `aioarp-0.0.4/aioarp/_backends/_mock.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/aioarp/_backends/_sync.py` & `aioarp-0.0.4/aioarp/_backends/_sync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/tests/test_async.py` & `aioarp-0.0.4/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/tests/test_client.py` & `aioarp-0.0.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/tests/test_proto.py` & `aioarp-0.0.4/tests/test_proto.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/tests/test_sync.py` & `aioarp-0.0.4/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/.gitignore` & `aioarp-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/LICENSE.txt` & `aioarp-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.3/README.md` & `aioarp-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # aioarp
 
 [![PyPI - Version](https://img.shields.io/pypi/v/aioarp.svg)](https://pypi.org/project/aioarp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aioarp.svg)](https://pypi.org/project/aioarp)
+[![coverage](https://img.shields.io/codecov/c/github/karosis88/aioarp/master)](https://app.codecov.io/gh/karosis88/aioarp)
+![license](https://img.shields.io/github/license/karosis88/aioarp)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [ARP request](#sending-arp-requests)
```

### Comparing `aioarp-0.0.3/pyproject.toml` & `aioarp-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aioarp"
 dynamic = ["version"]
-description = ''
+description = 'Aioarp is a ARP protocol implementation that provides synchronous and asynchronous interfaces and gives you complete control over how ARP packets are sent.'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Karen Petrosyan", email = "kar.petrosyanpy@gmail.com" },
 ]
@@ -56,8 +56,8 @@
 check_untyped_defs = true
 
 [tool.coverage.report]
 
 exclude_also = [
   '__repr__',
   'raise NotImplementedError()'
-]
+]
```

### Comparing `aioarp-0.0.3/PKG-INFO` & `aioarp-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: aioarp
-Version: 0.0.3
+Version: 0.0.4
+Summary: Aioarp is a ARP protocol implementation that provides synchronous and asynchronous interfaces and gives you complete control over how ARP packets are sent.
 Project-URL: Documentation, https://github.com/karosis88/aioarp#readme
 Project-URL: Issues, https://github.com/karosis88/aioarp/issues
 Project-URL: Source, https://github.com/karosis88/aioarp
 Author-email: Karen Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -21,14 +22,16 @@
 Requires-Dist: typing-extensions==4.6.3
 Description-Content-Type: text/markdown
 
 # aioarp
 
 [![PyPI - Version](https://img.shields.io/pypi/v/aioarp.svg)](https://pypi.org/project/aioarp)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aioarp.svg)](https://pypi.org/project/aioarp)
+[![coverage](https://img.shields.io/codecov/c/github/karosis88/aioarp/master)](https://app.codecov.io/gh/karosis88/aioarp)
+![license](https://img.shields.io/github/license/karosis88/aioarp)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [ARP request](#sending-arp-requests)
```

