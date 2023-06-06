# Comparing `tmp/crankshaft-0.3.0.tar.gz` & `tmp/crankshaft-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crankshaft-0.3.0.tar", max compression
+gzip compressed data, was "crankshaft-0.3.1.tar", max compression
```

## Comparing `crankshaft-0.3.0.tar` & `crankshaft-0.3.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1067 2023-05-31 20:05:59.557448 crankshaft-0.3.0/LICENSE
--rw-r--r--   0        0        0      336 2023-05-31 20:05:59.557448 crankshaft-0.3.0/README.md
--rw-r--r--   0        0        0      326 2023-05-31 20:07:08.962545 crankshaft-0.3.0/crankshaft/__init__.py
--rw-r--r--   0        0        0      120 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/api.bolt
--rw-r--r--   0        0        0      216 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/config.bolt
--rw-r--r--   0        0        0      512 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/defer.bolt
--rw-r--r--   0        0        0     3721 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/event_handler.bolt
--rw-r--r--   0        0        0     1441 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_entity_attack_player.bolt
--rw-r--r--   0        0        0      258 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_load.bolt
--rw-r--r--   0        0        0      355 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_airborne.bolt
--rw-r--r--   0        0        0      679 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_airborne_end.bolt
--rw-r--r--   0        0        0      680 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_airborne_start.bolt
--rw-r--r--   0        0        0     1441 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_attack_entity.bolt
--rw-r--r--   0        0        0      344 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_burn.bolt
--rw-r--r--   0        0        0      668 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_burn_end.bolt
--rw-r--r--   0        0        0      669 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_burn_start.bolt
--rw-r--r--   0        0        0      370 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_charge_bow.bolt
--rw-r--r--   0        0        0      797 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_charge_bow_end.bolt
--rw-r--r--   0        0        0      798 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_charge_bow_start.bolt
--rw-r--r--   0        0        0      346 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_glide.bolt
--rw-r--r--   0        0        0      671 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_glide_end.bolt
--rw-r--r--   0        0        0      672 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_glide_start.bolt
--rw-r--r--   0        0        0      637 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_inventory_change.bolt
--rw-r--r--   0        0        0      577 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_join.bolt
--rw-r--r--   0        0        0      585 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_jump.bolt
--rw-r--r--   0        0        0      686 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_land.bolt
--rw-r--r--   0        0        0      411 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_load.bolt
--rw-r--r--   0        0        0      597 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_shoot_bow.bolt
--rw-r--r--   0        0        0      349 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_sneak.bolt
--rw-r--r--   0        0        0      674 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_sneak_end.bolt
--rw-r--r--   0        0        0      675 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_sneak_start.bolt
--rw-r--r--   0        0        0      354 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_sprint.bolt
--rw-r--r--   0        0        0      679 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_sprint_end.bolt
--rw-r--r--   0        0        0      680 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_sprint_start.bolt
--rw-r--r--   0        0        0      347 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_swim.bolt
--rw-r--r--   0        0        0      672 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_swim_end.bolt
--rw-r--r--   0        0        0      673 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_swim_start.bolt
--rw-r--r--   0        0        0      271 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_tick.bolt
--rw-r--r--   0        0        0      537 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_player_use_coas.bolt
--rw-r--r--   0        0        0      258 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events/on_tick.bolt
--rw-r--r--   0        0        0     2007 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/events.bolt
--rw-r--r--   0        0        0     3722 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flag.bolt
--rw-r--r--   0        0        0      377 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_airborne.bolt
--rw-r--r--   0        0        0      402 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_baby.bolt
--rw-r--r--   0        0        0      411 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_burning.bolt
--rw-r--r--   0        0        0     1248 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_charging_bow.bolt
--rw-r--r--   0        0        0      377 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_gliding.bolt
--rw-r--r--   0        0        0      379 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_in_ground.bolt
--rw-r--r--   0        0        0      379 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_on_ground.bolt
--rw-r--r--   0        0        0      158 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_player.bolt
--rw-r--r--   0        0        0      414 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_sneaking.bolt
--rw-r--r--   0        0        0      417 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_sprinting.bolt
--rw-r--r--   0        0        0      414 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags/is_swimming.bolt
--rw-r--r--   0        0        0      535 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/flags.bolt
--rw-r--r--   0        0        0      407 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/lib/entity_hit_matching/api.bolt
--rw-r--r--   0        0        0      124 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/lib/entity_hit_matching/credits.txt
--rw-r--r--   0        0        0    58208 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/lib/entity_hit_matching/main.bolt
--rw-r--r--   0        0        0      207 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/modules/utils.bolt
--rw-r--r--   0        0        0        0 2023-05-31 20:05:59.557448 crankshaft-0.3.0/crankshaft/py.typed
--rw-r--r--   0        0        0     1260 2023-05-31 20:07:08.978545 crankshaft-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 crankshaft-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-06 01:30:16.404026 crankshaft-0.3.1/LICENSE
+-rw-r--r--   0        0        0      336 2023-06-06 01:30:16.404026 crankshaft-0.3.1/README.md
+-rw-r--r--   0        0        0      326 2023-06-06 01:31:29.404817 crankshaft-0.3.1/crankshaft/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/api.bolt
+-rw-r--r--   0        0        0      216 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/config.bolt
+-rw-r--r--   0        0        0      512 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/defer.bolt
+-rw-r--r--   0        0        0     3721 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/event_handler.bolt
+-rw-r--r--   0        0        0     1441 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_entity_attack_player.bolt
+-rw-r--r--   0        0        0      258 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_load.bolt
+-rw-r--r--   0        0        0      355 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_airborne.bolt
+-rw-r--r--   0        0        0      679 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_airborne_end.bolt
+-rw-r--r--   0        0        0      680 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_airborne_start.bolt
+-rw-r--r--   0        0        0     1441 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_attack_entity.bolt
+-rw-r--r--   0        0        0      344 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_burn.bolt
+-rw-r--r--   0        0        0      668 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_burn_end.bolt
+-rw-r--r--   0        0        0      669 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_burn_start.bolt
+-rw-r--r--   0        0        0      370 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_charge_bow.bolt
+-rw-r--r--   0        0        0      797 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_charge_bow_end.bolt
+-rw-r--r--   0        0        0      798 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_charge_bow_start.bolt
+-rw-r--r--   0        0        0      346 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_glide.bolt
+-rw-r--r--   0        0        0      671 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_glide_end.bolt
+-rw-r--r--   0        0        0      672 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_glide_start.bolt
+-rw-r--r--   0        0        0      637 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_inventory_change.bolt
+-rw-r--r--   0        0        0      577 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_join.bolt
+-rw-r--r--   0        0        0      585 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_jump.bolt
+-rw-r--r--   0        0        0      686 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_land.bolt
+-rw-r--r--   0        0        0      411 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_load.bolt
+-rw-r--r--   0        0        0      597 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_shoot_bow.bolt
+-rw-r--r--   0        0        0      349 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_sneak.bolt
+-rw-r--r--   0        0        0      674 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_sneak_end.bolt
+-rw-r--r--   0        0        0      675 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_sneak_start.bolt
+-rw-r--r--   0        0        0      354 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_sprint.bolt
+-rw-r--r--   0        0        0      679 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_sprint_end.bolt
+-rw-r--r--   0        0        0      680 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_sprint_start.bolt
+-rw-r--r--   0        0        0      347 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_swim.bolt
+-rw-r--r--   0        0        0      672 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_swim_end.bolt
+-rw-r--r--   0        0        0      673 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_swim_start.bolt
+-rw-r--r--   0        0        0      271 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_tick.bolt
+-rw-r--r--   0        0        0      537 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_player_use_coas.bolt
+-rw-r--r--   0        0        0      258 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events/on_tick.bolt
+-rw-r--r--   0        0        0     2007 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/events.bolt
+-rw-r--r--   0        0        0     3398 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flag.bolt
+-rw-r--r--   0        0        0      377 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_airborne.bolt
+-rw-r--r--   0        0        0      402 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_baby.bolt
+-rw-r--r--   0        0        0      411 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_burning.bolt
+-rw-r--r--   0        0        0     1248 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_charging_bow.bolt
+-rw-r--r--   0        0        0      377 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_gliding.bolt
+-rw-r--r--   0        0        0      379 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_in_ground.bolt
+-rw-r--r--   0        0        0      379 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_on_ground.bolt
+-rw-r--r--   0        0        0      158 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_player.bolt
+-rw-r--r--   0        0        0      414 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_sneaking.bolt
+-rw-r--r--   0        0        0      417 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_sprinting.bolt
+-rw-r--r--   0        0        0      414 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags/is_swimming.bolt
+-rw-r--r--   0        0        0      535 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/flags.bolt
+-rw-r--r--   0        0        0      407 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/lib/entity_hit_matching/api.bolt
+-rw-r--r--   0        0        0      124 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/lib/entity_hit_matching/credits.txt
+-rw-r--r--   0        0        0    58208 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/lib/entity_hit_matching/main.bolt
+-rw-r--r--   0        0        0      207 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/modules/utils.bolt
+-rw-r--r--   0        0        0        0 2023-06-06 01:30:16.404026 crankshaft-0.3.1/crankshaft/py.typed
+-rw-r--r--   0        0        0     1260 2023-06-06 01:31:29.420817 crankshaft-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 crankshaft-0.3.1/PKG-INFO
```

### Comparing `crankshaft-0.3.0/LICENSE` & `crankshaft-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/defer.bolt` & `crankshaft-0.3.1/crankshaft/modules/defer.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/event_handler.bolt` & `crankshaft-0.3.1/crankshaft/modules/event_handler.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_entity_attack_player.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_entity_attack_player.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_airborne_end.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_airborne_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_airborne_start.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_airborne_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_attack_entity.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_attack_entity.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_burn_end.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_burn_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_burn_start.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_burn_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_charge_bow_end.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_charge_bow_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_charge_bow_start.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_charge_bow_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_glide_end.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_glide_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_glide_start.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_glide_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_inventory_change.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_inventory_change.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_join.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_join.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_jump.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_jump.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_land.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_land.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_shoot_bow.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_shoot_bow.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_sneak_end.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_sneak_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_sneak_start.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_sneak_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_sprint_end.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_sprint_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_sprint_start.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_sprint_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_swim_end.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_swim_end.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_swim_start.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_swim_start.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events/on_player_use_coas.bolt` & `crankshaft-0.3.1/crankshaft/modules/events/on_player_use_coas.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/events.bolt` & `crankshaft-0.3.1/crankshaft/modules/events.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/flag.bolt` & `crankshaft-0.3.1/crankshaft/modules/flag.bolt`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 @dataclass
 class Flag:
     body: Callable = field(kw_only=True, repr=False)
     flag_id: str = field(kw_only=True)
 
     invert: bool = field(kw_only=True, default=False)
-    initialized: bool = field(kw_only=True, default=False)
     active: bool = field(default=False)
     # gate: ClassVar[ExpressionNode] = StaticVar(Bool)
 
     def __post_init__(self):
         self.gate = StaticVar(Bool)
 
         local_dir = f"{Config.ROOT_LOCAL}/flag/builtin/{self.flag_id}"
@@ -25,27 +24,25 @@
         self.root_dir = f"{global_dir}/__root__"
         self.condition_path = f"{global_dir}/__condition__"
 
     @contextmanager
     def __branch__(self):
         self.activate()
 
-        if not self.initialized:
-            self.check_condition()
-            self.initialized = True
+        self.check_condition()
 
         if not self.invert:
             if self.gate == 1:
                 yield True
         else:
             if self.gate == 0:
                 yield True
 
     def __not__(self):
-        return self.__class__(body=self.body, flag_id=self.flag_id, invert=not self.invert, initialized=self.initialized, active=self.active)
+        return self.__class__(body=self.body, flag_id=self.flag_id, invert=not self.invert, active=self.active)
 
     @contextmanager
     def set_condition(self):
         """Use along the 'with' statement to set the flag condition."""
 
         function self.condition_path:
             with self.gate.store(mode='success'):
@@ -67,15 +64,14 @@
         self.active = True
 
 @dataclass
 class CustomFlag:
     body: Callable = field(kw_only=True, repr=False)
 
     invert: bool = field(kw_only=True, default=False)
-    initialized: bool = field(kw_only=True, default=False)
     active: bool = field(default=False)
     next_id: ClassVar[int] = 0
 
     def __post_init__(self):
         self.gate = StaticVar(Bool)
         self.flag_id = f"{self._get_next_id()}__{ctx.project_id}"
 
@@ -84,27 +80,25 @@
         self.root_dir = f"{local_dir}/__root__"
         self.condition_path = f"{local_dir}/__condition__"
 
     @contextmanager
     def __branch__(self):
         self.activate()
 
-        if not self.initialized:
-            self.check_condition()
-            self.initialized = True
+        self.check_condition()
 
         if not self.invert:
             if self.gate == 1:
                 yield True
         else:
             if self.gate == 0:
                 yield True
 
     def __not__(self):
-        return self.__class__(body=self.body, invert=not self.invert, initialized=self.initialized, active=self.active)
+        return self.__class__(body=self.body, invert=not self.invert, active=self.active)
 
     @contextmanager
     def set_condition(self):
         """Use along the 'with' statement to set the flag condition."""
 
         function self.condition_path:
             with self.gate.store(mode='success'):
```

### Comparing `crankshaft-0.3.0/crankshaft/modules/flags/is_charging_bow.bolt` & `crankshaft-0.3.1/crankshaft/modules/flags/is_charging_bow.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/flags.bolt` & `crankshaft-0.3.1/crankshaft/modules/flags.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/crankshaft/modules/lib/entity_hit_matching/main.bolt` & `crankshaft-0.3.1/crankshaft/modules/lib/entity_hit_matching/main.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.0/pyproject.toml` & `crankshaft-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crankshaft"
-version = "0.3.0"
+version = "0.3.1"
 description = "Flow control library for the Bolt scripting language."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/crankshaft"
 readme = "README.md"
```

### Comparing `crankshaft-0.3.0/PKG-INFO` & `crankshaft-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crankshaft
-Version: 0.3.0
+Version: 0.3.1
 Summary: Flow control library for the Bolt scripting language.
 Home-page: https://github.com/reapermc/crankshaft
 License: MIT
 Keywords: beet,bolt,minecraft,datapack,minecraft-commands,mcfunction,library,reapermc
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

