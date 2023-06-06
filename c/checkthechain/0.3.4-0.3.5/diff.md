# Comparing `tmp/checkthechain-0.3.4.tar.gz` & `tmp/checkthechain-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkthechain-0.3.4.tar", last modified: Tue Jun  6 00:31:23 2023, max compression
+gzip compressed data, was "checkthechain-0.3.5.tar", last modified: Tue Jun  6 01:24:21 2023, max compression
```

## Comparing `checkthechain-0.3.4.tar` & `checkthechain-0.3.5.tar`

### file list

```diff
@@ -1,698 +1,698 @@
--rw-r--r--   0        0        0      217 2023-02-26 18:21:06.927738 checkthechain-0.3.4/.gitignore
--rw-r--r--   0        0        0     8294 2023-02-26 18:21:06.927914 checkthechain-0.3.4/CHANGELOG.md
--rw-r--r--   0        0        0     3117 2023-04-11 03:46:56.460577 checkthechain-0.3.4/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-02-26 18:21:06.928214 checkthechain-0.3.4/LICENSE-APACHE
--rw-r--r--   0        0        0     1093 2023-02-26 18:21:06.928570 checkthechain-0.3.4/LICENSE-MIT
--rw-r--r--   0        0        0     7487 2023-02-26 18:21:06.928884 checkthechain-0.3.4/README.md
--rw-r--r--   0        0        0       52 2022-11-23 19:36:31.097613 checkthechain-0.3.4/docs/README.md
--rw-r--r--   0        0        0     1167 2023-02-26 18:21:06.929180 checkthechain-0.3.4/docs/contributing_guides/adding_config_keys.md
--rw-r--r--   0        0        0      797 2023-02-26 18:21:06.929401 checkthechain-0.3.4/docs/contributing_guides/adding_db_caches.md
--rw-r--r--   0        0        0      243 2023-02-26 18:21:06.929558 checkthechain-0.3.4/docs/contributing_guides/upgrade_to_new_ctc_version.md
--rw-r--r--   0        0        0     4438 2023-06-06 00:15:39.725055 checkthechain-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      566 2023-04-29 01:37:54.115295 checkthechain-0.3.4/src/ctc/__init__.py
--rw-r--r--   0        0        0       35 2022-11-23 19:36:31.097865 checkthechain-0.3.4/src/ctc/__main__.py
--rw-r--r--   0        0        0       97 2023-02-26 18:21:06.930730 checkthechain-0.3.4/src/ctc/cli/__init__.py
--rw-r--r--   0        0        0    12631 2023-04-11 16:22:47.887085 checkthechain-0.3.4/src/ctc/cli/cli_run.py
--rw-r--r--   0        0        0      193 2023-02-26 18:21:06.931328 checkthechain-0.3.4/src/ctc/cli/cli_utils/__init__.py
--rw-r--r--   0        0        0     9052 2022-11-23 19:36:31.098221 checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_alias_utils.py
--rw-r--r--   0        0        0     8508 2023-02-26 18:21:06.931449 checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_charset_utils.py
--rw-r--r--   0        0        0     8581 2023-04-17 00:55:51.315895 checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_color_utils.py
--rw-r--r--   0        0        0      612 2022-11-23 19:36:31.098462 checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_execution_utils.py
--rw-r--r--   0        0        0     2308 2023-04-11 03:44:53.034908 checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_output_utils.py
--rw-r--r--   0        0        0     9184 2023-05-09 04:20:26.327124 checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_parse_utils.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.098735 checkthechain-0.3.4/src/ctc/cli/commands/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.098821 checkthechain-0.3.4/src/ctc/cli/commands/admin/__init__.py
--rw-r--r--   0        0        0     1952 2022-11-23 19:36:31.098935 checkthechain-0.3.4/src/ctc/cli/commands/admin/aliases_command.py
--rw-r--r--   0        0        0     2569 2022-11-23 19:36:31.099038 checkthechain-0.3.4/src/ctc/cli/commands/admin/chains_command.py
--rw-r--r--   0        0        0      939 2023-02-26 18:21:06.932612 checkthechain-0.3.4/src/ctc/cli/commands/admin/charset_command.py
--rw-r--r--   0        0        0     2796 2023-02-26 18:21:06.932700 checkthechain-0.3.4/src/ctc/cli/commands/admin/color_command.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.099306 checkthechain-0.3.4/src/ctc/cli/commands/admin/config/__init__.py
--rw-r--r--   0        0        0     1231 2023-02-26 18:21:06.932846 checkthechain-0.3.4/src/ctc/cli/commands/admin/config/edit_command.py
--rw-r--r--   0        0        0      341 2022-11-23 19:36:31.099535 checkthechain-0.3.4/src/ctc/cli/commands/admin/config/path_command.py
--rw-r--r--   0        0        0    11615 2023-05-09 03:03:31.696453 checkthechain-0.3.4/src/ctc/cli/commands/admin/config_command.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.099729 checkthechain-0.3.4/src/ctc/cli/commands/admin/db/__init__.py
--rw-r--r--   0        0        0     1310 2023-02-26 21:00:17.933995 checkthechain-0.3.4/src/ctc/cli/commands/admin/db/create_tables_command.py
--rw-r--r--   0        0        0     1410 2023-02-26 20:15:07.407580 checkthechain-0.3.4/src/ctc/cli/commands/admin/db/drop_command.py
--rw-r--r--   0        0        0      370 2023-04-12 04:04:05.737647 checkthechain-0.3.4/src/ctc/cli/commands/admin/db/login_command.py
--rw-r--r--   0        0        0     4772 2023-04-26 23:18:25.231255 checkthechain-0.3.4/src/ctc/cli/commands/admin/db/status_command.py
--rw-r--r--   0        0        0      858 2022-11-23 19:36:31.100027 checkthechain-0.3.4/src/ctc/cli/commands/admin/log_command.py
--rw-r--r--   0        0        0     3184 2022-11-23 19:36:31.100197 checkthechain-0.3.4/src/ctc/cli/commands/admin/setup_command.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.100283 checkthechain-0.3.4/src/ctc/cli/commands/compute/__init__.py
--rw-r--r--   0        0        0      491 2022-11-23 19:36:31.100403 checkthechain-0.3.4/src/ctc/cli/commands/compute/ascii_command.py
--rw-r--r--   0        0        0      530 2022-11-23 19:36:31.100502 checkthechain-0.3.4/src/ctc/cli/commands/compute/checksum_command.py
--rw-r--r--   0        0        0     1202 2022-11-23 19:36:31.100601 checkthechain-0.3.4/src/ctc/cli/commands/compute/create_address_command.py
--rw-r--r--   0        0        0    13751 2023-04-11 16:58:47.041829 checkthechain-0.3.4/src/ctc/cli/commands/compute/decode_call_command.py
--rw-r--r--   0        0        0      965 2023-04-11 16:55:27.846437 checkthechain-0.3.4/src/ctc/cli/commands/compute/decode_command.py
--rw-r--r--   0        0        0     1482 2023-04-11 16:55:12.443123 checkthechain-0.3.4/src/ctc/cli/commands/compute/encode_command.py
--rw-r--r--   0        0        0      760 2022-11-23 19:36:31.100956 checkthechain-0.3.4/src/ctc/cli/commands/compute/hex_command.py
--rw-r--r--   0        0        0      509 2022-11-23 19:36:31.101019 checkthechain-0.3.4/src/ctc/cli/commands/compute/integer_command.py
--rw-r--r--   0        0        0     1618 2022-11-23 19:36:31.101088 checkthechain-0.3.4/src/ctc/cli/commands/compute/keccak_command.py
--rw-r--r--   0        0        0     4730 2022-11-23 19:36:31.101172 checkthechain-0.3.4/src/ctc/cli/commands/compute/limits_command.py
--rw-r--r--   0        0        0      436 2022-11-23 19:36:31.101239 checkthechain-0.3.4/src/ctc/cli/commands/compute/lower_command.py
--rw-r--r--   0        0        0      993 2022-11-23 19:36:31.101312 checkthechain-0.3.4/src/ctc/cli/commands/compute/rlp_encode.py
--rw-r--r--   0        0        0      720 2022-11-23 19:36:31.101376 checkthechain-0.3.4/src/ctc/cli/commands/compute/selector_command.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.101442 checkthechain-0.3.4/src/ctc/cli/commands/data/__init__.py
--rw-r--r--   0        0        0     6408 2023-02-26 18:21:06.935201 checkthechain-0.3.4/src/ctc/cli/commands/data/abi_command.py
--rw-r--r--   0        0        0     1506 2022-11-23 19:36:31.101616 checkthechain-0.3.4/src/ctc/cli/commands/data/abi_diff_command.py
--rw-r--r--   0        0        0     1454 2023-02-26 18:21:06.935512 checkthechain-0.3.4/src/ctc/cli/commands/data/address_command.py
--rw-r--r--   0        0        0     2532 2023-01-07 08:13:49.926885 checkthechain-0.3.4/src/ctc/cli/commands/data/address_txs_command.py
--rw-r--r--   0        0        0     2593 2023-02-26 18:21:06.935644 checkthechain-0.3.4/src/ctc/cli/commands/data/block_command.py
--rw-r--r--   0        0        0     5173 2023-04-11 03:48:25.322507 checkthechain-0.3.4/src/ctc/cli/commands/data/blocks_command.py
--rw-r--r--   0        0        0      634 2022-11-23 19:36:31.101982 checkthechain-0.3.4/src/ctc/cli/commands/data/bytecode_command.py
--rw-r--r--   0        0        0     4642 2023-03-18 06:34:21.816682 checkthechain-0.3.4/src/ctc/cli/commands/data/call_all_command.py
--rw-r--r--   0        0        0     3224 2022-11-23 19:36:31.102138 checkthechain-0.3.4/src/ctc/cli/commands/data/call_command.py
--rw-r--r--   0        0        0    23122 2023-04-12 16:08:53.179783 checkthechain-0.3.4/src/ctc/cli/commands/data/calls_command.py
--rw-r--r--   0        0        0     2927 2023-02-26 18:21:06.936911 checkthechain-0.3.4/src/ctc/cli/commands/data/chain_command.py
--rw-r--r--   0        0        0     4207 2023-02-26 18:21:06.937286 checkthechain-0.3.4/src/ctc/cli/commands/data/decompile_command.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.102575 checkthechain-0.3.4/src/ctc/cli/commands/data/dex/__init__.py
--rw-r--r--   0        0        0     6890 2023-04-15 16:03:33.976343 checkthechain-0.3.4/src/ctc/cli/commands/data/dex/chart_command.py
--rw-r--r--   0        0        0     4813 2023-04-15 16:00:40.959584 checkthechain-0.3.4/src/ctc/cli/commands/data/dex/pool_command.py
--rw-r--r--   0        0        0     8639 2023-04-15 16:00:02.454511 checkthechain-0.3.4/src/ctc/cli/commands/data/dex/pools_command.py
--rw-r--r--   0        0        0     4354 2023-04-15 15:43:58.809999 checkthechain-0.3.4/src/ctc/cli/commands/data/dex/trades_command.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.103150 checkthechain-0.3.4/src/ctc/cli/commands/data/erc20/__init__.py
--rw-r--r--   0        0        0     1603 2022-11-23 19:36:31.103246 checkthechain-0.3.4/src/ctc/cli/commands/data/erc20/balance_command.py
--rw-r--r--   0        0        0     9969 2023-04-11 03:56:24.764985 checkthechain-0.3.4/src/ctc/cli/commands/data/erc20/balances_command.py
--rw-r--r--   0        0        0     1947 2023-04-10 04:18:22.101055 checkthechain-0.3.4/src/ctc/cli/commands/data/erc20/transfers_command.py
--rw-r--r--   0        0        0      881 2022-11-23 19:36:31.103509 checkthechain-0.3.4/src/ctc/cli/commands/data/erc20_command.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.103574 checkthechain-0.3.4/src/ctc/cli/commands/data/eth/__init__.py
--rw-r--r--   0        0        0     1334 2022-11-23 19:36:31.103652 checkthechain-0.3.4/src/ctc/cli/commands/data/eth/balance_command.py
--rw-r--r--   0        0        0     7719 2023-04-12 23:11:07.611640 checkthechain-0.3.4/src/ctc/cli/commands/data/eth/balances_command.py
--rw-r--r--   0        0        0     3653 2023-04-11 05:49:15.694208 checkthechain-0.3.4/src/ctc/cli/commands/data/events_command.py
--rw-r--r--   0        0        0    11909 2023-04-14 03:52:55.753011 checkthechain-0.3.4/src/ctc/cli/commands/data/gas_command.py
--rw-r--r--   0        0        0     2520 2022-11-23 19:36:31.104030 checkthechain-0.3.4/src/ctc/cli/commands/data/proxy_command.py
--rw-r--r--   0        0        0     2597 2023-02-26 18:21:06.939031 checkthechain-0.3.4/src/ctc/cli/commands/data/proxy_register_command.py
--rw-r--r--   0        0        0     1478 2023-04-11 17:03:09.850892 checkthechain-0.3.4/src/ctc/cli/commands/data/storage_command.py
--rw-r--r--   0        0        0      850 2022-11-23 19:36:31.104247 checkthechain-0.3.4/src/ctc/cli/commands/data/symbol_command.py
--rw-r--r--   0        0        0     1450 2022-11-23 19:36:31.104314 checkthechain-0.3.4/src/ctc/cli/commands/data/timestamp_command.py
--rw-r--r--   0        0        0     2050 2023-02-26 18:21:06.939163 checkthechain-0.3.4/src/ctc/cli/commands/data/tx_command.py
--rw-r--r--   0        0        0     2813 2022-11-23 19:36:31.104457 checkthechain-0.3.4/src/ctc/cli/commands/root_command.py
--rw-r--r--   0        0        0      226 2023-02-26 18:21:06.939627 checkthechain-0.3.4/src/ctc/config/__init__.py
--rw-r--r--   0        0        0     6947 2023-04-26 23:49:08.151324 checkthechain-0.3.4/src/ctc/config/config_defaults.py
--rw-r--r--   0        0        0     3987 2023-02-26 18:21:06.940408 checkthechain-0.3.4/src/ctc/config/config_env_vars.py
--rw-r--r--   0        0        0      687 2023-02-26 18:21:06.940691 checkthechain-0.3.4/src/ctc/config/config_overrides.py
--rw-r--r--   0        0        0     4267 2023-04-17 00:26:09.800618 checkthechain-0.3.4/src/ctc/config/config_read.py
--rw-r--r--   0        0        0      375 2023-02-26 18:21:06.941204 checkthechain-0.3.4/src/ctc/config/config_spec.py
--rw-r--r--   0        0        0    11474 2023-04-27 04:45:26.239328 checkthechain-0.3.4/src/ctc/config/config_validate.py
--rw-r--r--   0        0        0     4912 2023-04-17 01:15:59.426408 checkthechain-0.3.4/src/ctc/config/config_values.py
--rw-r--r--   0        0        0     1236 2023-04-17 00:11:55.733936 checkthechain-0.3.4/src/ctc/config/config_write.py
--rw-r--r--   0        0        0      121 2023-02-26 18:21:06.942475 checkthechain-0.3.4/src/ctc/config/context_utils/__init__.py
--rw-r--r--   0        0        0     7359 2023-04-11 22:37:33.866053 checkthechain-0.3.4/src/ctc/config/context_utils/context_caches.py
--rw-r--r--   0        0        0     1944 2023-02-26 18:21:06.943080 checkthechain-0.3.4/src/ctc/config/context_utils/context_crud.py
--rw-r--r--   0        0        0     3118 2023-04-10 23:34:05.929913 checkthechain-0.3.4/src/ctc/config/context_utils/context_sources.py
--rw-r--r--   0        0        0      506 2023-02-26 18:21:06.943482 checkthechain-0.3.4/src/ctc/config/context_utils/context_validate.py
--rw-r--r--   0        0        0       26 2022-11-23 19:36:31.105507 checkthechain-0.3.4/src/ctc/config/setup_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.105567 checkthechain-0.3.4/src/ctc/config/setup_utils/default_data/__init__.py
--rw-r--r--   0        0        0   142771 2023-04-12 02:21:19.579767 checkthechain-0.3.4/src/ctc/config/setup_utils/default_data/default_erc20s.py
--rw-r--r--   0        0        0     3629 2023-04-27 01:46:49.405189 checkthechain-0.3.4/src/ctc/config/setup_utils/main_setup.py
--rw-r--r--   0        0        0     7383 2023-04-17 00:15:05.747317 checkthechain-0.3.4/src/ctc/config/setup_utils/setup_io.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.106519 checkthechain-0.3.4/src/ctc/config/setup_utils/stages/__init__.py
--rw-r--r--   0        0        0     1622 2023-02-26 18:21:06.945600 checkthechain-0.3.4/src/ctc/config/setup_utils/stages/alias_setup.py
--rw-r--r--   0        0        0     4171 2023-02-26 18:21:06.945828 checkthechain-0.3.4/src/ctc/config/setup_utils/stages/cli_setup.py
--rw-r--r--   0        0        0     3309 2023-02-26 18:21:06.945947 checkthechain-0.3.4/src/ctc/config/setup_utils/stages/data_dir_setup.py
--rw-r--r--   0        0        0     8319 2023-04-27 04:36:30.568338 checkthechain-0.3.4/src/ctc/config/setup_utils/stages/db_setup.py
--rw-r--r--   0        0        0    16993 2023-04-12 02:20:49.003316 checkthechain-0.3.4/src/ctc/config/setup_utils/stages/network_setup.py
--rw-r--r--   0        0        0       59 2023-02-26 18:21:06.946626 checkthechain-0.3.4/src/ctc/config/upgrade_utils/__init__.py
--rw-r--r--   0        0        0     7078 2023-04-17 00:18:44.690569 checkthechain-0.3.4/src/ctc/config/upgrade_utils/config_upgrade.py
--rw-r--r--   0        0        0     7171 2023-04-17 01:16:23.566187 checkthechain-0.3.4/src/ctc/config/upgrade_utils/data_dir_versioning.py
--rw-r--r--   0        0        0     3026 2023-04-17 01:29:37.379812 checkthechain-0.3.4/src/ctc/config/upgrade_utils/legacy_types.py
--rw-r--r--   0        0        0      623 2023-02-26 18:21:06.947460 checkthechain-0.3.4/src/ctc/config/upgrade_utils/version_utils.py
--rw-r--r--   0        0        0        0 2023-03-04 19:50:23.525211 checkthechain-0.3.4/src/ctc/datasets/__init__.py
--rw-r--r--   0        0        0     6803 2023-06-03 00:20:08.970969 checkthechain-0.3.4/src/ctc/datasets/extract_blocks_and_transactions.py
--rw-r--r--   0        0        0     2348 2023-05-30 06:43:40.603733 checkthechain-0.3.4/src/ctc/datasets/extract_erc20_transfers.py
--rw-r--r--   0        0        0      162 2022-11-23 19:36:31.107400 checkthechain-0.3.4/src/ctc/db/__init__.py
--rw-r--r--   0        0        0     3217 2023-04-15 07:07:44.333514 checkthechain-0.3.4/src/ctc/db/connect_utils.py
--rw-r--r--   0        0        0     2890 2023-02-26 20:15:07.410640 checkthechain-0.3.4/src/ctc/db/intake_utils.py
--rw-r--r--   0        0        0      109 2023-02-26 20:15:07.410802 checkthechain-0.3.4/src/ctc/db/management/__init__.py
--rw-r--r--   0        0        0      997 2023-02-26 18:21:06.948577 checkthechain-0.3.4/src/ctc/db/management/active_utils.py
--rw-r--r--   0        0        0     8200 2023-03-24 17:28:52.210535 checkthechain-0.3.4/src/ctc/db/management/dba_utils.py
--rw-r--r--   0        0        0      634 2023-02-26 20:15:07.411288 checkthechain-0.3.4/src/ctc/db/management/reorg_utils.py
--rw-r--r--   0        0        0     3594 2023-02-27 18:50:47.123257 checkthechain-0.3.4/src/ctc/db/management/version_utils.py
--rw-r--r--   0        0        0     1879 2023-04-14 22:55:23.964370 checkthechain-0.3.4/src/ctc/db/query_utils.py
--rw-r--r--   0        0        0     4735 2023-04-27 20:25:01.753860 checkthechain-0.3.4/src/ctc/db/schema_utils.py
--rw-r--r--   0        0        0      285 2023-02-26 18:21:06.950384 checkthechain-0.3.4/src/ctc/db/schemas/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.108677 checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/__init__.py
--rw-r--r--   0        0        0       43 2022-11-23 19:36:31.108781 checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/block_gas_stats/__init__.py
--rw-r--r--   0        0        0     1138 2023-02-26 20:15:07.412506 checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/block_gas_stats/block_gas_stats_schema_defs.py
--rw-r--r--   0        0        0       39 2022-11-23 19:36:31.108986 checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/erc20_state/__init__.py
--rw-r--r--   0        0        0     1259 2023-02-26 20:15:07.412713 checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/erc20_state/erc20_state_schema_defs.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.109185 checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/protocol_schemas/__init__.py
--rw-r--r--   0        0        0      792 2023-02-26 20:15:07.412923 checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/protocol_schemas/fourbyte_schema_defs.py
--rw-r--r--   0        0        0      634 2023-02-26 20:15:07.413166 checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/protocol_schemas/fuse_pools_schema_defs.py
--rw-r--r--   0        0        0      387 2023-02-26 20:15:07.413408 checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/protocol_schemas/uniswap_v2_pools_schema_defs.py
--rw-r--r--   0        0        0      436 2023-02-26 20:15:07.413623 checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/protocol_schemas/uniswap_v3_pools_schema_defs.py
--rw-r--r--   0        0        0      106 2022-11-23 19:36:31.109629 checkthechain-0.3.4/src/ctc/db/schemas/block_gas/__init__.py
--rw-r--r--   0        0        0      420 2022-11-23 19:36:31.109689 checkthechain-0.3.4/src/ctc/db/schemas/block_gas/block_gas_queries.py
--rw-r--r--   0        0        0      629 2023-02-26 20:15:07.414036 checkthechain-0.3.4/src/ctc/db/schemas/block_gas/block_gas_schema_defs.py
--rw-r--r--   0        0        0     3001 2023-04-15 23:24:04.689689 checkthechain-0.3.4/src/ctc/db/schemas/block_gas/block_gas_statements.py
--rw-r--r--   0        0        0      194 2022-11-23 19:36:31.109953 checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/__init__.py
--rw-r--r--   0        0        0      562 2023-02-26 20:15:07.414563 checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/block_timestamps_schema_defs.py
--rw-r--r--   0        0        0     6162 2023-04-15 23:08:40.662417 checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/block_timestamps_statements.py
--rw-r--r--   0        0        0     1596 2022-11-23 19:36:31.110176 checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_queries.py
--rw-r--r--   0        0        0     4431 2023-04-17 01:12:40.874133 checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_search.py
--rw-r--r--   0        0        0     3058 2023-02-26 20:15:07.415190 checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_statements.py
--rw-r--r--   0        0        0      126 2022-11-23 19:36:31.110528 checkthechain-0.3.4/src/ctc/db/schemas/blocks/__init__.py
--rw-r--r--   0        0        0    10484 2023-02-26 21:02:01.364459 checkthechain-0.3.4/src/ctc/db/schemas/blocks/blocks_intake.py
--rw-r--r--   0        0        0      343 2022-11-23 19:36:31.110828 checkthechain-0.3.4/src/ctc/db/schemas/blocks/blocks_queries.py
--rw-r--r--   0        0        0      725 2023-02-26 20:15:07.415649 checkthechain-0.3.4/src/ctc/db/schemas/blocks/blocks_schema_defs.py
--rw-r--r--   0        0        0     7041 2023-02-27 06:50:44.454081 checkthechain-0.3.4/src/ctc/db/schemas/blocks/blocks_statements.py
--rw-r--r--   0        0        0      154 2022-11-23 19:36:31.111040 checkthechain-0.3.4/src/ctc/db/schemas/contract_abis/__init__.py
--rw-r--r--   0        0        0     1155 2023-02-26 20:15:07.416090 checkthechain-0.3.4/src/ctc/db/schemas/contract_abis/contract_abis_intake.py
--rw-r--r--   0        0        0      406 2022-11-23 19:36:31.111159 checkthechain-0.3.4/src/ctc/db/schemas/contract_abis/contract_abis_queries.py
--rw-r--r--   0        0        0      392 2023-02-26 20:15:07.416278 checkthechain-0.3.4/src/ctc/db/schemas/contract_abis/contract_abis_schema_defs.py
--rw-r--r--   0        0        0     2403 2023-03-04 08:00:44.984031 checkthechain-0.3.4/src/ctc/db/schemas/contract_abis/contract_abis_statements.py
--rw-r--r--   0        0        0      198 2022-11-23 19:36:31.111410 checkthechain-0.3.4/src/ctc/db/schemas/contract_creation_blocks/__init__.py
--rw-r--r--   0        0        0     1031 2023-02-26 20:15:07.416737 checkthechain-0.3.4/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_intake.py
--rw-r--r--   0        0        0      505 2022-11-23 19:36:31.111535 checkthechain-0.3.4/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_queries.py
--rw-r--r--   0        0        0      534 2023-02-26 20:15:07.416982 checkthechain-0.3.4/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_schema_defs.py
--rw-r--r--   0        0        0     2081 2023-03-06 04:31:37.480699 checkthechain-0.3.4/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_statements.py
--rw-r--r--   0        0        0      138 2022-11-23 19:36:31.111785 checkthechain-0.3.4/src/ctc/db/schemas/dex_pools/__init__.py
--rw-r--r--   0        0        0     1576 2023-02-26 20:15:07.417521 checkthechain-0.3.4/src/ctc/db/schemas/dex_pools/dex_pools_intake.py
--rw-r--r--   0        0        0      578 2022-11-23 19:36:31.111973 checkthechain-0.3.4/src/ctc/db/schemas/dex_pools/dex_pools_queries.py
--rw-r--r--   0        0        0     1094 2023-02-26 20:15:07.417730 checkthechain-0.3.4/src/ctc/db/schemas/dex_pools/dex_pools_schema_defs.py
--rw-r--r--   0        0        0     6060 2023-04-12 21:15:00.071455 checkthechain-0.3.4/src/ctc/db/schemas/dex_pools/dex_pools_statements.py
--rw-r--r--   0        0        0      158 2022-11-23 19:36:31.112442 checkthechain-0.3.4/src/ctc/db/schemas/erc20_metadata/__init__.py
--rw-r--r--   0        0        0      761 2023-02-26 20:15:07.418167 checkthechain-0.3.4/src/ctc/db/schemas/erc20_metadata/erc20_metadata_intake.py
--rw-r--r--   0        0        0      419 2023-02-26 18:21:06.953935 checkthechain-0.3.4/src/ctc/db/schemas/erc20_metadata/erc20_metadata_queries.py
--rw-r--r--   0        0        0      765 2023-02-26 20:15:07.418402 checkthechain-0.3.4/src/ctc/db/schemas/erc20_metadata/erc20_metadata_schema_defs.py
--rw-r--r--   0        0        0     3673 2023-04-11 21:30:22.630170 checkthechain-0.3.4/src/ctc/db/schemas/erc20_metadata/erc20_metadata_statements.py
--rw-r--r--   0        0        0      126 2023-02-26 18:21:06.954232 checkthechain-0.3.4/src/ctc/db/schemas/events/__init__.py
--rw-r--r--   0        0        0     2217 2023-04-10 04:00:25.884785 checkthechain-0.3.4/src/ctc/db/schemas/events/events_intake.py
--rw-r--r--   0        0        0      359 2023-04-10 23:47:03.987654 checkthechain-0.3.4/src/ctc/db/schemas/events/events_queries.py
--rw-r--r--   0        0        0     2896 2023-04-27 21:04:55.972761 checkthechain-0.3.4/src/ctc/db/schemas/events/events_schema_defs.py
--rw-r--r--   0        0        0    12138 2023-04-12 19:57:20.128959 checkthechain-0.3.4/src/ctc/db/schemas/events/events_statements.py
--rw-r--r--   0        0        0       43 2022-11-23 19:36:31.112900 checkthechain-0.3.4/src/ctc/db/schemas/schema_versions/__init__.py
--rw-r--r--   0        0        0      503 2023-02-26 20:15:07.419573 checkthechain-0.3.4/src/ctc/db/schemas/schema_versions/schema_versions_schema_defs.py
--rw-r--r--   0        0        0      151 2023-02-26 18:21:06.955047 checkthechain-0.3.4/src/ctc/db/schemas/transactions/__init__.py
--rw-r--r--   0        0        0     3065 2023-02-26 20:15:07.419798 checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_intake.py
--rw-r--r--   0        0        0     1084 2023-02-26 18:21:06.955542 checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_queries.py
--rw-r--r--   0        0        0     1505 2023-02-26 20:15:07.419998 checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_schema_defs.py
--rw-r--r--   0        0        0      125 2023-02-26 18:21:06.956032 checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_statements/__init__.py
--rw-r--r--   0        0        0     2343 2023-04-27 06:04:57.381242 checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_statements/composite_block_transactions.py
--rw-r--r--   0        0        0     3690 2023-02-27 06:48:19.824368 checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_statements/table_block_transaction_queries.py
--rw-r--r--   0        0        0     3251 2023-03-10 20:38:54.085113 checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_statements/table_transactions.py
--rw-r--r--   0        0        0        1 2022-11-23 19:36:31.148839 checkthechain-0.3.4/src/ctc/defi/__init__.py
--rw-r--r--   0        0        0    39847 2023-04-11 15:01:03.698383 checkthechain-0.3.4/src/ctc/defi/cex_utils.py
--rw-r--r--   0        0        0       21 2022-11-23 19:36:31.149006 checkthechain-0.3.4/src/ctc/defi/dex_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.149080 checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/__init__.py
--rw-r--r--   0        0        0     1056 2022-11-23 19:36:31.149155 checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/amm_spec.py
--rw-r--r--   0        0        0       84 2022-11-23 19:36:31.149422 checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/cpmm/__init__.py
--rw-r--r--   0        0        0     3241 2023-04-10 01:05:06.123710 checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_liquidity.py
--rw-r--r--   0        0        0     1292 2023-04-17 01:28:17.884516 checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_spec.py
--rw-r--r--   0        0        0     9425 2022-11-23 19:36:31.149776 checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_summary.py
--rw-r--r--   0        0        0     7780 2023-04-12 21:01:00.654910 checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_trade.py
--rw-r--r--   0        0        0       37 2022-11-23 19:36:31.149993 checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/stableswap/__init__.py
--rw-r--r--   0        0        0      333 2022-11-23 19:36:31.150062 checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/stableswap/stableswap_operations.py
--rw-r--r--   0        0        0      151 2022-11-23 19:36:31.150205 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/__init__.py
--rw-r--r--   0        0        0    22413 2023-05-03 23:49:39.987609 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_class.py
--rw-r--r--   0        0        0     3458 2023-02-26 18:21:07.009571 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_class_utils.py
--rw-r--r--   0        0        0     1523 2023-04-12 02:18:53.791732 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_directory.py
--rw-r--r--   0        0        0      145 2022-11-23 19:36:31.150615 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_functions/__init__.py
--rw-r--r--   0        0        0     2749 2023-02-26 18:21:07.009954 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_functions/dex_balance_functions.py
--rw-r--r--   0        0        0     1603 2023-02-26 18:21:07.010224 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_functions/dex_metadata_functions.py
--rw-r--r--   0        0        0     2038 2023-02-26 18:21:07.010390 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_functions/dex_pools_functions.py
--rw-r--r--   0        0        0     1510 2023-04-17 01:11:51.919003 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_functions/dex_trade_functions.py
--rw-r--r--   0        0        0      184 2022-11-23 19:36:31.151177 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_implementations/__init__.py
--rw-r--r--   0        0        0     5880 2023-04-11 02:43:28.475321 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_implementations/balancer_dex.py
--rw-r--r--   0        0        0     7488 2023-04-11 02:44:21.401565 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_implementations/curve_dex.py
--rw-r--r--   0        0        0      207 2022-11-23 19:36:31.151507 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_implementations/sushi_dex.py
--rw-r--r--   0        0        0     4350 2023-04-12 22:58:36.356923 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_implementations/uniswap_v2_dex.py
--rw-r--r--   0        0        0     3932 2023-04-11 00:19:46.796938 checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_implementations/uniswap_v3_dex.py
--rw-r--r--   0        0        0       31 2022-11-23 19:36:31.151852 checkthechain-0.3.4/src/ctc/defi/lending_utils/__init__.py
--rw-r--r--   0        0        0     7740 2023-04-11 05:05:46.922489 checkthechain-0.3.4/src/ctc/defi/lending_utils/lending_summary.py
--rw-r--r--   0        0        0        1 2023-04-15 16:02:19.893267 checkthechain-0.3.4/src/ctc/defi/metric_utils/__init__.py
--rw-r--r--   0        0        0     1965 2023-04-11 21:23:13.516151 checkthechain-0.3.4/src/ctc/defi/metric_utils/ohlc_utils.py
--rw-r--r--   0        0        0      346 2022-11-23 19:36:31.152114 checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/README.md
--rw-r--r--   0        0        0      103 2022-11-23 19:36:31.152177 checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/__init__.py
--rw-r--r--   0        0        0     4043 2023-02-26 18:21:07.012053 checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/feed_utils.py
--rw-r--r--   0        0        0     2824 2023-04-11 05:41:47.387268 checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/twap_crud.py
--rw-r--r--   0        0        0      936 2023-04-11 05:24:45.040006 checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/twap_data.py
--rw-r--r--   0        0        0     2630 2023-04-11 05:25:54.330704 checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/twap_data_sources.py
--rw-r--r--   0        0        0     1292 2023-04-11 04:55:26.105147 checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/twap_filter.py
--rw-r--r--   0        0        0      442 2023-04-17 01:29:49.343807 checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/twap_spec.py
--rw-r--r--   0        0        0      365 2023-02-26 18:21:06.956840 checkthechain-0.3.4/src/ctc/evm/__init__.py
--rw-r--r--   0        0        0      131 2022-11-23 19:36:31.113210 checkthechain-0.3.4/src/ctc/evm/abi_utils/__init__.py
--rw-r--r--   0        0        0     2256 2023-05-04 21:17:33.110466 checkthechain-0.3.4/src/ctc/evm/abi_utils/abi_coding_utils.py
--rw-r--r--   0        0        0      189 2022-11-23 19:36:31.113375 checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/__init__.py
--rw-r--r--   0        0        0     2698 2022-11-23 19:36:31.113461 checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_comparison.py
--rw-r--r--   0        0        0     1361 2023-02-26 18:21:06.957338 checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_decompilation.py
--rw-r--r--   0        0        0     2142 2023-02-26 18:21:06.957664 checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_io.py
--rw-r--r--   0        0        0      660 2022-11-23 19:36:31.113721 checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_modification.py
--rw-r--r--   0        0        0     9934 2023-04-11 03:28:48.635201 checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_summary.py
--rw-r--r--   0        0        0      137 2023-03-04 05:46:27.752144 checkthechain-0.3.4/src/ctc/evm/abi_utils/event_abi_utils/__init__.py
--rw-r--r--   0        0        0     6278 2023-04-11 17:04:41.509191 checkthechain-0.3.4/src/ctc/evm/abi_utils/event_abi_utils/event_abi_coding.py
--rw-r--r--   0        0        0    14548 2023-06-03 00:20:08.972191 checkthechain-0.3.4/src/ctc/evm/abi_utils/event_abi_utils/event_abi_coding_polars.py
--rw-r--r--   0        0        0     2650 2023-04-11 17:23:39.585194 checkthechain-0.3.4/src/ctc/evm/abi_utils/event_abi_utils/event_abi_parsing.py
--rw-r--r--   0        0        0     3660 2023-03-04 07:55:53.565102 checkthechain-0.3.4/src/ctc/evm/abi_utils/event_abi_utils/event_abi_queries.py
--rw-r--r--   0        0        0      107 2022-11-23 19:36:31.114446 checkthechain-0.3.4/src/ctc/evm/abi_utils/function_abi_utils/__init__.py
--rw-r--r--   0        0        0     8050 2023-04-11 16:54:40.278301 checkthechain-0.3.4/src/ctc/evm/abi_utils/function_abi_utils/function_abi_coding.py
--rw-r--r--   0        0        0     8453 2023-02-26 18:21:06.958642 checkthechain-0.3.4/src/ctc/evm/abi_utils/function_abi_utils/function_abi_parsing.py
--rw-r--r--   0        0        0     5155 2023-05-03 21:01:44.378805 checkthechain-0.3.4/src/ctc/evm/abi_utils/function_abi_utils/function_abi_queries.py
--rw-r--r--   0        0        0      129 2023-02-26 18:21:06.959059 checkthechain-0.3.4/src/ctc/evm/address_utils/__init__.py
--rw-r--r--   0        0        0     1555 2023-04-11 17:07:31.645090 checkthechain-0.3.4/src/ctc/evm/address_utils/address_data.py
--rw-r--r--   0        0        0     2881 2023-02-26 18:21:06.959458 checkthechain-0.3.4/src/ctc/evm/address_utils/address_resolution.py
--rw-r--r--   0        0        0     3628 2023-02-26 18:21:06.959812 checkthechain-0.3.4/src/ctc/evm/address_utils/address_summary.py
--rw-r--r--   0        0        0     6147 2023-04-11 03:41:52.412674 checkthechain-0.3.4/src/ctc/evm/address_utils/address_transactions.py
--rw-r--r--   0        0        0      177 2022-11-23 19:36:31.115455 checkthechain-0.3.4/src/ctc/evm/binary_utils/__init__.py
--rw-r--r--   0        0        0     7187 2023-04-11 17:24:12.284270 checkthechain-0.3.4/src/ctc/evm/binary_utils/format_utils.py
--rw-r--r--   0        0        0     3169 2023-04-17 01:02:40.149889 checkthechain-0.3.4/src/ctc/evm/binary_utils/hash_utils.py
--rw-r--r--   0        0        0     8948 2023-04-11 17:11:36.961031 checkthechain-0.3.4/src/ctc/evm/binary_utils/rlp_utils.py
--rw-r--r--   0        0        0      146 2022-11-23 19:36:31.115957 checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/__init__.py
--rw-r--r--   0        0        0     7465 2022-11-23 19:36:31.116055 checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/eip712_utils.py
--rw-r--r--   0        0        0     1407 2023-04-11 17:13:01.266528 checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/key_utils.py
--rw-r--r--   0        0        0     4915 2022-11-23 19:36:31.116213 checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/secp256k1_utils.py
--rw-r--r--   0        0        0     2850 2023-04-11 17:12:22.146113 checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/signature_creation.py
--rw-r--r--   0        0        0     2835 2023-04-11 17:11:56.281971 checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/signature_recovery.py
--rw-r--r--   0        0        0     1926 2023-04-11 17:16:27.004803 checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/vrs_utils.py
--rw-r--r--   0        0        0      280 2023-05-30 06:46:30.790511 checkthechain-0.3.4/src/ctc/evm/block_utils/__init__.py
--rw-r--r--   0        0        0     2750 2023-04-11 17:18:20.638063 checkthechain-0.3.4/src/ctc/evm/block_utils/block_coding.py
--rw-r--r--   0        0        0      608 2023-02-26 18:21:06.960791 checkthechain-0.3.4/src/ctc/evm/block_utils/block_convert.py
--rw-r--r--   0        0        0     6865 2023-05-09 04:17:37.723832 checkthechain-0.3.4/src/ctc/evm/block_utils/block_crud.py
--rw-r--r--   0        0        0     8315 2023-06-03 00:20:08.973363 checkthechain-0.3.4/src/ctc/evm/block_utils/block_gas.py
--rw-r--r--   0        0        0     1083 2023-02-26 18:21:06.961562 checkthechain-0.3.4/src/ctc/evm/block_utils/block_hashes.py
--rw-r--r--   0        0        0     1990 2023-02-26 18:21:06.961734 checkthechain-0.3.4/src/ctc/evm/block_utils/block_normalize.py
--rw-r--r--   0        0        0      662 2023-05-30 06:46:30.790714 checkthechain-0.3.4/src/ctc/evm/block_utils/block_prices.py
--rw-r--r--   0        0        0     5580 2023-05-27 19:14:13.240378 checkthechain-0.3.4/src/ctc/evm/block_utils/block_samples.py
--rw-r--r--   0        0        0     2759 2023-05-27 15:37:02.677178 checkthechain-0.3.4/src/ctc/evm/block_utils/block_summary.py
--rw-r--r--   0        0        0      137 2023-05-27 19:01:35.203629 checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/__init__.py
--rw-r--r--   0        0        0     3690 2023-05-30 06:46:30.791681 checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/block_time_bins.py
--rw-r--r--   0        0        0     6100 2023-02-26 18:21:06.962078 checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/block_time_predictions.py
--rw-r--r--   0        0        0     2437 2023-02-26 18:21:06.962477 checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/block_to_timestamp.py
--rw-r--r--   0        0        0      133 2022-11-23 19:36:31.118022 checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/timestamp_to_block/__init__.py
--rw-r--r--   0        0        0     3620 2023-02-26 18:21:06.962780 checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_plural.py
--rw-r--r--   0        0        0     4479 2023-02-26 18:21:06.962964 checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_range.py
--rw-r--r--   0        0        0     6005 2023-05-27 19:13:07.231807 checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_search.py
--rw-r--r--   0        0        0     4136 2023-05-27 19:13:12.416617 checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_singular.py
--rw-r--r--   0        0        0       64 2023-02-26 18:21:06.963936 checkthechain-0.3.4/src/ctc/evm/consensus_utils/__init__.py
--rw-r--r--   0        0        0     4002 2023-02-26 18:21:06.964193 checkthechain-0.3.4/src/ctc/evm/consensus_utils/consensus_queries.py
--rw-r--r--   0        0        0     1665 2023-04-28 23:57:21.283647 checkthechain-0.3.4/src/ctc/evm/consensus_utils/consensus_requests.py
--rw-r--r--   0        0        0     2118 2023-02-26 18:21:06.964748 checkthechain-0.3.4/src/ctc/evm/consensus_utils/consensus_spec.py
--rw-r--r--   0        0        0       96 2023-02-26 18:21:06.965010 checkthechain-0.3.4/src/ctc/evm/contract_utils/__init__.py
--rw-r--r--   0        0        0     6575 2023-04-11 17:04:21.999102 checkthechain-0.3.4/src/ctc/evm/contract_utils/contract_creations.py
--rw-r--r--   0        0        0     9875 2023-02-26 18:21:06.965502 checkthechain-0.3.4/src/ctc/evm/contract_utils/contract_proxies.py
--rw-r--r--   0        0        0      979 2023-02-26 18:21:06.965736 checkthechain-0.3.4/src/ctc/evm/contract_utils/contract_tests.py
--rw-r--r--   0        0        0      200 2022-11-23 19:36:31.118451 checkthechain-0.3.4/src/ctc/evm/erc20_utils/__init__.py
--rw-r--r--   0        0        0     5922 2023-04-11 15:05:42.419653 checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_events.py
--rw-r--r--   0        0        0     2179 2023-04-12 16:02:37.446080 checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_generic.py
--rw-r--r--   0        0        0    13187 2023-06-03 00:20:08.974291 checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_metadata.py
--rw-r--r--   0        0        0     6574 2023-04-12 16:01:20.761726 checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_normalize.py
--rw-r--r--   0        0        0     3433 2022-11-23 19:36:31.118864 checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_spec.py
--rw-r--r--   0        0        0    12612 2023-05-03 23:48:57.178118 checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_state.py
--rw-r--r--   0        0        0     1871 2023-02-26 18:21:06.967336 checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_summary.py
--rw-r--r--   0        0        0      188 2023-02-26 18:21:06.967455 checkthechain-0.3.4/src/ctc/evm/erc4626_utils/__init__.py
--rw-r--r--   0        0        0     4233 2023-04-12 06:22:58.195596 checkthechain-0.3.4/src/ctc/evm/erc4626_utils/erc4626_events.py
--rw-r--r--   0        0        0     1097 2023-02-26 18:21:06.967850 checkthechain-0.3.4/src/ctc/evm/erc4626_utils/erc4626_metadata.py
--rw-r--r--   0        0        0     5796 2023-04-10 06:23:55.747564 checkthechain-0.3.4/src/ctc/evm/erc4626_utils/erc4626_normalize.py
--rw-r--r--   0        0        0    10976 2023-02-26 18:21:06.968082 checkthechain-0.3.4/src/ctc/evm/erc4626_utils/erc4626_spec.py
--rw-r--r--   0        0        0    23565 2023-02-26 18:21:06.968309 checkthechain-0.3.4/src/ctc/evm/erc4626_utils/erc4626_state.py
--rw-r--r--   0        0        0      147 2023-02-26 18:21:06.968426 checkthechain-0.3.4/src/ctc/evm/erc721_utils/__init__.py
--rw-r--r--   0        0        0     1740 2023-04-11 15:04:56.245383 checkthechain-0.3.4/src/ctc/evm/erc721_utils/erc721_events.py
--rw-r--r--   0        0        0     1930 2023-02-26 18:21:06.968922 checkthechain-0.3.4/src/ctc/evm/erc721_utils/erc721_metadata.py
--rw-r--r--   0        0        0     2967 2023-04-11 15:04:52.910074 checkthechain-0.3.4/src/ctc/evm/erc721_utils/erc721_ownership.py
--rw-r--r--   0        0        0     5323 2023-02-26 18:21:06.969310 checkthechain-0.3.4/src/ctc/evm/erc721_utils/erc721_spec.py
--rw-r--r--   0        0        0     3108 2023-02-26 18:21:06.969455 checkthechain-0.3.4/src/ctc/evm/erc721_utils/erc721_state.py
--rw-r--r--   0        0        0       24 2022-11-23 19:36:31.120339 checkthechain-0.3.4/src/ctc/evm/eth_utils/__init__.py
--rw-r--r--   0        0        0     4151 2023-02-26 18:21:06.969708 checkthechain-0.3.4/src/ctc/evm/eth_utils/eth_crud.py
--rw-r--r--   0        0        0       96 2023-02-26 18:21:06.969843 checkthechain-0.3.4/src/ctc/evm/event_utils/__init__.py
--rw-r--r--   0        0        0    15537 2023-04-13 02:52:22.209972 checkthechain-0.3.4/src/ctc/evm/event_utils/event_crud.py
--rw-r--r--   0        0        0     6151 2023-05-02 21:14:45.321958 checkthechain-0.3.4/src/ctc/evm/event_utils/event_hybrid_queries.py
--rw-r--r--   0        0        0     1909 2023-04-11 15:05:32.152407 checkthechain-0.3.4/src/ctc/evm/event_utils/event_metadata.py
--rw-r--r--   0        0        0     7662 2023-04-11 17:14:11.631727 checkthechain-0.3.4/src/ctc/evm/event_utils/event_node_utils.py
--rw-r--r--   0        0        0    10602 2023-05-02 21:14:20.680012 checkthechain-0.3.4/src/ctc/evm/event_utils/event_query_utils.py
--rw-r--r--   0        0        0       33 2022-11-23 19:36:31.121258 checkthechain-0.3.4/src/ctc/evm/network_utils/__init__.py
--rw-r--r--   0        0        0     2501 2023-02-26 18:21:06.972751 checkthechain-0.3.4/src/ctc/evm/network_utils/network_directory.py
--rw-r--r--   0        0        0       89 2023-03-11 04:51:22.361782 checkthechain-0.3.4/src/ctc/evm/trace_utils/__init__.py
--rw-r--r--   0        0        0     4160 2023-05-05 05:28:17.202870 checkthechain-0.3.4/src/ctc/evm/trace_utils/specific_traces.py
--rw-r--r--   0        0        0     2259 2023-03-06 03:07:15.579397 checkthechain-0.3.4/src/ctc/evm/trace_utils/trace_crud.py
--rw-r--r--   0        0        0     4712 2023-02-26 20:15:07.421666 checkthechain-0.3.4/src/ctc/evm/trace_utils/trace_state_diff.py
--rw-r--r--   0        0        0      244 2023-02-26 18:21:06.973711 checkthechain-0.3.4/src/ctc/evm/transaction_utils/__init__.py
--rw-r--r--   0        0        0     3687 2023-04-27 06:18:19.829021 checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_convert.py
--rw-r--r--   0        0        0     6691 2023-02-26 20:15:07.422149 checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_crud.py
--rw-r--r--   0        0        0      722 2023-02-26 18:21:06.974413 checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_hashes.py
--rw-r--r--   0        0        0     3119 2023-04-12 19:53:53.308960 checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_serialize.py
--rw-r--r--   0        0        0     4298 2023-04-12 19:55:41.976804 checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_signatures.py
--rw-r--r--   0        0        0     7878 2023-04-11 17:08:12.970832 checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_summary.py
--rw-r--r--   0        0        0     2911 2023-04-12 16:41:24.818020 checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_types.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.122150 checkthechain-0.3.4/src/ctc/protocols/__init__.py
--rw-r--r--   0        0        0      210 2022-11-23 19:36:31.122290 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/__init__.py
--rw-r--r--   0        0        0     7437 2023-04-17 01:33:49.120175 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_interest_rates.py
--rw-r--r--   0        0        0     2271 2023-04-10 04:41:13.923918 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_lending_pool.py
--rw-r--r--   0        0        0     3034 2023-02-26 18:21:06.976319 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_oracle.py
--rw-r--r--   0        0        0     1198 2023-02-26 18:21:06.976540 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_pool_tokens.py
--rw-r--r--   0        0        0     3099 2023-02-26 18:21:06.976782 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_rewards.py
--rw-r--r--   0        0        0      953 2023-04-12 02:17:55.732920 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_spec.py
--rw-r--r--   0        0        0    14153 2023-04-12 02:17:27.412342 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_summaries.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.122992 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/cli/__init__.py
--rw-r--r--   0        0        0      870 2023-01-02 06:57:18.122699 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/cli/aave_addresses_command.py
--rw-r--r--   0        0        0     3072 2022-11-23 19:36:31.123144 checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/cli/aave_command.py
--rw-r--r--   0        0        0      165 2022-11-23 19:36:31.123232 checkthechain-0.3.4/src/ctc/protocols/balancer_utils/__init__.py
--rw-r--r--   0        0        0     4074 2023-02-26 18:21:06.977445 checkthechain-0.3.4/src/ctc/protocols/balancer_utils/balancer_spec.py
--rw-r--r--   0        0        0     3341 2023-04-11 02:48:49.301350 checkthechain-0.3.4/src/ctc/protocols/balancer_utils/pool_metadata.py
--rw-r--r--   0        0        0     4646 2023-04-11 05:41:02.218451 checkthechain-0.3.4/src/ctc/protocols/balancer_utils/pool_plots.py
--rw-r--r--   0        0        0     6265 2023-02-26 18:21:06.978055 checkthechain-0.3.4/src/ctc/protocols/balancer_utils/pool_state.py
--rw-r--r--   0        0        0     6171 2023-04-17 01:25:48.874215 checkthechain-0.3.4/src/ctc/protocols/balancer_utils/pool_summary.py
--rw-r--r--   0        0        0     1007 2022-11-23 19:36:31.123708 checkthechain-0.3.4/src/ctc/protocols/balancer_utils/pool_trades.py
--rw-r--r--   0        0        0      237 2022-11-23 19:36:31.123840 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/__init__.py
--rw-r--r--   0        0        0     6981 2023-02-26 18:21:06.978589 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_aggregators.py
--rw-r--r--   0        0        0      147 2022-11-23 19:36:31.124095 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/__init__.py
--rw-r--r--   0        0        0     2083 2023-04-11 05:31:39.920503 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/feed_composites.py
--rw-r--r--   0        0        0     3101 2023-04-11 05:27:03.456016 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/feed_data.py
--rw-r--r--   0        0        0     3181 2023-02-26 18:21:06.979122 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/feed_datum.py
--rw-r--r--   0        0        0     2291 2023-04-11 14:58:42.923101 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/feed_datum_by_block.py
--rw-r--r--   0        0        0     7300 2023-05-30 06:46:30.792533 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/feed_events.py
--rw-r--r--   0        0        0      138 2022-11-23 19:36:31.124610 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_db/__init__.py
--rw-r--r--   0        0        0     9709 2023-04-12 02:16:57.774414 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_intake.py
--rw-r--r--   0        0        0      509 2022-11-23 19:36:31.124755 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_queries.py
--rw-r--r--   0        0        0     1458 2023-02-26 20:15:07.422868 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_schema_defs.py
--rw-r--r--   0        0        0     6188 2023-02-27 06:48:28.002164 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_statements.py
--rw-r--r--   0        0        0     3742 2023-02-26 18:21:06.980172 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_feed_metadata.py
--rw-r--r--   0        0        0      818 2023-02-26 18:21:06.980357 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_helpers.py
--rw-r--r--   0        0        0     4401 2023-04-12 02:16:48.985174 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_registry.py
--rw-r--r--   0        0        0     2921 2023-04-17 01:06:07.155895 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_spec.py
--rw-r--r--   0        0        0     6328 2023-04-10 03:26:37.038448 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_summary.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.125353 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/cli/__init__.py
--rw-r--r--   0        0        0     4564 2023-04-10 03:42:49.095411 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/cli/chainlink_command.py
--rw-r--r--   0        0        0     2038 2023-02-26 18:21:06.981259 checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/cli/chainlink_ls_command.py
--rw-r--r--   0        0        0       55 2022-11-23 19:36:31.125633 checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.125714 checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/cli/__init__.py
--rw-r--r--   0        0        0     3751 2023-04-14 06:36:37.709398 checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/cli/cg_command.py
--rw-r--r--   0        0        0      138 2022-11-23 19:36:31.125960 checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/coingecko_db/__init__.py
--rw-r--r--   0        0        0      957 2023-02-26 20:15:07.423297 checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_intake.py
--rw-r--r--   0        0        0      331 2023-02-26 18:21:06.981971 checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_queries.py
--rw-r--r--   0        0        0      773 2023-04-17 01:08:19.565253 checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_schema_defs.py
--rw-r--r--   0        0        0     3074 2023-04-12 23:19:05.754820 checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_statements.py
--rw-r--r--   0        0        0     5795 2023-02-26 18:21:06.982284 checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/market_utils.py
--rw-r--r--   0        0        0    16600 2023-02-27 08:16:17.715834 checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/token_utils.py
--rw-r--r--   0        0        0       29 2022-11-23 19:36:31.126557 checkthechain-0.3.4/src/ctc/protocols/compound_utils/__init__.py
--rw-r--r--   0        0        0     2397 2023-02-26 18:21:06.982879 checkthechain-0.3.4/src/ctc/protocols/compound_utils/compound_crud.py
--rw-r--r--   0        0        0      168 2022-11-23 19:36:31.126693 checkthechain-0.3.4/src/ctc/protocols/curve_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.126751 checkthechain-0.3.4/src/ctc/protocols/curve_utils/cli/__init__.py
--rw-r--r--   0        0        0     1690 2022-11-23 19:36:31.126829 checkthechain-0.3.4/src/ctc/protocols/curve_utils/cli/curve_pools_command.py
--rw-r--r--   0        0        0     5258 2023-04-17 01:26:07.392801 checkthechain-0.3.4/src/ctc/protocols/curve_utils/curve_spec.py
--rw-r--r--   0        0        0     3714 2023-02-26 18:21:06.983220 checkthechain-0.3.4/src/ctc/protocols/curve_utils/metapool_utils.py
--rw-r--r--   0        0        0    15567 2023-04-17 01:36:34.284052 checkthechain-0.3.4/src/ctc/protocols/curve_utils/pool_lists.py
--rw-r--r--   0        0        0     4951 2023-02-26 18:21:06.983838 checkthechain-0.3.4/src/ctc/protocols/curve_utils/pool_metadata.py
--rw-r--r--   0        0        0     7351 2023-04-11 02:49:36.985754 checkthechain-0.3.4/src/ctc/protocols/curve_utils/pool_parameters.py
--rw-r--r--   0        0        0     4085 2023-02-26 18:21:06.984206 checkthechain-0.3.4/src/ctc/protocols/curve_utils/pool_state.py
--rw-r--r--   0        0        0       49 2022-11-23 19:36:31.127594 checkthechain-0.3.4/src/ctc/protocols/ens_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.127647 checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.127712 checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/__init__.py
--rw-r--r--   0        0        0      813 2022-11-23 19:36:31.127791 checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/exists_command.py
--rw-r--r--   0        0        0      441 2022-11-23 19:36:31.127871 checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/hash_command.py
--rw-r--r--   0        0        0      765 2022-11-23 19:36:31.127934 checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/owner_command.py
--rw-r--r--   0        0        0      625 2022-11-23 19:36:31.127994 checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/records_command.py
--rw-r--r--   0        0        0      862 2022-11-23 19:36:31.128056 checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/resolve_command.py
--rw-r--r--   0        0        0      876 2022-11-23 19:36:31.128123 checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/reverse_command.py
--rw-r--r--   0        0        0     4278 2023-04-17 01:27:38.950415 checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens_command.py
--rw-r--r--   0        0        0      482 2022-11-23 19:36:31.128261 checkthechain-0.3.4/src/ctc/protocols/ens_utils/ens_directory.py
--rw-r--r--   0        0        0     3782 2023-04-11 04:50:29.681889 checkthechain-0.3.4/src/ctc/protocols/ens_utils/registrar.py
--rw-r--r--   0        0        0     7572 2023-04-13 02:54:35.167992 checkthechain-0.3.4/src/ctc/protocols/ens_utils/resolver.py
--rw-r--r--   0        0        0      132 2023-02-26 18:21:06.984864 checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/__init__.py
--rw-r--r--   0        0        0     3353 2023-04-17 01:27:53.003738 checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/abi_crud.py
--rw-r--r--   0        0        0     2596 2023-04-12 02:18:49.893638 checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/browser_utils.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.128654 checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/cli/__init__.py
--rw-r--r--   0        0        0     2635 2023-02-26 18:21:06.985639 checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/cli/etherscan_command.py
--rw-r--r--   0        0        0      326 2023-04-12 02:18:22.167751 checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/etherscan_spec.py
--rw-r--r--   0        0        0      703 2023-04-12 02:18:27.736358 checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/misc_crud.py
--rw-r--r--   0        0        0     4951 2023-04-12 02:18:47.139319 checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/url_crud.py
--rw-r--r--   0        0        0      119 2022-11-23 19:36:31.133315 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.133373 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/cli/__init__.py
--rw-r--r--   0        0        0     1407 2022-11-23 19:36:31.133450 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/cli/fourbyte_build_command.py
--rw-r--r--   0        0        0     3849 2022-11-23 19:36:31.133514 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/cli/fourbyte_command.py
--rw-r--r--   0        0        0      102 2022-11-23 19:36:31.133597 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_db/__init__.py
--rw-r--r--   0        0        0     1846 2023-02-26 20:15:07.423891 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_intake.py
--rw-r--r--   0        0        0     1856 2023-04-27 20:09:32.665313 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_schema_defs.py
--rw-r--r--   0        0        0     5593 2023-04-27 20:23:37.596062 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_statements.py
--rw-r--r--   0        0        0       90 2022-11-23 19:36:31.133972 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_queries/__init__.py
--rw-r--r--   0        0        0     2746 2023-04-27 20:24:38.665613 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_queries/general_queries.py
--rw-r--r--   0        0        0      393 2023-02-26 18:21:06.990217 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_queries/local_queries.py
--rw-r--r--   0        0        0     4042 2023-04-17 01:28:43.369803 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_queries/remote_queries.py
--rw-r--r--   0        0        0     3580 2023-02-26 18:21:06.990325 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_scrape.py
--rw-r--r--   0        0        0     1420 2023-04-17 01:28:32.903495 checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_spec.py
--rw-r--r--   0        0        0       20 2022-11-23 19:36:31.134412 checkthechain-0.3.4/src/ctc/protocols/g_uni_utils/__init__.py
--rw-r--r--   0        0        0     3624 2023-02-26 18:21:06.990518 checkthechain-0.3.4/src/ctc/protocols/g_uni_utils/crud.py
--rw-r--r--   0        0        0      670 2022-11-23 19:36:31.134602 checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/README.md
--rw-r--r--   0        0        0      149 2022-11-23 19:36:31.134662 checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.134718 checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/cli/__init__.py
--rw-r--r--   0        0        0     1036 2022-11-23 19:36:31.134790 checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/cli/gnosis_command.py
--rw-r--r--   0        0        0     2976 2023-04-11 05:28:54.333360 checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_events.py
--rw-r--r--   0        0        0     3793 2023-04-11 14:59:17.679623 checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_factory_events.py
--rw-r--r--   0        0        0     1552 2023-02-26 18:21:06.991058 checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_metadata.py
--rw-r--r--   0        0        0     7390 2023-04-17 01:07:53.696824 checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_spec.py
--rw-r--r--   0        0        0     8950 2023-04-13 22:50:55.610898 checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_summary.py
--rw-r--r--   0        0        0     6520 2023-04-11 16:33:17.017825 checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_transactions.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.135334 checkthechain-0.3.4/src/ctc/protocols/llama_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.135412 checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/__init__.py
--rw-r--r--   0        0        0      563 2022-11-23 19:36:31.135510 checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_chain_command.py
--rw-r--r--   0        0        0      637 2022-11-23 19:36:31.135597 checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_chains_command.py
--rw-r--r--   0        0        0      355 2022-11-23 19:36:31.135677 checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_command.py
--rw-r--r--   0        0        0      627 2022-11-23 19:36:31.135766 checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_pool_command.py
--rw-r--r--   0        0        0     3756 2023-04-17 01:08:32.684084 checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_pools_command.py
--rw-r--r--   0        0        0      877 2022-11-23 19:36:31.135929 checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_protocol_command.py
--rw-r--r--   0        0        0     1307 2022-11-23 19:36:31.135982 checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_protocols_command.py
--rw-r--r--   0        0        0     4886 2023-04-17 01:06:44.638753 checkthechain-0.3.4/src/ctc/protocols/llama_utils/llama_requests.py
--rw-r--r--   0        0        0     6140 2023-02-26 18:21:06.991562 checkthechain-0.3.4/src/ctc/protocols/llama_utils/llama_tvls.py
--rw-r--r--   0        0        0    10185 2023-04-17 01:08:15.444434 checkthechain-0.3.4/src/ctc/protocols/llama_utils/llama_yields.py
--rw-r--r--   0        0        0       88 2022-11-23 19:36:31.136328 checkthechain-0.3.4/src/ctc/protocols/multicall_utils/__init__.py
--rw-r--r--   0        0        0     4439 2023-04-11 16:49:40.251517 checkthechain-0.3.4/src/ctc/protocols/multicall_utils/call_utils.py
--rw-r--r--   0        0        0     1511 2023-04-17 01:06:25.624061 checkthechain-0.3.4/src/ctc/protocols/multicall_utils/multicall_spec.py
--rw-r--r--   0        0        0     3738 2023-04-12 02:17:20.118623 checkthechain-0.3.4/src/ctc/protocols/multicall_utils/multicalls_utils.py
--rw-r--r--   0        0        0       57 2022-11-23 19:36:31.136829 checkthechain-0.3.4/src/ctc/protocols/rari_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.136919 checkthechain-0.3.4/src/ctc/protocols/rari_utils/cli/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.137039 checkthechain-0.3.4/src/ctc/protocols/rari_utils/cli/rari/__init__.py
--rw-r--r--   0        0        0     2938 2022-11-23 19:36:31.137166 checkthechain-0.3.4/src/ctc/protocols/rari_utils/cli/rari/fuse_command.py
--rw-r--r--   0        0        0     1584 2022-11-23 19:36:31.137258 checkthechain-0.3.4/src/ctc/protocols/rari_utils/cli/rari/pools_command.py
--rw-r--r--   0        0        0     1367 2022-11-23 19:36:31.137399 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_lens/README.md
--rw-r--r--   0        0        0      108 2022-11-23 19:36:31.137466 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_lens/__init__.py
--rw-r--r--   0        0        0    21649 2022-11-23 19:36:31.137582 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_lens/lens_abis.py
--rw-r--r--   0        0        0     8029 2023-04-17 01:30:37.145025 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_lens/lens_spec.py
--rw-r--r--   0        0        0    15145 2023-04-17 01:30:56.860930 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_lens/primary_lens.py
--rw-r--r--   0        0        0      205 2022-11-23 19:36:31.137849 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_lens/secondary_lens.py
--rw-r--r--   0        0        0      231 2022-11-23 19:36:31.137957 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/__init__.py
--rw-r--r--   0        0        0      794 2023-02-26 18:21:06.993247 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/directory_metadata.py
--rw-r--r--   0        0        0      711 2022-11-23 19:36:31.138102 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/irm_metadata.py
--rw-r--r--   0        0        0     2913 2022-11-23 19:36:31.138171 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/pool_metadata.py
--rw-r--r--   0        0        0     2704 2022-11-23 19:36:31.138236 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/pool_state.py
--rw-r--r--   0        0        0     3188 2022-11-23 19:36:31.138313 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/pool_summary.py
--rw-r--r--   0        0        0     1311 2022-11-23 19:36:31.138413 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_metadata.py
--rw-r--r--   0        0        0       84 2022-11-23 19:36:31.138564 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_state/__init__.py
--rw-r--r--   0        0        0     3627 2022-11-23 19:36:31.138668 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_interest.py
--rw-r--r--   0        0        0     2071 2022-11-23 19:36:31.138773 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_price.py
--rw-r--r--   0        0        0     3658 2022-11-23 19:36:31.138888 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_usage.py
--rw-r--r--   0        0        0     5852 2023-04-17 01:28:05.297767 checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_summary.py
--rw-r--r--   0        0        0    89362 2022-11-23 19:36:31.139251 checkthechain-0.3.4/src/ctc/protocols/rari_utils/rari_abis.py
--rw-r--r--   0        0        0    11979 2023-02-26 18:21:06.993503 checkthechain-0.3.4/src/ctc/protocols/rari_utils/summary_utils.py
--rw-r--r--   0        0        0       56 2022-11-23 19:36:31.139484 checkthechain-0.3.4/src/ctc/protocols/sushi_utils/__init__.py
--rw-r--r--   0        0        0      337 2022-11-23 19:36:31.139559 checkthechain-0.3.4/src/ctc/protocols/sushi_utils/sushi_spec.py
--rw-r--r--   0        0        0      918 2023-02-26 18:21:06.993785 checkthechain-0.3.4/src/ctc/protocols/sushi_utils/sushiswap_crud.py
--rw-r--r--   0        0        0      166 2022-11-23 19:36:31.139748 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.139808 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/__init__.py
--rw-r--r--   0        0        0     1423 2022-11-23 19:36:31.139896 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/burns_command.py
--rw-r--r--   0        0        0     6445 2023-04-15 16:03:17.419508 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/chart_command.py
--rw-r--r--   0        0        0     1423 2022-11-23 19:36:31.140033 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/mints_command.py
--rw-r--r--   0        0        0     1846 2023-04-15 15:59:51.449246 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/pool_command.py
--rw-r--r--   0        0        0     1440 2022-11-23 19:36:31.140220 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/swaps_command.py
--rw-r--r--   0        0        0     8203 2023-04-11 04:48:00.558717 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_deltas.py
--rw-r--r--   0        0        0     5717 2023-04-15 15:59:32.040213 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_events.py
--rw-r--r--   0        0        0     2776 2023-04-12 16:09:31.994054 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_metadata.py
--rw-r--r--   0        0        0     5089 2023-04-17 01:27:08.232982 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_spec.py
--rw-r--r--   0        0        0     3887 2023-05-03 23:41:11.177114 checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_state.py
--rw-r--r--   0        0        0      151 2023-06-03 00:20:08.975286 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/__init__.py
--rw-r--r--   0        0        0      138 2022-11-23 19:36:31.141120 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/__init__.py
--rw-r--r--   0        0        0     1443 2023-02-26 18:21:06.994940 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/pool_derived_state.py
--rw-r--r--   0        0        0     3240 2023-02-26 18:21:06.995117 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/pool_immutables.py
--rw-r--r--   0        0        0     6560 2023-04-17 01:31:30.100039 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/pool_state.py
--rw-r--r--   0        0        0     3006 2023-02-26 18:21:06.995466 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/quoter.py
--rw-r--r--   0        0        0      860 2023-02-26 18:21:06.995686 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/tick_lens.py
--rw-r--r--   0        0        0     3562 2023-04-17 01:31:50.529264 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_crud.py
--rw-r--r--   0        0        0     3751 2023-02-26 18:21:06.996225 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_depth.py
--rw-r--r--   0        0        0     3163 2023-02-26 18:21:06.996363 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_spec.py
--rw-r--r--   0        0        0     6720 2023-06-03 00:20:08.975536 checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_swaps.py
--rw-r--r--   0        0        0      140 2022-11-23 19:36:31.141857 checkthechain-0.3.4/src/ctc/protocols/yearn_utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.141930 checkthechain-0.3.4/src/ctc/protocols/yearn_utils/cli/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-12 02:18:13.432357 checkthechain-0.3.4/src/ctc/protocols/yearn_utils/cli/yearn_addresses_command.py
--rw-r--r--   0        0        0     2553 2023-04-12 02:18:04.750648 checkthechain-0.3.4/src/ctc/protocols/yearn_utils/cli/yearn_command.py
--rw-r--r--   0        0        0     5692 2023-04-12 02:17:48.585548 checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_addresses.py
--rw-r--r--   0        0        0     1864 2022-11-23 19:36:31.142281 checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_spec.py
--rw-r--r--   0        0        0     2885 2023-04-11 05:22:09.399822 checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_strategies.py
--rw-r--r--   0        0        0     1200 2023-02-26 18:21:06.996752 checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_tvls.py
--rw-r--r--   0        0        0    11227 2023-04-11 03:24:04.115576 checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_vaults.py
--rw-r--r--   0        0        0     2327 2022-11-23 19:36:31.142631 checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_web_api.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.142664 checkthechain-0.3.4/src/ctc/py.typed
--rw-r--r--   0        0        0      370 2023-04-29 02:18:16.632039 checkthechain-0.3.4/src/ctc/rpc/__init__.py
--rw-r--r--   0        0        0      104 2022-11-23 19:36:31.142859 checkthechain-0.3.4/src/ctc/rpc/rpc_batch/__init__.py
--rw-r--r--   0        0        0    16275 2023-03-04 19:50:23.519624 checkthechain-0.3.4/src/ctc/rpc/rpc_batch/rpc_batch_constructors.py
--rw-r--r--   0        0        0    13042 2023-03-04 19:50:23.520213 checkthechain-0.3.4/src/ctc/rpc/rpc_batch/rpc_batch_executors.py
--rw-r--r--   0        0        0     4185 2023-04-13 02:20:26.971506 checkthechain-0.3.4/src/ctc/rpc/rpc_batch/rpc_batch_utils.py
--rw-r--r--   0        0        0      389 2023-02-26 18:21:06.998278 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/__init__.py
--rw-r--r--   0        0        0     2442 2023-04-11 16:31:38.655891 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_block_constructors.py
--rw-r--r--   0        0        0      602 2023-02-26 18:21:06.998793 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_dev_constructors.py
--rw-r--r--   0        0        0     2486 2023-02-26 18:21:06.998980 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_log_constructors.py
--rw-r--r--   0        0        0      951 2023-02-26 18:21:06.999159 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_mining_constructors.py
--rw-r--r--   0        0        0     1004 2023-02-26 18:21:06.999424 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_node_constructors.py
--rw-r--r--   0        0        0     3443 2023-04-11 16:30:45.199617 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_state_constructors.py
--rw-r--r--   0        0        0     1916 2023-02-26 18:21:06.999889 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_submission_constructors.py
--rw-r--r--   0        0        0     7325 2023-06-03 00:20:08.976370 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_trace_constructors.py
--rw-r--r--   0        0        0     2138 2023-04-11 16:31:54.035220 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_transaction_constructors.py
--rw-r--r--   0        0        0     2069 2023-02-26 18:21:07.000693 checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_whisper_constructors.py
--rw-r--r--   0        0        0        0 2023-03-11 18:04:07.082068 checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/__init__.py
--rw-r--r--   0        0        0     4653 2023-05-03 06:18:05.706354 checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/call_trace_decoder.py
--rw-r--r--   0        0        0     2258 2023-04-21 15:41:10.224968 checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/create_trace_decoder.py
--rw-r--r--   0        0        0      998 2023-03-26 06:20:45.338428 checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/log_decoder.py
--rw-r--r--   0        0        0     4653 2023-05-02 22:58:53.788729 checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/native_transfer_decoder.py
--rw-r--r--   0        0        0     6779 2023-05-03 16:33:35.235586 checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/slot_diff_decoder.py
--rw-r--r--   0        0        0      359 2023-02-26 18:21:07.000942 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/__init__.py
--rw-r--r--   0        0        0     3589 2022-11-23 19:36:31.144157 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_block_digestors.py
--rw-r--r--   0        0        0      552 2022-11-23 19:36:31.144227 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_dev_digestors.py
--rw-r--r--   0        0        0     3831 2022-11-23 19:36:31.144290 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_log_digestors.py
--rw-r--r--   0        0        0      773 2022-11-23 19:36:31.144353 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_mining_digestors.py
--rw-r--r--   0        0        0     1465 2022-11-23 19:36:31.144412 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_node_digestors.py
--rw-r--r--   0        0        0     1738 2022-11-23 19:36:31.144465 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_state_digestors.py
--rw-r--r--   0        0        0     1197 2022-11-23 19:36:31.144518 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_submission_digestors.py
--rw-r--r--   0        0        0     7929 2023-03-04 19:50:23.521981 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_trace_digestors.py
--rw-r--r--   0        0        0     2747 2022-11-23 19:36:31.144581 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_transaction_digestors.py
--rw-r--r--   0        0        0     1269 2022-11-23 19:36:31.144661 checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_whisper_digestors.py
--rw-r--r--   0        0        0      380 2023-04-29 02:55:17.696175 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/__init__.py
--rw-r--r--   0        0        0     4628 2023-05-04 00:21:12.284488 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_block_executors_async.py
--rw-r--r--   0        0        0     1437 2023-03-27 22:28:00.721319 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_dev_executors_async.py
--rw-r--r--   0        0        0     5279 2023-03-26 06:20:39.297576 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_log_executors_async.py
--rw-r--r--   0        0        0     2190 2023-02-26 18:21:07.002129 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_mining_executors_async.py
--rw-r--r--   0        0        0     2851 2023-02-26 18:21:07.002296 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_node_executors_async.py
--rw-r--r--   0        0        0     6117 2023-04-13 02:15:46.804141 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_state_executors_async.py
--rw-r--r--   0        0        0     3168 2023-02-26 18:21:07.002644 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_submission_executors_async.py
--rw-r--r--   0        0        0    10219 2023-03-04 19:50:23.522274 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_trace_executors_async.py
--rw-r--r--   0        0        0     4590 2023-02-26 18:21:07.003081 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_transaction_executors_async.py
--rw-r--r--   0        0        0     3970 2023-02-26 18:21:07.003260 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_whisper_executors_async.py
--rw-r--r--   0        0        0      372 2023-04-29 02:20:39.544187 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/__init__.py
--rw-r--r--   0        0        0     4530 2023-04-29 02:40:39.931253 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_block_executors_sync.py
--rw-r--r--   0        0        0     1381 2023-04-29 02:41:16.847417 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_dev_executors_sync.py
--rw-r--r--   0        0        0     5174 2023-04-29 02:42:15.741339 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_log_executors_sync.py
--rw-r--r--   0        0        0     2106 2023-04-29 02:43:32.387691 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_mining_executors_sync.py
--rw-r--r--   0        0        0     2739 2023-04-29 02:44:35.472432 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_node_executors_sync.py
--rw-r--r--   0        0        0     6033 2023-04-29 02:48:08.574123 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_state_executors_sync.py
--rw-r--r--   0        0        0     3084 2023-04-29 02:49:21.046565 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_submission_executors_sync.py
--rw-r--r--   0        0        0    10030 2023-04-29 02:50:56.085928 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_trace_executors_sync.py
--rw-r--r--   0        0        0     4492 2023-04-29 02:51:37.478912 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_transaction_executors_sync.py
--rw-r--r--   0        0        0     3830 2023-04-29 02:53:28.556506 checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_whisper_executors_sync.py
--rw-r--r--   0        0        0     1068 2022-12-25 15:14:22.765380 checkthechain-0.3.4/src/ctc/rpc/rpc_format.py
--rw-r--r--   0        0        0     2051 2023-02-26 18:21:07.003537 checkthechain-0.3.4/src/ctc/rpc/rpc_lifecycle.py
--rw-r--r--   0        0        0     1999 2023-02-26 18:21:07.003667 checkthechain-0.3.4/src/ctc/rpc/rpc_logging.py
--rw-r--r--   0        0        0       47 2023-04-29 00:10:42.447596 checkthechain-0.3.4/src/ctc/rpc/rpc_protocols/__init__.py
--rw-r--r--   0        0        0     4255 2023-04-29 03:32:17.512979 checkthechain-0.3.4/src/ctc/rpc/rpc_protocols/rpc_http.py
--rw-r--r--   0        0        0      321 2023-04-29 00:13:48.363233 checkthechain-0.3.4/src/ctc/rpc/rpc_protocols/rpc_websocket.py
--rw-r--r--   0        0        0     9770 2023-04-17 01:11:21.303538 checkthechain-0.3.4/src/ctc/rpc/rpc_provider.py
--rw-r--r--   0        0        0     1128 2022-11-23 19:36:31.146057 checkthechain-0.3.4/src/ctc/rpc/rpc_registry.py
--rw-r--r--   0        0        0       86 2023-04-29 02:54:07.448132 checkthechain-0.3.4/src/ctc/rpc/rpc_request/__init__.py
--rw-r--r--   0        0        0     4730 2023-04-29 00:11:33.888738 checkthechain-0.3.4/src/ctc/rpc/rpc_request/request_async.py
--rw-r--r--   0        0        0     4620 2023-04-29 02:58:16.903919 checkthechain-0.3.4/src/ctc/rpc/rpc_request/request_sync.py
--rw-r--r--   0        0        0     4602 2023-06-02 23:42:32.086805 checkthechain-0.3.4/src/ctc/rpc/rpc_request/request_utils.py
--rw-r--r--   0        0        0     3688 2023-03-04 19:50:23.524532 checkthechain-0.3.4/src/ctc/rpc/rpc_spec.py
--rw-r--r--   0        0        0      102 2023-02-26 18:21:07.005328 checkthechain-0.3.4/src/ctc/spec/__init__.py
--rw-r--r--   0        0        0      126 2022-11-23 19:36:31.146419 checkthechain-0.3.4/src/ctc/spec/exceptions/__init__.py
--rw-r--r--   0        0        0       85 2022-11-23 19:36:31.146519 checkthechain-0.3.4/src/ctc/spec/exceptions/abi_exceptions.py
--rw-r--r--   0        0        0      230 2023-04-17 00:04:51.283975 checkthechain-0.3.4/src/ctc/spec/exceptions/config_exceptions.py
--rw-r--r--   0        0        0       87 2022-11-23 19:36:31.146696 checkthechain-0.3.4/src/ctc/spec/exceptions/oracle_exceptions.py
--rw-r--r--   0        0        0      131 2022-11-23 19:36:31.146783 checkthechain-0.3.4/src/ctc/spec/exceptions/rpc_exceptions.py
--rw-r--r--   0        0        0      487 2022-11-23 19:36:31.146870 checkthechain-0.3.4/src/ctc/spec/formatting.py
--rw-r--r--   0        0        0     4620 2023-04-12 16:44:13.479488 checkthechain-0.3.4/src/ctc/spec/typedata.py
--rw-r--r--   0        0        0      704 2023-02-26 18:21:07.005950 checkthechain-0.3.4/src/ctc/spec/typedefs/__init__.py
--rw-r--r--   0        0        0     2116 2023-04-17 01:15:16.387519 checkthechain-0.3.4/src/ctc/spec/typedefs/abi_types.py
--rw-r--r--   0        0        0     1012 2023-04-15 07:13:56.749794 checkthechain-0.3.4/src/ctc/spec/typedefs/address_types.py
--rw-r--r--   0        0        0      948 2022-11-23 19:36:31.147255 checkthechain-0.3.4/src/ctc/spec/typedefs/binary_types.py
--rw-r--r--   0        0        0     2239 2023-02-26 18:21:07.006211 checkthechain-0.3.4/src/ctc/spec/typedefs/block_types.py
--rw-r--r--   0        0        0     2019 2023-04-17 01:15:50.282375 checkthechain-0.3.4/src/ctc/spec/typedefs/config_types.py
--rw-r--r--   0        0        0      154 2023-02-26 18:21:07.006635 checkthechain-0.3.4/src/ctc/spec/typedefs/consensus_types.py
--rw-r--r--   0        0        0     1571 2023-04-12 00:25:44.366208 checkthechain-0.3.4/src/ctc/spec/typedefs/context_types.py
--rw-r--r--   0        0        0     1150 2023-04-17 01:34:02.808903 checkthechain-0.3.4/src/ctc/spec/typedefs/data_source_types.py
--rw-r--r--   0        0        0      752 2023-02-26 18:21:07.007297 checkthechain-0.3.4/src/ctc/spec/typedefs/db_types.py
--rw-r--r--   0        0        0      539 2023-04-10 06:29:29.191082 checkthechain-0.3.4/src/ctc/spec/typedefs/defi_types.py
--rw-r--r--   0        0        0     1178 2023-04-17 01:14:53.735415 checkthechain-0.3.4/src/ctc/spec/typedefs/event_types.py
--rw-r--r--   0        0        0      971 2023-04-13 02:34:03.315850 checkthechain-0.3.4/src/ctc/spec/typedefs/external_types.py
--rw-r--r--   0        0        0      728 2023-02-26 18:21:07.007839 checkthechain-0.3.4/src/ctc/spec/typedefs/log_types.py
--rw-r--r--   0        0        0      300 2023-04-17 01:28:53.685750 checkthechain-0.3.4/src/ctc/spec/typedefs/network_types.py
--rw-r--r--   0        0        0      165 2022-11-23 19:36:31.147653 checkthechain-0.3.4/src/ctc/spec/typedefs/number_types.py
--rw-r--r--   0        0        0     2178 2023-03-24 20:18:53.548764 checkthechain-0.3.4/src/ctc/spec/typedefs/rpc_types.py
--rw-r--r--   0        0        0      671 2022-11-23 19:36:31.147834 checkthechain-0.3.4/src/ctc/spec/typedefs/storage_types.py
--rw-r--r--   0        0        0     4523 2023-03-04 19:50:23.525113 checkthechain-0.3.4/src/ctc/spec/typedefs/trace_types.py
--rw-r--r--   0        0        0     4519 2023-04-17 01:29:16.409479 checkthechain-0.3.4/src/ctc/spec/typedefs/transaction_types.py
--rw-r--r--   0        0        0      129 2023-04-17 00:26:49.657179 checkthechain-0.3.4/src/ctc/spec/typeguards/__init__.py
--rw-r--r--   0        0        0     1637 2022-11-23 19:36:31.148153 checkthechain-0.3.4/src/ctc/spec/typeguards/binary_typeguards.py
--rw-r--r--   0        0        0     1708 2022-11-23 19:36:31.148252 checkthechain-0.3.4/src/ctc/spec/typeguards/block_typeguards.py
--rw-r--r--   0        0        0      289 2023-02-26 20:15:07.427239 checkthechain-0.3.4/src/ctc/spec/typeguards/db_typeguards.py
--rw-r--r--   0        0        0     1422 2023-04-11 15:03:04.546469 checkthechain-0.3.4/src/ctc/spec/typeguards/external_typeguards.py
--rw-r--r--   0        0        0        0 2022-11-23 19:36:31.148387 checkthechain-0.3.4/src/ctc/toolbox/__init__.py
--rw-r--r--   0        0        0     1441 2022-11-23 19:36:31.152899 checkthechain-0.3.4/src/ctc/toolbox/nested_utils.py
--rw-r--r--   0        0        0     3258 2023-04-15 07:19:21.326943 checkthechain-0.3.4/src/ctc/toolbox/optimize_utils.py
--rw-r--r--   0        0        0      175 2023-04-24 06:28:07.927137 checkthechain-0.3.4/src/ctc/toolbox/pl_utils/__init__.py
--rw-r--r--   0        0        0     2464 2023-04-11 15:01:28.142423 checkthechain-0.3.4/src/ctc/toolbox/pl_utils/binary_utils.py
--rw-r--r--   0        0        0     1002 2023-04-11 15:00:27.569336 checkthechain-0.3.4/src/ctc/toolbox/pl_utils/concat_utils.py
--rw-r--r--   0        0        0     2638 2023-04-24 06:28:56.069741 checkthechain-0.3.4/src/ctc/toolbox/pl_utils/file_utils.py
--rw-r--r--   0        0        0     3562 2023-05-30 06:46:30.793034 checkthechain-0.3.4/src/ctc/toolbox/pl_utils/interpolate_utils.py
--rw-r--r--   0        0        0    13676 2023-04-24 18:32:50.650896 checkthechain-0.3.4/src/ctc/toolbox/pl_utils/partition_utils.py
--rw-r--r--   0        0        0     7632 2023-05-03 17:48:02.702127 checkthechain-0.3.4/src/ctc/toolbox/pl_utils/summary_utils.py
--rw-r--r--   0        0        0     3512 2023-02-26 18:21:07.014557 checkthechain-0.3.4/src/ctc/toolbox/plot_utils.py
--rw-r--r--   0        0        0     8876 2023-03-04 19:50:23.527332 checkthechain-0.3.4/src/ctc/toolbox/range_utils.py
--rw-r--r--   0        0        0     9045 2022-11-23 19:36:31.153915 checkthechain-0.3.4/src/ctc/toolbox/search_utils.py
--rw-r--r--   0        0        0      719 2023-02-27 08:14:19.899656 checkthechain-0.3.4/tests/conftest.py
--rw-r--r--   0        0        0    20988 2022-11-23 19:36:31.154352 checkthechain-0.3.4/tests/ctc/binary/.hypothesis/unicode_data/13.0.0/charmap.json.gz
--rw-r--r--   0        0        0      789 2022-11-23 19:36:31.154466 checkthechain-0.3.4/tests/ctc/binary/test_eip712.py
--rw-r--r--   0        0        0     1224 2022-11-23 19:36:31.154549 checkthechain-0.3.4/tests/ctc/binary/test_format_utils.py
--rw-r--r--   0        0        0      795 2022-11-23 19:36:31.154622 checkthechain-0.3.4/tests/ctc/binary/test_hash_utils.py
--rw-r--r--   0        0        0     3946 2023-04-11 17:17:48.856155 checkthechain-0.3.4/tests/ctc/binary/test_rlp_encoding.py
--rw-r--r--   0        0        0     4888 2022-11-23 19:36:31.154783 checkthechain-0.3.4/tests/ctc/binary/test_signatures.py
--rw-r--r--   0        0        0     1702 2022-11-23 19:36:31.154907 checkthechain-0.3.4/tests/ctc/cli/test_cli_args.py
--rw-r--r--   0        0        0     3589 2022-11-23 19:36:31.155012 checkthechain-0.3.4/tests/ctc/cli/test_cli_subcommands.py
--rw-r--r--   0        0        0    16961 2023-02-26 18:21:07.015169 checkthechain-0.3.4/tests/ctc/config/contexts/test_cache_contexts.py
--rw-r--r--   0        0        0     5248 2023-04-12 02:20:12.521865 checkthechain-0.3.4/tests/ctc/config/contexts/test_network_contexts.py
--rw-r--r--   0        0        0      620 2022-11-23 19:36:31.155162 checkthechain-0.3.4/tests/ctc/config/test_config_defaults.py
--rw-r--r--   0        0        0     4545 2023-04-26 23:49:26.324218 checkthechain-0.3.4/tests/ctc/config/test_config_validators.py
--rw-r--r--   0        0        0     9776 2023-04-11 22:11:40.166308 checkthechain-0.3.4/tests/ctc/config/test_setup.py
--rw-r--r--   0        0        0     3387 2023-04-12 02:19:52.771416 checkthechain-0.3.4/tests/ctc/db/db_crud/test_db_block_timestamps.py
--rw-r--r--   0        0        0     5624 2023-04-12 02:23:22.803870 checkthechain-0.3.4/tests/ctc/db/db_crud/test_db_blocks.py
--rw-r--r--   0        0        0     2624 2023-04-12 02:19:46.343714 checkthechain-0.3.4/tests/ctc/db/db_crud/test_db_contract_abis.py
--rw-r--r--   0        0        0     1906 2023-04-12 02:23:17.026530 checkthechain-0.3.4/tests/ctc/db/db_crud/test_db_contract_creation.py
--rw-r--r--   0        0        0     3295 2023-04-12 02:19:42.769384 checkthechain-0.3.4/tests/ctc/db/db_crud/test_db_erc20_metadata.py
--rw-r--r--   0        0        0      446 2022-11-23 19:36:31.155877 checkthechain-0.3.4/tests/ctc/db/db_schemas.py
--rw-r--r--   0        0        0     1081 2023-02-27 08:07:49.692060 checkthechain-0.3.4/tests/ctc/db/dba_utils.py
--rw-r--r--   0        0        0    11873 2023-04-14 23:05:20.037248 checkthechain-0.3.4/tests/ctc/db/test_crud_problems.py
--rw-r--r--   0        0        0    20988 2022-11-23 19:36:31.156314 checkthechain-0.3.4/tests/ctc/directory/.hypothesis/unicode_data/13.0.0/charmap.json.gz
--rw-r--r--   0        0        0     1104 2023-04-17 00:07:23.260049 checkthechain-0.3.4/tests/ctc/directory/test_directory_networks.py
--rw-r--r--   0        0        0      588 2022-11-23 19:36:31.156484 checkthechain-0.3.4/tests/ctc/directory/test_directory_tokens.py
--rw-r--r--   0        0        0     1322 2022-11-23 19:36:31.156621 checkthechain-0.3.4/tests/ctc/docs/test_readme_examples.py
--rw-r--r--   0        0        0    20988 2022-11-23 19:36:31.156862 checkthechain-0.3.4/tests/ctc/evm/.hypothesis/unicode_data/13.0.0/charmap.json.gz
--rw-r--r--   0        0        0     3757 2022-11-23 19:36:31.156975 checkthechain-0.3.4/tests/ctc/evm/test_address_utils.py
--rw-r--r--   0        0        0     2687 2023-02-26 18:21:07.018040 checkthechain-0.3.4/tests/ctc/evm/test_block_utils.py
--rw-r--r--   0        0        0      514 2023-04-12 04:51:28.445072 checkthechain-0.3.4/tests/ctc/evm/test_erc20_utils/test_erc20_events.py
--rw-r--r--   0        0        0      588 2022-11-23 19:36:31.157327 checkthechain-0.3.4/tests/ctc/evm/test_erc20_utils/test_erc20_metadata.py
--rw-r--r--   0        0        0      650 2022-11-23 19:36:31.157422 checkthechain-0.3.4/tests/ctc/evm/test_erc20_utils/test_erc20_state.py
--rw-r--r--   0        0        0        0 2023-02-26 18:21:07.018238 checkthechain-0.3.4/tests/ctc/evm/test_erc4626_utils/__init__.py
--rw-r--r--   0        0        0      981 2023-02-26 18:21:07.018338 checkthechain-0.3.4/tests/ctc/evm/test_erc4626_utils/test_erc4626_events.py
--rw-r--r--   0        0        0     1085 2023-02-26 18:21:07.018415 checkthechain-0.3.4/tests/ctc/evm/test_erc4626_utils/test_erc4626_metadata.py
--rw-r--r--   0        0        0     2429 2023-02-26 18:21:07.018492 checkthechain-0.3.4/tests/ctc/evm/test_erc4626_utils/test_erc4626_normalize.py
--rw-r--r--   0        0        0    10489 2023-02-26 18:21:07.018576 checkthechain-0.3.4/tests/ctc/evm/test_erc4626_utils/test_erc4626_state.py
--rw-r--r--   0        0        0      300 2023-02-26 18:21:07.018842 checkthechain-0.3.4/tests/ctc/evm/test_eth_utils.py
--rw-r--r--   0        0        0      714 2023-04-12 04:52:01.852764 checkthechain-0.3.4/tests/ctc/evm/test_event_utils.py
--rw-r--r--   0        0        0     6573 2023-04-12 04:44:35.718866 checkthechain-0.3.4/tests/ctc/evm/test_event_utils_new.py
--rw-r--r--   0        0        0    20988 2022-11-23 19:36:31.158160 checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/.hypothesis/unicode_data/13.0.0/charmap.json.gz
--rw-r--r--   0        0        0     1690 2022-11-23 19:36:31.158245 checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_blocks.py
--rw-r--r--   0        0        0     2025 2023-04-12 18:13:33.792410 checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_logs.py
--rw-r--r--   0        0        0     1065 2022-11-23 19:36:31.158425 checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_node.py
--rw-r--r--   0        0        0     5693 2022-11-23 19:36:31.158531 checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_state.py
--rw-r--r--   0        0        0      325 2023-02-26 18:21:07.019547 checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_submission.py
--rw-r--r--   0        0        0     2185 2022-11-23 19:36:31.158726 checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_transactions.py
--rw-r--r--   0        0        0     3751 2023-04-12 18:09:08.234614 checkthechain-0.3.4/tests/ctc/evm/test_transaction_utils/test_transaction_utils.py
--rw-r--r--   0        0        0      915 2022-11-23 19:36:31.159046 checkthechain-0.3.4/tests/ctc/protocols/balancer_utils/test_balancer_utils.py
--rw-r--r--   0        0        0     3367 2023-04-12 02:19:29.511661 checkthechain-0.3.4/tests/ctc/protocols/chainlink_utils/test_chainlink_db.py
--rw-r--r--   0        0        0     2855 2023-04-27 22:25:08.354233 checkthechain-0.3.4/tests/ctc/protocols/fourbyte_utils/test_fourbyte_db.py
--rw-r--r--   0        0        0      668 2022-11-23 19:36:31.159439 checkthechain-0.3.4/tests/ctc/protocols/uniswap_v2_utils/test_uniswap_queries.py
--rw-r--r--   0        0        0     1483 2023-02-26 18:21:07.020336 checkthechain-0.3.4/tests/ctc/spec/test_typedata.py
--rw-r--r--   0        0        0      867 2023-02-26 18:21:07.020613 checkthechain-0.3.4/tests/ctc/spec/test_typedefs.py
--rw-r--r--   0        0        0    15225 2023-04-12 19:52:25.910305 checkthechain-0.3.4/tests/ctc/test_code.py
--rw-r--r--   0        0        0     2008 2023-04-15 22:53:54.067041 checkthechain-0.3.4/tests/ctc/test_config.py
--rw-r--r--   0        0        0      688 2023-04-15 22:49:32.487864 checkthechain-0.3.4/tests/ctc/toolbox/defi_utils/defi_directory.py
--rw-r--r--   0        0        0     4168 2023-04-15 22:49:37.457470 checkthechain-0.3.4/tests/ctc/toolbox/defi_utils/dex_utils.py
--rw-r--r--   0        0        0     5333 2023-04-15 22:49:24.672815 checkthechain-0.3.4/tests/ctc/toolbox/test_amm_utils.py
--rw-r--r--   0        0        0     6329 2023-02-26 18:21:07.020999 checkthechain-0.3.4/tests/ctc/toolbox/test_chunk_utils.py
--rw-r--r--   0        0        0      651 2022-11-23 19:36:31.160315 checkthechain-0.3.4/tests/ctc/toolbox/test_feed_utils.py
--rw-r--r--   0        0        0     4425 2023-03-04 18:28:55.366320 checkthechain-0.3.4/tests/ctc/toolbox/test_range_utils.py
--rwxr-xr-x   0        0        0      231 2022-11-23 19:36:31.160379 checkthechain-0.3.4/tests/run_type_checks.sh
--rw-r--r--   0        0        0     9798 1970-01-01 00:00:00.000000 checkthechain-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      217 2023-02-26 18:21:06.927738 checkthechain-0.3.5/.gitignore
+-rw-r--r--   0        0        0     8294 2023-02-26 18:21:06.927914 checkthechain-0.3.5/CHANGELOG.md
+-rw-r--r--   0        0        0     3117 2023-04-11 03:46:56.460577 checkthechain-0.3.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-02-26 18:21:06.928214 checkthechain-0.3.5/LICENSE-APACHE
+-rw-r--r--   0        0        0     1093 2023-02-26 18:21:06.928570 checkthechain-0.3.5/LICENSE-MIT
+-rw-r--r--   0        0        0     7487 2023-02-26 18:21:06.928884 checkthechain-0.3.5/README.md
+-rw-r--r--   0        0        0       52 2022-11-23 19:36:31.097613 checkthechain-0.3.5/docs/README.md
+-rw-r--r--   0        0        0     1167 2023-02-26 18:21:06.929180 checkthechain-0.3.5/docs/contributing_guides/adding_config_keys.md
+-rw-r--r--   0        0        0      797 2023-02-26 18:21:06.929401 checkthechain-0.3.5/docs/contributing_guides/adding_db_caches.md
+-rw-r--r--   0        0        0      243 2023-02-26 18:21:06.929558 checkthechain-0.3.5/docs/contributing_guides/upgrade_to_new_ctc_version.md
+-rw-r--r--   0        0        0     4411 2023-06-06 01:22:08.807392 checkthechain-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      566 2023-06-06 01:18:43.299218 checkthechain-0.3.5/src/ctc/__init__.py
+-rw-r--r--   0        0        0       35 2022-11-23 19:36:31.097865 checkthechain-0.3.5/src/ctc/__main__.py
+-rw-r--r--   0        0        0       97 2023-02-26 18:21:06.930730 checkthechain-0.3.5/src/ctc/cli/__init__.py
+-rw-r--r--   0        0        0    12631 2023-04-11 16:22:47.887085 checkthechain-0.3.5/src/ctc/cli/cli_run.py
+-rw-r--r--   0        0        0      193 2023-02-26 18:21:06.931328 checkthechain-0.3.5/src/ctc/cli/cli_utils/__init__.py
+-rw-r--r--   0        0        0     9052 2022-11-23 19:36:31.098221 checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_alias_utils.py
+-rw-r--r--   0        0        0     8508 2023-02-26 18:21:06.931449 checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_charset_utils.py
+-rw-r--r--   0        0        0     8581 2023-04-17 00:55:51.315895 checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_color_utils.py
+-rw-r--r--   0        0        0      612 2022-11-23 19:36:31.098462 checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_execution_utils.py
+-rw-r--r--   0        0        0     2308 2023-04-11 03:44:53.034908 checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_output_utils.py
+-rw-r--r--   0        0        0     9184 2023-05-09 04:20:26.327124 checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_parse_utils.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.098735 checkthechain-0.3.5/src/ctc/cli/commands/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.098821 checkthechain-0.3.5/src/ctc/cli/commands/admin/__init__.py
+-rw-r--r--   0        0        0     1952 2022-11-23 19:36:31.098935 checkthechain-0.3.5/src/ctc/cli/commands/admin/aliases_command.py
+-rw-r--r--   0        0        0     2569 2022-11-23 19:36:31.099038 checkthechain-0.3.5/src/ctc/cli/commands/admin/chains_command.py
+-rw-r--r--   0        0        0      939 2023-02-26 18:21:06.932612 checkthechain-0.3.5/src/ctc/cli/commands/admin/charset_command.py
+-rw-r--r--   0        0        0     2796 2023-02-26 18:21:06.932700 checkthechain-0.3.5/src/ctc/cli/commands/admin/color_command.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.099306 checkthechain-0.3.5/src/ctc/cli/commands/admin/config/__init__.py
+-rw-r--r--   0        0        0     1231 2023-02-26 18:21:06.932846 checkthechain-0.3.5/src/ctc/cli/commands/admin/config/edit_command.py
+-rw-r--r--   0        0        0      341 2022-11-23 19:36:31.099535 checkthechain-0.3.5/src/ctc/cli/commands/admin/config/path_command.py
+-rw-r--r--   0        0        0    11615 2023-05-09 03:03:31.696453 checkthechain-0.3.5/src/ctc/cli/commands/admin/config_command.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.099729 checkthechain-0.3.5/src/ctc/cli/commands/admin/db/__init__.py
+-rw-r--r--   0        0        0     1310 2023-02-26 21:00:17.933995 checkthechain-0.3.5/src/ctc/cli/commands/admin/db/create_tables_command.py
+-rw-r--r--   0        0        0     1410 2023-02-26 20:15:07.407580 checkthechain-0.3.5/src/ctc/cli/commands/admin/db/drop_command.py
+-rw-r--r--   0        0        0      370 2023-04-12 04:04:05.737647 checkthechain-0.3.5/src/ctc/cli/commands/admin/db/login_command.py
+-rw-r--r--   0        0        0     4772 2023-04-26 23:18:25.231255 checkthechain-0.3.5/src/ctc/cli/commands/admin/db/status_command.py
+-rw-r--r--   0        0        0      858 2022-11-23 19:36:31.100027 checkthechain-0.3.5/src/ctc/cli/commands/admin/log_command.py
+-rw-r--r--   0        0        0     3184 2022-11-23 19:36:31.100197 checkthechain-0.3.5/src/ctc/cli/commands/admin/setup_command.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.100283 checkthechain-0.3.5/src/ctc/cli/commands/compute/__init__.py
+-rw-r--r--   0        0        0      491 2022-11-23 19:36:31.100403 checkthechain-0.3.5/src/ctc/cli/commands/compute/ascii_command.py
+-rw-r--r--   0        0        0      530 2022-11-23 19:36:31.100502 checkthechain-0.3.5/src/ctc/cli/commands/compute/checksum_command.py
+-rw-r--r--   0        0        0     1202 2022-11-23 19:36:31.100601 checkthechain-0.3.5/src/ctc/cli/commands/compute/create_address_command.py
+-rw-r--r--   0        0        0    13751 2023-04-11 16:58:47.041829 checkthechain-0.3.5/src/ctc/cli/commands/compute/decode_call_command.py
+-rw-r--r--   0        0        0      965 2023-04-11 16:55:27.846437 checkthechain-0.3.5/src/ctc/cli/commands/compute/decode_command.py
+-rw-r--r--   0        0        0     1482 2023-04-11 16:55:12.443123 checkthechain-0.3.5/src/ctc/cli/commands/compute/encode_command.py
+-rw-r--r--   0        0        0      760 2022-11-23 19:36:31.100956 checkthechain-0.3.5/src/ctc/cli/commands/compute/hex_command.py
+-rw-r--r--   0        0        0      509 2022-11-23 19:36:31.101019 checkthechain-0.3.5/src/ctc/cli/commands/compute/integer_command.py
+-rw-r--r--   0        0        0     1618 2022-11-23 19:36:31.101088 checkthechain-0.3.5/src/ctc/cli/commands/compute/keccak_command.py
+-rw-r--r--   0        0        0     4730 2022-11-23 19:36:31.101172 checkthechain-0.3.5/src/ctc/cli/commands/compute/limits_command.py
+-rw-r--r--   0        0        0      436 2022-11-23 19:36:31.101239 checkthechain-0.3.5/src/ctc/cli/commands/compute/lower_command.py
+-rw-r--r--   0        0        0      993 2022-11-23 19:36:31.101312 checkthechain-0.3.5/src/ctc/cli/commands/compute/rlp_encode.py
+-rw-r--r--   0        0        0      720 2022-11-23 19:36:31.101376 checkthechain-0.3.5/src/ctc/cli/commands/compute/selector_command.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.101442 checkthechain-0.3.5/src/ctc/cli/commands/data/__init__.py
+-rw-r--r--   0        0        0     6408 2023-02-26 18:21:06.935201 checkthechain-0.3.5/src/ctc/cli/commands/data/abi_command.py
+-rw-r--r--   0        0        0     1506 2022-11-23 19:36:31.101616 checkthechain-0.3.5/src/ctc/cli/commands/data/abi_diff_command.py
+-rw-r--r--   0        0        0     1454 2023-02-26 18:21:06.935512 checkthechain-0.3.5/src/ctc/cli/commands/data/address_command.py
+-rw-r--r--   0        0        0     2532 2023-01-07 08:13:49.926885 checkthechain-0.3.5/src/ctc/cli/commands/data/address_txs_command.py
+-rw-r--r--   0        0        0     2593 2023-02-26 18:21:06.935644 checkthechain-0.3.5/src/ctc/cli/commands/data/block_command.py
+-rw-r--r--   0        0        0     5173 2023-04-11 03:48:25.322507 checkthechain-0.3.5/src/ctc/cli/commands/data/blocks_command.py
+-rw-r--r--   0        0        0      634 2022-11-23 19:36:31.101982 checkthechain-0.3.5/src/ctc/cli/commands/data/bytecode_command.py
+-rw-r--r--   0        0        0     4642 2023-03-18 06:34:21.816682 checkthechain-0.3.5/src/ctc/cli/commands/data/call_all_command.py
+-rw-r--r--   0        0        0     3224 2022-11-23 19:36:31.102138 checkthechain-0.3.5/src/ctc/cli/commands/data/call_command.py
+-rw-r--r--   0        0        0    23122 2023-04-12 16:08:53.179783 checkthechain-0.3.5/src/ctc/cli/commands/data/calls_command.py
+-rw-r--r--   0        0        0     2927 2023-02-26 18:21:06.936911 checkthechain-0.3.5/src/ctc/cli/commands/data/chain_command.py
+-rw-r--r--   0        0        0     4207 2023-02-26 18:21:06.937286 checkthechain-0.3.5/src/ctc/cli/commands/data/decompile_command.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.102575 checkthechain-0.3.5/src/ctc/cli/commands/data/dex/__init__.py
+-rw-r--r--   0        0        0     6890 2023-04-15 16:03:33.976343 checkthechain-0.3.5/src/ctc/cli/commands/data/dex/chart_command.py
+-rw-r--r--   0        0        0     4813 2023-04-15 16:00:40.959584 checkthechain-0.3.5/src/ctc/cli/commands/data/dex/pool_command.py
+-rw-r--r--   0        0        0     8639 2023-04-15 16:00:02.454511 checkthechain-0.3.5/src/ctc/cli/commands/data/dex/pools_command.py
+-rw-r--r--   0        0        0     4354 2023-04-15 15:43:58.809999 checkthechain-0.3.5/src/ctc/cli/commands/data/dex/trades_command.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.103150 checkthechain-0.3.5/src/ctc/cli/commands/data/erc20/__init__.py
+-rw-r--r--   0        0        0     1603 2022-11-23 19:36:31.103246 checkthechain-0.3.5/src/ctc/cli/commands/data/erc20/balance_command.py
+-rw-r--r--   0        0        0     9969 2023-04-11 03:56:24.764985 checkthechain-0.3.5/src/ctc/cli/commands/data/erc20/balances_command.py
+-rw-r--r--   0        0        0     1947 2023-04-10 04:18:22.101055 checkthechain-0.3.5/src/ctc/cli/commands/data/erc20/transfers_command.py
+-rw-r--r--   0        0        0      881 2022-11-23 19:36:31.103509 checkthechain-0.3.5/src/ctc/cli/commands/data/erc20_command.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.103574 checkthechain-0.3.5/src/ctc/cli/commands/data/eth/__init__.py
+-rw-r--r--   0        0        0     1334 2022-11-23 19:36:31.103652 checkthechain-0.3.5/src/ctc/cli/commands/data/eth/balance_command.py
+-rw-r--r--   0        0        0     7719 2023-04-12 23:11:07.611640 checkthechain-0.3.5/src/ctc/cli/commands/data/eth/balances_command.py
+-rw-r--r--   0        0        0     3653 2023-04-11 05:49:15.694208 checkthechain-0.3.5/src/ctc/cli/commands/data/events_command.py
+-rw-r--r--   0        0        0    11909 2023-04-14 03:52:55.753011 checkthechain-0.3.5/src/ctc/cli/commands/data/gas_command.py
+-rw-r--r--   0        0        0     2520 2022-11-23 19:36:31.104030 checkthechain-0.3.5/src/ctc/cli/commands/data/proxy_command.py
+-rw-r--r--   0        0        0     2597 2023-02-26 18:21:06.939031 checkthechain-0.3.5/src/ctc/cli/commands/data/proxy_register_command.py
+-rw-r--r--   0        0        0     1478 2023-04-11 17:03:09.850892 checkthechain-0.3.5/src/ctc/cli/commands/data/storage_command.py
+-rw-r--r--   0        0        0      850 2022-11-23 19:36:31.104247 checkthechain-0.3.5/src/ctc/cli/commands/data/symbol_command.py
+-rw-r--r--   0        0        0     1450 2022-11-23 19:36:31.104314 checkthechain-0.3.5/src/ctc/cli/commands/data/timestamp_command.py
+-rw-r--r--   0        0        0     2050 2023-02-26 18:21:06.939163 checkthechain-0.3.5/src/ctc/cli/commands/data/tx_command.py
+-rw-r--r--   0        0        0     2813 2022-11-23 19:36:31.104457 checkthechain-0.3.5/src/ctc/cli/commands/root_command.py
+-rw-r--r--   0        0        0      226 2023-02-26 18:21:06.939627 checkthechain-0.3.5/src/ctc/config/__init__.py
+-rw-r--r--   0        0        0     6947 2023-04-26 23:49:08.151324 checkthechain-0.3.5/src/ctc/config/config_defaults.py
+-rw-r--r--   0        0        0     3987 2023-02-26 18:21:06.940408 checkthechain-0.3.5/src/ctc/config/config_env_vars.py
+-rw-r--r--   0        0        0      687 2023-02-26 18:21:06.940691 checkthechain-0.3.5/src/ctc/config/config_overrides.py
+-rw-r--r--   0        0        0     4267 2023-04-17 00:26:09.800618 checkthechain-0.3.5/src/ctc/config/config_read.py
+-rw-r--r--   0        0        0      375 2023-02-26 18:21:06.941204 checkthechain-0.3.5/src/ctc/config/config_spec.py
+-rw-r--r--   0        0        0    11474 2023-04-27 04:45:26.239328 checkthechain-0.3.5/src/ctc/config/config_validate.py
+-rw-r--r--   0        0        0     4912 2023-04-17 01:15:59.426408 checkthechain-0.3.5/src/ctc/config/config_values.py
+-rw-r--r--   0        0        0     1236 2023-04-17 00:11:55.733936 checkthechain-0.3.5/src/ctc/config/config_write.py
+-rw-r--r--   0        0        0      121 2023-02-26 18:21:06.942475 checkthechain-0.3.5/src/ctc/config/context_utils/__init__.py
+-rw-r--r--   0        0        0     7359 2023-04-11 22:37:33.866053 checkthechain-0.3.5/src/ctc/config/context_utils/context_caches.py
+-rw-r--r--   0        0        0     1944 2023-02-26 18:21:06.943080 checkthechain-0.3.5/src/ctc/config/context_utils/context_crud.py
+-rw-r--r--   0        0        0     3118 2023-04-10 23:34:05.929913 checkthechain-0.3.5/src/ctc/config/context_utils/context_sources.py
+-rw-r--r--   0        0        0      506 2023-02-26 18:21:06.943482 checkthechain-0.3.5/src/ctc/config/context_utils/context_validate.py
+-rw-r--r--   0        0        0       26 2022-11-23 19:36:31.105507 checkthechain-0.3.5/src/ctc/config/setup_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.105567 checkthechain-0.3.5/src/ctc/config/setup_utils/default_data/__init__.py
+-rw-r--r--   0        0        0   142771 2023-04-12 02:21:19.579767 checkthechain-0.3.5/src/ctc/config/setup_utils/default_data/default_erc20s.py
+-rw-r--r--   0        0        0     3629 2023-04-27 01:46:49.405189 checkthechain-0.3.5/src/ctc/config/setup_utils/main_setup.py
+-rw-r--r--   0        0        0     7383 2023-04-17 00:15:05.747317 checkthechain-0.3.5/src/ctc/config/setup_utils/setup_io.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.106519 checkthechain-0.3.5/src/ctc/config/setup_utils/stages/__init__.py
+-rw-r--r--   0        0        0     1622 2023-02-26 18:21:06.945600 checkthechain-0.3.5/src/ctc/config/setup_utils/stages/alias_setup.py
+-rw-r--r--   0        0        0     4171 2023-02-26 18:21:06.945828 checkthechain-0.3.5/src/ctc/config/setup_utils/stages/cli_setup.py
+-rw-r--r--   0        0        0     3309 2023-02-26 18:21:06.945947 checkthechain-0.3.5/src/ctc/config/setup_utils/stages/data_dir_setup.py
+-rw-r--r--   0        0        0     8319 2023-04-27 04:36:30.568338 checkthechain-0.3.5/src/ctc/config/setup_utils/stages/db_setup.py
+-rw-r--r--   0        0        0    16993 2023-04-12 02:20:49.003316 checkthechain-0.3.5/src/ctc/config/setup_utils/stages/network_setup.py
+-rw-r--r--   0        0        0       59 2023-02-26 18:21:06.946626 checkthechain-0.3.5/src/ctc/config/upgrade_utils/__init__.py
+-rw-r--r--   0        0        0     7367 2023-06-06 01:21:15.832678 checkthechain-0.3.5/src/ctc/config/upgrade_utils/config_upgrade.py
+-rw-r--r--   0        0        0     7171 2023-04-17 01:16:23.566187 checkthechain-0.3.5/src/ctc/config/upgrade_utils/data_dir_versioning.py
+-rw-r--r--   0        0        0     3026 2023-04-17 01:29:37.379812 checkthechain-0.3.5/src/ctc/config/upgrade_utils/legacy_types.py
+-rw-r--r--   0        0        0      623 2023-02-26 18:21:06.947460 checkthechain-0.3.5/src/ctc/config/upgrade_utils/version_utils.py
+-rw-r--r--   0        0        0        0 2023-03-04 19:50:23.525211 checkthechain-0.3.5/src/ctc/datasets/__init__.py
+-rw-r--r--   0        0        0     6803 2023-06-03 00:20:08.970969 checkthechain-0.3.5/src/ctc/datasets/extract_blocks_and_transactions.py
+-rw-r--r--   0        0        0     2348 2023-05-30 06:43:40.603733 checkthechain-0.3.5/src/ctc/datasets/extract_erc20_transfers.py
+-rw-r--r--   0        0        0      162 2022-11-23 19:36:31.107400 checkthechain-0.3.5/src/ctc/db/__init__.py
+-rw-r--r--   0        0        0     3217 2023-04-15 07:07:44.333514 checkthechain-0.3.5/src/ctc/db/connect_utils.py
+-rw-r--r--   0        0        0     2890 2023-02-26 20:15:07.410640 checkthechain-0.3.5/src/ctc/db/intake_utils.py
+-rw-r--r--   0        0        0      109 2023-02-26 20:15:07.410802 checkthechain-0.3.5/src/ctc/db/management/__init__.py
+-rw-r--r--   0        0        0      997 2023-02-26 18:21:06.948577 checkthechain-0.3.5/src/ctc/db/management/active_utils.py
+-rw-r--r--   0        0        0     8200 2023-03-24 17:28:52.210535 checkthechain-0.3.5/src/ctc/db/management/dba_utils.py
+-rw-r--r--   0        0        0      634 2023-02-26 20:15:07.411288 checkthechain-0.3.5/src/ctc/db/management/reorg_utils.py
+-rw-r--r--   0        0        0     3594 2023-02-27 18:50:47.123257 checkthechain-0.3.5/src/ctc/db/management/version_utils.py
+-rw-r--r--   0        0        0     1879 2023-04-14 22:55:23.964370 checkthechain-0.3.5/src/ctc/db/query_utils.py
+-rw-r--r--   0        0        0     4735 2023-04-27 20:25:01.753860 checkthechain-0.3.5/src/ctc/db/schema_utils.py
+-rw-r--r--   0        0        0      285 2023-02-26 18:21:06.950384 checkthechain-0.3.5/src/ctc/db/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.108677 checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/__init__.py
+-rw-r--r--   0        0        0       43 2022-11-23 19:36:31.108781 checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/block_gas_stats/__init__.py
+-rw-r--r--   0        0        0     1138 2023-02-26 20:15:07.412506 checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/block_gas_stats/block_gas_stats_schema_defs.py
+-rw-r--r--   0        0        0       39 2022-11-23 19:36:31.108986 checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/erc20_state/__init__.py
+-rw-r--r--   0        0        0     1259 2023-02-26 20:15:07.412713 checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/erc20_state/erc20_state_schema_defs.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.109185 checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/protocol_schemas/__init__.py
+-rw-r--r--   0        0        0      792 2023-02-26 20:15:07.412923 checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/protocol_schemas/fourbyte_schema_defs.py
+-rw-r--r--   0        0        0      634 2023-02-26 20:15:07.413166 checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/protocol_schemas/fuse_pools_schema_defs.py
+-rw-r--r--   0        0        0      387 2023-02-26 20:15:07.413408 checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/protocol_schemas/uniswap_v2_pools_schema_defs.py
+-rw-r--r--   0        0        0      436 2023-02-26 20:15:07.413623 checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/protocol_schemas/uniswap_v3_pools_schema_defs.py
+-rw-r--r--   0        0        0      106 2022-11-23 19:36:31.109629 checkthechain-0.3.5/src/ctc/db/schemas/block_gas/__init__.py
+-rw-r--r--   0        0        0      420 2022-11-23 19:36:31.109689 checkthechain-0.3.5/src/ctc/db/schemas/block_gas/block_gas_queries.py
+-rw-r--r--   0        0        0      629 2023-02-26 20:15:07.414036 checkthechain-0.3.5/src/ctc/db/schemas/block_gas/block_gas_schema_defs.py
+-rw-r--r--   0        0        0     3001 2023-04-15 23:24:04.689689 checkthechain-0.3.5/src/ctc/db/schemas/block_gas/block_gas_statements.py
+-rw-r--r--   0        0        0      194 2022-11-23 19:36:31.109953 checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/__init__.py
+-rw-r--r--   0        0        0      562 2023-02-26 20:15:07.414563 checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/block_timestamps_schema_defs.py
+-rw-r--r--   0        0        0     6162 2023-04-15 23:08:40.662417 checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/block_timestamps_statements.py
+-rw-r--r--   0        0        0     1596 2022-11-23 19:36:31.110176 checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_queries.py
+-rw-r--r--   0        0        0     4431 2023-04-17 01:12:40.874133 checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_search.py
+-rw-r--r--   0        0        0     3058 2023-02-26 20:15:07.415190 checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_statements.py
+-rw-r--r--   0        0        0      126 2022-11-23 19:36:31.110528 checkthechain-0.3.5/src/ctc/db/schemas/blocks/__init__.py
+-rw-r--r--   0        0        0    10484 2023-02-26 21:02:01.364459 checkthechain-0.3.5/src/ctc/db/schemas/blocks/blocks_intake.py
+-rw-r--r--   0        0        0      343 2022-11-23 19:36:31.110828 checkthechain-0.3.5/src/ctc/db/schemas/blocks/blocks_queries.py
+-rw-r--r--   0        0        0      725 2023-02-26 20:15:07.415649 checkthechain-0.3.5/src/ctc/db/schemas/blocks/blocks_schema_defs.py
+-rw-r--r--   0        0        0     7041 2023-02-27 06:50:44.454081 checkthechain-0.3.5/src/ctc/db/schemas/blocks/blocks_statements.py
+-rw-r--r--   0        0        0      154 2022-11-23 19:36:31.111040 checkthechain-0.3.5/src/ctc/db/schemas/contract_abis/__init__.py
+-rw-r--r--   0        0        0     1155 2023-02-26 20:15:07.416090 checkthechain-0.3.5/src/ctc/db/schemas/contract_abis/contract_abis_intake.py
+-rw-r--r--   0        0        0      406 2022-11-23 19:36:31.111159 checkthechain-0.3.5/src/ctc/db/schemas/contract_abis/contract_abis_queries.py
+-rw-r--r--   0        0        0      392 2023-02-26 20:15:07.416278 checkthechain-0.3.5/src/ctc/db/schemas/contract_abis/contract_abis_schema_defs.py
+-rw-r--r--   0        0        0     2403 2023-03-04 08:00:44.984031 checkthechain-0.3.5/src/ctc/db/schemas/contract_abis/contract_abis_statements.py
+-rw-r--r--   0        0        0      198 2022-11-23 19:36:31.111410 checkthechain-0.3.5/src/ctc/db/schemas/contract_creation_blocks/__init__.py
+-rw-r--r--   0        0        0     1031 2023-02-26 20:15:07.416737 checkthechain-0.3.5/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_intake.py
+-rw-r--r--   0        0        0      505 2022-11-23 19:36:31.111535 checkthechain-0.3.5/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_queries.py
+-rw-r--r--   0        0        0      534 2023-02-26 20:15:07.416982 checkthechain-0.3.5/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_schema_defs.py
+-rw-r--r--   0        0        0     2081 2023-03-06 04:31:37.480699 checkthechain-0.3.5/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_statements.py
+-rw-r--r--   0        0        0      138 2022-11-23 19:36:31.111785 checkthechain-0.3.5/src/ctc/db/schemas/dex_pools/__init__.py
+-rw-r--r--   0        0        0     1576 2023-02-26 20:15:07.417521 checkthechain-0.3.5/src/ctc/db/schemas/dex_pools/dex_pools_intake.py
+-rw-r--r--   0        0        0      578 2022-11-23 19:36:31.111973 checkthechain-0.3.5/src/ctc/db/schemas/dex_pools/dex_pools_queries.py
+-rw-r--r--   0        0        0     1094 2023-02-26 20:15:07.417730 checkthechain-0.3.5/src/ctc/db/schemas/dex_pools/dex_pools_schema_defs.py
+-rw-r--r--   0        0        0     6060 2023-04-12 21:15:00.071455 checkthechain-0.3.5/src/ctc/db/schemas/dex_pools/dex_pools_statements.py
+-rw-r--r--   0        0        0      158 2022-11-23 19:36:31.112442 checkthechain-0.3.5/src/ctc/db/schemas/erc20_metadata/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-26 20:15:07.418167 checkthechain-0.3.5/src/ctc/db/schemas/erc20_metadata/erc20_metadata_intake.py
+-rw-r--r--   0        0        0      419 2023-02-26 18:21:06.953935 checkthechain-0.3.5/src/ctc/db/schemas/erc20_metadata/erc20_metadata_queries.py
+-rw-r--r--   0        0        0      765 2023-02-26 20:15:07.418402 checkthechain-0.3.5/src/ctc/db/schemas/erc20_metadata/erc20_metadata_schema_defs.py
+-rw-r--r--   0        0        0     3673 2023-04-11 21:30:22.630170 checkthechain-0.3.5/src/ctc/db/schemas/erc20_metadata/erc20_metadata_statements.py
+-rw-r--r--   0        0        0      126 2023-02-26 18:21:06.954232 checkthechain-0.3.5/src/ctc/db/schemas/events/__init__.py
+-rw-r--r--   0        0        0     2217 2023-04-10 04:00:25.884785 checkthechain-0.3.5/src/ctc/db/schemas/events/events_intake.py
+-rw-r--r--   0        0        0      359 2023-04-10 23:47:03.987654 checkthechain-0.3.5/src/ctc/db/schemas/events/events_queries.py
+-rw-r--r--   0        0        0     2896 2023-04-27 21:04:55.972761 checkthechain-0.3.5/src/ctc/db/schemas/events/events_schema_defs.py
+-rw-r--r--   0        0        0    12138 2023-04-12 19:57:20.128959 checkthechain-0.3.5/src/ctc/db/schemas/events/events_statements.py
+-rw-r--r--   0        0        0       43 2022-11-23 19:36:31.112900 checkthechain-0.3.5/src/ctc/db/schemas/schema_versions/__init__.py
+-rw-r--r--   0        0        0      503 2023-02-26 20:15:07.419573 checkthechain-0.3.5/src/ctc/db/schemas/schema_versions/schema_versions_schema_defs.py
+-rw-r--r--   0        0        0      151 2023-02-26 18:21:06.955047 checkthechain-0.3.5/src/ctc/db/schemas/transactions/__init__.py
+-rw-r--r--   0        0        0     3065 2023-02-26 20:15:07.419798 checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_intake.py
+-rw-r--r--   0        0        0     1084 2023-02-26 18:21:06.955542 checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_queries.py
+-rw-r--r--   0        0        0     1505 2023-02-26 20:15:07.419998 checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_schema_defs.py
+-rw-r--r--   0        0        0      125 2023-02-26 18:21:06.956032 checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_statements/__init__.py
+-rw-r--r--   0        0        0     2343 2023-04-27 06:04:57.381242 checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_statements/composite_block_transactions.py
+-rw-r--r--   0        0        0     3690 2023-02-27 06:48:19.824368 checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_statements/table_block_transaction_queries.py
+-rw-r--r--   0        0        0     3251 2023-03-10 20:38:54.085113 checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_statements/table_transactions.py
+-rw-r--r--   0        0        0        1 2022-11-23 19:36:31.148839 checkthechain-0.3.5/src/ctc/defi/__init__.py
+-rw-r--r--   0        0        0    39847 2023-04-11 15:01:03.698383 checkthechain-0.3.5/src/ctc/defi/cex_utils.py
+-rw-r--r--   0        0        0       21 2022-11-23 19:36:31.149006 checkthechain-0.3.5/src/ctc/defi/dex_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.149080 checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/__init__.py
+-rw-r--r--   0        0        0     1056 2022-11-23 19:36:31.149155 checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/amm_spec.py
+-rw-r--r--   0        0        0       84 2022-11-23 19:36:31.149422 checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/cpmm/__init__.py
+-rw-r--r--   0        0        0     3241 2023-04-10 01:05:06.123710 checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_liquidity.py
+-rw-r--r--   0        0        0     1292 2023-04-17 01:28:17.884516 checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_spec.py
+-rw-r--r--   0        0        0     9425 2022-11-23 19:36:31.149776 checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_summary.py
+-rw-r--r--   0        0        0     7780 2023-04-12 21:01:00.654910 checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_trade.py
+-rw-r--r--   0        0        0       37 2022-11-23 19:36:31.149993 checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/stableswap/__init__.py
+-rw-r--r--   0        0        0      333 2022-11-23 19:36:31.150062 checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/stableswap/stableswap_operations.py
+-rw-r--r--   0        0        0      151 2022-11-23 19:36:31.150205 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/__init__.py
+-rw-r--r--   0        0        0    22413 2023-05-03 23:49:39.987609 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_class.py
+-rw-r--r--   0        0        0     3458 2023-02-26 18:21:07.009571 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_class_utils.py
+-rw-r--r--   0        0        0     1523 2023-04-12 02:18:53.791732 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_directory.py
+-rw-r--r--   0        0        0      145 2022-11-23 19:36:31.150615 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_functions/__init__.py
+-rw-r--r--   0        0        0     2749 2023-02-26 18:21:07.009954 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_functions/dex_balance_functions.py
+-rw-r--r--   0        0        0     1603 2023-02-26 18:21:07.010224 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_functions/dex_metadata_functions.py
+-rw-r--r--   0        0        0     2038 2023-02-26 18:21:07.010390 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_functions/dex_pools_functions.py
+-rw-r--r--   0        0        0     1510 2023-04-17 01:11:51.919003 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_functions/dex_trade_functions.py
+-rw-r--r--   0        0        0      184 2022-11-23 19:36:31.151177 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_implementations/__init__.py
+-rw-r--r--   0        0        0     5880 2023-04-11 02:43:28.475321 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_implementations/balancer_dex.py
+-rw-r--r--   0        0        0     7488 2023-04-11 02:44:21.401565 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_implementations/curve_dex.py
+-rw-r--r--   0        0        0      207 2022-11-23 19:36:31.151507 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_implementations/sushi_dex.py
+-rw-r--r--   0        0        0     4350 2023-04-12 22:58:36.356923 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_implementations/uniswap_v2_dex.py
+-rw-r--r--   0        0        0     3932 2023-04-11 00:19:46.796938 checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_implementations/uniswap_v3_dex.py
+-rw-r--r--   0        0        0       31 2022-11-23 19:36:31.151852 checkthechain-0.3.5/src/ctc/defi/lending_utils/__init__.py
+-rw-r--r--   0        0        0     7740 2023-04-11 05:05:46.922489 checkthechain-0.3.5/src/ctc/defi/lending_utils/lending_summary.py
+-rw-r--r--   0        0        0        1 2023-04-15 16:02:19.893267 checkthechain-0.3.5/src/ctc/defi/metric_utils/__init__.py
+-rw-r--r--   0        0        0     1965 2023-04-11 21:23:13.516151 checkthechain-0.3.5/src/ctc/defi/metric_utils/ohlc_utils.py
+-rw-r--r--   0        0        0      346 2022-11-23 19:36:31.152114 checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/README.md
+-rw-r--r--   0        0        0      103 2022-11-23 19:36:31.152177 checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/__init__.py
+-rw-r--r--   0        0        0     4043 2023-02-26 18:21:07.012053 checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/feed_utils.py
+-rw-r--r--   0        0        0     2824 2023-04-11 05:41:47.387268 checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/twap_crud.py
+-rw-r--r--   0        0        0      936 2023-04-11 05:24:45.040006 checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/twap_data.py
+-rw-r--r--   0        0        0     2630 2023-04-11 05:25:54.330704 checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/twap_data_sources.py
+-rw-r--r--   0        0        0     1292 2023-04-11 04:55:26.105147 checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/twap_filter.py
+-rw-r--r--   0        0        0      442 2023-04-17 01:29:49.343807 checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/twap_spec.py
+-rw-r--r--   0        0        0      365 2023-02-26 18:21:06.956840 checkthechain-0.3.5/src/ctc/evm/__init__.py
+-rw-r--r--   0        0        0      131 2022-11-23 19:36:31.113210 checkthechain-0.3.5/src/ctc/evm/abi_utils/__init__.py
+-rw-r--r--   0        0        0     2256 2023-05-04 21:17:33.110466 checkthechain-0.3.5/src/ctc/evm/abi_utils/abi_coding_utils.py
+-rw-r--r--   0        0        0      189 2022-11-23 19:36:31.113375 checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/__init__.py
+-rw-r--r--   0        0        0     2698 2022-11-23 19:36:31.113461 checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_comparison.py
+-rw-r--r--   0        0        0     1361 2023-02-26 18:21:06.957338 checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_decompilation.py
+-rw-r--r--   0        0        0     2142 2023-02-26 18:21:06.957664 checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_io.py
+-rw-r--r--   0        0        0      660 2022-11-23 19:36:31.113721 checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_modification.py
+-rw-r--r--   0        0        0     9934 2023-04-11 03:28:48.635201 checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_summary.py
+-rw-r--r--   0        0        0      137 2023-03-04 05:46:27.752144 checkthechain-0.3.5/src/ctc/evm/abi_utils/event_abi_utils/__init__.py
+-rw-r--r--   0        0        0     6278 2023-04-11 17:04:41.509191 checkthechain-0.3.5/src/ctc/evm/abi_utils/event_abi_utils/event_abi_coding.py
+-rw-r--r--   0        0        0    14548 2023-06-03 00:20:08.972191 checkthechain-0.3.5/src/ctc/evm/abi_utils/event_abi_utils/event_abi_coding_polars.py
+-rw-r--r--   0        0        0     2650 2023-04-11 17:23:39.585194 checkthechain-0.3.5/src/ctc/evm/abi_utils/event_abi_utils/event_abi_parsing.py
+-rw-r--r--   0        0        0     3660 2023-03-04 07:55:53.565102 checkthechain-0.3.5/src/ctc/evm/abi_utils/event_abi_utils/event_abi_queries.py
+-rw-r--r--   0        0        0      107 2022-11-23 19:36:31.114446 checkthechain-0.3.5/src/ctc/evm/abi_utils/function_abi_utils/__init__.py
+-rw-r--r--   0        0        0     8050 2023-04-11 16:54:40.278301 checkthechain-0.3.5/src/ctc/evm/abi_utils/function_abi_utils/function_abi_coding.py
+-rw-r--r--   0        0        0     8453 2023-02-26 18:21:06.958642 checkthechain-0.3.5/src/ctc/evm/abi_utils/function_abi_utils/function_abi_parsing.py
+-rw-r--r--   0        0        0     5155 2023-05-03 21:01:44.378805 checkthechain-0.3.5/src/ctc/evm/abi_utils/function_abi_utils/function_abi_queries.py
+-rw-r--r--   0        0        0      129 2023-02-26 18:21:06.959059 checkthechain-0.3.5/src/ctc/evm/address_utils/__init__.py
+-rw-r--r--   0        0        0     1555 2023-04-11 17:07:31.645090 checkthechain-0.3.5/src/ctc/evm/address_utils/address_data.py
+-rw-r--r--   0        0        0     2881 2023-02-26 18:21:06.959458 checkthechain-0.3.5/src/ctc/evm/address_utils/address_resolution.py
+-rw-r--r--   0        0        0     3628 2023-02-26 18:21:06.959812 checkthechain-0.3.5/src/ctc/evm/address_utils/address_summary.py
+-rw-r--r--   0        0        0     6147 2023-04-11 03:41:52.412674 checkthechain-0.3.5/src/ctc/evm/address_utils/address_transactions.py
+-rw-r--r--   0        0        0      177 2022-11-23 19:36:31.115455 checkthechain-0.3.5/src/ctc/evm/binary_utils/__init__.py
+-rw-r--r--   0        0        0     7187 2023-04-11 17:24:12.284270 checkthechain-0.3.5/src/ctc/evm/binary_utils/format_utils.py
+-rw-r--r--   0        0        0     3169 2023-04-17 01:02:40.149889 checkthechain-0.3.5/src/ctc/evm/binary_utils/hash_utils.py
+-rw-r--r--   0        0        0     8948 2023-04-11 17:11:36.961031 checkthechain-0.3.5/src/ctc/evm/binary_utils/rlp_utils.py
+-rw-r--r--   0        0        0      146 2022-11-23 19:36:31.115957 checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/__init__.py
+-rw-r--r--   0        0        0     7465 2022-11-23 19:36:31.116055 checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/eip712_utils.py
+-rw-r--r--   0        0        0     1407 2023-04-11 17:13:01.266528 checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/key_utils.py
+-rw-r--r--   0        0        0     4915 2022-11-23 19:36:31.116213 checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/secp256k1_utils.py
+-rw-r--r--   0        0        0     2850 2023-04-11 17:12:22.146113 checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/signature_creation.py
+-rw-r--r--   0        0        0     2835 2023-04-11 17:11:56.281971 checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/signature_recovery.py
+-rw-r--r--   0        0        0     1926 2023-04-11 17:16:27.004803 checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/vrs_utils.py
+-rw-r--r--   0        0        0      280 2023-05-30 06:46:30.790511 checkthechain-0.3.5/src/ctc/evm/block_utils/__init__.py
+-rw-r--r--   0        0        0     2750 2023-04-11 17:18:20.638063 checkthechain-0.3.5/src/ctc/evm/block_utils/block_coding.py
+-rw-r--r--   0        0        0      608 2023-02-26 18:21:06.960791 checkthechain-0.3.5/src/ctc/evm/block_utils/block_convert.py
+-rw-r--r--   0        0        0     6865 2023-05-09 04:17:37.723832 checkthechain-0.3.5/src/ctc/evm/block_utils/block_crud.py
+-rw-r--r--   0        0        0     8315 2023-06-03 00:20:08.973363 checkthechain-0.3.5/src/ctc/evm/block_utils/block_gas.py
+-rw-r--r--   0        0        0     1083 2023-02-26 18:21:06.961562 checkthechain-0.3.5/src/ctc/evm/block_utils/block_hashes.py
+-rw-r--r--   0        0        0     1990 2023-02-26 18:21:06.961734 checkthechain-0.3.5/src/ctc/evm/block_utils/block_normalize.py
+-rw-r--r--   0        0        0      662 2023-05-30 06:46:30.790714 checkthechain-0.3.5/src/ctc/evm/block_utils/block_prices.py
+-rw-r--r--   0        0        0     5580 2023-05-27 19:14:13.240378 checkthechain-0.3.5/src/ctc/evm/block_utils/block_samples.py
+-rw-r--r--   0        0        0     2759 2023-05-27 15:37:02.677178 checkthechain-0.3.5/src/ctc/evm/block_utils/block_summary.py
+-rw-r--r--   0        0        0      137 2023-05-27 19:01:35.203629 checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/__init__.py
+-rw-r--r--   0        0        0     3690 2023-05-30 06:46:30.791681 checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/block_time_bins.py
+-rw-r--r--   0        0        0     6100 2023-02-26 18:21:06.962078 checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/block_time_predictions.py
+-rw-r--r--   0        0        0     2437 2023-02-26 18:21:06.962477 checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/block_to_timestamp.py
+-rw-r--r--   0        0        0      133 2022-11-23 19:36:31.118022 checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/timestamp_to_block/__init__.py
+-rw-r--r--   0        0        0     3620 2023-02-26 18:21:06.962780 checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_plural.py
+-rw-r--r--   0        0        0     4479 2023-02-26 18:21:06.962964 checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_range.py
+-rw-r--r--   0        0        0     6005 2023-05-27 19:13:07.231807 checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_search.py
+-rw-r--r--   0        0        0     4136 2023-05-27 19:13:12.416617 checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_singular.py
+-rw-r--r--   0        0        0       64 2023-02-26 18:21:06.963936 checkthechain-0.3.5/src/ctc/evm/consensus_utils/__init__.py
+-rw-r--r--   0        0        0     4002 2023-02-26 18:21:06.964193 checkthechain-0.3.5/src/ctc/evm/consensus_utils/consensus_queries.py
+-rw-r--r--   0        0        0     1665 2023-04-28 23:57:21.283647 checkthechain-0.3.5/src/ctc/evm/consensus_utils/consensus_requests.py
+-rw-r--r--   0        0        0     2118 2023-02-26 18:21:06.964748 checkthechain-0.3.5/src/ctc/evm/consensus_utils/consensus_spec.py
+-rw-r--r--   0        0        0       96 2023-02-26 18:21:06.965010 checkthechain-0.3.5/src/ctc/evm/contract_utils/__init__.py
+-rw-r--r--   0        0        0     6575 2023-04-11 17:04:21.999102 checkthechain-0.3.5/src/ctc/evm/contract_utils/contract_creations.py
+-rw-r--r--   0        0        0     9875 2023-02-26 18:21:06.965502 checkthechain-0.3.5/src/ctc/evm/contract_utils/contract_proxies.py
+-rw-r--r--   0        0        0      979 2023-02-26 18:21:06.965736 checkthechain-0.3.5/src/ctc/evm/contract_utils/contract_tests.py
+-rw-r--r--   0        0        0      200 2022-11-23 19:36:31.118451 checkthechain-0.3.5/src/ctc/evm/erc20_utils/__init__.py
+-rw-r--r--   0        0        0     5922 2023-04-11 15:05:42.419653 checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_events.py
+-rw-r--r--   0        0        0     2179 2023-04-12 16:02:37.446080 checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_generic.py
+-rw-r--r--   0        0        0    13187 2023-06-03 00:20:08.974291 checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_metadata.py
+-rw-r--r--   0        0        0     6574 2023-04-12 16:01:20.761726 checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_normalize.py
+-rw-r--r--   0        0        0     3433 2022-11-23 19:36:31.118864 checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_spec.py
+-rw-r--r--   0        0        0    12612 2023-05-03 23:48:57.178118 checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_state.py
+-rw-r--r--   0        0        0     1871 2023-02-26 18:21:06.967336 checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_summary.py
+-rw-r--r--   0        0        0      188 2023-02-26 18:21:06.967455 checkthechain-0.3.5/src/ctc/evm/erc4626_utils/__init__.py
+-rw-r--r--   0        0        0     4233 2023-04-12 06:22:58.195596 checkthechain-0.3.5/src/ctc/evm/erc4626_utils/erc4626_events.py
+-rw-r--r--   0        0        0     1097 2023-02-26 18:21:06.967850 checkthechain-0.3.5/src/ctc/evm/erc4626_utils/erc4626_metadata.py
+-rw-r--r--   0        0        0     5796 2023-04-10 06:23:55.747564 checkthechain-0.3.5/src/ctc/evm/erc4626_utils/erc4626_normalize.py
+-rw-r--r--   0        0        0    10976 2023-02-26 18:21:06.968082 checkthechain-0.3.5/src/ctc/evm/erc4626_utils/erc4626_spec.py
+-rw-r--r--   0        0        0    23565 2023-02-26 18:21:06.968309 checkthechain-0.3.5/src/ctc/evm/erc4626_utils/erc4626_state.py
+-rw-r--r--   0        0        0      147 2023-02-26 18:21:06.968426 checkthechain-0.3.5/src/ctc/evm/erc721_utils/__init__.py
+-rw-r--r--   0        0        0     1740 2023-04-11 15:04:56.245383 checkthechain-0.3.5/src/ctc/evm/erc721_utils/erc721_events.py
+-rw-r--r--   0        0        0     1930 2023-02-26 18:21:06.968922 checkthechain-0.3.5/src/ctc/evm/erc721_utils/erc721_metadata.py
+-rw-r--r--   0        0        0     2967 2023-04-11 15:04:52.910074 checkthechain-0.3.5/src/ctc/evm/erc721_utils/erc721_ownership.py
+-rw-r--r--   0        0        0     5323 2023-02-26 18:21:06.969310 checkthechain-0.3.5/src/ctc/evm/erc721_utils/erc721_spec.py
+-rw-r--r--   0        0        0     3108 2023-02-26 18:21:06.969455 checkthechain-0.3.5/src/ctc/evm/erc721_utils/erc721_state.py
+-rw-r--r--   0        0        0       24 2022-11-23 19:36:31.120339 checkthechain-0.3.5/src/ctc/evm/eth_utils/__init__.py
+-rw-r--r--   0        0        0     4151 2023-02-26 18:21:06.969708 checkthechain-0.3.5/src/ctc/evm/eth_utils/eth_crud.py
+-rw-r--r--   0        0        0       96 2023-02-26 18:21:06.969843 checkthechain-0.3.5/src/ctc/evm/event_utils/__init__.py
+-rw-r--r--   0        0        0    15537 2023-04-13 02:52:22.209972 checkthechain-0.3.5/src/ctc/evm/event_utils/event_crud.py
+-rw-r--r--   0        0        0     6151 2023-05-02 21:14:45.321958 checkthechain-0.3.5/src/ctc/evm/event_utils/event_hybrid_queries.py
+-rw-r--r--   0        0        0     1909 2023-04-11 15:05:32.152407 checkthechain-0.3.5/src/ctc/evm/event_utils/event_metadata.py
+-rw-r--r--   0        0        0     7662 2023-04-11 17:14:11.631727 checkthechain-0.3.5/src/ctc/evm/event_utils/event_node_utils.py
+-rw-r--r--   0        0        0    10602 2023-05-02 21:14:20.680012 checkthechain-0.3.5/src/ctc/evm/event_utils/event_query_utils.py
+-rw-r--r--   0        0        0       33 2022-11-23 19:36:31.121258 checkthechain-0.3.5/src/ctc/evm/network_utils/__init__.py
+-rw-r--r--   0        0        0     2501 2023-02-26 18:21:06.972751 checkthechain-0.3.5/src/ctc/evm/network_utils/network_directory.py
+-rw-r--r--   0        0        0       89 2023-03-11 04:51:22.361782 checkthechain-0.3.5/src/ctc/evm/trace_utils/__init__.py
+-rw-r--r--   0        0        0     4160 2023-05-05 05:28:17.202870 checkthechain-0.3.5/src/ctc/evm/trace_utils/specific_traces.py
+-rw-r--r--   0        0        0     2259 2023-03-06 03:07:15.579397 checkthechain-0.3.5/src/ctc/evm/trace_utils/trace_crud.py
+-rw-r--r--   0        0        0     4712 2023-02-26 20:15:07.421666 checkthechain-0.3.5/src/ctc/evm/trace_utils/trace_state_diff.py
+-rw-r--r--   0        0        0      244 2023-02-26 18:21:06.973711 checkthechain-0.3.5/src/ctc/evm/transaction_utils/__init__.py
+-rw-r--r--   0        0        0     3687 2023-04-27 06:18:19.829021 checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_convert.py
+-rw-r--r--   0        0        0     6691 2023-02-26 20:15:07.422149 checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_crud.py
+-rw-r--r--   0        0        0      722 2023-02-26 18:21:06.974413 checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_hashes.py
+-rw-r--r--   0        0        0     3119 2023-04-12 19:53:53.308960 checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_serialize.py
+-rw-r--r--   0        0        0     4298 2023-04-12 19:55:41.976804 checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_signatures.py
+-rw-r--r--   0        0        0     7878 2023-04-11 17:08:12.970832 checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_summary.py
+-rw-r--r--   0        0        0     2911 2023-04-12 16:41:24.818020 checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_types.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.122150 checkthechain-0.3.5/src/ctc/protocols/__init__.py
+-rw-r--r--   0        0        0      210 2022-11-23 19:36:31.122290 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/__init__.py
+-rw-r--r--   0        0        0     7437 2023-04-17 01:33:49.120175 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_interest_rates.py
+-rw-r--r--   0        0        0     2271 2023-04-10 04:41:13.923918 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_lending_pool.py
+-rw-r--r--   0        0        0     3034 2023-02-26 18:21:06.976319 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_oracle.py
+-rw-r--r--   0        0        0     1198 2023-02-26 18:21:06.976540 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_pool_tokens.py
+-rw-r--r--   0        0        0     3099 2023-02-26 18:21:06.976782 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_rewards.py
+-rw-r--r--   0        0        0      953 2023-04-12 02:17:55.732920 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_spec.py
+-rw-r--r--   0        0        0    14153 2023-04-12 02:17:27.412342 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_summaries.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.122992 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/cli/__init__.py
+-rw-r--r--   0        0        0      870 2023-01-02 06:57:18.122699 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/cli/aave_addresses_command.py
+-rw-r--r--   0        0        0     3072 2022-11-23 19:36:31.123144 checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/cli/aave_command.py
+-rw-r--r--   0        0        0      165 2022-11-23 19:36:31.123232 checkthechain-0.3.5/src/ctc/protocols/balancer_utils/__init__.py
+-rw-r--r--   0        0        0     4074 2023-02-26 18:21:06.977445 checkthechain-0.3.5/src/ctc/protocols/balancer_utils/balancer_spec.py
+-rw-r--r--   0        0        0     3341 2023-04-11 02:48:49.301350 checkthechain-0.3.5/src/ctc/protocols/balancer_utils/pool_metadata.py
+-rw-r--r--   0        0        0     4646 2023-04-11 05:41:02.218451 checkthechain-0.3.5/src/ctc/protocols/balancer_utils/pool_plots.py
+-rw-r--r--   0        0        0     6265 2023-02-26 18:21:06.978055 checkthechain-0.3.5/src/ctc/protocols/balancer_utils/pool_state.py
+-rw-r--r--   0        0        0     6171 2023-04-17 01:25:48.874215 checkthechain-0.3.5/src/ctc/protocols/balancer_utils/pool_summary.py
+-rw-r--r--   0        0        0     1007 2022-11-23 19:36:31.123708 checkthechain-0.3.5/src/ctc/protocols/balancer_utils/pool_trades.py
+-rw-r--r--   0        0        0      237 2022-11-23 19:36:31.123840 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/__init__.py
+-rw-r--r--   0        0        0     6981 2023-02-26 18:21:06.978589 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_aggregators.py
+-rw-r--r--   0        0        0      147 2022-11-23 19:36:31.124095 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/__init__.py
+-rw-r--r--   0        0        0     2083 2023-04-11 05:31:39.920503 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/feed_composites.py
+-rw-r--r--   0        0        0     3101 2023-04-11 05:27:03.456016 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/feed_data.py
+-rw-r--r--   0        0        0     3181 2023-02-26 18:21:06.979122 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/feed_datum.py
+-rw-r--r--   0        0        0     2291 2023-04-11 14:58:42.923101 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/feed_datum_by_block.py
+-rw-r--r--   0        0        0     7300 2023-05-30 06:46:30.792533 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/feed_events.py
+-rw-r--r--   0        0        0      138 2022-11-23 19:36:31.124610 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_db/__init__.py
+-rw-r--r--   0        0        0     9709 2023-04-12 02:16:57.774414 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_intake.py
+-rw-r--r--   0        0        0      509 2022-11-23 19:36:31.124755 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_queries.py
+-rw-r--r--   0        0        0     1458 2023-02-26 20:15:07.422868 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_schema_defs.py
+-rw-r--r--   0        0        0     6188 2023-02-27 06:48:28.002164 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_statements.py
+-rw-r--r--   0        0        0     3742 2023-02-26 18:21:06.980172 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_feed_metadata.py
+-rw-r--r--   0        0        0      818 2023-02-26 18:21:06.980357 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_helpers.py
+-rw-r--r--   0        0        0     4401 2023-04-12 02:16:48.985174 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_registry.py
+-rw-r--r--   0        0        0     2921 2023-04-17 01:06:07.155895 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_spec.py
+-rw-r--r--   0        0        0     6328 2023-04-10 03:26:37.038448 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_summary.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.125353 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/cli/__init__.py
+-rw-r--r--   0        0        0     4564 2023-04-10 03:42:49.095411 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/cli/chainlink_command.py
+-rw-r--r--   0        0        0     2038 2023-02-26 18:21:06.981259 checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/cli/chainlink_ls_command.py
+-rw-r--r--   0        0        0       55 2022-11-23 19:36:31.125633 checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.125714 checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/cli/__init__.py
+-rw-r--r--   0        0        0     3751 2023-04-14 06:36:37.709398 checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/cli/cg_command.py
+-rw-r--r--   0        0        0      138 2022-11-23 19:36:31.125960 checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/coingecko_db/__init__.py
+-rw-r--r--   0        0        0      957 2023-02-26 20:15:07.423297 checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_intake.py
+-rw-r--r--   0        0        0      331 2023-02-26 18:21:06.981971 checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_queries.py
+-rw-r--r--   0        0        0      773 2023-04-17 01:08:19.565253 checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_schema_defs.py
+-rw-r--r--   0        0        0     3074 2023-04-12 23:19:05.754820 checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_statements.py
+-rw-r--r--   0        0        0     5795 2023-02-26 18:21:06.982284 checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/market_utils.py
+-rw-r--r--   0        0        0    16600 2023-02-27 08:16:17.715834 checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/token_utils.py
+-rw-r--r--   0        0        0       29 2022-11-23 19:36:31.126557 checkthechain-0.3.5/src/ctc/protocols/compound_utils/__init__.py
+-rw-r--r--   0        0        0     2397 2023-02-26 18:21:06.982879 checkthechain-0.3.5/src/ctc/protocols/compound_utils/compound_crud.py
+-rw-r--r--   0        0        0      168 2022-11-23 19:36:31.126693 checkthechain-0.3.5/src/ctc/protocols/curve_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.126751 checkthechain-0.3.5/src/ctc/protocols/curve_utils/cli/__init__.py
+-rw-r--r--   0        0        0     1690 2022-11-23 19:36:31.126829 checkthechain-0.3.5/src/ctc/protocols/curve_utils/cli/curve_pools_command.py
+-rw-r--r--   0        0        0     5258 2023-04-17 01:26:07.392801 checkthechain-0.3.5/src/ctc/protocols/curve_utils/curve_spec.py
+-rw-r--r--   0        0        0     3714 2023-02-26 18:21:06.983220 checkthechain-0.3.5/src/ctc/protocols/curve_utils/metapool_utils.py
+-rw-r--r--   0        0        0    15567 2023-04-17 01:36:34.284052 checkthechain-0.3.5/src/ctc/protocols/curve_utils/pool_lists.py
+-rw-r--r--   0        0        0     4951 2023-02-26 18:21:06.983838 checkthechain-0.3.5/src/ctc/protocols/curve_utils/pool_metadata.py
+-rw-r--r--   0        0        0     7351 2023-04-11 02:49:36.985754 checkthechain-0.3.5/src/ctc/protocols/curve_utils/pool_parameters.py
+-rw-r--r--   0        0        0     4085 2023-02-26 18:21:06.984206 checkthechain-0.3.5/src/ctc/protocols/curve_utils/pool_state.py
+-rw-r--r--   0        0        0       49 2022-11-23 19:36:31.127594 checkthechain-0.3.5/src/ctc/protocols/ens_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.127647 checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.127712 checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/__init__.py
+-rw-r--r--   0        0        0      813 2022-11-23 19:36:31.127791 checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/exists_command.py
+-rw-r--r--   0        0        0      441 2022-11-23 19:36:31.127871 checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/hash_command.py
+-rw-r--r--   0        0        0      765 2022-11-23 19:36:31.127934 checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/owner_command.py
+-rw-r--r--   0        0        0      625 2022-11-23 19:36:31.127994 checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/records_command.py
+-rw-r--r--   0        0        0      862 2022-11-23 19:36:31.128056 checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/resolve_command.py
+-rw-r--r--   0        0        0      876 2022-11-23 19:36:31.128123 checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/reverse_command.py
+-rw-r--r--   0        0        0     4278 2023-04-17 01:27:38.950415 checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens_command.py
+-rw-r--r--   0        0        0      482 2022-11-23 19:36:31.128261 checkthechain-0.3.5/src/ctc/protocols/ens_utils/ens_directory.py
+-rw-r--r--   0        0        0     3782 2023-04-11 04:50:29.681889 checkthechain-0.3.5/src/ctc/protocols/ens_utils/registrar.py
+-rw-r--r--   0        0        0     7572 2023-04-13 02:54:35.167992 checkthechain-0.3.5/src/ctc/protocols/ens_utils/resolver.py
+-rw-r--r--   0        0        0      132 2023-02-26 18:21:06.984864 checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/__init__.py
+-rw-r--r--   0        0        0     3353 2023-04-17 01:27:53.003738 checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/abi_crud.py
+-rw-r--r--   0        0        0     2596 2023-04-12 02:18:49.893638 checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/browser_utils.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.128654 checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/cli/__init__.py
+-rw-r--r--   0        0        0     2635 2023-02-26 18:21:06.985639 checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/cli/etherscan_command.py
+-rw-r--r--   0        0        0      326 2023-04-12 02:18:22.167751 checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/etherscan_spec.py
+-rw-r--r--   0        0        0      703 2023-04-12 02:18:27.736358 checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/misc_crud.py
+-rw-r--r--   0        0        0     4951 2023-04-12 02:18:47.139319 checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/url_crud.py
+-rw-r--r--   0        0        0      119 2022-11-23 19:36:31.133315 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.133373 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/cli/__init__.py
+-rw-r--r--   0        0        0     1407 2022-11-23 19:36:31.133450 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/cli/fourbyte_build_command.py
+-rw-r--r--   0        0        0     3849 2022-11-23 19:36:31.133514 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/cli/fourbyte_command.py
+-rw-r--r--   0        0        0      102 2022-11-23 19:36:31.133597 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_db/__init__.py
+-rw-r--r--   0        0        0     1846 2023-02-26 20:15:07.423891 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_intake.py
+-rw-r--r--   0        0        0     1856 2023-04-27 20:09:32.665313 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_schema_defs.py
+-rw-r--r--   0        0        0     5593 2023-04-27 20:23:37.596062 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_statements.py
+-rw-r--r--   0        0        0       90 2022-11-23 19:36:31.133972 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_queries/__init__.py
+-rw-r--r--   0        0        0     2746 2023-04-27 20:24:38.665613 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_queries/general_queries.py
+-rw-r--r--   0        0        0      393 2023-02-26 18:21:06.990217 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_queries/local_queries.py
+-rw-r--r--   0        0        0     4042 2023-04-17 01:28:43.369803 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_queries/remote_queries.py
+-rw-r--r--   0        0        0     3580 2023-02-26 18:21:06.990325 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_scrape.py
+-rw-r--r--   0        0        0     1420 2023-04-17 01:28:32.903495 checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_spec.py
+-rw-r--r--   0        0        0       20 2022-11-23 19:36:31.134412 checkthechain-0.3.5/src/ctc/protocols/g_uni_utils/__init__.py
+-rw-r--r--   0        0        0     3624 2023-02-26 18:21:06.990518 checkthechain-0.3.5/src/ctc/protocols/g_uni_utils/crud.py
+-rw-r--r--   0        0        0      670 2022-11-23 19:36:31.134602 checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/README.md
+-rw-r--r--   0        0        0      149 2022-11-23 19:36:31.134662 checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.134718 checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/cli/__init__.py
+-rw-r--r--   0        0        0     1036 2022-11-23 19:36:31.134790 checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/cli/gnosis_command.py
+-rw-r--r--   0        0        0     2976 2023-04-11 05:28:54.333360 checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_events.py
+-rw-r--r--   0        0        0     3793 2023-04-11 14:59:17.679623 checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_factory_events.py
+-rw-r--r--   0        0        0     1552 2023-02-26 18:21:06.991058 checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_metadata.py
+-rw-r--r--   0        0        0     7390 2023-04-17 01:07:53.696824 checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_spec.py
+-rw-r--r--   0        0        0     8950 2023-04-13 22:50:55.610898 checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_summary.py
+-rw-r--r--   0        0        0     6520 2023-04-11 16:33:17.017825 checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_transactions.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.135334 checkthechain-0.3.5/src/ctc/protocols/llama_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.135412 checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/__init__.py
+-rw-r--r--   0        0        0      563 2022-11-23 19:36:31.135510 checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_chain_command.py
+-rw-r--r--   0        0        0      637 2022-11-23 19:36:31.135597 checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_chains_command.py
+-rw-r--r--   0        0        0      355 2022-11-23 19:36:31.135677 checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_command.py
+-rw-r--r--   0        0        0      627 2022-11-23 19:36:31.135766 checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_pool_command.py
+-rw-r--r--   0        0        0     3756 2023-04-17 01:08:32.684084 checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_pools_command.py
+-rw-r--r--   0        0        0      877 2022-11-23 19:36:31.135929 checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_protocol_command.py
+-rw-r--r--   0        0        0     1307 2022-11-23 19:36:31.135982 checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_protocols_command.py
+-rw-r--r--   0        0        0     4886 2023-04-17 01:06:44.638753 checkthechain-0.3.5/src/ctc/protocols/llama_utils/llama_requests.py
+-rw-r--r--   0        0        0     6140 2023-02-26 18:21:06.991562 checkthechain-0.3.5/src/ctc/protocols/llama_utils/llama_tvls.py
+-rw-r--r--   0        0        0    10185 2023-04-17 01:08:15.444434 checkthechain-0.3.5/src/ctc/protocols/llama_utils/llama_yields.py
+-rw-r--r--   0        0        0       88 2022-11-23 19:36:31.136328 checkthechain-0.3.5/src/ctc/protocols/multicall_utils/__init__.py
+-rw-r--r--   0        0        0     4439 2023-04-11 16:49:40.251517 checkthechain-0.3.5/src/ctc/protocols/multicall_utils/call_utils.py
+-rw-r--r--   0        0        0     1511 2023-04-17 01:06:25.624061 checkthechain-0.3.5/src/ctc/protocols/multicall_utils/multicall_spec.py
+-rw-r--r--   0        0        0     3738 2023-04-12 02:17:20.118623 checkthechain-0.3.5/src/ctc/protocols/multicall_utils/multicalls_utils.py
+-rw-r--r--   0        0        0       57 2022-11-23 19:36:31.136829 checkthechain-0.3.5/src/ctc/protocols/rari_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.136919 checkthechain-0.3.5/src/ctc/protocols/rari_utils/cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.137039 checkthechain-0.3.5/src/ctc/protocols/rari_utils/cli/rari/__init__.py
+-rw-r--r--   0        0        0     2938 2022-11-23 19:36:31.137166 checkthechain-0.3.5/src/ctc/protocols/rari_utils/cli/rari/fuse_command.py
+-rw-r--r--   0        0        0     1584 2022-11-23 19:36:31.137258 checkthechain-0.3.5/src/ctc/protocols/rari_utils/cli/rari/pools_command.py
+-rw-r--r--   0        0        0     1367 2022-11-23 19:36:31.137399 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_lens/README.md
+-rw-r--r--   0        0        0      108 2022-11-23 19:36:31.137466 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_lens/__init__.py
+-rw-r--r--   0        0        0    21649 2022-11-23 19:36:31.137582 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_lens/lens_abis.py
+-rw-r--r--   0        0        0     8029 2023-04-17 01:30:37.145025 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_lens/lens_spec.py
+-rw-r--r--   0        0        0    15145 2023-04-17 01:30:56.860930 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_lens/primary_lens.py
+-rw-r--r--   0        0        0      205 2022-11-23 19:36:31.137849 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_lens/secondary_lens.py
+-rw-r--r--   0        0        0      231 2022-11-23 19:36:31.137957 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/__init__.py
+-rw-r--r--   0        0        0      794 2023-02-26 18:21:06.993247 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/directory_metadata.py
+-rw-r--r--   0        0        0      711 2022-11-23 19:36:31.138102 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/irm_metadata.py
+-rw-r--r--   0        0        0     2913 2022-11-23 19:36:31.138171 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/pool_metadata.py
+-rw-r--r--   0        0        0     2704 2022-11-23 19:36:31.138236 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/pool_state.py
+-rw-r--r--   0        0        0     3188 2022-11-23 19:36:31.138313 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/pool_summary.py
+-rw-r--r--   0        0        0     1311 2022-11-23 19:36:31.138413 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_metadata.py
+-rw-r--r--   0        0        0       84 2022-11-23 19:36:31.138564 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_state/__init__.py
+-rw-r--r--   0        0        0     3627 2022-11-23 19:36:31.138668 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_interest.py
+-rw-r--r--   0        0        0     2071 2022-11-23 19:36:31.138773 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_price.py
+-rw-r--r--   0        0        0     3658 2022-11-23 19:36:31.138888 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_usage.py
+-rw-r--r--   0        0        0     5852 2023-04-17 01:28:05.297767 checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_summary.py
+-rw-r--r--   0        0        0    89362 2022-11-23 19:36:31.139251 checkthechain-0.3.5/src/ctc/protocols/rari_utils/rari_abis.py
+-rw-r--r--   0        0        0    11979 2023-02-26 18:21:06.993503 checkthechain-0.3.5/src/ctc/protocols/rari_utils/summary_utils.py
+-rw-r--r--   0        0        0       56 2022-11-23 19:36:31.139484 checkthechain-0.3.5/src/ctc/protocols/sushi_utils/__init__.py
+-rw-r--r--   0        0        0      337 2022-11-23 19:36:31.139559 checkthechain-0.3.5/src/ctc/protocols/sushi_utils/sushi_spec.py
+-rw-r--r--   0        0        0      918 2023-02-26 18:21:06.993785 checkthechain-0.3.5/src/ctc/protocols/sushi_utils/sushiswap_crud.py
+-rw-r--r--   0        0        0      166 2022-11-23 19:36:31.139748 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.139808 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/__init__.py
+-rw-r--r--   0        0        0     1423 2022-11-23 19:36:31.139896 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/burns_command.py
+-rw-r--r--   0        0        0     6445 2023-04-15 16:03:17.419508 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/chart_command.py
+-rw-r--r--   0        0        0     1423 2022-11-23 19:36:31.140033 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/mints_command.py
+-rw-r--r--   0        0        0     1846 2023-04-15 15:59:51.449246 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/pool_command.py
+-rw-r--r--   0        0        0     1440 2022-11-23 19:36:31.140220 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/swaps_command.py
+-rw-r--r--   0        0        0     8203 2023-04-11 04:48:00.558717 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_deltas.py
+-rw-r--r--   0        0        0     5717 2023-04-15 15:59:32.040213 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_events.py
+-rw-r--r--   0        0        0     2776 2023-04-12 16:09:31.994054 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_metadata.py
+-rw-r--r--   0        0        0     5089 2023-04-17 01:27:08.232982 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_spec.py
+-rw-r--r--   0        0        0     3887 2023-05-03 23:41:11.177114 checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_state.py
+-rw-r--r--   0        0        0      151 2023-06-03 00:20:08.975286 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/__init__.py
+-rw-r--r--   0        0        0      138 2022-11-23 19:36:31.141120 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/__init__.py
+-rw-r--r--   0        0        0     1443 2023-02-26 18:21:06.994940 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/pool_derived_state.py
+-rw-r--r--   0        0        0     3240 2023-02-26 18:21:06.995117 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/pool_immutables.py
+-rw-r--r--   0        0        0     6560 2023-04-17 01:31:30.100039 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/pool_state.py
+-rw-r--r--   0        0        0     3006 2023-02-26 18:21:06.995466 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/quoter.py
+-rw-r--r--   0        0        0      860 2023-02-26 18:21:06.995686 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/tick_lens.py
+-rw-r--r--   0        0        0     3562 2023-04-17 01:31:50.529264 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_crud.py
+-rw-r--r--   0        0        0     3751 2023-02-26 18:21:06.996225 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_depth.py
+-rw-r--r--   0        0        0     3163 2023-02-26 18:21:06.996363 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_spec.py
+-rw-r--r--   0        0        0     6720 2023-06-03 00:20:08.975536 checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_swaps.py
+-rw-r--r--   0        0        0      140 2022-11-23 19:36:31.141857 checkthechain-0.3.5/src/ctc/protocols/yearn_utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.141930 checkthechain-0.3.5/src/ctc/protocols/yearn_utils/cli/__init__.py
+-rw-r--r--   0        0        0     1073 2023-04-12 02:18:13.432357 checkthechain-0.3.5/src/ctc/protocols/yearn_utils/cli/yearn_addresses_command.py
+-rw-r--r--   0        0        0     2553 2023-04-12 02:18:04.750648 checkthechain-0.3.5/src/ctc/protocols/yearn_utils/cli/yearn_command.py
+-rw-r--r--   0        0        0     5692 2023-04-12 02:17:48.585548 checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_addresses.py
+-rw-r--r--   0        0        0     1864 2022-11-23 19:36:31.142281 checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_spec.py
+-rw-r--r--   0        0        0     2885 2023-04-11 05:22:09.399822 checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_strategies.py
+-rw-r--r--   0        0        0     1200 2023-02-26 18:21:06.996752 checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_tvls.py
+-rw-r--r--   0        0        0    11227 2023-04-11 03:24:04.115576 checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_vaults.py
+-rw-r--r--   0        0        0     2327 2022-11-23 19:36:31.142631 checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_web_api.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.142664 checkthechain-0.3.5/src/ctc/py.typed
+-rw-r--r--   0        0        0      370 2023-04-29 02:18:16.632039 checkthechain-0.3.5/src/ctc/rpc/__init__.py
+-rw-r--r--   0        0        0      104 2022-11-23 19:36:31.142859 checkthechain-0.3.5/src/ctc/rpc/rpc_batch/__init__.py
+-rw-r--r--   0        0        0    16275 2023-03-04 19:50:23.519624 checkthechain-0.3.5/src/ctc/rpc/rpc_batch/rpc_batch_constructors.py
+-rw-r--r--   0        0        0    13042 2023-03-04 19:50:23.520213 checkthechain-0.3.5/src/ctc/rpc/rpc_batch/rpc_batch_executors.py
+-rw-r--r--   0        0        0     4185 2023-04-13 02:20:26.971506 checkthechain-0.3.5/src/ctc/rpc/rpc_batch/rpc_batch_utils.py
+-rw-r--r--   0        0        0      389 2023-02-26 18:21:06.998278 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/__init__.py
+-rw-r--r--   0        0        0     2442 2023-04-11 16:31:38.655891 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_block_constructors.py
+-rw-r--r--   0        0        0      602 2023-02-26 18:21:06.998793 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_dev_constructors.py
+-rw-r--r--   0        0        0     2486 2023-02-26 18:21:06.998980 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_log_constructors.py
+-rw-r--r--   0        0        0      951 2023-02-26 18:21:06.999159 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_mining_constructors.py
+-rw-r--r--   0        0        0     1004 2023-02-26 18:21:06.999424 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_node_constructors.py
+-rw-r--r--   0        0        0     3443 2023-04-11 16:30:45.199617 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_state_constructors.py
+-rw-r--r--   0        0        0     1916 2023-02-26 18:21:06.999889 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_submission_constructors.py
+-rw-r--r--   0        0        0     7325 2023-06-03 00:20:08.976370 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_trace_constructors.py
+-rw-r--r--   0        0        0     2138 2023-04-11 16:31:54.035220 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_transaction_constructors.py
+-rw-r--r--   0        0        0     2069 2023-02-26 18:21:07.000693 checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_whisper_constructors.py
+-rw-r--r--   0        0        0        0 2023-03-11 18:04:07.082068 checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/__init__.py
+-rw-r--r--   0        0        0     4653 2023-05-03 06:18:05.706354 checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/call_trace_decoder.py
+-rw-r--r--   0        0        0     2258 2023-04-21 15:41:10.224968 checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/create_trace_decoder.py
+-rw-r--r--   0        0        0      998 2023-03-26 06:20:45.338428 checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/log_decoder.py
+-rw-r--r--   0        0        0     4653 2023-05-02 22:58:53.788729 checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/native_transfer_decoder.py
+-rw-r--r--   0        0        0     6779 2023-05-03 16:33:35.235586 checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/slot_diff_decoder.py
+-rw-r--r--   0        0        0      359 2023-02-26 18:21:07.000942 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/__init__.py
+-rw-r--r--   0        0        0     3589 2022-11-23 19:36:31.144157 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_block_digestors.py
+-rw-r--r--   0        0        0      552 2022-11-23 19:36:31.144227 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_dev_digestors.py
+-rw-r--r--   0        0        0     3831 2022-11-23 19:36:31.144290 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_log_digestors.py
+-rw-r--r--   0        0        0      773 2022-11-23 19:36:31.144353 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_mining_digestors.py
+-rw-r--r--   0        0        0     1465 2022-11-23 19:36:31.144412 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_node_digestors.py
+-rw-r--r--   0        0        0     1738 2022-11-23 19:36:31.144465 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_state_digestors.py
+-rw-r--r--   0        0        0     1197 2022-11-23 19:36:31.144518 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_submission_digestors.py
+-rw-r--r--   0        0        0     7929 2023-03-04 19:50:23.521981 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_trace_digestors.py
+-rw-r--r--   0        0        0     2747 2022-11-23 19:36:31.144581 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_transaction_digestors.py
+-rw-r--r--   0        0        0     1269 2022-11-23 19:36:31.144661 checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_whisper_digestors.py
+-rw-r--r--   0        0        0      380 2023-04-29 02:55:17.696175 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/__init__.py
+-rw-r--r--   0        0        0     4628 2023-05-04 00:21:12.284488 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_block_executors_async.py
+-rw-r--r--   0        0        0     1437 2023-03-27 22:28:00.721319 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_dev_executors_async.py
+-rw-r--r--   0        0        0     5279 2023-03-26 06:20:39.297576 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_log_executors_async.py
+-rw-r--r--   0        0        0     2190 2023-02-26 18:21:07.002129 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_mining_executors_async.py
+-rw-r--r--   0        0        0     2851 2023-02-26 18:21:07.002296 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_node_executors_async.py
+-rw-r--r--   0        0        0     6117 2023-04-13 02:15:46.804141 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_state_executors_async.py
+-rw-r--r--   0        0        0     3168 2023-02-26 18:21:07.002644 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_submission_executors_async.py
+-rw-r--r--   0        0        0    10219 2023-03-04 19:50:23.522274 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_trace_executors_async.py
+-rw-r--r--   0        0        0     4590 2023-02-26 18:21:07.003081 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_transaction_executors_async.py
+-rw-r--r--   0        0        0     3970 2023-02-26 18:21:07.003260 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_whisper_executors_async.py
+-rw-r--r--   0        0        0      372 2023-04-29 02:20:39.544187 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/__init__.py
+-rw-r--r--   0        0        0     4530 2023-04-29 02:40:39.931253 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_block_executors_sync.py
+-rw-r--r--   0        0        0     1381 2023-04-29 02:41:16.847417 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_dev_executors_sync.py
+-rw-r--r--   0        0        0     5174 2023-04-29 02:42:15.741339 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_log_executors_sync.py
+-rw-r--r--   0        0        0     2106 2023-04-29 02:43:32.387691 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_mining_executors_sync.py
+-rw-r--r--   0        0        0     2739 2023-04-29 02:44:35.472432 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_node_executors_sync.py
+-rw-r--r--   0        0        0     6033 2023-04-29 02:48:08.574123 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_state_executors_sync.py
+-rw-r--r--   0        0        0     3084 2023-04-29 02:49:21.046565 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_submission_executors_sync.py
+-rw-r--r--   0        0        0    10030 2023-04-29 02:50:56.085928 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_trace_executors_sync.py
+-rw-r--r--   0        0        0     4492 2023-04-29 02:51:37.478912 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_transaction_executors_sync.py
+-rw-r--r--   0        0        0     3830 2023-04-29 02:53:28.556506 checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_whisper_executors_sync.py
+-rw-r--r--   0        0        0     1068 2022-12-25 15:14:22.765380 checkthechain-0.3.5/src/ctc/rpc/rpc_format.py
+-rw-r--r--   0        0        0     2051 2023-02-26 18:21:07.003537 checkthechain-0.3.5/src/ctc/rpc/rpc_lifecycle.py
+-rw-r--r--   0        0        0     1999 2023-02-26 18:21:07.003667 checkthechain-0.3.5/src/ctc/rpc/rpc_logging.py
+-rw-r--r--   0        0        0       47 2023-04-29 00:10:42.447596 checkthechain-0.3.5/src/ctc/rpc/rpc_protocols/__init__.py
+-rw-r--r--   0        0        0     4255 2023-04-29 03:32:17.512979 checkthechain-0.3.5/src/ctc/rpc/rpc_protocols/rpc_http.py
+-rw-r--r--   0        0        0      321 2023-04-29 00:13:48.363233 checkthechain-0.3.5/src/ctc/rpc/rpc_protocols/rpc_websocket.py
+-rw-r--r--   0        0        0     9770 2023-04-17 01:11:21.303538 checkthechain-0.3.5/src/ctc/rpc/rpc_provider.py
+-rw-r--r--   0        0        0     1128 2022-11-23 19:36:31.146057 checkthechain-0.3.5/src/ctc/rpc/rpc_registry.py
+-rw-r--r--   0        0        0       86 2023-04-29 02:54:07.448132 checkthechain-0.3.5/src/ctc/rpc/rpc_request/__init__.py
+-rw-r--r--   0        0        0     4730 2023-04-29 00:11:33.888738 checkthechain-0.3.5/src/ctc/rpc/rpc_request/request_async.py
+-rw-r--r--   0        0        0     4620 2023-04-29 02:58:16.903919 checkthechain-0.3.5/src/ctc/rpc/rpc_request/request_sync.py
+-rw-r--r--   0        0        0     4602 2023-06-02 23:42:32.086805 checkthechain-0.3.5/src/ctc/rpc/rpc_request/request_utils.py
+-rw-r--r--   0        0        0     3688 2023-03-04 19:50:23.524532 checkthechain-0.3.5/src/ctc/rpc/rpc_spec.py
+-rw-r--r--   0        0        0      102 2023-02-26 18:21:07.005328 checkthechain-0.3.5/src/ctc/spec/__init__.py
+-rw-r--r--   0        0        0      126 2022-11-23 19:36:31.146419 checkthechain-0.3.5/src/ctc/spec/exceptions/__init__.py
+-rw-r--r--   0        0        0       85 2022-11-23 19:36:31.146519 checkthechain-0.3.5/src/ctc/spec/exceptions/abi_exceptions.py
+-rw-r--r--   0        0        0      230 2023-04-17 00:04:51.283975 checkthechain-0.3.5/src/ctc/spec/exceptions/config_exceptions.py
+-rw-r--r--   0        0        0       87 2022-11-23 19:36:31.146696 checkthechain-0.3.5/src/ctc/spec/exceptions/oracle_exceptions.py
+-rw-r--r--   0        0        0      131 2022-11-23 19:36:31.146783 checkthechain-0.3.5/src/ctc/spec/exceptions/rpc_exceptions.py
+-rw-r--r--   0        0        0      487 2022-11-23 19:36:31.146870 checkthechain-0.3.5/src/ctc/spec/formatting.py
+-rw-r--r--   0        0        0     4620 2023-04-12 16:44:13.479488 checkthechain-0.3.5/src/ctc/spec/typedata.py
+-rw-r--r--   0        0        0      704 2023-02-26 18:21:07.005950 checkthechain-0.3.5/src/ctc/spec/typedefs/__init__.py
+-rw-r--r--   0        0        0     2116 2023-04-17 01:15:16.387519 checkthechain-0.3.5/src/ctc/spec/typedefs/abi_types.py
+-rw-r--r--   0        0        0     1012 2023-04-15 07:13:56.749794 checkthechain-0.3.5/src/ctc/spec/typedefs/address_types.py
+-rw-r--r--   0        0        0      948 2022-11-23 19:36:31.147255 checkthechain-0.3.5/src/ctc/spec/typedefs/binary_types.py
+-rw-r--r--   0        0        0     2239 2023-02-26 18:21:07.006211 checkthechain-0.3.5/src/ctc/spec/typedefs/block_types.py
+-rw-r--r--   0        0        0     2019 2023-04-17 01:15:50.282375 checkthechain-0.3.5/src/ctc/spec/typedefs/config_types.py
+-rw-r--r--   0        0        0      154 2023-02-26 18:21:07.006635 checkthechain-0.3.5/src/ctc/spec/typedefs/consensus_types.py
+-rw-r--r--   0        0        0     1571 2023-04-12 00:25:44.366208 checkthechain-0.3.5/src/ctc/spec/typedefs/context_types.py
+-rw-r--r--   0        0        0     1150 2023-04-17 01:34:02.808903 checkthechain-0.3.5/src/ctc/spec/typedefs/data_source_types.py
+-rw-r--r--   0        0        0      752 2023-02-26 18:21:07.007297 checkthechain-0.3.5/src/ctc/spec/typedefs/db_types.py
+-rw-r--r--   0        0        0      539 2023-04-10 06:29:29.191082 checkthechain-0.3.5/src/ctc/spec/typedefs/defi_types.py
+-rw-r--r--   0        0        0     1178 2023-04-17 01:14:53.735415 checkthechain-0.3.5/src/ctc/spec/typedefs/event_types.py
+-rw-r--r--   0        0        0      971 2023-04-13 02:34:03.315850 checkthechain-0.3.5/src/ctc/spec/typedefs/external_types.py
+-rw-r--r--   0        0        0      728 2023-02-26 18:21:07.007839 checkthechain-0.3.5/src/ctc/spec/typedefs/log_types.py
+-rw-r--r--   0        0        0      300 2023-04-17 01:28:53.685750 checkthechain-0.3.5/src/ctc/spec/typedefs/network_types.py
+-rw-r--r--   0        0        0      165 2022-11-23 19:36:31.147653 checkthechain-0.3.5/src/ctc/spec/typedefs/number_types.py
+-rw-r--r--   0        0        0     2178 2023-03-24 20:18:53.548764 checkthechain-0.3.5/src/ctc/spec/typedefs/rpc_types.py
+-rw-r--r--   0        0        0      671 2022-11-23 19:36:31.147834 checkthechain-0.3.5/src/ctc/spec/typedefs/storage_types.py
+-rw-r--r--   0        0        0     4523 2023-03-04 19:50:23.525113 checkthechain-0.3.5/src/ctc/spec/typedefs/trace_types.py
+-rw-r--r--   0        0        0     4519 2023-04-17 01:29:16.409479 checkthechain-0.3.5/src/ctc/spec/typedefs/transaction_types.py
+-rw-r--r--   0        0        0      129 2023-04-17 00:26:49.657179 checkthechain-0.3.5/src/ctc/spec/typeguards/__init__.py
+-rw-r--r--   0        0        0     1637 2022-11-23 19:36:31.148153 checkthechain-0.3.5/src/ctc/spec/typeguards/binary_typeguards.py
+-rw-r--r--   0        0        0     1708 2022-11-23 19:36:31.148252 checkthechain-0.3.5/src/ctc/spec/typeguards/block_typeguards.py
+-rw-r--r--   0        0        0      289 2023-02-26 20:15:07.427239 checkthechain-0.3.5/src/ctc/spec/typeguards/db_typeguards.py
+-rw-r--r--   0        0        0     1422 2023-04-11 15:03:04.546469 checkthechain-0.3.5/src/ctc/spec/typeguards/external_typeguards.py
+-rw-r--r--   0        0        0        0 2022-11-23 19:36:31.148387 checkthechain-0.3.5/src/ctc/toolbox/__init__.py
+-rw-r--r--   0        0        0     1441 2022-11-23 19:36:31.152899 checkthechain-0.3.5/src/ctc/toolbox/nested_utils.py
+-rw-r--r--   0        0        0     3258 2023-04-15 07:19:21.326943 checkthechain-0.3.5/src/ctc/toolbox/optimize_utils.py
+-rw-r--r--   0        0        0      175 2023-04-24 06:28:07.927137 checkthechain-0.3.5/src/ctc/toolbox/pl_utils/__init__.py
+-rw-r--r--   0        0        0     2464 2023-04-11 15:01:28.142423 checkthechain-0.3.5/src/ctc/toolbox/pl_utils/binary_utils.py
+-rw-r--r--   0        0        0     1002 2023-04-11 15:00:27.569336 checkthechain-0.3.5/src/ctc/toolbox/pl_utils/concat_utils.py
+-rw-r--r--   0        0        0     2638 2023-04-24 06:28:56.069741 checkthechain-0.3.5/src/ctc/toolbox/pl_utils/file_utils.py
+-rw-r--r--   0        0        0     3562 2023-05-30 06:46:30.793034 checkthechain-0.3.5/src/ctc/toolbox/pl_utils/interpolate_utils.py
+-rw-r--r--   0        0        0    13676 2023-04-24 18:32:50.650896 checkthechain-0.3.5/src/ctc/toolbox/pl_utils/partition_utils.py
+-rw-r--r--   0        0        0     7632 2023-05-03 17:48:02.702127 checkthechain-0.3.5/src/ctc/toolbox/pl_utils/summary_utils.py
+-rw-r--r--   0        0        0     3512 2023-02-26 18:21:07.014557 checkthechain-0.3.5/src/ctc/toolbox/plot_utils.py
+-rw-r--r--   0        0        0     8876 2023-03-04 19:50:23.527332 checkthechain-0.3.5/src/ctc/toolbox/range_utils.py
+-rw-r--r--   0        0        0     9045 2022-11-23 19:36:31.153915 checkthechain-0.3.5/src/ctc/toolbox/search_utils.py
+-rw-r--r--   0        0        0      719 2023-02-27 08:14:19.899656 checkthechain-0.3.5/tests/conftest.py
+-rw-r--r--   0        0        0    20988 2022-11-23 19:36:31.154352 checkthechain-0.3.5/tests/ctc/binary/.hypothesis/unicode_data/13.0.0/charmap.json.gz
+-rw-r--r--   0        0        0      789 2022-11-23 19:36:31.154466 checkthechain-0.3.5/tests/ctc/binary/test_eip712.py
+-rw-r--r--   0        0        0     1224 2022-11-23 19:36:31.154549 checkthechain-0.3.5/tests/ctc/binary/test_format_utils.py
+-rw-r--r--   0        0        0      795 2022-11-23 19:36:31.154622 checkthechain-0.3.5/tests/ctc/binary/test_hash_utils.py
+-rw-r--r--   0        0        0     3946 2023-04-11 17:17:48.856155 checkthechain-0.3.5/tests/ctc/binary/test_rlp_encoding.py
+-rw-r--r--   0        0        0     4888 2022-11-23 19:36:31.154783 checkthechain-0.3.5/tests/ctc/binary/test_signatures.py
+-rw-r--r--   0        0        0     1702 2022-11-23 19:36:31.154907 checkthechain-0.3.5/tests/ctc/cli/test_cli_args.py
+-rw-r--r--   0        0        0     3589 2022-11-23 19:36:31.155012 checkthechain-0.3.5/tests/ctc/cli/test_cli_subcommands.py
+-rw-r--r--   0        0        0    16961 2023-02-26 18:21:07.015169 checkthechain-0.3.5/tests/ctc/config/contexts/test_cache_contexts.py
+-rw-r--r--   0        0        0     5248 2023-04-12 02:20:12.521865 checkthechain-0.3.5/tests/ctc/config/contexts/test_network_contexts.py
+-rw-r--r--   0        0        0      620 2022-11-23 19:36:31.155162 checkthechain-0.3.5/tests/ctc/config/test_config_defaults.py
+-rw-r--r--   0        0        0     4545 2023-04-26 23:49:26.324218 checkthechain-0.3.5/tests/ctc/config/test_config_validators.py
+-rw-r--r--   0        0        0     9776 2023-04-11 22:11:40.166308 checkthechain-0.3.5/tests/ctc/config/test_setup.py
+-rw-r--r--   0        0        0     3387 2023-04-12 02:19:52.771416 checkthechain-0.3.5/tests/ctc/db/db_crud/test_db_block_timestamps.py
+-rw-r--r--   0        0        0     5624 2023-04-12 02:23:22.803870 checkthechain-0.3.5/tests/ctc/db/db_crud/test_db_blocks.py
+-rw-r--r--   0        0        0     2624 2023-04-12 02:19:46.343714 checkthechain-0.3.5/tests/ctc/db/db_crud/test_db_contract_abis.py
+-rw-r--r--   0        0        0     1906 2023-04-12 02:23:17.026530 checkthechain-0.3.5/tests/ctc/db/db_crud/test_db_contract_creation.py
+-rw-r--r--   0        0        0     3295 2023-04-12 02:19:42.769384 checkthechain-0.3.5/tests/ctc/db/db_crud/test_db_erc20_metadata.py
+-rw-r--r--   0        0        0      446 2022-11-23 19:36:31.155877 checkthechain-0.3.5/tests/ctc/db/db_schemas.py
+-rw-r--r--   0        0        0     1081 2023-02-27 08:07:49.692060 checkthechain-0.3.5/tests/ctc/db/dba_utils.py
+-rw-r--r--   0        0        0    11873 2023-04-14 23:05:20.037248 checkthechain-0.3.5/tests/ctc/db/test_crud_problems.py
+-rw-r--r--   0        0        0    20988 2022-11-23 19:36:31.156314 checkthechain-0.3.5/tests/ctc/directory/.hypothesis/unicode_data/13.0.0/charmap.json.gz
+-rw-r--r--   0        0        0     1104 2023-04-17 00:07:23.260049 checkthechain-0.3.5/tests/ctc/directory/test_directory_networks.py
+-rw-r--r--   0        0        0      588 2022-11-23 19:36:31.156484 checkthechain-0.3.5/tests/ctc/directory/test_directory_tokens.py
+-rw-r--r--   0        0        0     1322 2022-11-23 19:36:31.156621 checkthechain-0.3.5/tests/ctc/docs/test_readme_examples.py
+-rw-r--r--   0        0        0    20988 2022-11-23 19:36:31.156862 checkthechain-0.3.5/tests/ctc/evm/.hypothesis/unicode_data/13.0.0/charmap.json.gz
+-rw-r--r--   0        0        0     3757 2022-11-23 19:36:31.156975 checkthechain-0.3.5/tests/ctc/evm/test_address_utils.py
+-rw-r--r--   0        0        0     2687 2023-02-26 18:21:07.018040 checkthechain-0.3.5/tests/ctc/evm/test_block_utils.py
+-rw-r--r--   0        0        0      514 2023-04-12 04:51:28.445072 checkthechain-0.3.5/tests/ctc/evm/test_erc20_utils/test_erc20_events.py
+-rw-r--r--   0        0        0      588 2022-11-23 19:36:31.157327 checkthechain-0.3.5/tests/ctc/evm/test_erc20_utils/test_erc20_metadata.py
+-rw-r--r--   0        0        0      650 2022-11-23 19:36:31.157422 checkthechain-0.3.5/tests/ctc/evm/test_erc20_utils/test_erc20_state.py
+-rw-r--r--   0        0        0        0 2023-02-26 18:21:07.018238 checkthechain-0.3.5/tests/ctc/evm/test_erc4626_utils/__init__.py
+-rw-r--r--   0        0        0      981 2023-02-26 18:21:07.018338 checkthechain-0.3.5/tests/ctc/evm/test_erc4626_utils/test_erc4626_events.py
+-rw-r--r--   0        0        0     1085 2023-02-26 18:21:07.018415 checkthechain-0.3.5/tests/ctc/evm/test_erc4626_utils/test_erc4626_metadata.py
+-rw-r--r--   0        0        0     2429 2023-02-26 18:21:07.018492 checkthechain-0.3.5/tests/ctc/evm/test_erc4626_utils/test_erc4626_normalize.py
+-rw-r--r--   0        0        0    10489 2023-02-26 18:21:07.018576 checkthechain-0.3.5/tests/ctc/evm/test_erc4626_utils/test_erc4626_state.py
+-rw-r--r--   0        0        0      300 2023-02-26 18:21:07.018842 checkthechain-0.3.5/tests/ctc/evm/test_eth_utils.py
+-rw-r--r--   0        0        0      714 2023-04-12 04:52:01.852764 checkthechain-0.3.5/tests/ctc/evm/test_event_utils.py
+-rw-r--r--   0        0        0     6573 2023-04-12 04:44:35.718866 checkthechain-0.3.5/tests/ctc/evm/test_event_utils_new.py
+-rw-r--r--   0        0        0    20988 2022-11-23 19:36:31.158160 checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/.hypothesis/unicode_data/13.0.0/charmap.json.gz
+-rw-r--r--   0        0        0     1690 2022-11-23 19:36:31.158245 checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_blocks.py
+-rw-r--r--   0        0        0     2025 2023-04-12 18:13:33.792410 checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_logs.py
+-rw-r--r--   0        0        0     1065 2022-11-23 19:36:31.158425 checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_node.py
+-rw-r--r--   0        0        0     5693 2022-11-23 19:36:31.158531 checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_state.py
+-rw-r--r--   0        0        0      325 2023-02-26 18:21:07.019547 checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_submission.py
+-rw-r--r--   0        0        0     2185 2022-11-23 19:36:31.158726 checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_transactions.py
+-rw-r--r--   0        0        0     3751 2023-04-12 18:09:08.234614 checkthechain-0.3.5/tests/ctc/evm/test_transaction_utils/test_transaction_utils.py
+-rw-r--r--   0        0        0      915 2022-11-23 19:36:31.159046 checkthechain-0.3.5/tests/ctc/protocols/balancer_utils/test_balancer_utils.py
+-rw-r--r--   0        0        0     3367 2023-04-12 02:19:29.511661 checkthechain-0.3.5/tests/ctc/protocols/chainlink_utils/test_chainlink_db.py
+-rw-r--r--   0        0        0     2855 2023-04-27 22:25:08.354233 checkthechain-0.3.5/tests/ctc/protocols/fourbyte_utils/test_fourbyte_db.py
+-rw-r--r--   0        0        0      668 2022-11-23 19:36:31.159439 checkthechain-0.3.5/tests/ctc/protocols/uniswap_v2_utils/test_uniswap_queries.py
+-rw-r--r--   0        0        0     1483 2023-02-26 18:21:07.020336 checkthechain-0.3.5/tests/ctc/spec/test_typedata.py
+-rw-r--r--   0        0        0      867 2023-02-26 18:21:07.020613 checkthechain-0.3.5/tests/ctc/spec/test_typedefs.py
+-rw-r--r--   0        0        0    15225 2023-04-12 19:52:25.910305 checkthechain-0.3.5/tests/ctc/test_code.py
+-rw-r--r--   0        0        0     2008 2023-04-15 22:53:54.067041 checkthechain-0.3.5/tests/ctc/test_config.py
+-rw-r--r--   0        0        0      688 2023-04-15 22:49:32.487864 checkthechain-0.3.5/tests/ctc/toolbox/defi_utils/defi_directory.py
+-rw-r--r--   0        0        0     4168 2023-04-15 22:49:37.457470 checkthechain-0.3.5/tests/ctc/toolbox/defi_utils/dex_utils.py
+-rw-r--r--   0        0        0     5333 2023-04-15 22:49:24.672815 checkthechain-0.3.5/tests/ctc/toolbox/test_amm_utils.py
+-rw-r--r--   0        0        0     6329 2023-02-26 18:21:07.020999 checkthechain-0.3.5/tests/ctc/toolbox/test_chunk_utils.py
+-rw-r--r--   0        0        0      651 2022-11-23 19:36:31.160315 checkthechain-0.3.5/tests/ctc/toolbox/test_feed_utils.py
+-rw-r--r--   0        0        0     4425 2023-03-04 18:28:55.366320 checkthechain-0.3.5/tests/ctc/toolbox/test_range_utils.py
+-rwxr-xr-x   0        0        0      231 2022-11-23 19:36:31.160379 checkthechain-0.3.5/tests/run_type_checks.sh
+-rw-r--r--   0        0        0     9763 1970-01-01 00:00:00.000000 checkthechain-0.3.5/PKG-INFO
```

### Comparing `checkthechain-0.3.4/CHANGELOG.md` & `checkthechain-0.3.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/CONTRIBUTING.md` & `checkthechain-0.3.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/LICENSE-APACHE` & `checkthechain-0.3.5/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/LICENSE-MIT` & `checkthechain-0.3.5/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/README.md` & `checkthechain-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/docs/contributing_guides/adding_config_keys.md` & `checkthechain-0.3.5/docs/contributing_guides/adding_config_keys.md`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/docs/contributing_guides/adding_db_caches.md` & `checkthechain-0.3.5/docs/contributing_guides/adding_db_caches.md`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/pyproject.toml` & `checkthechain-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -46,25 +46,24 @@
     # data science
     'numpy >=1.19.0, <1.24',
     'polars >=0.17.3, <0.18',
     'pyarrow >=12.0.0, <13',
     #
     # io dependencies
     'aiohttp >=3.7.4, <4',
