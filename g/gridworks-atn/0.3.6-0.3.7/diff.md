# Comparing `tmp/gridworks_atn-0.3.6.tar.gz` & `tmp/gridworks_atn-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_atn-0.3.6.tar", max compression
+gzip compressed data, was "gridworks_atn-0.3.7.tar", max compression
```

## Comparing `gridworks_atn-0.3.6.tar` & `gridworks_atn-0.3.7.tar`

### file list

```diff
@@ -1,228 +1,228 @@
--rw-r--r--   0        0        0     1065 2023-05-16 15:15:56.124967 gridworks_atn-0.3.6/LICENSE
--rw-r--r--   0        0        0     3002 2023-05-16 15:15:56.124967 gridworks_atn-0.3.6/README.md
--rw-r--r--   0        0        0     2193 2023-05-16 15:16:10.672885 gridworks_atn-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      681 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/__init__.py
--rw-r--r--   0        0        0      226 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/__main__.py
--rw-r--r--   0        0        0    13411 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/api_types.py
--rw-r--r--   0        0        0    21728 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/atn_actor_base.py
--rw-r--r--   0        0        0     3114 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/atn_utils.py
--rw-r--r--   0        0        0    19983 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/atn.py
--rw-r--r--   0        0        0       98 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/dev_atn_params_data.csv
--rw-r--r--   0        0        0     7337 2023-05-16 15:16:10.672885 gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/dev_io.py
--rw-r--r--   0        0        0      867 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/edge.py
--rw-r--r--   0        0        0     7536 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/flo.py
--rw-r--r--   0        0        0    18355 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/flo_output.py
--rw-r--r--   0        0        0     1508 2023-05-16 15:16:10.672885 gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/make_dev_input_data.py
--rw-r--r--   0        0        0      841 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/node.py
--rw-r--r--   0        0        0     6963 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/simple_scada_sim.py
--rw-r--r--   0        0        0     2671 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/strategy_utils.py
--rw-r--r--   0        0        0     4575 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/config.py
--rw-r--r--   0        0        0       43 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/conversion_factors.py
--rw-r--r--   0        0        0     6148 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/data_classes/.DS_Store
--rw-r--r--   0        0        0      935 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/data_classes/__init__.py
--rw-r--r--   0        0        0      577 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/data_classes/d_edge.py
--rw-r--r--   0        0        0     7812 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/data_classes/d_graph.py
--rw-r--r--   0        0        0     1508 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/data_classes/d_node.py
--rw-r--r--   0        0        0     8684 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/data_classes/hack_price_method.py
--rw-r--r--   0        0        0     4082 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/data_classes/hack_weather_location.py
--rw-r--r--   0        0        0     2104 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/data_classes/hack_weather_source.py
--rw-r--r--   0        0        0    14466 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/demo_methods.py
--rw-r--r--   0        0        0      276 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/dev_utils/__init__.py
--rw-r--r--   0        0        0     1792 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/dev_utils/dev_discoverer.py
--rw-r--r--   0        0        0    11883 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/dev_utils/dev_ta_owner.py
--rw-r--r--   0        0        0    10994 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/dev_utils/dev_validator.py
--rw-r--r--   0        0        0     1171 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/dev_utils/make_plants.py
--rw-r--r--   0        0        0    11409 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/dispatch_contract.py
--rw-r--r--   0        0        0    12463 2023-05-16 15:15:56.132967 gridworks_atn-0.3.6/src/gwatn/dispatch_contract_artifacts/application.json
--rw-r--r--   0        0        0     5229 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/dispatch_contract_artifacts/approval.teal
--rw-r--r--   0        0        0       40 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/dispatch_contract_artifacts/clear.teal
--rw-r--r--   0        0        0     3937 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/dispatch_contract_artifacts/contract.json
--rw-r--r--   0        0        0     2402 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/enums/__init__.py
--rw-r--r--   0        0        0      700 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/enums/distribution_tariff.py
--rw-r--r--   0        0        0      614 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/enums/energy_supply_type.py
--rw-r--r--   0        0        0     1308 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/enums/hack_price_method.py
--rw-r--r--   0        0        0      415 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/enums/hack_recognized_p_node_alias.py
--rw-r--r--   0        0        0      590 2023-05-16 15:16:10.672885 gridworks_atn-0.3.6/src/gwatn/enums/hack_weather_method.py
--rw-r--r--   0        0        0      132 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/enums/hack_weather_source.py
--rw-r--r--   0        0        0      947 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/enums/recognized_irradiance_type.py
--rw-r--r--   0        0        0      570 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/enums/recognized_temperature_unit.py
--rw-r--r--   0        0        0      122 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/errors.py
--rw-r--r--   0        0        0        0 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/py.typed
--rw-r--r--   0        0        0     7945 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/python_ta_daemon.json
--rw-r--r--   0        0        0    12518 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/python_ta_daemon.py
--rw-r--r--   0        0        0      834 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/scada_codec.py
--rw-r--r--   0        0        0     4870 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/simple_atn_actor.py
--rw-r--r--   0        0        0    26139 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/simple_scada_sim_actor_base.py
--rw-r--r--   0        0        0     3169 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/ta_daemon_rest_api.py
--rw-r--r--   0        0        0      460 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/ta_validator_rest_api.py
--rw-r--r--   0        0        0    47761 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/two_channel_actor_base.py
--rw-r--r--   0        0        0    13145 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/__init__.py
--rw-r--r--   0        0        0     7868 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/accepted_bid.py
--rw-r--r--   0        0        0    20222 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/atn_bid.py
--rw-r--r--   0        0        0     4288 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/atn_params.py
--rw-r--r--   0        0        0    22335 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/atn_params_brickstorageheater.py
--rw-r--r--   0        0        0     8144 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/atn_params_report.py
--rw-r--r--   0        0        0     8321 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/basegnode_scada_create.py
--rw-r--r--   0        0        0     1067 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/data_channel.py
--rw-r--r--   0        0        0     9885 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/discoverycert_algo_create.py
--rw-r--r--   0        0        0     8092 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/dispatch_contract_confirmed.py
--rw-r--r--   0        0        0     3235 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/epda/gt_epda_actual_1_0_0.py
--rw-r--r--   0        0        0      555 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3959 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3338 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py
--rw-r--r--   0        0        0      555 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3959 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3658 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0     1690 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     4905 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7648 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/flo_params.py
--rw-r--r--   0        0        0    22826 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/flo_params_brickstorageheater.py
--rw-r--r--   0        0        0     8827 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/flo_params_report.py
--rw-r--r--   0        0        0     3885 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py
--rw-r--r--   0        0        0      600 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4184 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5457 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py
--rw-r--r--   0        0        0      620 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0     7905 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5419 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0      625 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7913 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5176 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py
--rw-r--r--   0        0        0      649 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py
--rw-r--r--   0        0        0     8053 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3885 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py
--rw-r--r--   0        0        0      593 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4203 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5392 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py
--rw-r--r--   0        0        0      613 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0     7891 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3909 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py
--rw-r--r--   0        0        0      609 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4212 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7507 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py
--rw-r--r--   0        0        0     1453 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py
--rw-r--r--   0        0        0    12856 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7530 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py
--rw-r--r--   0        0        0     1453 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0    11873 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3980 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py
--rw-r--r--   0        0        0      611 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4060 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4083 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py
--rw-r--r--   0        0        0      627 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4430 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3879 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py
--rw-r--r--   0        0        0      595 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4196 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5398 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py
--rw-r--r--   0        0        0      615 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0     7901 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     8206 2023-05-16 15:15:56.136967 gridworks_atn-0.3.6/src/gwatn/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0    14769 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/hack_property_format.py
--rw-r--r--   0        0        0      194 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/hack_test_dummy.py
--rw-r--r--   0        0        0      781 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/hack_type_base.py
--rw-r--r--   0        0        0      990 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/hack_utils.py
--rw-r--r--   0        0        0     9155 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/heartbeat_b.py
--rw-r--r--   0        0        0     6154 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/initial_tadeed_algo_create.py
--rw-r--r--   0        0        0     7610 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/initial_tadeed_algo_optin.py
--rw-r--r--   0        0        0     8932 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/initial_tadeed_algo_transfer.py
--rw-r--r--   0        0        0     7959 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/join_dispatch_contract.py
--rw-r--r--   0        0        0    12429 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/latest_price.py
--rw-r--r--   0        0        0     5028 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/market_slot.py
--rw-r--r--   0        0        0    17161 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/market_type_gt.py
--rw-r--r--   0        0        0     5294 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/new_tadeed_algo_optin.py
--rw-r--r--   0        0        0     5196 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/new_tadeed_send.py
--rw-r--r--   0        0        0     5024 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/old_tadeed_algo_return.py
--rw-r--r--   0        0        0     8461 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/price_quantity.py
--rw-r--r--   0        0        0     2492 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/price_quantity_unitless.py
--rw-r--r--   0        0        0    13837 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py
--rw-r--r--   0        0        0    13162 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py
--rw-r--r--   0        0        0    14105 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py
--rw-r--r--   0        0        0     5624 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py
--rw-r--r--   0        0        0      558 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py
--rw-r--r--   0        0        0     8026 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5026 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py
--rw-r--r--   0        0        0      594 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py
--rw-r--r--   0        0        0     7236 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5890 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py
--rw-r--r--   0        0        0      578 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7750 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7618 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py
--rw-r--r--   0        0        0    13827 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py
--rw-r--r--   0        0        0     7319 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py
--rw-r--r--   0        0        0    12667 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py
--rw-r--r--   0        0        0     8872 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0    10345 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py
--rw-r--r--   0        0        0    14435 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py
--rw-r--r--   0        0        0     4044 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py
--rw-r--r--   0        0        0      589 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3804 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5402 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py
--rw-r--r--   0        0        0      561 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py
--rw-r--r--   0        0        0     7263 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4044 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py
--rw-r--r--   0        0        0      589 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3804 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5661 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py
--rw-r--r--   0        0        0      597 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py
--rw-r--r--   0        0        0     7829 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3535 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py
--rw-r--r--   0        0        0      653 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py
--rw-r--r--   0        0        0     3064 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4184 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0      586 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     3863 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5892 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py
--rw-r--r--   0        0        0      581 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7746 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3707 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py
--rw-r--r--   0        0        0      581 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py
--rw-r--r--   0        0        0     3547 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py
--rw-r--r--   0        0        0    13926 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py
--rw-r--r--   0        0        0    14182 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py
--rw-r--r--   0        0        0     5617 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py
--rw-r--r--   0        0        0      544 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py
--rw-r--r--   0        0        0     8022 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5864 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py
--rw-r--r--   0        0        0      573 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7746 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5004 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/scada_cert_transfer.py
--rw-r--r--   0        0        0     3682 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/simplesim_driver_data.py
--rw-r--r--   0        0        0     4166 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/simplesim_driver_data_bsh.py
--rw-r--r--   0        0        0     6534 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/simplesim_driver_report.py
--rw-r--r--   0        0        0     6774 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/simplesim_snapshot_brickstorageheater.py
--rw-r--r--   0        0        0     3220 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/sla_enter.py
--rw-r--r--   0        0        0     4101 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/tadeed_specs_hack.py
--rw-r--r--   0        0        0     5734 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/tavalidatorcert_algo_create.py
--rw-r--r--   0        0        0     6371 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/tavalidatorcert_algo_transfer.py
--rw-r--r--   0        0        0     5242 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/terminalasset_certify_hack.py
--rw-r--r--   0        0        0    30475 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py
--rw-r--r--   0        0        0    29247 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0     8474 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py
--rw-r--r--   0        0        0     1920 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py
--rw-r--r--   0        0        0    13416 2023-05-16 15:15:56.140967 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3535 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py
--rw-r--r--   0        0        0      686 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py
--rw-r--r--   0        0        0     3076 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7834 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py
--rw-r--r--   0        0        0      829 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py
--rw-r--r--   0        0        0    12801 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py
--rw-r--r--   0        0        0     8628 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0     1153 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0    12807 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3671 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py
--rw-r--r--   0        0        0      572 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py
--rw-r--r--   0        0        0     3547 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py
--rw-r--r--   0        0        0    14909 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py
--rw-r--r--   0        0        0    11616 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py
--rw-r--r--   0        0        0     4544 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py
--rw-r--r--   0        0        0      631 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py
--rw-r--r--   0        0        0     6001 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py
--rw-r--r--   0        0        0    12321 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py
--rw-r--r--   0        0        0     6939 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py
--rw-r--r--   0        0        0      642 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py
--rw-r--r--   0        0        0    10751 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4677 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py
--rw-r--r--   0        0        0      610 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py
--rw-r--r--   0        0        0     6741 2023-05-16 15:15:56.144966 gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 gridworks_atn-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-05 22:56:56.785578 gridworks_atn-0.3.7/LICENSE
+-rw-r--r--   0        0        0     3002 2023-06-05 22:56:56.785578 gridworks_atn-0.3.7/README.md
+-rw-r--r--   0        0        0     2193 2023-06-05 22:57:11.781770 gridworks_atn-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      681 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/__init__.py
+-rw-r--r--   0        0        0      226 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/__main__.py
+-rw-r--r--   0        0        0    13411 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/api_types.py
+-rw-r--r--   0        0        0    24496 2023-06-05 22:57:11.781770 gridworks_atn-0.3.7/src/gwatn/atn_actor_base.py
+-rw-r--r--   0        0        0     3114 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/atn_utils.py
+-rw-r--r--   0        0        0    19983 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/atn.py
+-rw-r--r--   0        0        0       98 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/dev_atn_params_data.csv
+-rw-r--r--   0        0        0     7337 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/dev_io.py
+-rw-r--r--   0        0        0      867 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/edge.py
+-rw-r--r--   0        0        0     7536 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/flo.py
+-rw-r--r--   0        0        0    18355 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/flo_output.py
+-rw-r--r--   0        0        0     1508 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/make_dev_input_data.py
+-rw-r--r--   0        0        0      841 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/node.py
+-rw-r--r--   0        0        0     6963 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/simple_scada_sim.py
+-rw-r--r--   0        0        0     2671 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/strategy_utils.py
+-rw-r--r--   0        0        0     4575 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/config.py
+-rw-r--r--   0        0        0       43 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/conversion_factors.py
+-rw-r--r--   0        0        0     6148 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/data_classes/.DS_Store
+-rw-r--r--   0        0        0      935 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/d_edge.py
+-rw-r--r--   0        0        0     7812 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/d_graph.py
+-rw-r--r--   0        0        0     1508 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/d_node.py
+-rw-r--r--   0        0        0     8684 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/hack_price_method.py
+-rw-r--r--   0        0        0     4082 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/hack_weather_location.py
+-rw-r--r--   0        0        0     2104 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/hack_weather_source.py
+-rw-r--r--   0        0        0    14466 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/demo_methods.py
+-rw-r--r--   0        0        0      276 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dev_utils/__init__.py
+-rw-r--r--   0        0        0     1792 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_discoverer.py
+-rw-r--r--   0        0        0    11883 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_ta_owner.py
+-rw-r--r--   0        0        0    10994 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_validator.py
+-rw-r--r--   0        0        0     1171 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dev_utils/make_plants.py
+-rw-r--r--   0        0        0    11409 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dispatch_contract.py
+-rw-r--r--   0        0        0    12463 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/application.json
+-rw-r--r--   0        0        0     5229 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/approval.teal
+-rw-r--r--   0        0        0       40 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/clear.teal
+-rw-r--r--   0        0        0     3937 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/contract.json
+-rw-r--r--   0        0        0     2402 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/__init__.py
+-rw-r--r--   0        0        0      700 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/distribution_tariff.py
+-rw-r--r--   0        0        0      614 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/energy_supply_type.py
+-rw-r--r--   0        0        0     1308 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/hack_price_method.py
+-rw-r--r--   0        0        0      415 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/hack_recognized_p_node_alias.py
+-rw-r--r--   0        0        0      590 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/hack_weather_method.py
+-rw-r--r--   0        0        0      132 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/hack_weather_source.py
+-rw-r--r--   0        0        0      947 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/recognized_irradiance_type.py
+-rw-r--r--   0        0        0      570 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/recognized_temperature_unit.py
+-rw-r--r--   0        0        0      122 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/errors.py
+-rw-r--r--   0        0        0        0 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/py.typed
+-rw-r--r--   0        0        0     7945 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/python_ta_daemon.json
+-rw-r--r--   0        0        0    12518 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/python_ta_daemon.py
+-rw-r--r--   0        0        0      834 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/scada_codec.py
+-rw-r--r--   0        0        0     3523 2023-06-05 22:57:11.781770 gridworks_atn-0.3.7/src/gwatn/simple_atn_actor.py
+-rw-r--r--   0        0        0    26139 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/simple_scada_sim_actor_base.py
+-rw-r--r--   0        0        0     3169 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/ta_daemon_rest_api.py
+-rw-r--r--   0        0        0      460 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/ta_validator_rest_api.py
+-rw-r--r--   0        0        0    47761 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/two_channel_actor_base.py
+-rw-r--r--   0        0        0    13145 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/__init__.py
+-rw-r--r--   0        0        0     7868 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/accepted_bid.py
+-rw-r--r--   0        0        0    20222 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/atn_bid.py
+-rw-r--r--   0        0        0     4288 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/atn_params.py
+-rw-r--r--   0        0        0    22335 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/atn_params_brickstorageheater.py
+-rw-r--r--   0        0        0     8144 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/atn_params_report.py
+-rw-r--r--   0        0        0     8321 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/basegnode_scada_create.py
+-rw-r--r--   0        0        0     1067 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/data_channel.py
+-rw-r--r--   0        0        0     9885 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/discoverycert_algo_create.py
+-rw-r--r--   0        0        0     8092 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/dispatch_contract_confirmed.py
+-rw-r--r--   0        0        0     3235 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0      555 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3959 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3338 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0      555 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3959 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3658 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     1690 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     4905 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7648 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/flo_params.py
+-rw-r--r--   0        0        0    22826 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/flo_params_brickstorageheater.py
+-rw-r--r--   0        0        0     8827 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/flo_params_report.py
+-rw-r--r--   0        0        0     3885 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py
+-rw-r--r--   0        0        0      600 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4184 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5457 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      620 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7905 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5419 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0      625 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7913 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5176 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py
+-rw-r--r--   0        0        0      649 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     8053 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3885 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py
+-rw-r--r--   0        0        0      593 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4203 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5392 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      613 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7891 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3909 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py
+-rw-r--r--   0        0        0      609 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4212 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7507 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py
+-rw-r--r--   0        0        0     1453 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py
+-rw-r--r--   0        0        0    12856 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7530 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py
+-rw-r--r--   0        0        0     1453 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0    11873 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3980 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py
+-rw-r--r--   0        0        0      611 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4060 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4083 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py
+-rw-r--r--   0        0        0      627 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4430 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3879 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py
+-rw-r--r--   0        0        0      595 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4196 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5398 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      615 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7901 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     8206 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0    14769 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/hack_property_format.py
+-rw-r--r--   0        0        0      194 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/hack_test_dummy.py
+-rw-r--r--   0        0        0      781 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/hack_type_base.py
+-rw-r--r--   0        0        0      990 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/hack_utils.py
+-rw-r--r--   0        0        0     9155 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/heartbeat_b.py
+-rw-r--r--   0        0        0     6154 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_create.py
+-rw-r--r--   0        0        0     7610 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     8932 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_transfer.py
+-rw-r--r--   0        0        0     7959 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/join_dispatch_contract.py
+-rw-r--r--   0        0        0    12429 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/latest_price.py
+-rw-r--r--   0        0        0     5028 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/market_slot.py
+-rw-r--r--   0        0        0    17161 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/market_type_gt.py
+-rw-r--r--   0        0        0     5294 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/new_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     5196 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/new_tadeed_send.py
+-rw-r--r--   0        0        0     5024 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/old_tadeed_algo_return.py
+-rw-r--r--   0        0        0     8461 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/price_quantity.py
+-rw-r--r--   0        0        0     2492 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/price_quantity_unitless.py
+-rw-r--r--   0        0        0    13837 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py
+-rw-r--r--   0        0        0    13162 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py
+-rw-r--r--   0        0        0    14105 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py
+-rw-r--r--   0        0        0     5624 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py
+-rw-r--r--   0        0        0      558 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py
+-rw-r--r--   0        0        0     8026 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5026 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py
+-rw-r--r--   0        0        0      594 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py
+-rw-r--r--   0        0        0     7236 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5890 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py
+-rw-r--r--   0        0        0      578 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7750 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7618 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0    13827 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py
+-rw-r--r--   0        0        0     7319 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0    12667 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py
+-rw-r--r--   0        0        0     8872 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0    10345 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py
+-rw-r--r--   0        0        0    14435 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py
+-rw-r--r--   0        0        0     4044 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0      589 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3804 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5402 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py
+-rw-r--r--   0        0        0      561 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py
+-rw-r--r--   0        0        0     7263 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4044 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0      589 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3804 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5661 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py
+-rw-r--r--   0        0        0      597 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py
+-rw-r--r--   0        0        0     7829 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3535 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py
+-rw-r--r--   0        0        0      653 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py
+-rw-r--r--   0        0        0     3064 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4184 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0      586 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     3863 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5892 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py
+-rw-r--r--   0        0        0      581 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7746 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3707 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py
+-rw-r--r--   0        0        0      581 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py
+-rw-r--r--   0        0        0     3547 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    13926 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py
+-rw-r--r--   0        0        0    14182 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py
+-rw-r--r--   0        0        0     5617 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py
+-rw-r--r--   0        0        0      544 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py
+-rw-r--r--   0        0        0     8022 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5864 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py
+-rw-r--r--   0        0        0      573 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7746 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5004 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/scada_cert_transfer.py
+-rw-r--r--   0        0        0     3682 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_data.py
+-rw-r--r--   0        0        0     4166 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_data_bsh.py
+-rw-r--r--   0        0        0     6534 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_report.py
+-rw-r--r--   0        0        0     6774 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/simplesim_snapshot_brickstorageheater.py
+-rw-r--r--   0        0        0     3220 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/sla_enter.py
+-rw-r--r--   0        0        0     4101 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/tadeed_specs_hack.py
+-rw-r--r--   0        0        0     5734 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/tavalidatorcert_algo_create.py
+-rw-r--r--   0        0        0     6371 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/tavalidatorcert_algo_transfer.py
+-rw-r--r--   0        0        0     5242 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/terminalasset_certify_hack.py
+-rw-r--r--   0        0        0    30475 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py
+-rw-r--r--   0        0        0    29247 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     8474 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py
+-rw-r--r--   0        0        0     1920 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py
+-rw-r--r--   0        0        0    13416 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3535 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py
+-rw-r--r--   0        0        0      686 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py
+-rw-r--r--   0        0        0     3076 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7834 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py
+-rw-r--r--   0        0        0      829 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py
+-rw-r--r--   0        0        0    12801 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     8628 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     1153 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0    12807 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3671 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py
+-rw-r--r--   0        0        0      572 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py
+-rw-r--r--   0        0        0     3547 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    14909 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py
+-rw-r--r--   0        0        0    11616 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py
+-rw-r--r--   0        0        0     4544 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py
+-rw-r--r--   0        0        0      631 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py
+-rw-r--r--   0        0        0     6001 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    12321 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py
+-rw-r--r--   0        0        0     6939 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py
+-rw-r--r--   0        0        0      642 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py
+-rw-r--r--   0        0        0    10751 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4677 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py
+-rw-r--r--   0        0        0      610 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py
+-rw-r--r--   0        0        0     6741 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 gridworks_atn-0.3.7/PKG-INFO
```

### Comparing `gridworks_atn-0.3.6/LICENSE` & `gridworks_atn-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/README.md` & `gridworks_atn-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/pyproject.toml` & `gridworks_atn-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-atn"
-version = "0.3.6"
+version = "0.3.7"
 description = "Gridworks Atn Spaceheat"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "None"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-atn"
 repository = "https://github.com/thegridelectric/gridworks-atn"
 documentation = "https://gridworks-atn.readthedocs.io"
