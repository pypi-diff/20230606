# Comparing `tmp/dfktools-0.3.1.tar.gz` & `tmp/dfktools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfktools-0.3.1.tar", last modified: Mon May 29 11:40:57 2023, max compression
+gzip compressed data, was "dfktools-0.3.2.tar", last modified: Tue Jun  6 12:00:39 2023, max compression
```

## Comparing `dfktools-0.3.1.tar` & `dfktools-0.3.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.841551 dfktools-0.3.1/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 dfktools-0.3.1/LICENSE
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     9848 2023-05-29 11:40:57.841551 dfktools-0.3.1/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     8304 2023-05-20 12:43:55.000000 dfktools-0.3.1/README.md
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      563 2023-05-29 11:40:23.000000 dfktools-0.3.1/pyproject.toml
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      579 2023-05-29 11:40:57.845551 dfktools-0.3.1/setup.cfg
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.785551 dfktools-0.3.1/src/
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.805551 dfktools-0.3.1/src/dfktools/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/__init__.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.805551 dfktools-0.3.1/src/dfktools/airdrop/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-09-02 13:16:15.000000 dfktools-0.3.1/src/dfktools/airdrop/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     8867 2023-05-20 13:32:46.000000 dfktools-0.3.1/src/dfktools/airdrop/airdrop.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1320 2023-05-17 06:47:32.000000 dfktools-0.3.1/src/dfktools/airdrop_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.805551 dfktools-0.3.1/src/dfktools/alchemist/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/alchemist/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    10440 2023-05-20 13:33:08.000000 dfktools-0.3.1/src/dfktools/alchemist/alchemist.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1791 2023-05-17 06:47:32.000000 dfktools-0.3.1/src/dfktools/alchemist_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      681 2022-08-15 13:56:20.000000 dfktools-0.3.1/src/dfktools/assisting_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3706 2023-05-17 06:47:32.000000 dfktools-0.3.1/src/dfktools/auction_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.809551 dfktools-0.3.1/src/dfktools/auctions/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/auctions/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1918 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/auctions/auction.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    17481 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/auctions/auction_core.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.809551 dfktools-0.3.1/src/dfktools/auctions/hero/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/auctions/hero/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1874 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/auctions/hero/rent_auctions.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    32597 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/auctions/hero/sale_auctions.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      164 2022-12-08 06:49:54.000000 dfktools-0.3.1/src/dfktools/auctions/land.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      248 2022-12-08 06:51:07.000000 dfktools-0.3.1/src/dfktools/auctions/pet.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.809551 dfktools-0.3.1/src/dfktools/auctions/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/auctions/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      439 2022-07-17 14:24:54.000000 dfktools-0.3.1/src/dfktools/auctions/utils/utils.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.813551 dfktools-0.3.1/src/dfktools/bridge/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-18 04:09:41.000000 dfktools-0.3.1/src/dfktools/bridge/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     6047 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/bridge/dfktears_bridge.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     8688 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/bridge/hero_bridge.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1810 2023-05-17 06:47:32.000000 dfktools-0.3.1/src/dfktools/bridge_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.813551 dfktools-0.3.1/src/dfktools/consumable/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/consumable/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    12941 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/consumable/consumable.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1068 2023-05-17 06:47:32.000000 dfktools-0.3.1/src/dfktools/consumable_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.817551 dfktools-0.3.1/src/dfktools/dex/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/dex/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3084 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/dex/crystal.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5487 2023-05-17 06:28:12.000000 dfktools-0.3.1/src/dfktools/dex/erc1155.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    34859 2023-05-20 13:02:18.000000 dfktools-0.3.1/src/dfktools/dex/erc20.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    12438 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/dex/item_erc1155.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3066 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/dex/jade.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3070 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/dex/jewel.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    21910 2023-05-17 06:28:12.000000 dfktools-0.3.1/src/dfktools/dex/master_gardener.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3572 2023-05-17 06:28:12.000000 dfktools-0.3.1/src/dfktools/dex/uniswap_v2_factory.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    14189 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/dex/uniswap_v2_pair.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    18811 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/dex/uniswap_v2_router.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.817551 dfktools-0.3.1/src/dfktools/dex/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/dex/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1078 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/dex/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     4400 2023-05-17 06:49:25.000000 dfktools-0.3.1/src/dfktools/dex_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.817551 dfktools-0.3.1/src/dfktools/duel/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:15:15.000000 dfktools-0.3.1/src/dfktools/duel/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    44461 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/duel/duel.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.821551 dfktools-0.3.1/src/dfktools/duel/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:15:15.000000 dfktools-0.3.1/src/dfktools/duel/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      934 2022-09-19 15:24:02.000000 dfktools-0.3.1/src/dfktools/duel/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1798 2023-05-17 06:47:32.000000 dfktools-0.3.1/src/dfktools/duel_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1066 2022-12-08 09:31:30.000000 dfktools-0.3.1/src/dfktools/erc20_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.821551 dfktools-0.3.1/src/dfktools/genes/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/genes/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1828 2023-05-17 06:28:12.000000 dfktools-0.3.1/src/dfktools/genes/gene_science_v1.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2168 2023-05-17 06:28:11.000000 dfktools-0.3.1/src/dfktools/genes/gene_science_v2.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1885 2023-01-16 12:58:12.000000 dfktools-0.3.1/src/dfktools/genes_encode_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1423 2022-07-17 11:30:49.000000 dfktools-0.3.1/src/dfktools/genes_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.821551 dfktools-0.3.1/src/dfktools/hero/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/hero/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    85130 2023-05-24 13:11:07.000000 dfktools-0.3.1/src/dfktools/hero/hero_core.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1808 2023-05-20 14:18:48.000000 dfktools-0.3.1/src/dfktools/hero/heroes.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.821551 dfktools-0.3.1/src/dfktools/hero/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/hero/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     7937 2023-05-21 13:34:56.000000 dfktools-0.3.1/src/dfktools/hero/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2222 2023-05-21 13:28:44.000000 dfktools-0.3.1/src/dfktools/hero_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.821551 dfktools-0.3.1/src/dfktools/land/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/land/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    16757 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/land/land.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.825551 dfktools-0.3.1/src/dfktools/land/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/land/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      347 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/land/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1218 2022-12-08 07:01:50.000000 dfktools-0.3.1/src/dfktools/land_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.825551 dfktools-0.3.1/src/dfktools/meditation/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/meditation/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    32044 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/meditation/meditation.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3691 2023-05-17 06:33:36.000000 dfktools-0.3.1/src/dfktools/meditation_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.825551 dfktools-0.3.1/src/dfktools/perilous_journey/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/perilous_journey/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    10077 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/perilous_journey/perilous_journey.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3043 2023-05-21 13:28:44.000000 dfktools-0.3.1/src/dfktools/pet_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.829551 dfktools-0.3.1/src/dfktools/pets/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 13:32:00.000000 dfktools-0.3.1/src/dfktools/pets/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    13128 2023-05-17 09:17:54.000000 dfktools-0.3.1/src/dfktools/pets/exchange.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    15150 2023-05-17 09:17:54.000000 dfktools-0.3.1/src/dfktools/pets/hatchery.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    48917 2023-05-24 13:26:25.000000 dfktools-0.3.1/src/dfktools/pets/pet_core.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1479 2023-05-20 14:19:35.000000 dfktools-0.3.1/src/dfktools/pets/pets.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.829551 dfktools-0.3.1/src/dfktools/pets/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 14:45:38.000000 dfktools-0.3.1/src/dfktools/pets/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5642 2023-05-20 03:57:10.000000 dfktools-0.3.1/src/dfktools/pets/utils/utils.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.829551 dfktools-0.3.1/src/dfktools/profile/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/profile/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     7565 2023-05-17 06:28:12.000000 dfktools-0.3.1/src/dfktools/profile/profile.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    11703 2023-05-17 06:28:12.000000 dfktools-0.3.1/src/dfktools/profile/profile_v2.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      821 2023-02-02 10:29:02.000000 dfktools-0.3.1/src/dfktools/profile_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5500 2023-05-25 00:04:40.000000 dfktools-0.3.1/src/dfktools/quest_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.833551 dfktools-0.3.1/src/dfktools/quests/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/quests/__init__.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.833551 dfktools-0.3.1/src/dfktools/quests/professions/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/quests/professions/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      329 2022-12-08 06:24:10.000000 dfktools-0.3.1/src/dfktools/quests/professions/fishing.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      329 2022-12-08 06:24:41.000000 dfktools-0.3.1/src/dfktools/quests/professions/foraging.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3345 2022-12-08 07:25:12.000000 dfktools-0.3.1/src/dfktools/quests/professions/gardening.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      521 2022-12-08 06:25:47.000000 dfktools-0.3.1/src/dfktools/quests/professions/mining.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    40741 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/quests/quest_core_v1.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    32248 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/quests/quest_core_v2.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    29501 2023-05-29 11:39:28.000000 dfktools-0.3.1/src/dfktools/quests/quest_core_v3.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2479 2022-07-18 04:06:28.000000 dfktools-0.3.1/src/dfktools/quests/quest_v1.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2308 2022-09-19 15:00:40.000000 dfktools-0.3.1/src/dfktools/quests/quest_v2.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2117 2023-05-21 12:28:14.000000 dfktools-0.3.1/src/dfktools/quests/quest_v3.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.837551 dfktools-0.3.1/src/dfktools/quests/training/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/quests/training/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      259 2022-12-08 06:33:57.000000 dfktools-0.3.1/src/dfktools/quests/training/agility_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:44:01.000000 dfktools-0.3.1/src/dfktools/quests/training/dexterity_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:44:14.000000 dfktools-0.3.1/src/dfktools/quests/training/endurance_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      263 2022-12-08 06:44:28.000000 dfktools-0.3.1/src/dfktools/quests/training/intelligence_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      255 2022-12-08 06:44:45.000000 dfktools-0.3.1/src/dfktools/quests/training/luck_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:46:04.000000 dfktools-0.3.1/src/dfktools/quests/training/strength_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      259 2022-12-08 06:45:11.000000 dfktools-0.3.1/src/dfktools/quests/training/vitality_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      257 2022-12-08 06:44:57.000000 dfktools-0.3.1/src/dfktools/quests/training/wisdom_training.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.837551 dfktools-0.3.1/src/dfktools/quests/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/quests/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5519 2023-05-23 22:26:44.000000 dfktools-0.3.1/src/dfktools/quests/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    15405 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/quests/wishing_well.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.837551 dfktools-0.3.1/src/dfktools/raffle/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:27:09.000000 dfktools-0.3.1/src/dfktools/raffle/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    21612 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/raffle/raffle_master.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.837551 dfktools-0.3.1/src/dfktools/raffle/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:27:09.000000 dfktools-0.3.1/src/dfktools/raffle/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      738 2022-07-17 06:27:09.000000 dfktools-0.3.1/src/dfktools/raffle/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2219 2023-05-17 06:47:32.000000 dfktools-0.3.1/src/dfktools/raffle_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.837551 dfktools-0.3.1/src/dfktools/stone_carver/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-09-02 13:16:15.000000 dfktools-0.3.1/src/dfktools/stone_carver/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    12747 2023-05-20 13:34:51.000000 dfktools-0.3.1/src/dfktools/stone_carver/stone_carver.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1835 2023-05-17 06:47:32.000000 dfktools-0.3.1/src/dfktools/stone_carver_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.841551 dfktools-0.3.1/src/dfktools/summoning/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.1/src/dfktools/summoning/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    16129 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/summoning/assisting.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    11172 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/summoning/crystals.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    26787 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/summoning/crystals_v2.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    10930 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/summoning/serendale_assisting.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    26272 2023-05-17 09:17:55.000000 dfktools-0.3.1/src/dfktools/summoning/summoning.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2934 2023-05-17 06:33:36.000000 dfktools-0.3.1/src/dfktools/summoning_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1411 2023-05-17 06:47:32.000000 dfktools-0.3.1/src/dfktools/wishing_well_quest_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-29 11:40:57.805551 dfktools-0.3.1/src/dfktools.egg-info/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     9848 2023-05-29 11:40:57.000000 dfktools-0.3.1/src/dfktools.egg-info/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     4471 2023-05-29 11:40:57.000000 dfktools-0.3.1/src/dfktools.egg-info/SOURCES.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-05-29 11:40:57.000000 dfktools-0.3.1/src/dfktools.egg-info/dependency_links.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-05-29 11:40:57.000000 dfktools-0.3.1/src/dfktools.egg-info/requires.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        9 2023-05-29 11:40:57.000000 dfktools-0.3.1/src/dfktools.egg-info/top_level.txt
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.289310 dfktools-0.3.2/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 dfktools-0.3.2/LICENSE
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     9848 2023-06-06 12:00:39.289310 dfktools-0.3.2/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     8304 2023-05-20 12:43:55.000000 dfktools-0.3.2/README.md
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      563 2023-06-06 12:00:17.000000 dfktools-0.3.2/pyproject.toml
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      579 2023-06-06 12:00:39.289310 dfktools-0.3.2/setup.cfg
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.241310 dfktools-0.3.2/src/
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.253310 dfktools-0.3.2/src/dfktools/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/__init__.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.253310 dfktools-0.3.2/src/dfktools/airdrop/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-09-02 13:16:15.000000 dfktools-0.3.2/src/dfktools/airdrop/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     8867 2023-05-20 13:32:46.000000 dfktools-0.3.2/src/dfktools/airdrop/airdrop.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1320 2023-05-17 06:47:32.000000 dfktools-0.3.2/src/dfktools/airdrop_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.253310 dfktools-0.3.2/src/dfktools/alchemist/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/alchemist/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    10440 2023-05-20 13:33:08.000000 dfktools-0.3.2/src/dfktools/alchemist/alchemist.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1791 2023-05-17 06:47:32.000000 dfktools-0.3.2/src/dfktools/alchemist_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      681 2022-08-15 13:56:20.000000 dfktools-0.3.2/src/dfktools/assisting_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3706 2023-05-17 06:47:32.000000 dfktools-0.3.2/src/dfktools/auction_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.257310 dfktools-0.3.2/src/dfktools/auctions/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/auctions/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1918 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/auctions/auction.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    17481 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/auctions/auction_core.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.257310 dfktools-0.3.2/src/dfktools/auctions/hero/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/auctions/hero/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1874 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/auctions/hero/rent_auctions.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    32597 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/auctions/hero/sale_auctions.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      164 2022-12-08 06:49:54.000000 dfktools-0.3.2/src/dfktools/auctions/land.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      248 2022-12-08 06:51:07.000000 dfktools-0.3.2/src/dfktools/auctions/pet.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.257310 dfktools-0.3.2/src/dfktools/auctions/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/auctions/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      439 2022-07-17 14:24:54.000000 dfktools-0.3.2/src/dfktools/auctions/utils/utils.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.257310 dfktools-0.3.2/src/dfktools/bridge/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-18 04:09:41.000000 dfktools-0.3.2/src/dfktools/bridge/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     6047 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/bridge/dfktears_bridge.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     8688 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/bridge/hero_bridge.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1810 2023-05-17 06:47:32.000000 dfktools-0.3.2/src/dfktools/bridge_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.261310 dfktools-0.3.2/src/dfktools/consumable/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/consumable/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    12941 2023-06-06 11:58:52.000000 dfktools-0.3.2/src/dfktools/consumable/consumable.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1068 2023-05-17 06:47:32.000000 dfktools-0.3.2/src/dfktools/consumable_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.265310 dfktools-0.3.2/src/dfktools/dex/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/dex/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3084 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/dex/crystal.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5487 2023-05-17 06:28:12.000000 dfktools-0.3.2/src/dfktools/dex/erc1155.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    34859 2023-05-20 13:02:18.000000 dfktools-0.3.2/src/dfktools/dex/erc20.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    12438 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/dex/item_erc1155.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3066 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/dex/jade.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3070 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/dex/jewel.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    21910 2023-05-17 06:28:12.000000 dfktools-0.3.2/src/dfktools/dex/master_gardener.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3572 2023-05-17 06:28:12.000000 dfktools-0.3.2/src/dfktools/dex/uniswap_v2_factory.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    14189 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/dex/uniswap_v2_pair.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    18811 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/dex/uniswap_v2_router.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.265310 dfktools-0.3.2/src/dfktools/dex/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/dex/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1078 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/dex/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     4400 2023-05-17 06:49:25.000000 dfktools-0.3.2/src/dfktools/dex_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.265310 dfktools-0.3.2/src/dfktools/duel/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:15:15.000000 dfktools-0.3.2/src/dfktools/duel/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    44461 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/duel/duel.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.265310 dfktools-0.3.2/src/dfktools/duel/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:15:15.000000 dfktools-0.3.2/src/dfktools/duel/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      934 2022-09-19 15:24:02.000000 dfktools-0.3.2/src/dfktools/duel/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1798 2023-05-17 06:47:32.000000 dfktools-0.3.2/src/dfktools/duel_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1066 2022-12-08 09:31:30.000000 dfktools-0.3.2/src/dfktools/erc20_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.265310 dfktools-0.3.2/src/dfktools/genes/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/genes/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1828 2023-05-17 06:28:12.000000 dfktools-0.3.2/src/dfktools/genes/gene_science_v1.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2168 2023-05-17 06:28:11.000000 dfktools-0.3.2/src/dfktools/genes/gene_science_v2.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1885 2023-01-16 12:58:12.000000 dfktools-0.3.2/src/dfktools/genes_encode_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1423 2022-07-17 11:30:49.000000 dfktools-0.3.2/src/dfktools/genes_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.269310 dfktools-0.3.2/src/dfktools/hero/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/hero/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    85130 2023-05-24 13:11:07.000000 dfktools-0.3.2/src/dfktools/hero/hero_core.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1808 2023-05-20 14:18:48.000000 dfktools-0.3.2/src/dfktools/hero/heroes.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.269310 dfktools-0.3.2/src/dfktools/hero/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/hero/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     7937 2023-05-21 13:34:56.000000 dfktools-0.3.2/src/dfktools/hero/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2222 2023-05-21 13:28:44.000000 dfktools-0.3.2/src/dfktools/hero_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.269310 dfktools-0.3.2/src/dfktools/land/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/land/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    16757 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/land/land.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.269310 dfktools-0.3.2/src/dfktools/land/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/land/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      347 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/land/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1218 2022-12-08 07:01:50.000000 dfktools-0.3.2/src/dfktools/land_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.269310 dfktools-0.3.2/src/dfktools/meditation/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/meditation/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    32044 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/meditation/meditation.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3691 2023-05-17 06:33:36.000000 dfktools-0.3.2/src/dfktools/meditation_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.269310 dfktools-0.3.2/src/dfktools/perilous_journey/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/perilous_journey/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    10077 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/perilous_journey/perilous_journey.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3043 2023-05-21 13:28:44.000000 dfktools-0.3.2/src/dfktools/pet_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.273310 dfktools-0.3.2/src/dfktools/pets/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 13:32:00.000000 dfktools-0.3.2/src/dfktools/pets/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    13128 2023-05-17 09:17:54.000000 dfktools-0.3.2/src/dfktools/pets/exchange.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    15150 2023-05-17 09:17:54.000000 dfktools-0.3.2/src/dfktools/pets/hatchery.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    48917 2023-05-24 13:26:25.000000 dfktools-0.3.2/src/dfktools/pets/pet_core.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1479 2023-05-20 14:19:35.000000 dfktools-0.3.2/src/dfktools/pets/pets.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.273310 dfktools-0.3.2/src/dfktools/pets/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 14:45:38.000000 dfktools-0.3.2/src/dfktools/pets/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5642 2023-05-20 03:57:10.000000 dfktools-0.3.2/src/dfktools/pets/utils/utils.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.273310 dfktools-0.3.2/src/dfktools/profile/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/profile/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     7565 2023-05-17 06:28:12.000000 dfktools-0.3.2/src/dfktools/profile/profile.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    11703 2023-05-17 06:28:12.000000 dfktools-0.3.2/src/dfktools/profile/profile_v2.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      821 2023-02-02 10:29:02.000000 dfktools-0.3.2/src/dfktools/profile_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5500 2023-05-25 00:04:40.000000 dfktools-0.3.2/src/dfktools/quest_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.281310 dfktools-0.3.2/src/dfktools/quests/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/quests/__init__.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.281310 dfktools-0.3.2/src/dfktools/quests/professions/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/quests/professions/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      329 2022-12-08 06:24:10.000000 dfktools-0.3.2/src/dfktools/quests/professions/fishing.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      329 2022-12-08 06:24:41.000000 dfktools-0.3.2/src/dfktools/quests/professions/foraging.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3345 2022-12-08 07:25:12.000000 dfktools-0.3.2/src/dfktools/quests/professions/gardening.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      521 2022-12-08 06:25:47.000000 dfktools-0.3.2/src/dfktools/quests/professions/mining.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    40741 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/quests/quest_core_v1.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    32248 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/quests/quest_core_v2.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    29501 2023-05-29 11:39:28.000000 dfktools-0.3.2/src/dfktools/quests/quest_core_v3.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2479 2022-07-18 04:06:28.000000 dfktools-0.3.2/src/dfktools/quests/quest_v1.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2308 2022-09-19 15:00:40.000000 dfktools-0.3.2/src/dfktools/quests/quest_v2.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2117 2023-05-21 12:28:14.000000 dfktools-0.3.2/src/dfktools/quests/quest_v3.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.285310 dfktools-0.3.2/src/dfktools/quests/training/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/quests/training/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      259 2022-12-08 06:33:57.000000 dfktools-0.3.2/src/dfktools/quests/training/agility_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:44:01.000000 dfktools-0.3.2/src/dfktools/quests/training/dexterity_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:44:14.000000 dfktools-0.3.2/src/dfktools/quests/training/endurance_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      263 2022-12-08 06:44:28.000000 dfktools-0.3.2/src/dfktools/quests/training/intelligence_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      255 2022-12-08 06:44:45.000000 dfktools-0.3.2/src/dfktools/quests/training/luck_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:46:04.000000 dfktools-0.3.2/src/dfktools/quests/training/strength_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      259 2022-12-08 06:45:11.000000 dfktools-0.3.2/src/dfktools/quests/training/vitality_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      257 2022-12-08 06:44:57.000000 dfktools-0.3.2/src/dfktools/quests/training/wisdom_training.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.285310 dfktools-0.3.2/src/dfktools/quests/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/quests/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5519 2023-05-23 22:26:44.000000 dfktools-0.3.2/src/dfktools/quests/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    15405 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/quests/wishing_well.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.285310 dfktools-0.3.2/src/dfktools/raffle/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:27:09.000000 dfktools-0.3.2/src/dfktools/raffle/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    21612 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/raffle/raffle_master.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.285310 dfktools-0.3.2/src/dfktools/raffle/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:27:09.000000 dfktools-0.3.2/src/dfktools/raffle/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      738 2022-07-17 06:27:09.000000 dfktools-0.3.2/src/dfktools/raffle/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2219 2023-05-17 06:47:32.000000 dfktools-0.3.2/src/dfktools/raffle_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.285310 dfktools-0.3.2/src/dfktools/stone_carver/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-09-02 13:16:15.000000 dfktools-0.3.2/src/dfktools/stone_carver/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    12747 2023-05-20 13:34:51.000000 dfktools-0.3.2/src/dfktools/stone_carver/stone_carver.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1835 2023-05-17 06:47:32.000000 dfktools-0.3.2/src/dfktools/stone_carver_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.289310 dfktools-0.3.2/src/dfktools/summoning/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.2/src/dfktools/summoning/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    16129 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/summoning/assisting.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    11172 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/summoning/crystals.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    26787 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/summoning/crystals_v2.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    10930 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/summoning/serendale_assisting.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    26272 2023-05-17 09:17:55.000000 dfktools-0.3.2/src/dfktools/summoning/summoning.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2934 2023-05-17 06:33:36.000000 dfktools-0.3.2/src/dfktools/summoning_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1411 2023-05-17 06:47:32.000000 dfktools-0.3.2/src/dfktools/wishing_well_quest_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-06 12:00:39.253310 dfktools-0.3.2/src/dfktools.egg-info/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     9848 2023-06-06 12:00:39.000000 dfktools-0.3.2/src/dfktools.egg-info/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     4471 2023-06-06 12:00:39.000000 dfktools-0.3.2/src/dfktools.egg-info/SOURCES.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-06 12:00:39.000000 dfktools-0.3.2/src/dfktools.egg-info/dependency_links.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-06 12:00:39.000000 dfktools-0.3.2/src/dfktools.egg-info/requires.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        9 2023-06-06 12:00:39.000000 dfktools-0.3.2/src/dfktools.egg-info/top_level.txt
```

### Comparing `dfktools-0.3.1/LICENSE` & `dfktools-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/PKG-INFO` & `dfktools-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfktools
-Version: 0.3.1
+Version: 0.3.2
 Summary: A toolbox for DefiKingdoms
 Home-page: https://github.com/0rtis/dfktools
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
```

### Comparing `dfktools-0.3.1/README.md` & `dfktools-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/pyproject.toml` & `dfktools-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=57"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfktools"
 description = "A toolbox for DefiKingdoms"
 authors = [{name = "Ortis", email = "ortis@ortis.io"}]