-    'connectorx==0.3.2a5',
     'loguru >=0.5.3, <0.7',
     'msgspec >=0.14.1, <0.15',
     'orjson >=3.7.9, <4',
     'requests >=2.20.0, <3',
     'toml >=0.10.2, <0.11',
     #
     # tool suite
     'toolcli >=0.6.13, <0.7',
     'toolconf >=0.1.2, <0.2',
-    'toolsql >=0.6.0, <0.7',
+    'toolsql >=0.6.1, <0.7',
     'toolstr >=0.9.3, <0.10',
     'tooltime >=0.2.10, <0.3',
     #
     # EVM dependencies
     'pycryptodome >=3.9.1, <4',  # for keccak()
     'eth_abi_lite >=3.2.0, <4',  # for abi encoding
     'idna >=2.10, <4',  # ENS resolution
```

### Comparing `checkthechain-0.3.4/src/ctc/__init__.py` & `checkthechain-0.3.5/src/ctc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ctc is a tool for collecting and processing historical EVM data"""
 
 from .evm import *
 
 
-__version__ = '0.3.4'
+__version__ = '0.3.5'
 
 
 def _clean_package_imports() -> None:
     """remove deep nested modules from ctc namespace"""
 
     import sys
```

### Comparing `checkthechain-0.3.4/src/ctc/cli/cli_run.py` & `checkthechain-0.3.5/src/ctc/cli/cli_run.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_alias_utils.py` & `checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_alias_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_charset_utils.py` & `checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_charset_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_color_utils.py` & `checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_color_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_execution_utils.py` & `checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_execution_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_output_utils.py` & `checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_output_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/cli_utils/cli_parse_utils.py` & `checkthechain-0.3.5/src/ctc/cli/cli_utils/cli_parse_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/aliases_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/aliases_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/chains_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/chains_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/charset_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/charset_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/color_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/color_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/config/edit_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/config/edit_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/config_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/config_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/db/create_tables_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/db/create_tables_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/db/drop_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/db/drop_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/db/status_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/db/status_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/log_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/log_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/admin/setup_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/admin/setup_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/compute/checksum_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/compute/checksum_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/compute/create_address_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/compute/create_address_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/compute/decode_call_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/compute/decode_call_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/compute/decode_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/compute/decode_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/compute/encode_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/compute/encode_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/compute/hex_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/compute/hex_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/compute/keccak_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/compute/keccak_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/compute/limits_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/compute/limits_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/compute/rlp_encode.py` & `checkthechain-0.3.5/src/ctc/cli/commands/compute/rlp_encode.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/compute/selector_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/compute/selector_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/abi_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/abi_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/abi_diff_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/abi_diff_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/address_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/address_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/address_txs_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/address_txs_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/block_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/block_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/blocks_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/blocks_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/bytecode_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/bytecode_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/call_all_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/call_all_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/call_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/call_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/calls_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/calls_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/chain_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/chain_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/decompile_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/decompile_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/dex/chart_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/dex/chart_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/dex/pool_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/dex/pool_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/dex/pools_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/dex/pools_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/dex/trades_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/dex/trades_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/erc20/balance_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/erc20/balance_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/erc20/balances_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/erc20/balances_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/erc20/transfers_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/erc20/transfers_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/erc20_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/erc20_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/eth/balance_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/eth/balance_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/eth/balances_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/eth/balances_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/events_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/events_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/gas_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/gas_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/proxy_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/proxy_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/proxy_register_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/proxy_register_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/storage_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/storage_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/symbol_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/symbol_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/timestamp_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/timestamp_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/data/tx_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/data/tx_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/cli/commands/root_command.py` & `checkthechain-0.3.5/src/ctc/cli/commands/root_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/config_defaults.py` & `checkthechain-0.3.5/src/ctc/config/config_defaults.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/config_env_vars.py` & `checkthechain-0.3.5/src/ctc/config/config_env_vars.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/config_overrides.py` & `checkthechain-0.3.5/src/ctc/config/config_overrides.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/config_read.py` & `checkthechain-0.3.5/src/ctc/config/config_read.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/config_validate.py` & `checkthechain-0.3.5/src/ctc/config/config_validate.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/config_values.py` & `checkthechain-0.3.5/src/ctc/config/config_values.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/config_write.py` & `checkthechain-0.3.5/src/ctc/config/config_write.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/context_utils/context_caches.py` & `checkthechain-0.3.5/src/ctc/config/context_utils/context_caches.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/context_utils/context_crud.py` & `checkthechain-0.3.5/src/ctc/config/context_utils/context_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/context_utils/context_sources.py` & `checkthechain-0.3.5/src/ctc/config/context_utils/context_sources.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/setup_utils/default_data/default_erc20s.py` & `checkthechain-0.3.5/src/ctc/config/setup_utils/default_data/default_erc20s.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/setup_utils/main_setup.py` & `checkthechain-0.3.5/src/ctc/config/setup_utils/main_setup.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/setup_utils/setup_io.py` & `checkthechain-0.3.5/src/ctc/config/setup_utils/setup_io.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/setup_utils/stages/alias_setup.py` & `checkthechain-0.3.5/src/ctc/config/setup_utils/stages/alias_setup.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/setup_utils/stages/cli_setup.py` & `checkthechain-0.3.5/src/ctc/config/setup_utils/stages/cli_setup.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/setup_utils/stages/data_dir_setup.py` & `checkthechain-0.3.5/src/ctc/config/setup_utils/stages/data_dir_setup.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/setup_utils/stages/db_setup.py` & `checkthechain-0.3.5/src/ctc/config/setup_utils/stages/db_setup.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/setup_utils/stages/network_setup.py` & `checkthechain-0.3.5/src/ctc/config/setup_utils/stages/network_setup.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/upgrade_utils/config_upgrade.py` & `checkthechain-0.3.5/src/ctc/config/upgrade_utils/config_upgrade.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ]:
     return {
         '0.2.': upgrade__0_2_0__to__0_3_0,
         '0.3.0': upgrade__0_3_0__to__0_3_1,
         '0.3.1': upgrade__0_3_1__to__0_3_2,
         '0.3.2': upgrade__0_3_2__to__0_3_3,
         '0.3.3': upgrade__0_3_3__to__0_3_4,
+        '0.3.4': upgrade__0_3_4__to__0_3_5,
     }
 
 
 def upgrade_config(
     old_config: typing.Mapping[typing.Any, typing.Any]
 ) -> typing.MutableMapping[str, typing.Any]:
     """upgrade config to latest version as much as possible"""
@@ -205,14 +206,22 @@
         provider.setdefault('disable_batch_requests', False)
     for network in upgraded['networks'].values():
         if network['name'] == 'mainnet':
             network['name'] = 'ethereum'
     return upgraded
 
 
+def upgrade__0_3_4__to__0_3_5(
+    old_config: typing.MutableMapping[typing.Any, typing.Any]
+) -> typing.MutableMapping[typing.Any, typing.Any]:
+    upgraded = dict(old_config)
+    upgraded['config_spec_version'] = '0.3.5'
+    return upgraded
+
+
 def omit_extra_version_data(version: str) -> str:
     for substr in ['a', 'b', 'rc']:
         if substr in version:
             index = version.index(substr)
             version = version[:index]
     return version
```

### Comparing `checkthechain-0.3.4/src/ctc/config/upgrade_utils/data_dir_versioning.py` & `checkthechain-0.3.5/src/ctc/config/upgrade_utils/data_dir_versioning.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/upgrade_utils/legacy_types.py` & `checkthechain-0.3.5/src/ctc/config/upgrade_utils/legacy_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/config/upgrade_utils/version_utils.py` & `checkthechain-0.3.5/src/ctc/config/upgrade_utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/datasets/extract_blocks_and_transactions.py` & `checkthechain-0.3.5/src/ctc/datasets/extract_blocks_and_transactions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/datasets/extract_erc20_transfers.py` & `checkthechain-0.3.5/src/ctc/datasets/extract_erc20_transfers.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/connect_utils.py` & `checkthechain-0.3.5/src/ctc/db/connect_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/intake_utils.py` & `checkthechain-0.3.5/src/ctc/db/intake_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/management/active_utils.py` & `checkthechain-0.3.5/src/ctc/db/management/active_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/management/dba_utils.py` & `checkthechain-0.3.5/src/ctc/db/management/dba_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/management/reorg_utils.py` & `checkthechain-0.3.5/src/ctc/db/management/reorg_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/management/version_utils.py` & `checkthechain-0.3.5/src/ctc/db/management/version_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/query_utils.py` & `checkthechain-0.3.5/src/ctc/db/query_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schema_utils.py` & `checkthechain-0.3.5/src/ctc/db/schema_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/block_gas_stats/block_gas_stats_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/block_gas_stats/block_gas_stats_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/erc20_state/erc20_state_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/erc20_state/erc20_state_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/protocol_schemas/fourbyte_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/protocol_schemas/fourbyte_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/__upcoming__/protocol_schemas/fuse_pools_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/__upcoming__/protocol_schemas/fuse_pools_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/block_gas/block_gas_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/block_gas/block_gas_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/block_gas/block_gas_statements.py` & `checkthechain-0.3.5/src/ctc/db/schemas/block_gas/block_gas_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/block_timestamps_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/block_timestamps_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/block_timestamps_statements.py` & `checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/block_timestamps_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_queries.py` & `checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_search.py` & `checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_search.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_statements.py` & `checkthechain-0.3.5/src/ctc/db/schemas/block_timestamps/multischema_block_timestamps_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/blocks/blocks_intake.py` & `checkthechain-0.3.5/src/ctc/db/schemas/blocks/blocks_intake.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/blocks/blocks_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/blocks/blocks_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/blocks/blocks_statements.py` & `checkthechain-0.3.5/src/ctc/db/schemas/blocks/blocks_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/contract_abis/contract_abis_intake.py` & `checkthechain-0.3.5/src/ctc/db/schemas/contract_abis/contract_abis_intake.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/contract_abis/contract_abis_statements.py` & `checkthechain-0.3.5/src/ctc/db/schemas/contract_abis/contract_abis_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_intake.py` & `checkthechain-0.3.5/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_intake.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_statements.py` & `checkthechain-0.3.5/src/ctc/db/schemas/contract_creation_blocks/contract_creation_blocks_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/dex_pools/dex_pools_intake.py` & `checkthechain-0.3.5/src/ctc/db/schemas/dex_pools/dex_pools_intake.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/dex_pools/dex_pools_queries.py` & `checkthechain-0.3.5/src/ctc/db/schemas/dex_pools/dex_pools_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/dex_pools/dex_pools_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/dex_pools/dex_pools_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/dex_pools/dex_pools_statements.py` & `checkthechain-0.3.5/src/ctc/db/schemas/dex_pools/dex_pools_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/erc20_metadata/erc20_metadata_intake.py` & `checkthechain-0.3.5/src/ctc/db/schemas/erc20_metadata/erc20_metadata_intake.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/erc20_metadata/erc20_metadata_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/erc20_metadata/erc20_metadata_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/erc20_metadata/erc20_metadata_statements.py` & `checkthechain-0.3.5/src/ctc/db/schemas/erc20_metadata/erc20_metadata_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/events/events_intake.py` & `checkthechain-0.3.5/src/ctc/db/schemas/events/events_intake.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/events/events_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/events/events_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/events/events_statements.py` & `checkthechain-0.3.5/src/ctc/db/schemas/events/events_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_intake.py` & `checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_intake.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_queries.py` & `checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_schema_defs.py` & `checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_statements/composite_block_transactions.py` & `checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_statements/composite_block_transactions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_statements/table_block_transaction_queries.py` & `checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_statements/table_block_transaction_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/db/schemas/transactions/transactions_statements/table_transactions.py` & `checkthechain-0.3.5/src/ctc/db/schemas/transactions/transactions_statements/table_transactions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/cex_utils.py` & `checkthechain-0.3.5/src/ctc/defi/cex_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/amm_spec.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/amm_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_liquidity.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_liquidity.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_spec.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_summary.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_trade.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/amm_utils/cpmm/cpmm_trade.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_class.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_class.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_class_utils.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_class_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_directory.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_directory.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_functions/dex_balance_functions.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_functions/dex_balance_functions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_functions/dex_metadata_functions.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_functions/dex_metadata_functions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_functions/dex_pools_functions.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_functions/dex_pools_functions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_functions/dex_trade_functions.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_functions/dex_trade_functions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_implementations/balancer_dex.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_implementations/balancer_dex.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_implementations/curve_dex.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_implementations/curve_dex.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_implementations/uniswap_v2_dex.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_implementations/uniswap_v2_dex.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/dex_utils/dexes/dex_implementations/uniswap_v3_dex.py` & `checkthechain-0.3.5/src/ctc/defi/dex_utils/dexes/dex_implementations/uniswap_v3_dex.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/lending_utils/lending_summary.py` & `checkthechain-0.3.5/src/ctc/defi/lending_utils/lending_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/metric_utils/ohlc_utils.py` & `checkthechain-0.3.5/src/ctc/defi/metric_utils/ohlc_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/feed_utils.py` & `checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/feed_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/twap_crud.py` & `checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/twap_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/twap_data.py` & `checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/twap_data.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/twap_data_sources.py` & `checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/twap_data_sources.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/defi/metric_utils/twap_utils/twap_filter.py` & `checkthechain-0.3.5/src/ctc/defi/metric_utils/twap_utils/twap_filter.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/abi_coding_utils.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/abi_coding_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_comparison.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_comparison.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_decompilation.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_decompilation.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_io.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_io.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_modification.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_modification.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_summary.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/contract_abi_utils/contract_abi_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/event_abi_utils/event_abi_coding.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/event_abi_utils/event_abi_coding.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/event_abi_utils/event_abi_coding_polars.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/event_abi_utils/event_abi_coding_polars.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/event_abi_utils/event_abi_parsing.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/event_abi_utils/event_abi_parsing.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/event_abi_utils/event_abi_queries.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/event_abi_utils/event_abi_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/function_abi_utils/function_abi_coding.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/function_abi_utils/function_abi_coding.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/function_abi_utils/function_abi_parsing.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/function_abi_utils/function_abi_parsing.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/abi_utils/function_abi_utils/function_abi_queries.py` & `checkthechain-0.3.5/src/ctc/evm/abi_utils/function_abi_utils/function_abi_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/address_utils/address_data.py` & `checkthechain-0.3.5/src/ctc/evm/address_utils/address_data.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/address_utils/address_resolution.py` & `checkthechain-0.3.5/src/ctc/evm/address_utils/address_resolution.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/address_utils/address_summary.py` & `checkthechain-0.3.5/src/ctc/evm/address_utils/address_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/address_utils/address_transactions.py` & `checkthechain-0.3.5/src/ctc/evm/address_utils/address_transactions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/binary_utils/format_utils.py` & `checkthechain-0.3.5/src/ctc/evm/binary_utils/format_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/binary_utils/hash_utils.py` & `checkthechain-0.3.5/src/ctc/evm/binary_utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/binary_utils/rlp_utils.py` & `checkthechain-0.3.5/src/ctc/evm/binary_utils/rlp_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/eip712_utils.py` & `checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/eip712_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/key_utils.py` & `checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/secp256k1_utils.py` & `checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/secp256k1_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/signature_creation.py` & `checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/signature_creation.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/signature_recovery.py` & `checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/signature_recovery.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/binary_utils/signature_utils/vrs_utils.py` & `checkthechain-0.3.5/src/ctc/evm/binary_utils/signature_utils/vrs_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_coding.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_coding.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_convert.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_convert.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_crud.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_gas.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_gas.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_hashes.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_hashes.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_normalize.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_normalize.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_prices.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_prices.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_samples.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_samples.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_summary.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/block_time_bins.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/block_time_bins.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/block_time_predictions.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/block_time_predictions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/block_to_timestamp.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/block_to_timestamp.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_plural.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_plural.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_range.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_range.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_search.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_search.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_singular.py` & `checkthechain-0.3.5/src/ctc/evm/block_utils/block_times/timestamp_to_block/block_time_singular.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/consensus_utils/consensus_queries.py` & `checkthechain-0.3.5/src/ctc/evm/consensus_utils/consensus_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/consensus_utils/consensus_requests.py` & `checkthechain-0.3.5/src/ctc/evm/consensus_utils/consensus_requests.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/consensus_utils/consensus_spec.py` & `checkthechain-0.3.5/src/ctc/evm/consensus_utils/consensus_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/contract_utils/contract_creations.py` & `checkthechain-0.3.5/src/ctc/evm/contract_utils/contract_creations.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/contract_utils/contract_proxies.py` & `checkthechain-0.3.5/src/ctc/evm/contract_utils/contract_proxies.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/contract_utils/contract_tests.py` & `checkthechain-0.3.5/src/ctc/evm/contract_utils/contract_tests.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_events.py` & `checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_events.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_generic.py` & `checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_generic.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_metadata.py` & `checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_normalize.py` & `checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_normalize.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_spec.py` & `checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_state.py` & `checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc20_utils/erc20_summary.py` & `checkthechain-0.3.5/src/ctc/evm/erc20_utils/erc20_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc4626_utils/erc4626_events.py` & `checkthechain-0.3.5/src/ctc/evm/erc4626_utils/erc4626_events.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc4626_utils/erc4626_metadata.py` & `checkthechain-0.3.5/src/ctc/evm/erc4626_utils/erc4626_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc4626_utils/erc4626_normalize.py` & `checkthechain-0.3.5/src/ctc/evm/erc4626_utils/erc4626_normalize.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc4626_utils/erc4626_spec.py` & `checkthechain-0.3.5/src/ctc/evm/erc4626_utils/erc4626_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc4626_utils/erc4626_state.py` & `checkthechain-0.3.5/src/ctc/evm/erc4626_utils/erc4626_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc721_utils/erc721_events.py` & `checkthechain-0.3.5/src/ctc/evm/erc721_utils/erc721_events.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc721_utils/erc721_metadata.py` & `checkthechain-0.3.5/src/ctc/evm/erc721_utils/erc721_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc721_utils/erc721_ownership.py` & `checkthechain-0.3.5/src/ctc/evm/erc721_utils/erc721_ownership.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc721_utils/erc721_spec.py` & `checkthechain-0.3.5/src/ctc/evm/erc721_utils/erc721_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/erc721_utils/erc721_state.py` & `checkthechain-0.3.5/src/ctc/evm/erc721_utils/erc721_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/eth_utils/eth_crud.py` & `checkthechain-0.3.5/src/ctc/evm/eth_utils/eth_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/event_utils/event_crud.py` & `checkthechain-0.3.5/src/ctc/evm/event_utils/event_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/event_utils/event_hybrid_queries.py` & `checkthechain-0.3.5/src/ctc/evm/event_utils/event_hybrid_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/event_utils/event_metadata.py` & `checkthechain-0.3.5/src/ctc/evm/event_utils/event_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/event_utils/event_node_utils.py` & `checkthechain-0.3.5/src/ctc/evm/event_utils/event_node_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/event_utils/event_query_utils.py` & `checkthechain-0.3.5/src/ctc/evm/event_utils/event_query_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/network_utils/network_directory.py` & `checkthechain-0.3.5/src/ctc/evm/network_utils/network_directory.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/trace_utils/specific_traces.py` & `checkthechain-0.3.5/src/ctc/evm/trace_utils/specific_traces.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/trace_utils/trace_crud.py` & `checkthechain-0.3.5/src/ctc/evm/trace_utils/trace_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/trace_utils/trace_state_diff.py` & `checkthechain-0.3.5/src/ctc/evm/trace_utils/trace_state_diff.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_convert.py` & `checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_convert.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_crud.py` & `checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_hashes.py` & `checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_hashes.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_serialize.py` & `checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_serialize.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_signatures.py` & `checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_signatures.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_summary.py` & `checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/evm/transaction_utils/transaction_types.py` & `checkthechain-0.3.5/src/ctc/evm/transaction_utils/transaction_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_interest_rates.py` & `checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_interest_rates.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_lending_pool.py` & `checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_lending_pool.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_oracle.py` & `checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_oracle.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_pool_tokens.py` & `checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_pool_tokens.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_rewards.py` & `checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_rewards.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/aave_summaries.py` & `checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/aave_summaries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/cli/aave_addresses_command.py` & `checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/cli/aave_addresses_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/aave_v2_utils/cli/aave_command.py` & `checkthechain-0.3.5/src/ctc/protocols/aave_v2_utils/cli/aave_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/balancer_utils/balancer_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/balancer_utils/balancer_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/balancer_utils/pool_metadata.py` & `checkthechain-0.3.5/src/ctc/protocols/balancer_utils/pool_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/balancer_utils/pool_plots.py` & `checkthechain-0.3.5/src/ctc/protocols/balancer_utils/pool_plots.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/balancer_utils/pool_state.py` & `checkthechain-0.3.5/src/ctc/protocols/balancer_utils/pool_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/balancer_utils/pool_summary.py` & `checkthechain-0.3.5/src/ctc/protocols/balancer_utils/pool_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/balancer_utils/pool_trades.py` & `checkthechain-0.3.5/src/ctc/protocols/balancer_utils/pool_trades.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_aggregators.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_aggregators.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/feed_composites.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/feed_composites.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/feed_data.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/feed_data.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/feed_datum.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/feed_datum.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/feed_datum_by_block.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/feed_datum_by_block.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_data/feed_events.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_data/feed_events.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_intake.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_intake.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_schema_defs.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_statements.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_db/chainlink_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_feed_metadata.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_feed_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_helpers.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_helpers.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_registry.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_registry.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/chainlink_summary.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/chainlink_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/cli/chainlink_command.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/cli/chainlink_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/chainlink_utils/cli/chainlink_ls_command.py` & `checkthechain-0.3.5/src/ctc/protocols/chainlink_utils/cli/chainlink_ls_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/cli/cg_command.py` & `checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/cli/cg_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_intake.py` & `checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_intake.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_schema_defs.py` & `checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_statements.py` & `checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/coingecko_db/coingecko_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/market_utils.py` & `checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/market_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/coingecko_utils/token_utils.py` & `checkthechain-0.3.5/src/ctc/protocols/coingecko_utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/compound_utils/compound_crud.py` & `checkthechain-0.3.5/src/ctc/protocols/compound_utils/compound_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/curve_utils/cli/curve_pools_command.py` & `checkthechain-0.3.5/src/ctc/protocols/curve_utils/cli/curve_pools_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/curve_utils/curve_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/curve_utils/curve_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/curve_utils/metapool_utils.py` & `checkthechain-0.3.5/src/ctc/protocols/curve_utils/metapool_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/curve_utils/pool_lists.py` & `checkthechain-0.3.5/src/ctc/protocols/curve_utils/pool_lists.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/curve_utils/pool_metadata.py` & `checkthechain-0.3.5/src/ctc/protocols/curve_utils/pool_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/curve_utils/pool_parameters.py` & `checkthechain-0.3.5/src/ctc/protocols/curve_utils/pool_parameters.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/curve_utils/pool_state.py` & `checkthechain-0.3.5/src/ctc/protocols/curve_utils/pool_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/exists_command.py` & `checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/exists_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/owner_command.py` & `checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/owner_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/records_command.py` & `checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/records_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/resolve_command.py` & `checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/resolve_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens/reverse_command.py` & `checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens/reverse_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/ens_utils/cli/ens_command.py` & `checkthechain-0.3.5/src/ctc/protocols/ens_utils/cli/ens_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/ens_utils/registrar.py` & `checkthechain-0.3.5/src/ctc/protocols/ens_utils/registrar.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/ens_utils/resolver.py` & `checkthechain-0.3.5/src/ctc/protocols/ens_utils/resolver.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/abi_crud.py` & `checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/abi_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/browser_utils.py` & `checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/browser_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/cli/etherscan_command.py` & `checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/cli/etherscan_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/misc_crud.py` & `checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/misc_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/etherscan_utils/url_crud.py` & `checkthechain-0.3.5/src/ctc/protocols/etherscan_utils/url_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/cli/fourbyte_build_command.py` & `checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/cli/fourbyte_build_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/cli/fourbyte_command.py` & `checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/cli/fourbyte_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_intake.py` & `checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_intake.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_schema_defs.py` & `checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_schema_defs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_statements.py` & `checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_db/fourbyte_statements.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_queries/general_queries.py` & `checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_queries/general_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_queries/remote_queries.py` & `checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_queries/remote_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_scrape.py` & `checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_scrape.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/fourbyte_utils/fourbyte_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/fourbyte_utils/fourbyte_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/g_uni_utils/crud.py` & `checkthechain-0.3.5/src/ctc/protocols/g_uni_utils/crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/README.md` & `checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/README.md`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/cli/gnosis_command.py` & `checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/cli/gnosis_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_events.py` & `checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_events.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_factory_events.py` & `checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_factory_events.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_metadata.py` & `checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_summary.py` & `checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/gnosis_utils/safe_transactions.py` & `checkthechain-0.3.5/src/ctc/protocols/gnosis_utils/safe_transactions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_chain_command.py` & `checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_chain_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_chains_command.py` & `checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_chains_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_pool_command.py` & `checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_pool_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_pools_command.py` & `checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_pools_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_protocol_command.py` & `checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_protocol_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/llama_utils/cli/llama_protocols_command.py` & `checkthechain-0.3.5/src/ctc/protocols/llama_utils/cli/llama_protocols_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/llama_utils/llama_requests.py` & `checkthechain-0.3.5/src/ctc/protocols/llama_utils/llama_requests.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/llama_utils/llama_tvls.py` & `checkthechain-0.3.5/src/ctc/protocols/llama_utils/llama_tvls.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/llama_utils/llama_yields.py` & `checkthechain-0.3.5/src/ctc/protocols/llama_utils/llama_yields.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/multicall_utils/call_utils.py` & `checkthechain-0.3.5/src/ctc/protocols/multicall_utils/call_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/multicall_utils/multicall_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/multicall_utils/multicall_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/multicall_utils/multicalls_utils.py` & `checkthechain-0.3.5/src/ctc/protocols/multicall_utils/multicalls_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/cli/rari/fuse_command.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/cli/rari/fuse_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/cli/rari/pools_command.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/cli/rari/pools_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_lens/README.md` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_lens/README.md`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_lens/lens_abis.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_lens/lens_abis.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_lens/lens_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_lens/lens_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_lens/primary_lens.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_lens/primary_lens.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/directory_metadata.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/directory_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/irm_metadata.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/irm_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/pool_metadata.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/pool_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/pool_state.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/pool_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/pool_summary.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/pool_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_metadata.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_interest.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_interest.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_price.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_price.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_usage.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_state/token_usage.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/fuse_queries/token_summary.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/fuse_queries/token_summary.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/rari_abis.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/rari_abis.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/rari_utils/summary_utils.py` & `checkthechain-0.3.5/src/ctc/protocols/rari_utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/sushi_utils/sushiswap_crud.py` & `checkthechain-0.3.5/src/ctc/protocols/sushi_utils/sushiswap_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/burns_command.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/burns_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/chart_command.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/chart_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/mints_command.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/mints_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/pool_command.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/pool_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/cli/swaps_command.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/cli/swaps_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_deltas.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_deltas.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_events.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_events.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_metadata.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_state.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v2_utils/uniswap_v2_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/pool_derived_state.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/pool_derived_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/pool_immutables.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/pool_immutables.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/pool_state.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/pool_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/quoter.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/quoter.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/contracts/tick_lens.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/contracts/tick_lens.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_crud.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_crud.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_depth.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_depth.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_swaps.py` & `checkthechain-0.3.5/src/ctc/protocols/uniswap_v3_utils/uniswap_v3_swaps.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/yearn_utils/cli/yearn_addresses_command.py` & `checkthechain-0.3.5/src/ctc/protocols/yearn_utils/cli/yearn_addresses_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/yearn_utils/cli/yearn_command.py` & `checkthechain-0.3.5/src/ctc/protocols/yearn_utils/cli/yearn_command.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_addresses.py` & `checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_addresses.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_spec.py` & `checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_strategies.py` & `checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_strategies.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_tvls.py` & `checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_tvls.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_vaults.py` & `checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_vaults.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/protocols/yearn_utils/yearn_web_api.py` & `checkthechain-0.3.5/src/ctc/protocols/yearn_utils/yearn_web_api.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_batch/rpc_batch_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_batch/rpc_batch_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_batch/rpc_batch_executors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_batch/rpc_batch_executors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_batch/rpc_batch_utils.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_batch/rpc_batch_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_block_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_block_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_dev_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_dev_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_log_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_log_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_mining_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_mining_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_node_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_node_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_state_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_state_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_submission_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_submission_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_trace_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_trace_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_transaction_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_transaction_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_constructors/rpc_whisper_constructors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_constructors/rpc_whisper_constructors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/call_trace_decoder.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/call_trace_decoder.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/create_trace_decoder.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/create_trace_decoder.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/log_decoder.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/log_decoder.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/native_transfer_decoder.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/native_transfer_decoder.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_decoders/slot_diff_decoder.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_decoders/slot_diff_decoder.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_block_digestors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_block_digestors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_dev_digestors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_dev_digestors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_log_digestors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_log_digestors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_mining_digestors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_mining_digestors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_node_digestors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_node_digestors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_state_digestors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_state_digestors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_submission_digestors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_submission_digestors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_trace_digestors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_trace_digestors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_transaction_digestors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_transaction_digestors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_digestors/rpc_whisper_digestors.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_digestors/rpc_whisper_digestors.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_block_executors_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_block_executors_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_dev_executors_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_dev_executors_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_log_executors_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_log_executors_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_mining_executors_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_mining_executors_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_node_executors_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_node_executors_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_state_executors_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_state_executors_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_submission_executors_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_submission_executors_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_trace_executors_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_trace_executors_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_transaction_executors_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_transaction_executors_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_async/rpc_whisper_executors_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_async/rpc_whisper_executors_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_block_executors_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_block_executors_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_dev_executors_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_dev_executors_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_log_executors_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_log_executors_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_mining_executors_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_mining_executors_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_node_executors_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_node_executors_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_state_executors_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_state_executors_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_submission_executors_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_submission_executors_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_trace_executors_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_trace_executors_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_transaction_executors_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_transaction_executors_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_executors_sync/rpc_whisper_executors_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_executors_sync/rpc_whisper_executors_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_format.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_format.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_lifecycle.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_lifecycle.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_logging.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_logging.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_protocols/rpc_http.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_protocols/rpc_http.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_provider.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_provider.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_registry.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_registry.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_request/request_async.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_request/request_async.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_request/request_sync.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_request/request_sync.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_request/request_utils.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_request/request_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/rpc/rpc_spec.py` & `checkthechain-0.3.5/src/ctc/rpc/rpc_spec.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedata.py` & `checkthechain-0.3.5/src/ctc/spec/typedata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/__init__.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/__init__.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/abi_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/abi_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/address_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/address_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/binary_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/binary_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/block_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/block_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/config_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/config_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/context_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/context_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/data_source_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/data_source_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/db_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/db_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/defi_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/defi_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/event_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/event_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/external_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/external_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/log_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/log_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/rpc_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/rpc_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/storage_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/storage_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/trace_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/trace_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typedefs/transaction_types.py` & `checkthechain-0.3.5/src/ctc/spec/typedefs/transaction_types.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typeguards/binary_typeguards.py` & `checkthechain-0.3.5/src/ctc/spec/typeguards/binary_typeguards.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typeguards/block_typeguards.py` & `checkthechain-0.3.5/src/ctc/spec/typeguards/block_typeguards.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/spec/typeguards/external_typeguards.py` & `checkthechain-0.3.5/src/ctc/spec/typeguards/external_typeguards.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/nested_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/nested_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/optimize_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/optimize_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/pl_utils/binary_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/pl_utils/binary_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/pl_utils/concat_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/pl_utils/concat_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/pl_utils/file_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/pl_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/pl_utils/interpolate_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/pl_utils/interpolate_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/pl_utils/partition_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/pl_utils/partition_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/pl_utils/summary_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/pl_utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/plot_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/plot_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/range_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/range_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/src/ctc/toolbox/search_utils.py` & `checkthechain-0.3.5/src/ctc/toolbox/search_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/conftest.py` & `checkthechain-0.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/binary/.hypothesis/unicode_data/13.0.0/charmap.json.gz` & `checkthechain-0.3.5/tests/ctc/binary/.hypothesis/unicode_data/13.0.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/binary/test_eip712.py` & `checkthechain-0.3.5/tests/ctc/binary/test_eip712.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/binary/test_format_utils.py` & `checkthechain-0.3.5/tests/ctc/binary/test_format_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/binary/test_hash_utils.py` & `checkthechain-0.3.5/tests/ctc/binary/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/binary/test_rlp_encoding.py` & `checkthechain-0.3.5/tests/ctc/binary/test_rlp_encoding.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/binary/test_signatures.py` & `checkthechain-0.3.5/tests/ctc/binary/test_signatures.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/cli/test_cli_args.py` & `checkthechain-0.3.5/tests/ctc/cli/test_cli_args.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/cli/test_cli_subcommands.py` & `checkthechain-0.3.5/tests/ctc/cli/test_cli_subcommands.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/config/contexts/test_cache_contexts.py` & `checkthechain-0.3.5/tests/ctc/config/contexts/test_cache_contexts.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/config/contexts/test_network_contexts.py` & `checkthechain-0.3.5/tests/ctc/config/contexts/test_network_contexts.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/config/test_config_defaults.py` & `checkthechain-0.3.5/tests/ctc/config/test_config_defaults.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/config/test_config_validators.py` & `checkthechain-0.3.5/tests/ctc/config/test_config_validators.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/config/test_setup.py` & `checkthechain-0.3.5/tests/ctc/config/test_setup.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/db/db_crud/test_db_block_timestamps.py` & `checkthechain-0.3.5/tests/ctc/db/db_crud/test_db_block_timestamps.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/db/db_crud/test_db_blocks.py` & `checkthechain-0.3.5/tests/ctc/db/db_crud/test_db_blocks.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/db/db_crud/test_db_contract_abis.py` & `checkthechain-0.3.5/tests/ctc/db/db_crud/test_db_contract_abis.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/db/db_crud/test_db_contract_creation.py` & `checkthechain-0.3.5/tests/ctc/db/db_crud/test_db_contract_creation.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/db/db_crud/test_db_erc20_metadata.py` & `checkthechain-0.3.5/tests/ctc/db/db_crud/test_db_erc20_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/db/dba_utils.py` & `checkthechain-0.3.5/tests/ctc/db/dba_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/db/test_crud_problems.py` & `checkthechain-0.3.5/tests/ctc/db/test_crud_problems.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/directory/.hypothesis/unicode_data/13.0.0/charmap.json.gz` & `checkthechain-0.3.5/tests/ctc/directory/.hypothesis/unicode_data/13.0.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/directory/test_directory_networks.py` & `checkthechain-0.3.5/tests/ctc/directory/test_directory_networks.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/directory/test_directory_tokens.py` & `checkthechain-0.3.5/tests/ctc/directory/test_directory_tokens.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/docs/test_readme_examples.py` & `checkthechain-0.3.5/tests/ctc/docs/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/.hypothesis/unicode_data/13.0.0/charmap.json.gz` & `checkthechain-0.3.5/tests/ctc/evm/.hypothesis/unicode_data/13.0.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_address_utils.py` & `checkthechain-0.3.5/tests/ctc/evm/test_address_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_block_utils.py` & `checkthechain-0.3.5/tests/ctc/evm/test_block_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_erc20_utils/test_erc20_events.py` & `checkthechain-0.3.5/tests/ctc/evm/test_erc20_utils/test_erc20_events.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_erc20_utils/test_erc20_metadata.py` & `checkthechain-0.3.5/tests/ctc/evm/test_erc20_utils/test_erc20_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_erc20_utils/test_erc20_state.py` & `checkthechain-0.3.5/tests/ctc/evm/test_erc20_utils/test_erc20_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_erc4626_utils/test_erc4626_events.py` & `checkthechain-0.3.5/tests/ctc/evm/test_erc4626_utils/test_erc4626_events.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_erc4626_utils/test_erc4626_metadata.py` & `checkthechain-0.3.5/tests/ctc/evm/test_erc4626_utils/test_erc4626_metadata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_erc4626_utils/test_erc4626_normalize.py` & `checkthechain-0.3.5/tests/ctc/evm/test_erc4626_utils/test_erc4626_normalize.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_erc4626_utils/test_erc4626_state.py` & `checkthechain-0.3.5/tests/ctc/evm/test_erc4626_utils/test_erc4626_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_event_utils.py` & `checkthechain-0.3.5/tests/ctc/evm/test_event_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_event_utils_new.py` & `checkthechain-0.3.5/tests/ctc/evm/test_event_utils_new.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/.hypothesis/unicode_data/13.0.0/charmap.json.gz` & `checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/.hypothesis/unicode_data/13.0.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_blocks.py` & `checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_blocks.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_logs.py` & `checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_logs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_node.py` & `checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_node.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_state.py` & `checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_state.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_rpc_utils/test_rpc_transactions.py` & `checkthechain-0.3.5/tests/ctc/evm/test_rpc_utils/test_rpc_transactions.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/evm/test_transaction_utils/test_transaction_utils.py` & `checkthechain-0.3.5/tests/ctc/evm/test_transaction_utils/test_transaction_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/protocols/balancer_utils/test_balancer_utils.py` & `checkthechain-0.3.5/tests/ctc/protocols/balancer_utils/test_balancer_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/protocols/chainlink_utils/test_chainlink_db.py` & `checkthechain-0.3.5/tests/ctc/protocols/chainlink_utils/test_chainlink_db.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/protocols/fourbyte_utils/test_fourbyte_db.py` & `checkthechain-0.3.5/tests/ctc/protocols/fourbyte_utils/test_fourbyte_db.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/protocols/uniswap_v2_utils/test_uniswap_queries.py` & `checkthechain-0.3.5/tests/ctc/protocols/uniswap_v2_utils/test_uniswap_queries.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/spec/test_typedata.py` & `checkthechain-0.3.5/tests/ctc/spec/test_typedata.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/spec/test_typedefs.py` & `checkthechain-0.3.5/tests/ctc/spec/test_typedefs.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/test_code.py` & `checkthechain-0.3.5/tests/ctc/test_code.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/test_config.py` & `checkthechain-0.3.5/tests/ctc/test_config.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/toolbox/defi_utils/defi_directory.py` & `checkthechain-0.3.5/tests/ctc/toolbox/defi_utils/defi_directory.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/toolbox/defi_utils/dex_utils.py` & `checkthechain-0.3.5/tests/ctc/toolbox/defi_utils/dex_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/toolbox/test_amm_utils.py` & `checkthechain-0.3.5/tests/ctc/toolbox/test_amm_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/toolbox/test_chunk_utils.py` & `checkthechain-0.3.5/tests/ctc/toolbox/test_chunk_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/toolbox/test_feed_utils.py` & `checkthechain-0.3.5/tests/ctc/toolbox/test_feed_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/tests/ctc/toolbox/test_range_utils.py` & `checkthechain-0.3.5/tests/ctc/toolbox/test_range_utils.py`

 * *Files identical despite different names*

### Comparing `checkthechain-0.3.4/PKG-INFO` & `checkthechain-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkthechain
-Version: 0.3.4
+Version: 0.3.5
 Summary: ctc is a tool for collecting and processing historical EVM data
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
@@ -21,23 +21,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: typing-extensions >=4.2.0, <5
 Requires-Dist: numpy >=1.19.0, <1.24
 Requires-Dist: polars >=0.17.3, <0.18
 Requires-Dist: pyarrow >=12.0.0, <13
 Requires-Dist: aiohttp >=3.7.4, <4
-Requires-Dist: connectorx==0.3.2a5
 Requires-Dist: loguru >=0.5.3, <0.7
 Requires-Dist: msgspec >=0.14.1, <0.15
 Requires-Dist: orjson >=3.7.9, <4
 Requires-Dist: requests >=2.20.0, <3
 Requires-Dist: toml >=0.10.2, <0.11
 Requires-Dist: toolcli >=0.6.13, <0.7
 Requires-Dist: toolconf >=0.1.2, <0.2
-Requires-Dist: toolsql >=0.6.0, <0.7
+Requires-Dist: toolsql >=0.6.1, <0.7
 Requires-Dist: toolstr >=0.9.3, <0.10
 Requires-Dist: tooltime >=0.2.10, <0.3
 Requires-Dist: pycryptodome >=3.9.1, <4
 Requires-Dist: eth_abi_lite >=3.2.0, <4
 Requires-Dist: idna >=2.10, <4
 Requires-Dist: mypy ==1.2.0 ; extra == "test"
 Requires-Dist: mypy_extensions >= 1.0.0, <1.1.0 ; extra == "test"
```