```

### Comparing `gridworks_atn-0.3.6/src/gwatn/__init__.py` & `gridworks_atn-0.3.7/src/gwatn/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/api_types.py` & `gridworks_atn-0.3.7/src/gwatn/api_types.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/atn_actor_base.py` & `gridworks_atn-0.3.7/src/gwatn/atn_actor_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from gwatn.dispatch_contract import DispatchContract
 from gwatn.enums import AlgoCertType
 from gwatn.enums import MessageCategorySymbol
 from gwatn.enums import UniverseType
 from gwatn.two_channel_actor_base import TwoChannelActorBase
 from gwatn.types import AtnParams
 from gwatn.types import DispatchContractConfirmed_Maker
+from gwatn.types import GtDispatchBoolean_Maker
+from gwatn.types import GtShCliAtnCmd_Maker
 from gwatn.types import GtShStatus
 from gwatn.types import GwCertId
 from gwatn.types import GwCertId_Maker
 from gwatn.types import HeartbeatA
 from gwatn.types import HeartbeatA_Maker
 from gwatn.types import HeartbeatB
 from gwatn.types import HeartbeatB_Maker
@@ -337,14 +339,78 @@
         self.hb_status.ScadaLastHex = ping.MyHex
         self.hb_status.AtnLastHex = str(random.choice("0123456789abcdef"))
         LOGGER.info(f"Got {ping.MyHex}")
         # Does not send back. Atn waits for the DispatchContract's expected
         # one minute before sending.
         # print(f"Got heartbeat from scada: {ping}")
 
