# Comparing `tmp/pyteal-0.9.0.tar.gz` & `tmp/pyteal-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyteal-0.9.0.tar", last modified: Wed Sep 29 15:41:35 2021, max compression
+gzip compressed data, was "pyteal-0.9.1.tar", last modified: Tue Nov  9 16:06:42 2021, max compression
```

## Comparing `pyteal-0.9.0.tar` & `pyteal-0.9.1.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:35.156411 pyteal-0.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1065 2021-09-29 15:41:14.000000 pyteal-0.9.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2631 2021-09-29 15:41:35.152413 pyteal-0.9.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2166 2021-09-29 15:41:14.000000 pyteal-0.9.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:35.132423 pyteal-0.9.0/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:35.132423 pyteal-0.9.0/examples/application/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/application/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4479 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/application/asset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11621 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/application/security_token.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3429 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/application/vote.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12667 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/application/vote_deploy.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:35.136421 pyteal-0.9.0/examples/signature/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/signature/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/signature/atomic_swap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1037 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/signature/basic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5387 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/signature/dutch_auction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/signature/periodic_payment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2364 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/signature/periodic_payment_deploy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2269 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/signature/recurring_swap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3808 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/signature/recurring_swap_deploy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1659 2021-09-29 15:41:14.000000 pyteal-0.9.0/examples/signature/split.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:35.136421 pyteal-0.9.0/pyteal/
--rw-rw-r--   0 travis    (2000) travis    (2000)      767 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:35.148415 pyteal-0.9.0/pyteal/ast/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4013 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      876 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/addr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      780 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/addr_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13340 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18548 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/app_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1779 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/arg.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1198 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/arg_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      407 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/array.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1516 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/assert_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1149 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/assert_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8972 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/asset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20335 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/asset_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16916 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/binaryexpr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38440 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/binaryexpr_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      892 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/break_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      856 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/break_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3442 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/bytes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4993 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/bytes_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3555 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/cond.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3458 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/cond_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      913 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/continue_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      876 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/continue_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/err.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/err_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3602 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/expr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3291 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/for_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5348 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/for_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/gaid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1314 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/gaid_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2662 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/gload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1413 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/gload_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4286 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/global_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3696 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/global_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4123 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/gtxn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/gtxn_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4883 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/if_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7979 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/if_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/int.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      956 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/int_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5844 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/itxn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3410 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/itxn_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/leafexpr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2715 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/maybe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2663 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/maybe_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3013 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/naryexpr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5749 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/naryexpr_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1584 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/nonce.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5317 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/nonce_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4189 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/return_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3047 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/return_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4978 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/scratch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2766 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/scratch_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1639 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/scratchvar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2725 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/scratchvar_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2606 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/seq.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2829 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/seq_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7263 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/subroutine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9919 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/subroutine_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5944 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/ternaryexpr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5528 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/ternaryexpr_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1899 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/tmpl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1200 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/tmpl_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27963 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/txn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9672 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/txn_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5299 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/unaryexpr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9515 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/unaryexpr_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2413 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/while_.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3842 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/while_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5946 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ast/widemath.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:35.152413 pyteal-0.9.0/pyteal/compiler/
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8095 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/compiler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25262 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/compiler_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7419 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16789 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/constants_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4346 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/flatten.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17485 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/flatten_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5300 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/scratchslots.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13313 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/scratchslots_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1029 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/sort.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2877 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/sort_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10578 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/subroutines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    43793 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/compiler/subroutines_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/errors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:35.152413 pyteal-0.9.0/pyteal/ir/
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      521 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/labelref.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13718 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/ops.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8342 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/tealblock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7557 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/tealblock_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1401 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/tealcomponent.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      418 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/tealcomponent_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/tealconditionalblock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/tealconditionalblock_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1210 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/teallabel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2619 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/tealop.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/tealsimpleblock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      810 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/ir/tealsimpleblock_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2493 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2241 2021-09-29 15:41:14.000000 pyteal-0.9.0/pyteal/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:35.136421 pyteal-0.9.0/pyteal.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2631 2021-09-29 15:41:35.000000 pyteal-0.9.0/pyteal.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3163 2021-09-29 15:41:35.000000 pyteal-0.9.0/pyteal.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-09-29 15:41:35.000000 pyteal-0.9.0/pyteal.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2021-09-29 15:41:35.000000 pyteal-0.9.0/pyteal.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2021-09-29 15:41:35.000000 pyteal-0.9.0/pyteal.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-09-29 15:41:35.156411 pyteal-0.9.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      710 2021-09-29 15:41:14.000000 pyteal-0.9.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:35.152413 pyteal-0.9.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-09-29 15:41:14.000000 pyteal-0.9.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4657 2021-09-29 15:41:14.000000 pyteal-0.9.0/tests/compile_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2021-09-29 15:41:14.000000 pyteal-0.9.0/tests/module_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:42.252986 pyteal-0.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1065 2021-11-09 16:06:22.000000 pyteal-0.9.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2631 2021-11-09 16:06:42.252986 pyteal-0.9.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2166 2021-11-09 16:06:22.000000 pyteal-0.9.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:42.232986 pyteal-0.9.1/examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:42.232986 pyteal-0.9.1/examples/application/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/application/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4479 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/application/asset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11621 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/application/security_token.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3429 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/application/vote.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12667 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/application/vote_deploy.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:42.236986 pyteal-0.9.1/examples/signature/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/signature/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/signature/atomic_swap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1037 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/signature/basic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5387 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/signature/dutch_auction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/signature/periodic_payment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2364 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/signature/periodic_payment_deploy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2269 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/signature/recurring_swap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3808 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/signature/recurring_swap_deploy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1659 2021-11-09 16:06:22.000000 pyteal-0.9.1/examples/signature/split.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:42.236986 pyteal-0.9.1/pyteal/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      797 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2754 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/__init__.pyi
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:42.244986 pyteal-0.9.1/pyteal/ast/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4013 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      876 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/addr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      780 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/addr_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13340 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18548 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/app_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1779 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/arg.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1198 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/arg_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      407 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/array.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1516 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/assert_.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1149 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/assert_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8972 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/asset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20335 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/asset_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16916 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/binaryexpr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38440 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/binaryexpr_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      892 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/break_.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      856 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/break_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3442 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/bytes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4993 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/bytes_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3555 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/cond.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3458 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/cond_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      913 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/continue_.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      876 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/continue_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      591 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/err.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/err_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3602 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/expr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3291 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/for_.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5348 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/for_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/gaid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1314 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/gaid_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2662 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/gload.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1413 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/gload_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4286 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/global_.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3696 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/global_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4123 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/gtxn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      402 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/gtxn_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4883 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/if_.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7979 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/if_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/int.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      956 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/int_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5844 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/itxn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3410 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/itxn_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/leafexpr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2715 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/maybe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2663 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/maybe_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3013 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/naryexpr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5749 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/naryexpr_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1584 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/nonce.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5317 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/nonce_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4189 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/return_.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3047 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/return_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4978 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/scratch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2766 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/scratch_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1639 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/scratchvar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2725 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/scratchvar_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2606 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/seq.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2829 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/seq_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7263 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/subroutine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9919 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/subroutine_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5944 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/ternaryexpr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5528 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/ternaryexpr_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1899 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/tmpl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1200 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/tmpl_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27963 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/txn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9672 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/txn_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5299 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/unaryexpr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9515 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/unaryexpr_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2413 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/while_.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3842 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/while_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5946 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ast/widemath.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:42.248986 pyteal-0.9.1/pyteal/compiler/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8095 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/compiler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25262 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/compiler_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7419 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16789 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/constants_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4346 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/flatten.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17485 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/flatten_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5300 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/scratchslots.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13313 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/scratchslots_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1029 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/sort.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2877 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/sort_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10578 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/subroutines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43793 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/compiler/subroutines_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      127 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/errors.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:42.248986 pyteal-0.9.1/pyteal/ir/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      521 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/labelref.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13718 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/ops.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8342 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/tealblock.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7557 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/tealblock_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1401 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/tealcomponent.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      418 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/tealcomponent_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/tealconditionalblock.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/tealconditionalblock_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1210 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/teallabel.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2619 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/tealop.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1628 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/tealsimpleblock.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      810 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/ir/tealsimpleblock_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2493 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2241 2021-11-09 16:06:22.000000 pyteal-0.9.1/pyteal/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:42.236986 pyteal-0.9.1/pyteal.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2631 2021-11-09 16:06:42.000000 pyteal-0.9.1/pyteal.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3183 2021-11-09 16:06:42.000000 pyteal-0.9.1/pyteal.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-11-09 16:06:42.000000 pyteal-0.9.1/pyteal.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2021-11-09 16:06:42.000000 pyteal-0.9.1/pyteal.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2021-11-09 16:06:42.000000 pyteal-0.9.1/pyteal.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-11-09 16:06:42.252986 pyteal-0.9.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      750 2021-11-09 16:06:22.000000 pyteal-0.9.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:42.248986 pyteal-0.9.1/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-11-09 16:06:22.000000 pyteal-0.9.1/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4657 2021-11-09 16:06:22.000000 pyteal-0.9.1/tests/compile_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2021-11-09 16:06:22.000000 pyteal-0.9.1/tests/module_test.py
```

### Comparing `pyteal-0.9.0/LICENSE` & `pyteal-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/PKG-INFO` & `pyteal-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyteal
-Version: 0.9.0
+Version: 0.9.1
 Summary: Algorand Smart Contracts in Python
 Home-page: https://github.com/algorand/pyteal
 Author: Algorand
 Author-email: pypiservice@algorand.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyteal-0.9.0/README.md` & `pyteal-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/application/asset.py` & `pyteal-0.9.1/examples/application/asset.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/application/security_token.py` & `pyteal-0.9.1/examples/application/security_token.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/application/vote.py` & `pyteal-0.9.1/examples/application/vote.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/application/vote_deploy.py` & `pyteal-0.9.1/examples/application/vote_deploy.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/signature/atomic_swap.py` & `pyteal-0.9.1/examples/signature/atomic_swap.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/signature/basic.py` & `pyteal-0.9.1/examples/signature/basic.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/signature/dutch_auction.py` & `pyteal-0.9.1/examples/signature/dutch_auction.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/signature/periodic_payment.py` & `pyteal-0.9.1/examples/signature/periodic_payment.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/signature/periodic_payment_deploy.py` & `pyteal-0.9.1/examples/signature/periodic_payment_deploy.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/signature/recurring_swap.py` & `pyteal-0.9.1/examples/signature/recurring_swap.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/signature/recurring_swap_deploy.py` & `pyteal-0.9.1/examples/signature/recurring_swap_deploy.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/examples/signature/split.py` & `pyteal-0.9.1/examples/signature/split.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/__init__.py` & `pyteal-0.9.1/pyteal/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     CompileOptions,
     compileTeal,
 )
 from .types import TealType
 from .errors import TealInternalError, TealTypeError, TealInputError, TealCompileError
 from .config import MAX_GROUP_SIZE, NUM_SLOTS
 