-version = "0.3.1"
+version = "0.3.2"
 readme = "README.md"
 keywords = ["blockchain", "web3", "NFT", "etherum", "game"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Programming Language :: Python :: 3",
```

### Comparing `dfktools-0.3.1/setup.cfg` & `dfktools-0.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dfktools
-version = 0.3.1
+version = 0.3.2
 author = Ortis
 author_email = ortis@ortis.io
 description = A toolbox for DefiKingdoms
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0rtis/dfktools
 project_urls =
```

### Comparing `dfktools-0.3.1/src/dfktools/airdrop/airdrop.py` & `dfktools-0.3.2/src/dfktools/airdrop/airdrop.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/airdrop_example.py` & `dfktools-0.3.2/src/dfktools/airdrop_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/alchemist/alchemist.py` & `dfktools-0.3.2/src/dfktools/alchemist/alchemist.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/alchemist_example.py` & `dfktools-0.3.2/src/dfktools/alchemist_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/assisting_example.py` & `dfktools-0.3.2/src/dfktools/assisting_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/auction_example.py` & `dfktools-0.3.2/src/dfktools/auction_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/auctions/auction.py` & `dfktools-0.3.2/src/dfktools/auctions/auction.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/auctions/auction_core.py` & `dfktools-0.3.2/src/dfktools/auctions/auction_core.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/auctions/hero/rent_auctions.py` & `dfktools-0.3.2/src/dfktools/auctions/hero/rent_auctions.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/auctions/hero/sale_auctions.py` & `dfktools-0.3.2/src/dfktools/auctions/hero/sale_auctions.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/bridge/dfktears_bridge.py` & `dfktools-0.3.2/src/dfktools/bridge/dfktears_bridge.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/bridge/hero_bridge.py` & `dfktools-0.3.2/src/dfktools/bridge/hero_bridge.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/bridge_example.py` & `dfktools-0.3.2/src/dfktools/bridge_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/consumable/consumable.py` & `dfktools-0.3.2/src/dfktools/consumable/consumable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from web3 import Web3
 
 SERENDALE_CONTRACT_ADDRESS = "0x38e76972bd173901b5e5e43ba5cb464293b80c31"
 CRYSTALVALE_CONTRACT_ADDRESS = "0xc9A9F352Aa188f422A8f8902B547FB3E59D37210"
-SERENDALE2_CONTRACT_ADDRESS = "0x38e76972bd173901b5e5e43ba5cb464293b80c31"
+SERENDALE2_CONTRACT_ADDRESS = "0xF78cA21d7Da3227457138714F5bEd08D2604A156"
 
 ABI = '''
 	[
 		{"anonymous":false,"inputs":[{"indexed":false,"internalType":"address","name":"player","type":"address"},{"indexed":false,"internalType":"address","name":"item","type":"address"},{"indexed":false,"internalType":"uint256","name":"heroId","type":"uint256"},{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"components":[{"internalType":"uint256","name":"summonedTime","type":"uint256"},{"internalType":"uint256","name":"nextSummonTime","type":"uint256"},{"internalType":"uint256","name":"summonerId","type":"uint256"},{"internalType":"uint256","name":"assistantId","type":"uint256"},{"internalType":"uint32","name":"summons","type":"uint32"},{"internalType":"uint32","name":"maxSummons","type":"uint32"}],"internalType":"struct IHeroTypes.SummoningInfo","name":"summoningInfo","type":"tuple"},{"components":[{"internalType":"uint256","name":"statGenes","type":"uint256"},{"internalType":"uint256","name":"visualGenes","type":"uint256"},{"internalType":"enum IHeroTypes.Rarity","name":"rarity","type":"uint8"},{"internalType":"bool","name":"shiny","type":"bool"},{"internalType":"uint16","name":"generation","type":"uint16"},{"internalType":"uint32","name":"firstName","type":"uint32"},{"internalType":"uint32","name":"lastName","type":"uint32"},{"internalType":"uint8","name":"shinyStyle","type":"uint8"},{"internalType":"uint8","name":"class","type":"uint8"},{"internalType":"uint8","name":"subClass","type":"uint8"}],"internalType":"struct IHeroTypes.HeroInfo","name":"info","type":"tuple"},{"components":[{"internalType":"uint256","name":"staminaFullAt","type":"uint256"},{"internalType":"uint256","name":"hpFullAt","type":"uint256"},{"internalType":"uint256","name":"mpFullAt","type":"uint256"},{"internalType":"uint16","name":"level","type":"uint16"},{"internalType":"uint64","name":"xp","type":"uint64"},{"internalType":"address","name":"currentQuest","type":"address"},{"internalType":"uint8","name":"sp","type":"uint8"},{"internalType":"enum IHeroTypes.HeroStatus","name":"status","type":"uint8"}],"internalType":"struct IHeroTypes.HeroState","name":"state","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hp","type":"uint16"},{"internalType":"uint16","name":"mp","type":"uint16"},{"internalType":"uint16","name":"stamina","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStats","name":"stats","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hpSm","type":"uint16"},{"internalType":"uint16","name":"hpRg","type":"uint16"},{"internalType":"uint16","name":"hpLg","type":"uint16"},{"internalType":"uint16","name":"mpSm","type":"uint16"},{"internalType":"uint16","name":"mpRg","type":"uint16"},{"internalType":"uint16","name":"mpLg","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStatGrowth","name":"primaryStatGrowth","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hpSm","type":"uint16"},{"internalType":"uint16","name":"hpRg","type":"uint16"},{"internalType":"uint16","name":"hpLg","type":"uint16"},{"internalType":"uint16","name":"mpSm","type":"uint16"},{"internalType":"uint16","name":"mpRg","type":"uint16"},{"internalType":"uint16","name":"mpLg","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStatGrowth","name":"secondaryStatGrowth","type":"tuple"},{"components":[{"internalType":"uint16","name":"mining","type":"uint16"},{"internalType":"uint16","name":"gardening","type":"uint16"},{"internalType":"uint16","name":"foraging","type":"uint16"},{"internalType":"uint16","name":"fishing","type":"uint16"}],"internalType":"struct IHeroTypes.HeroProfessions","name":"professions","type":"tuple"}],"indexed":false,"internalType":"struct IHeroTypes.Hero","name":"oldHero","type":"tuple"},{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"components":[{"internalType":"uint256","name":"summonedTime","type":"uint256"},{"internalType":"uint256","name":"nextSummonTime","type":"uint256"},{"internalType":"uint256","name":"summonerId","type":"uint256"},{"internalType":"uint256","name":"assistantId","type":"uint256"},{"internalType":"uint32","name":"summons","type":"uint32"},{"internalType":"uint32","name":"maxSummons","type":"uint32"}],"internalType":"struct IHeroTypes.SummoningInfo","name":"summoningInfo","type":"tuple"},{"components":[{"internalType":"uint256","name":"statGenes","type":"uint256"},{"internalType":"uint256","name":"visualGenes","type":"uint256"},{"internalType":"enum IHeroTypes.Rarity","name":"rarity","type":"uint8"},{"internalType":"bool","name":"shiny","type":"bool"},{"internalType":"uint16","name":"generation","type":"uint16"},{"internalType":"uint32","name":"firstName","type":"uint32"},{"internalType":"uint32","name":"lastName","type":"uint32"},{"internalType":"uint8","name":"shinyStyle","type":"uint8"},{"internalType":"uint8","name":"class","type":"uint8"},{"internalType":"uint8","name":"subClass","type":"uint8"}],"internalType":"struct IHeroTypes.HeroInfo","name":"info","type":"tuple"},{"components":[{"internalType":"uint256","name":"staminaFullAt","type":"uint256"},{"internalType":"uint256","name":"hpFullAt","type":"uint256"},{"internalType":"uint256","name":"mpFullAt","type":"uint256"},{"internalType":"uint16","name":"level","type":"uint16"},{"internalType":"uint64","name":"xp","type":"uint64"},{"internalType":"address","name":"currentQuest","type":"address"},{"internalType":"uint8","name":"sp","type":"uint8"},{"internalType":"enum IHeroTypes.HeroStatus","name":"status","type":"uint8"}],"internalType":"struct IHeroTypes.HeroState","name":"state","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hp","type":"uint16"},{"internalType":"uint16","name":"mp","type":"uint16"},{"internalType":"uint16","name":"stamina","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStats","name":"stats","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hpSm","type":"uint16"},{"internalType":"uint16","name":"hpRg","type":"uint16"},{"internalType":"uint16","name":"hpLg","type":"uint16"},{"internalType":"uint16","name":"mpSm","type":"uint16"},{"internalType":"uint16","name":"mpRg","type":"uint16"},{"internalType":"uint16","name":"mpLg","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStatGrowth","name":"primaryStatGrowth","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hpSm","type":"uint16"},{"internalType":"uint16","name":"hpRg","type":"uint16"},{"internalType":"uint16","name":"hpLg","type":"uint16"},{"internalType":"uint16","name":"mpSm","type":"uint16"},{"internalType":"uint16","name":"mpRg","type":"uint16"},{"internalType":"uint16","name":"mpLg","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStatGrowth","name":"secondaryStatGrowth","type":"tuple"},{"components":[{"internalType":"uint16","name":"mining","type":"uint16"},{"internalType":"uint16","name":"gardening","type":"uint16"},{"internalType":"uint16","name":"foraging","type":"uint16"},{"internalType":"uint16","name":"fishing","type":"uint16"}],"internalType":"struct IHeroTypes.HeroProfessions","name":"professions","type":"tuple"}],"indexed":false,"internalType":"struct IHeroTypes.Hero","name":"newHero","type":"tuple"}],"name":"ItemConsumed","type":"event"},
 		{"inputs":[{"internalType":"address","name":"_consumableAddress","type":"address"},{"internalType":"uint256","name":"_heroId","type":"uint256"}],"name":"consumeItem","outputs":[],"stateMutability":"nonpayable","type":"function"},
 		{"inputs":[{"internalType":"address","name":"_heroCoreAddress","type":"address"}],"name":"initialize","outputs":[],"stateMutability":"nonpayable","type":"function"}
 	]
```

### Comparing `dfktools-0.3.1/src/dfktools/consumable_example.py` & `dfktools-0.3.2/src/dfktools/consumable_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/crystal.py` & `dfktools-0.3.2/src/dfktools/dex/crystal.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/erc1155.py` & `dfktools-0.3.2/src/dfktools/dex/erc1155.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/erc20.py` & `dfktools-0.3.2/src/dfktools/dex/erc20.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/item_erc1155.py` & `dfktools-0.3.2/src/dfktools/dex/item_erc1155.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/jade.py` & `dfktools-0.3.2/src/dfktools/dex/jade.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/jewel.py` & `dfktools-0.3.2/src/dfktools/dex/jewel.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/master_gardener.py` & `dfktools-0.3.2/src/dfktools/dex/master_gardener.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/uniswap_v2_factory.py` & `dfktools-0.3.2/src/dfktools/dex/uniswap_v2_factory.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/uniswap_v2_pair.py` & `dfktools-0.3.2/src/dfktools/dex/uniswap_v2_pair.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/uniswap_v2_router.py` & `dfktools-0.3.2/src/dfktools/dex/uniswap_v2_router.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex/utils/utils.py` & `dfktools-0.3.2/src/dfktools/dex/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/dex_example.py` & `dfktools-0.3.2/src/dfktools/dex_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/duel/duel.py` & `dfktools-0.3.2/src/dfktools/duel/duel.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/duel/utils/utils.py` & `dfktools-0.3.2/src/dfktools/duel/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/duel_example.py` & `dfktools-0.3.2/src/dfktools/duel_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/erc20_example.py` & `dfktools-0.3.2/src/dfktools/erc20_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/genes/gene_science_v1.py` & `dfktools-0.3.2/src/dfktools/genes/gene_science_v1.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/genes/gene_science_v2.py` & `dfktools-0.3.2/src/dfktools/genes/gene_science_v2.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/genes_encode_example.py` & `dfktools-0.3.2/src/dfktools/genes_encode_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/genes_example.py` & `dfktools-0.3.2/src/dfktools/genes_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/hero/hero_core.py` & `dfktools-0.3.2/src/dfktools/hero/hero_core.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/hero/heroes.py` & `dfktools-0.3.2/src/dfktools/hero/heroes.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/hero/utils/utils.py` & `dfktools-0.3.2/src/dfktools/hero/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/hero_example.py` & `dfktools-0.3.2/src/dfktools/hero_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/land/land.py` & `dfktools-0.3.2/src/dfktools/land/land.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/land_example.py` & `dfktools-0.3.2/src/dfktools/land_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/meditation/meditation.py` & `dfktools-0.3.2/src/dfktools/meditation/meditation.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/meditation_example.py` & `dfktools-0.3.2/src/dfktools/meditation_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/perilous_journey/perilous_journey.py` & `dfktools-0.3.2/src/dfktools/perilous_journey/perilous_journey.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/pet_example.py` & `dfktools-0.3.2/src/dfktools/pet_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/pets/exchange.py` & `dfktools-0.3.2/src/dfktools/pets/exchange.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/pets/hatchery.py` & `dfktools-0.3.2/src/dfktools/pets/hatchery.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/pets/pet_core.py` & `dfktools-0.3.2/src/dfktools/pets/pet_core.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/pets/pets.py` & `dfktools-0.3.2/src/dfktools/pets/pets.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/pets/utils/utils.py` & `dfktools-0.3.2/src/dfktools/pets/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/profile/profile.py` & `dfktools-0.3.2/src/dfktools/profile/profile.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/profile/profile_v2.py` & `dfktools-0.3.2/src/dfktools/profile/profile_v2.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/profile_example.py` & `dfktools-0.3.2/src/dfktools/profile_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quest_example.py` & `dfktools-0.3.2/src/dfktools/quest_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quests/professions/gardening.py` & `dfktools-0.3.2/src/dfktools/quests/professions/gardening.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quests/professions/mining.py` & `dfktools-0.3.2/src/dfktools/quests/professions/mining.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quests/quest_core_v1.py` & `dfktools-0.3.2/src/dfktools/quests/quest_core_v1.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quests/quest_core_v2.py` & `dfktools-0.3.2/src/dfktools/quests/quest_core_v2.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quests/quest_core_v3.py` & `dfktools-0.3.2/src/dfktools/quests/quest_core_v3.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quests/quest_v1.py` & `dfktools-0.3.2/src/dfktools/quests/quest_v1.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quests/quest_v2.py` & `dfktools-0.3.2/src/dfktools/quests/quest_v2.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quests/quest_v3.py` & `dfktools-0.3.2/src/dfktools/quests/quest_v3.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quests/utils/utils.py` & `dfktools-0.3.2/src/dfktools/quests/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/quests/wishing_well.py` & `dfktools-0.3.2/src/dfktools/quests/wishing_well.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/raffle/raffle_master.py` & `dfktools-0.3.2/src/dfktools/raffle/raffle_master.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/raffle/utils/utils.py` & `dfktools-0.3.2/src/dfktools/raffle/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/raffle_example.py` & `dfktools-0.3.2/src/dfktools/raffle_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/stone_carver/stone_carver.py` & `dfktools-0.3.2/src/dfktools/stone_carver/stone_carver.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/stone_carver_example.py` & `dfktools-0.3.2/src/dfktools/stone_carver_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/summoning/assisting.py` & `dfktools-0.3.2/src/dfktools/summoning/assisting.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/summoning/crystals.py` & `dfktools-0.3.2/src/dfktools/summoning/crystals.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/summoning/crystals_v2.py` & `dfktools-0.3.2/src/dfktools/summoning/crystals_v2.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/summoning/serendale_assisting.py` & `dfktools-0.3.2/src/dfktools/summoning/serendale_assisting.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/summoning/summoning.py` & `dfktools-0.3.2/src/dfktools/summoning/summoning.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/summoning_example.py` & `dfktools-0.3.2/src/dfktools/summoning_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools/wishing_well_quest_example.py` & `dfktools-0.3.2/src/dfktools/wishing_well_quest_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.3.1/src/dfktools.egg-info/PKG-INFO` & `dfktools-0.3.2/src/dfktools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfktools
-Version: 0.3.1
+Version: 0.3.2
 Summary: A toolbox for DefiKingdoms
 Home-page: https://github.com/0rtis/dfktools
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
```

### Comparing `dfktools-0.3.1/src/dfktools.egg-info/SOURCES.txt` & `dfktools-0.3.2/src/dfktools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