+    # Sends to SCADA
+
+    def snap(self):
+        """Ask SCADA for a snapshot of the current state of the TerminalAsset"""
+        self.send_scada_message(
+            payload=GtShCliAtnCmd_Maker(
+                from_g_node_alias=self.alias,
+                from_g_node_id=self.g_node_instance_id,
+                send_snapshot=True,
+            ).tuple
+        )
+
+    def turn_on(self, relay_node_name: str) -> None:
+        """
+        Turn ON a relay (i.e. closes the electrical circuit so that current can flow),
+        using the name of the relay as represented in the hardware layout as a Spaceheat
+        Node with role "BooleanActuator"
+
+        [SpaceheatNode](https://gridworks-protocol.readthedocs.io/en/latest/spaceheat-node.html)
+        [BooleanActuator Role](https://gridworks-protocol.readthedocs.io/en/latest/enums.html#gwproto.enums.Role)
+        Args:
+            relay_node_name: the name of the relay, as string in LeftRightDot format. This must be the
+            name of a SpaceheatNode in the hardware layout with role "BooleanActuator"
+
+        Returns:
+            None
+        """
+        self.send_scada_message(
+            payload=GtDispatchBoolean_Maker(
+                about_node_name=relay_node_name,
+                to_g_node_alias=self.scada_alias,
+                from_g_node_alias=self.alias,
+                from_g_node_instance_id=self.g_node_instance_id,
+                relay_state=1,
+                send_time_unix_ms=int(time.time() * 1000),
+            ).tuple
+        )
+
+    def turn_off(self, relay_node_name: str) -> None:
+        """
+        Turn OFF a relay (i.e. closes the electrical circuit so that current can flow),
+        using the name of the relay as represented in the hardware layout as a Spaceheat
+        Node with role "BooleanActuator"
+
+        [SpaceheatNode](https://gridworks-protocol.readthedocs.io/en/latest/spaceheat-node.html)
+        [BooleanActuator Role](https://gridworks-protocol.readthedocs.io/en/latest/enums.html#gwproto.enums.Role)
+        Args:
+            relay_node_name: the name of the relay, as string in LeftRightDot format. This must be the
+            name of a SpaceheatNode in the hardware layout with role "BooleanActuator"
+
+        Returns:
+            None
+        """
+        self.send_scada_message(
+            payload=GtDispatchBoolean_Maker(
+                about_node_name=relay_node_name,
+                to_g_node_alias=self.scada_alias,
+                from_g_node_alias=self.alias,
+                from_g_node_instance_id=self.g_node_instance_id,
+                relay_state=0,
+                send_time_unix_ms=int(time.time() * 1000),
+            ).tuple
+        )
+
     def hb_to_scada(self):
         """Checks that Atn is in Dispatch Contract, sends a HeartbeatB to Scada,
         and then reports to DispatchContract"""
         if not self.in_dispatch_contract():
             LOGGER.info("Not sending hb to Scada - not in DispatchContract yet")
         ping = HeartbeatB_Maker(
             from_g_node_alias=self.alias,
```

### Comparing `gridworks_atn-0.3.6/src/gwatn/atn_utils.py` & `gridworks_atn-0.3.7/src/gwatn/atn_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/atn.py` & `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/atn.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/dev_io.py` & `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/dev_io.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/edge.py` & `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/edge.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/flo.py` & `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/flo.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/flo_output.py` & `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/flo_output.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/make_dev_input_data.py` & `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/make_dev_input_data.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/node.py` & `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/simple_scada_sim.py` & `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/simple_scada_sim.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/brick_storage_heater/strategy_utils.py` & `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/strategy_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/config.py` & `gridworks_atn-0.3.7/src/gwatn/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/data_classes/.DS_Store` & `gridworks_atn-0.3.7/src/gwatn/data_classes/.DS_Store`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/data_classes/__init__.py` & `gridworks_atn-0.3.7/src/gwatn/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/data_classes/d_edge.py` & `gridworks_atn-0.3.7/src/gwatn/data_classes/d_edge.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/data_classes/d_graph.py` & `gridworks_atn-0.3.7/src/gwatn/data_classes/d_graph.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/data_classes/d_node.py` & `gridworks_atn-0.3.7/src/gwatn/data_classes/d_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/data_classes/hack_price_method.py` & `gridworks_atn-0.3.7/src/gwatn/data_classes/hack_price_method.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/data_classes/hack_weather_location.py` & `gridworks_atn-0.3.7/src/gwatn/data_classes/hack_weather_location.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/data_classes/hack_weather_source.py` & `gridworks_atn-0.3.7/src/gwatn/data_classes/hack_weather_source.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/demo_methods.py` & `gridworks_atn-0.3.7/src/gwatn/demo_methods.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/dev_utils/dev_discoverer.py` & `gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_discoverer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/dev_utils/dev_ta_owner.py` & `gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_ta_owner.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/dev_utils/dev_validator.py` & `gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_validator.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/dev_utils/make_plants.py` & `gridworks_atn-0.3.7/src/gwatn/dev_utils/make_plants.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/dispatch_contract.py` & `gridworks_atn-0.3.7/src/gwatn/dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/dispatch_contract_artifacts/application.json` & `gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/application.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/dispatch_contract_artifacts/approval.teal` & `gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/approval.teal`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/dispatch_contract_artifacts/contract.json` & `gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/contract.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/enums/__init__.py` & `gridworks_atn-0.3.7/src/gwatn/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/enums/distribution_tariff.py` & `gridworks_atn-0.3.7/src/gwatn/enums/distribution_tariff.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/enums/energy_supply_type.py` & `gridworks_atn-0.3.7/src/gwatn/enums/energy_supply_type.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/enums/hack_price_method.py` & `gridworks_atn-0.3.7/src/gwatn/enums/hack_price_method.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/enums/hack_weather_method.py` & `gridworks_atn-0.3.7/src/gwatn/enums/hack_weather_method.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/enums/recognized_irradiance_type.py` & `gridworks_atn-0.3.7/src/gwatn/enums/recognized_irradiance_type.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/enums/recognized_temperature_unit.py` & `gridworks_atn-0.3.7/src/gwatn/enums/recognized_temperature_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/python_ta_daemon.json` & `gridworks_atn-0.3.7/src/gwatn/python_ta_daemon.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/python_ta_daemon.py` & `gridworks_atn-0.3.7/src/gwatn/python_ta_daemon.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/scada_codec.py` & `gridworks_atn-0.3.7/src/gwatn/scada_codec.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/simple_scada_sim_actor_base.py` & `gridworks_atn-0.3.7/src/gwatn/simple_scada_sim_actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/ta_daemon_rest_api.py` & `gridworks_atn-0.3.7/src/gwatn/ta_daemon_rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/two_channel_actor_base.py` & `gridworks_atn-0.3.7/src/gwatn/two_channel_actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/__init__.py` & `gridworks_atn-0.3.7/src/gwatn/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/accepted_bid.py` & `gridworks_atn-0.3.7/src/gwatn/types/accepted_bid.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/atn_bid.py` & `gridworks_atn-0.3.7/src/gwatn/types/atn_bid.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/atn_params.py` & `gridworks_atn-0.3.7/src/gwatn/types/atn_params.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/atn_params_brickstorageheater.py` & `gridworks_atn-0.3.7/src/gwatn/types/atn_params_brickstorageheater.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/atn_params_report.py` & `gridworks_atn-0.3.7/src/gwatn/types/atn_params_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/basegnode_scada_create.py` & `gridworks_atn-0.3.7/src/gwatn/types/basegnode_scada_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/data_channel.py` & `gridworks_atn-0.3.7/src/gwatn/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/discoverycert_algo_create.py` & `gridworks_atn-0.3.7/src/gwatn/types/discoverycert_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/dispatch_contract_confirmed.py` & `gridworks_atn-0.3.7/src/gwatn/types/dispatch_contract_confirmed.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/epda/gt_epda_actual_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/flo_params.py` & `gridworks_atn-0.3.7/src/gwatn/types/flo_params.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/flo_params_brickstorageheater.py` & `gridworks_atn-0.3.7/src/gwatn/types/flo_params_brickstorageheater.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/flo_params_report.py` & `gridworks_atn-0.3.7/src/gwatn/types/flo_params_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/gt_dispatch_boolean.py` & `gridworks_atn-0.3.7/src/gwatn/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/hack_property_format.py` & `gridworks_atn-0.3.7/src/gwatn/types/hack_property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/hack_type_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/hack_type_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/hack_utils.py` & `gridworks_atn-0.3.7/src/gwatn/types/hack_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/heartbeat_b.py` & `gridworks_atn-0.3.7/src/gwatn/types/heartbeat_b.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/initial_tadeed_algo_create.py` & `gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/initial_tadeed_algo_optin.py` & `gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/initial_tadeed_algo_transfer.py` & `gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/join_dispatch_contract.py` & `gridworks_atn-0.3.7/src/gwatn/types/join_dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/latest_price.py` & `gridworks_atn-0.3.7/src/gwatn/types/latest_price.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/market_slot.py` & `gridworks_atn-0.3.7/src/gwatn/types/market_slot.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/market_type_gt.py` & `gridworks_atn-0.3.7/src/gwatn/types/market_type_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/new_tadeed_algo_optin.py` & `gridworks_atn-0.3.7/src/gwatn/types/new_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/new_tadeed_send.py` & `gridworks_atn-0.3.7/src/gwatn/types/new_tadeed_send.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/old_tadeed_algo_return.py` & `gridworks_atn-0.3.7/src/gwatn/types/old_tadeed_algo_return.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/price_quantity.py` & `gridworks_atn-0.3.7/src/gwatn/types/price_quantity.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/price_quantity_unitless.py` & `gridworks_atn-0.3.7/src/gwatn/types/price_quantity_unitless.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/scada_cert_transfer.py` & `gridworks_atn-0.3.7/src/gwatn/types/scada_cert_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/simplesim_driver_data.py` & `gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_data.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/simplesim_driver_data_bsh.py` & `gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_data_bsh.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/simplesim_driver_report.py` & `gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/simplesim_snapshot_brickstorageheater.py` & `gridworks_atn-0.3.7/src/gwatn/types/simplesim_snapshot_brickstorageheater.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/sla_enter.py` & `gridworks_atn-0.3.7/src/gwatn/types/sla_enter.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/tadeed_specs_hack.py` & `gridworks_atn-0.3.7/src/gwatn/types/tadeed_specs_hack.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/tavalidatorcert_algo_create.py` & `gridworks_atn-0.3.7/src/gwatn/types/tavalidatorcert_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/tavalidatorcert_algo_transfer.py` & `gridworks_atn-0.3.7/src/gwatn/types/tavalidatorcert_algo_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/terminalasset_certify_hack.py` & `gridworks_atn-0.3.7/src/gwatn/types/terminalasset_certify_hack.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py` & `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.6/PKG-INFO` & `gridworks_atn-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-atn
-Version: 0.3.6
+Version: 0.3.7
 Summary: Gridworks Atn Spaceheat
 Home-page: https://github.com/thegridelectric/gridworks-atn
 License: None
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