+# begin __all__
 __all__ = (
     ast_all
     + ir_all
     + [
         "MAX_TEAL_VERSION",
         "MIN_TEAL_VERSION",
         "DEFAULT_TEAL_VERSION",
@@ -27,7 +28,8 @@
         "TealTypeError",
         "TealInputError",
         "TealCompileError",
         "MAX_GROUP_SIZE",
         "NUM_SLOTS",
     ]
 )
+# end __all__
```

### Comparing `pyteal-0.9.0/pyteal/ast/__init__.py` & `pyteal-0.9.1/pyteal/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/addr.py` & `pyteal-0.9.1/pyteal/ast/addr.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/addr_test.py` & `pyteal-0.9.1/pyteal/ast/addr_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/app.py` & `pyteal-0.9.1/pyteal/ast/app.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/app_test.py` & `pyteal-0.9.1/pyteal/ast/app_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/arg.py` & `pyteal-0.9.1/pyteal/ast/arg.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/arg_test.py` & `pyteal-0.9.1/pyteal/ast/arg_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/assert_.py` & `pyteal-0.9.1/pyteal/ast/assert_.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/assert_test.py` & `pyteal-0.9.1/pyteal/ast/assert_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/asset.py` & `pyteal-0.9.1/pyteal/ast/asset.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/asset_test.py` & `pyteal-0.9.1/pyteal/ast/asset_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/binaryexpr.py` & `pyteal-0.9.1/pyteal/ast/binaryexpr.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/binaryexpr_test.py` & `pyteal-0.9.1/pyteal/ast/binaryexpr_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/break_.py` & `pyteal-0.9.1/pyteal/ast/break_.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/break_test.py` & `pyteal-0.9.1/pyteal/ast/break_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/bytes.py` & `pyteal-0.9.1/pyteal/ast/bytes.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/bytes_test.py` & `pyteal-0.9.1/pyteal/ast/bytes_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/cond.py` & `pyteal-0.9.1/pyteal/ast/cond.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/cond_test.py` & `pyteal-0.9.1/pyteal/ast/cond_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/continue_.py` & `pyteal-0.9.1/pyteal/ast/continue_.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/continue_test.py` & `pyteal-0.9.1/pyteal/ast/continue_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/err.py` & `pyteal-0.9.1/pyteal/ast/err.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/expr.py` & `pyteal-0.9.1/pyteal/ast/expr.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/for_.py` & `pyteal-0.9.1/pyteal/ast/for_.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/for_test.py` & `pyteal-0.9.1/pyteal/ast/for_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/gaid.py` & `pyteal-0.9.1/pyteal/ast/gaid.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/gaid_test.py` & `pyteal-0.9.1/pyteal/ast/gaid_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/gload.py` & `pyteal-0.9.1/pyteal/ast/gload.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/gload_test.py` & `pyteal-0.9.1/pyteal/ast/gload_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/global_.py` & `pyteal-0.9.1/pyteal/ast/global_.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/global_test.py` & `pyteal-0.9.1/pyteal/ast/global_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/gtxn.py` & `pyteal-0.9.1/pyteal/ast/gtxn.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/if_.py` & `pyteal-0.9.1/pyteal/ast/if_.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/if_test.py` & `pyteal-0.9.1/pyteal/ast/if_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/int.py` & `pyteal-0.9.1/pyteal/ast/int.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/int_test.py` & `pyteal-0.9.1/pyteal/ast/int_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/itxn.py` & `pyteal-0.9.1/pyteal/ast/itxn.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/itxn_test.py` & `pyteal-0.9.1/pyteal/ast/itxn_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/maybe.py` & `pyteal-0.9.1/pyteal/ast/maybe.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/maybe_test.py` & `pyteal-0.9.1/pyteal/ast/maybe_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/naryexpr.py` & `pyteal-0.9.1/pyteal/ast/naryexpr.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/naryexpr_test.py` & `pyteal-0.9.1/pyteal/ast/naryexpr_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/nonce.py` & `pyteal-0.9.1/pyteal/ast/nonce.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/nonce_test.py` & `pyteal-0.9.1/pyteal/ast/nonce_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/return_.py` & `pyteal-0.9.1/pyteal/ast/return_.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/return_test.py` & `pyteal-0.9.1/pyteal/ast/return_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/scratch.py` & `pyteal-0.9.1/pyteal/ast/scratch.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/scratch_test.py` & `pyteal-0.9.1/pyteal/ast/scratch_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/scratchvar.py` & `pyteal-0.9.1/pyteal/ast/scratchvar.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/scratchvar_test.py` & `pyteal-0.9.1/pyteal/ast/scratchvar_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/seq.py` & `pyteal-0.9.1/pyteal/ast/seq.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/seq_test.py` & `pyteal-0.9.1/pyteal/ast/seq_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/subroutine.py` & `pyteal-0.9.1/pyteal/ast/subroutine.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/subroutine_test.py` & `pyteal-0.9.1/pyteal/ast/subroutine_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/ternaryexpr.py` & `pyteal-0.9.1/pyteal/ast/ternaryexpr.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/ternaryexpr_test.py` & `pyteal-0.9.1/pyteal/ast/ternaryexpr_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/tmpl.py` & `pyteal-0.9.1/pyteal/ast/tmpl.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/tmpl_test.py` & `pyteal-0.9.1/pyteal/ast/tmpl_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/txn.py` & `pyteal-0.9.1/pyteal/ast/txn.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/txn_test.py` & `pyteal-0.9.1/pyteal/ast/txn_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/unaryexpr.py` & `pyteal-0.9.1/pyteal/ast/unaryexpr.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/unaryexpr_test.py` & `pyteal-0.9.1/pyteal/ast/unaryexpr_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/while_.py` & `pyteal-0.9.1/pyteal/ast/while_.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/while_test.py` & `pyteal-0.9.1/pyteal/ast/while_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ast/widemath.py` & `pyteal-0.9.1/pyteal/ast/widemath.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/compiler.py` & `pyteal-0.9.1/pyteal/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/compiler_test.py` & `pyteal-0.9.1/pyteal/compiler/compiler_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/constants.py` & `pyteal-0.9.1/pyteal/compiler/constants.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/constants_test.py` & `pyteal-0.9.1/pyteal/compiler/constants_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/flatten.py` & `pyteal-0.9.1/pyteal/compiler/flatten.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/flatten_test.py` & `pyteal-0.9.1/pyteal/compiler/flatten_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/scratchslots.py` & `pyteal-0.9.1/pyteal/compiler/scratchslots.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/scratchslots_test.py` & `pyteal-0.9.1/pyteal/compiler/scratchslots_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/sort.py` & `pyteal-0.9.1/pyteal/compiler/sort.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/sort_test.py` & `pyteal-0.9.1/pyteal/compiler/sort_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/subroutines.py` & `pyteal-0.9.1/pyteal/compiler/subroutines.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/compiler/subroutines_test.py` & `pyteal-0.9.1/pyteal/compiler/subroutines_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/errors.py` & `pyteal-0.9.1/pyteal/errors.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/labelref.py` & `pyteal-0.9.1/pyteal/ir/labelref.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/ops.py` & `pyteal-0.9.1/pyteal/ir/ops.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/tealblock.py` & `pyteal-0.9.1/pyteal/ir/tealblock.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/tealblock_test.py` & `pyteal-0.9.1/pyteal/ir/tealblock_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/tealcomponent.py` & `pyteal-0.9.1/pyteal/ir/tealcomponent.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/tealconditionalblock.py` & `pyteal-0.9.1/pyteal/ir/tealconditionalblock.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/tealconditionalblock_test.py` & `pyteal-0.9.1/pyteal/ir/tealconditionalblock_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/teallabel.py` & `pyteal-0.9.1/pyteal/ir/teallabel.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/tealop.py` & `pyteal-0.9.1/pyteal/ir/tealop.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/tealsimpleblock.py` & `pyteal-0.9.1/pyteal/ir/tealsimpleblock.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/ir/tealsimpleblock_test.py` & `pyteal-0.9.1/pyteal/ir/tealsimpleblock_test.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/types.py` & `pyteal-0.9.1/pyteal/types.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal/util.py` & `pyteal-0.9.1/pyteal/util.py`

 * *Files identical despite different names*

### Comparing `pyteal-0.9.0/pyteal.egg-info/PKG-INFO` & `pyteal-0.9.1/pyteal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyteal
-Version: 0.9.0
+Version: 0.9.1
 Summary: Algorand Smart Contracts in Python
 Home-page: https://github.com/algorand/pyteal
 Author: Algorand
 Author-email: pypiservice@algorand.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyteal-0.9.0/pyteal.egg-info/SOURCES.txt` & `pyteal-0.9.1/pyteal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 examples/signature/dutch_auction.py
 examples/signature/periodic_payment.py
 examples/signature/periodic_payment_deploy.py
 examples/signature/recurring_swap.py
 examples/signature/recurring_swap_deploy.py
 examples/signature/split.py
 pyteal/__init__.py
+pyteal/__init__.pyi
 pyteal/config.py
 pyteal/errors.py
 pyteal/types.py
 pyteal/util.py
 pyteal.egg-info/PKG-INFO
 pyteal.egg-info/SOURCES.txt
 pyteal.egg-info/dependency_links.txt
```

### Comparing `pyteal-0.9.0/setup.py` & `pyteal-0.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyteal",
-    version="0.9.0",
+    version="0.9.1",
     author="Algorand",
     author_email="pypiservice@algorand.com",
     description="Algorand Smart Contracts in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/algorand/pyteal",
     packages=setuptools.find_packages(),
     install_requires=["py-algorand-sdk"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    package_data={"pyteal": ["*.pyi"]},
     python_requires=">=3.6",
 )
```

### Comparing `pyteal-0.9.0/tests/compile_test.py` & `pyteal-0.9.1/tests/compile_test.py`

 * *Files identical despite different names*

