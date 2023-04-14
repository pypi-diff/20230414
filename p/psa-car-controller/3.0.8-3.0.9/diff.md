# Comparing `tmp/psa_car_controller-3.0.8.tar.gz` & `tmp/psa_car_controller-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psa_car_controller-3.0.8.tar", max compression
+gzip compressed data, was "psa_car_controller-3.0.9.tar", max compression
```

## Comparing `psa_car_controller-3.0.8.tar` & `psa_car_controller-3.0.9.tar`

### file list

```diff
@@ -1,212 +1,211 @@
--rw-r--r--   0        0        0    35149 2023-01-09 22:27:43.504077 psa_car_controller-3.0.8/LICENSE
--rw-r--r--   0        0        0      138 2023-01-09 22:27:43.512077 psa_car_controller-3.0.8/psa_car_controller/__init__.py
--rwxr-xr-x   0        0        0      753 2023-01-09 22:27:43.512077 psa_car_controller-3.0.8/psa_car_controller/__main__.py
--rw-r--r--   0        0        0        0 2023-01-09 22:27:43.512077 psa_car_controller-3.0.8/psa_car_controller/common/__init__.py
--rw-r--r--   0        0        0     1802 2023-01-09 22:27:43.512077 psa_car_controller-3.0.8/psa_car_controller/common/mylogger.py
--rw-r--r--   0        0        0     1551 2023-01-09 22:27:43.512077 psa_car_controller-3.0.8/psa_car_controller/common/utils.py
--rw-r--r--   0        0        0      458 2023-01-09 22:27:43.512077 psa_car_controller-3.0.8/psa_car_controller/psa/AccountInformation.py
--rw-r--r--   0        0        0    12324 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/RemoteClient.py
--rw-r--r--   0        0        0      678 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/RemoteCredentials.py
--rw-r--r--   0        0        0        0 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/__init__.py
--rw-r--r--   0        0        0    13601 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/__init__.py
--rw-r--r--   0        0        0      319 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/api/__init__.py
--rw-r--r--   0        0        0   102100 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/api/trips_api.py
--rw-r--r--   0        0        0     4895 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/api/user_api.py
--rw-r--r--   0        0        0    81355 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/api/vehicles_api.py
--rw-r--r--   0        0        0    26152 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/api_client.py
--rw-r--r--   0        0        0     9746 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/configuration.py
--rw-r--r--   0        0        0    13204 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/__init__.py
--rw-r--r--   0        0        0    14820 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/adas.py
--rw-r--r--   0        0        0     5627 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/adas_park_assist.py
--rw-r--r--   0        0        0     9420 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alert.py
--rw-r--r--   0        0        0     3512 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alert_end_position.py
--rw-r--r--   0        0        0     5935 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alert_links.py
--rw-r--r--   0        0        0     7817 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alert_msg_enum.py
--rw-r--r--   0        0        0     4139 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alerts.py
--rw-r--r--   0        0        0     4153 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alerts_embedded.py
--rw-r--r--   0        0        0     4722 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/battery.py
--rw-r--r--   0        0        0     4546 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/bounded_program.py
--rw-r--r--   0        0        0     3699 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/charging_status_enum.py
--rw-r--r--   0        0        0     5092 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/circle_zone.py
--rw-r--r--   0        0        0     5020 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/circle_zone_coordinates.py
--rw-r--r--   0        0        0     7252 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collection_result.py
--rw-r--r--   0        0        0     9937 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collision.py
--rw-r--r--   0        0        0     5347 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collision_links.py
--rw-r--r--   0        0        0     8727 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collision_obj.py
--rw-r--r--   0        0        0     4434 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collision_obj_front.py
--rw-r--r--   0        0        0     4183 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collisions.py
--rw-r--r--   0        0        0     4277 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collisions_embedded.py
--rw-r--r--   0        0        0     4349 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/created_at_field.py
--rw-r--r--   0        0        0     6734 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/data_monitor_trigger.py
--rw-r--r--   0        0        0    11217 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/data_trigger.py
--rw-r--r--   0        0        0     5064 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/default_alert_push.py
--rw-r--r--   0        0        0     4984 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/default_alert_push_attributes.py
--rw-r--r--   0        0        0     6197 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/doors_state.py
--rw-r--r--   0        0        0     5478 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/doors_state_opening.py
--rw-r--r--   0        0        0     5417 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/e_coaching.py
--rw-r--r--   0        0        0     5347 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/e_coaching_links.py
--rw-r--r--   0        0        0     5871 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/e_coaching_scores.py
--rw-r--r--   0        0        0     9824 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/energy.py
--rw-r--r--   0        0        0     4982 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/energy_battery.py
--rw-r--r--   0        0        0     5286 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/energy_battery_health.py
--rw-r--r--   0        0        0     9612 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/energy_charging.py
--rw-r--r--   0        0        0     5435 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/engine.py
--rw-r--r--   0        0        0     4055 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/engine_oil.py
--rw-r--r--   0        0        0     5643 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/environment.py
--rw-r--r--   0        0        0     4128 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/environment_luminosity.py
--rw-r--r--   0        0        0     7583 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/event.py
--rw-r--r--   0        0        0     4079 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/event_links.py
--rw-r--r--   0        0        0     4802 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/extension.py
--rw-r--r--   0        0        0     3500 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/extension_type.py
--rw-r--r--   0        0        0     5295 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/geometry.py
--rw-r--r--   0        0        0     4329 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/ignition.py
--rw-r--r--   0        0        0     3488 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/index_range.py
--rw-r--r--   0        0        0     5945 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/kinetic.py
--rw-r--r--   0        0        0     5463 2023-01-09 22:27:43.516078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/lighting.py
--rw-r--r--   0        0        0     9859 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/link.py
--rw-r--r--   0        0        0     4209 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/maintenance.py
--rw-r--r--   0        0        0     5419 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/maintenance_links.py
--rw-r--r--   0        0        0     6315 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/maintenance_obj.py
--rw-r--r--   0        0        0     6172 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor.py
--rw-r--r--   0        0        0     3484 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_id.py
--rw-r--r--   0        0        0     4695 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_links.py
--rw-r--r--   0        0        0    10499 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_parameter.py
--rw-r--r--   0        0        0     8856 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_parameter_trigger_param.py
--rw-r--r--   0        0        0     4820 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_ref.py
--rw-r--r--   0        0        0     5444 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_ref_links.py
--rw-r--r--   0        0        0     3609 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_status.py
--rw-r--r--   0        0        0     4448 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_status_setter.py
--rw-r--r--   0        0        0     7349 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_subscribe.py
--rw-r--r--   0        0        0     5397 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_batch_notify.py
--rw-r--r--   0        0        0     7551 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_retry_policy.py
--rw-r--r--   0        0        0     6109 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_trigger.py
--rw-r--r--   0        0        0     6320 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_webhook.py
--rw-r--r--   0        0        0     6610 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_webhook_attributes.py
--rw-r--r--   0        0        0     4161 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitors.py
--rw-r--r--   0        0        0     4242 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitors_embedded.py
--rw-r--r--   0        0        0     4309 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/overall_autonomy.py
--rw-r--r--   0        0        0     4979 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/point.py
--rw-r--r--   0        0        0     5073 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/polygon_zone.py
--rw-r--r--   0        0        0     5682 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/position.py
--rw-r--r--   0        0        0     6993 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/position_properties.py
--rw-r--r--   0        0        0     4417 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/preconditioning.py
--rw-r--r--   0        0        0     7536 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/preconditioning_air_conditioning.py
--rw-r--r--   0        0        0     3536 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/preconditioning_program.py
--rw-r--r--   0        0        0     4339 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/privacy.py
--rw-r--r--   0        0        0     6995 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/program.py
--rw-r--r--   0        0        0     5226 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/program_occurence.py
--rw-r--r--   0        0        0     5810 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/safety.py
--rw-r--r--   0        0        0     5057 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/service_type.py
--rw-r--r--   0        0        0    13190 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/status.py
--rw-r--r--   0        0        0     4207 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/status_embedded.py
--rw-r--r--   0        0        0     3524 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/status_extension_type.py
--rw-r--r--   0        0        0     4723 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/status_links.py
--rw-r--r--   0        0        0     6339 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/tab_links.py
--rw-r--r--   0        0        0     4172 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry.py
--rw-r--r--   0        0        0     4310 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_embedded.py
--rw-r--r--   0        0        0     3500 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_enum.py
--rw-r--r--   0        0        0     6374 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_extension.py
--rw-r--r--   0        0        0     3536 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_extension_type.py
--rw-r--r--   0        0        0     7575 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message.py
--rw-r--r--   0        0        0     4314 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_embedded.py
--rw-r--r--   0        0        0    10914 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle.py
--rw-r--r--   0        0        0     4328 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_braking_system.py
--rw-r--r--   0        0        0     4434 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission.py
--rw-r--r--   0        0        0     5268 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox.py
--rw-r--r--   0        0        0     4790 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_gear.py
--rw-r--r--   0        0        0     5900 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_mode.py
--rw-r--r--   0        0        0     4784 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_monitor_trigger.py
--rw-r--r--   0        0        0     3484 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_range.py
--rw-r--r--   0        0        0     4199 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_stamped.py
--rw-r--r--   0        0        0     5591 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_trigger.py
--rw-r--r--   0        0        0     6021 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_zone_monitor_trigger.py
--rw-r--r--   0        0        0     5052 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_zone_trigger.py
--rw-r--r--   0        0        0    14784 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/trip.py
--rw-r--r--   0        0        0     5020 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/trip_avg_consumption.py
--rw-r--r--   0        0        0     5975 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/trip_links.py
--rw-r--r--   0        0        0     6658 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/trips.py
--rw-r--r--   0        0        0     4122 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/trips_embedded.py
--rw-r--r--   0        0        0     4333 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/updated_field.py
--rw-r--r--   0        0        0     3460 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/url.py
--rw-r--r--   0        0        0     7611 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/user.py
--rw-r--r--   0        0        0     4183 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/user_embedded.py
--rw-r--r--   0        0        0     4719 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/user_links.py
--rw-r--r--   0        0        0     3472 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vect2_d.py
--rw-r--r--   0        0        0     9581 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicle.py
--rw-r--r--   0        0        0     5494 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicle_engine.py
--rw-r--r--   0        0        0     8094 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicle_links.py
--rw-r--r--   0        0        0     5122 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicle_odometer.py
--rw-r--r--   0        0        0     4161 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicles.py
--rw-r--r--   0        0        0     4215 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicles_embedded.py
--rw-r--r--   0        0        0     4172 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/way_points.py
--rw-r--r--   0        0        0     5596 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/way_points_embedded.py
--rw-r--r--   0        0        0     5211 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/x_error.py
--rw-r--r--   0        0        0     5949 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/zone_monitor_trigger.py
--rw-r--r--   0        0        0     5507 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/zone_trigger.py
--rw-r--r--   0        0        0     5119 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/zone_trigger_place.py
--rw-r--r--   0        0        0     5137 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/zone_trigger_place_center.py
--rw-r--r--   0        0        0    14251 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/rest.py
--rw-r--r--   0        0        0     2138 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/constants.py
--rw-r--r--   0        0        0     1564 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/mqtt_request.py
--rw-r--r--   0        0        0     4279 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/oauth.py
--rw-r--r--   0        0        0        0 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/otp/__init__.py
--rw-r--r--   0        0        0     7320 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/otp/load.py
--rw-r--r--   0        0        0     2962 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/otp/oaep.py
--rw-r--r--   0        0        0    11574 2023-01-09 22:27:43.520078 psa_car_controller-3.0.8/psa_car_controller/psa/otp/otp.py
--rw-r--r--   0        0        0      876 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psa/otp/tokenizer.py
--rw-r--r--   0        0        0        0 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psa/setup/__init__.py
--rw-r--r--   0        0        0     2416 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psa/setup/apk_parser.py
--rwxr-xr-x   0        0        0     4485 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psa/setup/app_decoder.py
--rw-r--r--   0        0        0     1810 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psa/setup/github.py
--rw-r--r--   0        0        0        0 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/__init__.py
--rw-r--r--   0        0        0        0 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/application/__init__.py
--rw-r--r--   0        0        0     2533 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/application/abrp.py
--rw-r--r--   0        0        0     2624 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/application/battery_charge_curve.py
--rw-r--r--   0        0        0     5321 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/application/car_controller.py
--rw-r--r--   0        0        0     7216 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/application/charge_control.py
--rw-r--r--   0        0        0     4213 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/application/charging.py
--rw-r--r--   0        0        0     4991 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/application/ecomix.py
--rw-r--r--   0        0        0    10395 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/application/psa_client.py
--rw-r--r--   0        0        0     2747 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/application/trip_parser.py
--rw-r--r--   0        0        0        0 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/model/__init__.py
--rw-r--r--   0        0        0      186 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/model/battery_curve.py
--rw-r--r--   0        0        0     4435 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/model/car.py
--rw-r--r--   0        0        0     1178 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/model/car_model.py
--rw-r--r--   0        0        0     2806 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/model/car_status.py
--rw-r--r--   0        0        0      809 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/model/charge.py
--rw-r--r--   0        0        0     3746 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/model/trip.py
--rw-r--r--   0        0        0     1349 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/repository/car_model.py
--rw-r--r--   0        0        0     6844 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/repository/config_repository.py
--rw-r--r--   0        0        0    13186 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/repository/db.py
--rw-r--r--   0        0        0     7012 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/repository/trips.py
--rw-r--r--   0        0        0     5536 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/resources/car_models.yml
--rw-r--r--   0        0        0     1372 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/psacc/utils/utils.py
--rw-r--r--   0        0        0       18 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/__init__.py
--rw-r--r--   0        0        0     3281 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/app.py
--rw-r--r--   0        0        0     8418 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/clientside.js
--rw-r--r--   0        0        0     3588 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/images/battery-charge-line.svg
--rw-r--r--   0        0        0      295 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/images/battery-charge.svg
--rw-r--r--   0        0        0     3577 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/images/consumption.svg
--rw-r--r--   0        0        0     7480 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/images/electricity bill.svg
--rw-r--r--   0        0        0     2040 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/images/mileage.svg
--rw-r--r--   0        0        0     3094 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/images/pollution.svg
--rw-r--r--   0        0        0     1070 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/images/settings.svg
--rw-r--r--   0        0        0      582 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/images/sync.svg
--rw-r--r--   0        0        0    26505 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/sprites/osm-liberty.json
--rw-r--r--   0        0        0   103877 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/sprites/osm-liberty.png
--rw-r--r--   0        0        0    26581 2023-01-09 22:27:43.524078 psa_car_controller-3.0.8/psa_car_controller/web/assets/sprites/osm-liberty@2x.json
--rw-r--r--   0        0        0   202875 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/assets/sprites/osm-liberty@2x.png
--rw-r--r--   0        0        0      908 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/assets/style.json
--rw-r--r--   0        0        0     1238 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/dash_custom.py
--rw-r--r--   0        0        0     8787 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/figures.py
--rw-r--r--   0        0        0     1568 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/tools/Button.py
--rw-r--r--   0        0        0     1030 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/tools/Switch.py
--rw-r--r--   0        0        0     4876 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/tools/figurefilter.py
--rw-r--r--   0        0        0     3030 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/tools/utils.py
--rw-r--r--   0        0        0        0 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/view/__init__.py
--rw-r--r--   0        0        0     6793 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/view/config_views.py
--rw-r--r--   0        0        0     3233 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/view/control.py
--rw-r--r--   0        0        0    17501 2023-01-09 22:27:43.528078 psa_car_controller-3.0.8/psa_car_controller/web/view/views.py
--rw-r--r--   0        0        0     1455 2023-01-09 22:28:03.208239 psa_car_controller-3.0.8/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 psa_car_controller-3.0.8/setup.py
--rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 psa_car_controller-3.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-13 07:09:29.036944 psa_car_controller-3.0.9/LICENSE
+-rw-r--r--   0        0        0      138 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/__init__.py
+-rwxr-xr-x   0        0        0      753 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/common/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/common/mylogger.py
+-rw-r--r--   0        0        0     1551 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/common/utils.py
+-rw-r--r--   0        0        0      458 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/psa/AccountInformation.py
+-rw-r--r--   0        0        0    12324 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/psa/RemoteClient.py
+-rw-r--r--   0        0        0      678 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/psa/RemoteCredentials.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/psa/__init__.py
+-rw-r--r--   0        0        0    13601 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/__init__.py
+-rw-r--r--   0        0        0      319 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/api/__init__.py
+-rw-r--r--   0        0        0   102100 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/api/trips_api.py
+-rw-r--r--   0        0        0     4895 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/api/user_api.py
+-rw-r--r--   0        0        0    81355 2023-04-13 07:09:29.044944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/api/vehicles_api.py
+-rw-r--r--   0        0        0    26152 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/api_client.py
+-rw-r--r--   0        0        0     9746 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/configuration.py
+-rw-r--r--   0        0        0    13204 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/__init__.py
+-rw-r--r--   0        0        0    14820 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/adas.py
+-rw-r--r--   0        0        0     5627 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/adas_park_assist.py
+-rw-r--r--   0        0        0     9420 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alert.py
+-rw-r--r--   0        0        0     3512 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alert_end_position.py
+-rw-r--r--   0        0        0     5935 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alert_links.py
+-rw-r--r--   0        0        0     7817 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alert_msg_enum.py
+-rw-r--r--   0        0        0     4139 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alerts.py
+-rw-r--r--   0        0        0     4153 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alerts_embedded.py
+-rw-r--r--   0        0        0     4722 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/battery.py
+-rw-r--r--   0        0        0     4546 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/bounded_program.py
+-rw-r--r--   0        0        0     3699 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/charging_status_enum.py
+-rw-r--r--   0        0        0     5092 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/circle_zone.py
+-rw-r--r--   0        0        0     5020 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/circle_zone_coordinates.py
+-rw-r--r--   0        0        0     7252 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collection_result.py
+-rw-r--r--   0        0        0     9937 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collision.py
+-rw-r--r--   0        0        0     5347 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collision_links.py
+-rw-r--r--   0        0        0     8727 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collision_obj.py
+-rw-r--r--   0        0        0     4434 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collision_obj_front.py
+-rw-r--r--   0        0        0     4183 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collisions.py
+-rw-r--r--   0        0        0     4277 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collisions_embedded.py
+-rw-r--r--   0        0        0     4349 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/created_at_field.py
+-rw-r--r--   0        0        0     6734 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/data_monitor_trigger.py
+-rw-r--r--   0        0        0    11217 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/data_trigger.py
+-rw-r--r--   0        0        0     5064 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/default_alert_push.py
+-rw-r--r--   0        0        0     4984 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/default_alert_push_attributes.py
+-rw-r--r--   0        0        0     6197 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/doors_state.py
+-rw-r--r--   0        0        0     5478 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/doors_state_opening.py
+-rw-r--r--   0        0        0     5417 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/e_coaching.py
+-rw-r--r--   0        0        0     5347 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/e_coaching_links.py
+-rw-r--r--   0        0        0     5871 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/e_coaching_scores.py
+-rw-r--r--   0        0        0     9824 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/energy.py
+-rw-r--r--   0        0        0     4982 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/energy_battery.py
+-rw-r--r--   0        0        0     5286 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/energy_battery_health.py
+-rw-r--r--   0        0        0     9612 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/energy_charging.py
+-rw-r--r--   0        0        0     5435 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/engine.py
+-rw-r--r--   0        0        0     4055 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/engine_oil.py
+-rw-r--r--   0        0        0     5643 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/environment.py
+-rw-r--r--   0        0        0     4128 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/environment_luminosity.py
+-rw-r--r--   0        0        0     7583 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/event.py
+-rw-r--r--   0        0        0     4079 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/event_links.py
+-rw-r--r--   0        0        0     4802 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/extension.py
+-rw-r--r--   0        0        0     3500 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/extension_type.py
+-rw-r--r--   0        0        0     5295 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/geometry.py
+-rw-r--r--   0        0        0     4329 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/ignition.py
+-rw-r--r--   0        0        0     3488 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/index_range.py
+-rw-r--r--   0        0        0     5945 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/kinetic.py
+-rw-r--r--   0        0        0     5463 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/lighting.py
+-rw-r--r--   0        0        0     9859 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/link.py
+-rw-r--r--   0        0        0     4209 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/maintenance.py
+-rw-r--r--   0        0        0     5419 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/maintenance_links.py
+-rw-r--r--   0        0        0     6315 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/maintenance_obj.py
+-rw-r--r--   0        0        0     6172 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor.py
+-rw-r--r--   0        0        0     3484 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_id.py
+-rw-r--r--   0        0        0     4695 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_links.py
+-rw-r--r--   0        0        0    10499 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_parameter.py
+-rw-r--r--   0        0        0     8856 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_parameter_trigger_param.py
+-rw-r--r--   0        0        0     4820 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_ref.py
+-rw-r--r--   0        0        0     5444 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_ref_links.py
+-rw-r--r--   0        0        0     3609 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_status.py
+-rw-r--r--   0        0        0     4448 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_status_setter.py
+-rw-r--r--   0        0        0     7349 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_subscribe.py
+-rw-r--r--   0        0        0     5397 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_batch_notify.py
+-rw-r--r--   0        0        0     7551 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_retry_policy.py
+-rw-r--r--   0        0        0     6109 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_trigger.py
+-rw-r--r--   0        0        0     6320 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_webhook.py
+-rw-r--r--   0        0        0     6610 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_webhook_attributes.py
+-rw-r--r--   0        0        0     4161 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitors.py
+-rw-r--r--   0        0        0     4242 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitors_embedded.py
+-rw-r--r--   0        0        0     4309 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/overall_autonomy.py
+-rw-r--r--   0        0        0     4979 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/point.py
+-rw-r--r--   0        0        0     5073 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/polygon_zone.py
+-rw-r--r--   0        0        0     5682 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/position.py
+-rw-r--r--   0        0        0     6994 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/position_properties.py
+-rw-r--r--   0        0        0     4417 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/preconditioning.py
+-rw-r--r--   0        0        0     7536 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/preconditioning_air_conditioning.py
+-rw-r--r--   0        0        0     3536 2023-04-13 07:09:29.048944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/preconditioning_program.py
+-rw-r--r--   0        0        0     4339 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/privacy.py
+-rw-r--r--   0        0        0     6995 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/program.py
+-rw-r--r--   0        0        0     5226 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/program_occurence.py
+-rw-r--r--   0        0        0     5810 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/safety.py
+-rw-r--r--   0        0        0     5057 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/service_type.py
+-rw-r--r--   0        0        0    13190 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/status.py
+-rw-r--r--   0        0        0     4207 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/status_embedded.py
+-rw-r--r--   0        0        0     3524 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/status_extension_type.py
+-rw-r--r--   0        0        0     4723 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/status_links.py
+-rw-r--r--   0        0        0     6339 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/tab_links.py
+-rw-r--r--   0        0        0     4172 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry.py
+-rw-r--r--   0        0        0     4310 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_embedded.py
+-rw-r--r--   0        0        0     3500 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_enum.py
+-rw-r--r--   0        0        0     6374 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_extension.py
+-rw-r--r--   0        0        0     3536 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_extension_type.py
+-rw-r--r--   0        0        0     7575 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message.py
+-rw-r--r--   0        0        0     4314 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_embedded.py
+-rw-r--r--   0        0        0    10914 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle.py
+-rw-r--r--   0        0        0     4328 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_braking_system.py
+-rw-r--r--   0        0        0     4434 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission.py
+-rw-r--r--   0        0        0     5268 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox.py
+-rw-r--r--   0        0        0     4790 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_gear.py
+-rw-r--r--   0        0        0     5900 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_mode.py
+-rw-r--r--   0        0        0     4784 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_monitor_trigger.py
+-rw-r--r--   0        0        0     3484 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_range.py
+-rw-r--r--   0        0        0     4199 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_stamped.py
+-rw-r--r--   0        0        0     5591 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_trigger.py
+-rw-r--r--   0        0        0     6021 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_zone_monitor_trigger.py
+-rw-r--r--   0        0        0     5052 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_zone_trigger.py
+-rw-r--r--   0        0        0    14784 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/trip.py
+-rw-r--r--   0        0        0     5020 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/trip_avg_consumption.py
+-rw-r--r--   0        0        0     5975 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/trip_links.py
+-rw-r--r--   0        0        0     6658 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/trips.py
+-rw-r--r--   0        0        0     4122 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/trips_embedded.py
+-rw-r--r--   0        0        0     4333 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/updated_field.py
+-rw-r--r--   0        0        0     3460 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/url.py
+-rw-r--r--   0        0        0     7611 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/user.py
+-rw-r--r--   0        0        0     4183 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/user_embedded.py
+-rw-r--r--   0        0        0     4719 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/user_links.py
+-rw-r--r--   0        0        0     3472 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vect2_d.py
+-rw-r--r--   0        0        0     9581 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicle.py
+-rw-r--r--   0        0        0     5494 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicle_engine.py
+-rw-r--r--   0        0        0     8094 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicle_links.py
+-rw-r--r--   0        0        0     5122 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicle_odometer.py
+-rw-r--r--   0        0        0     4161 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicles.py
+-rw-r--r--   0        0        0     4215 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicles_embedded.py
+-rw-r--r--   0        0        0     4172 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/way_points.py
+-rw-r--r--   0        0        0     5596 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/way_points_embedded.py
+-rw-r--r--   0        0        0     5211 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/x_error.py
+-rw-r--r--   0        0        0     5949 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/zone_monitor_trigger.py
+-rw-r--r--   0        0        0     5507 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/zone_trigger.py
+-rw-r--r--   0        0        0     5119 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/zone_trigger_place.py
+-rw-r--r--   0        0        0     5137 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/zone_trigger_place_center.py
+-rw-r--r--   0        0        0    14251 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/rest.py
+-rw-r--r--   0        0        0     2138 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/constants.py
+-rw-r--r--   0        0        0     1564 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/mqtt_request.py
+-rw-r--r--   0        0        0     4279 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/oauth.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/otp/__init__.py
+-rw-r--r--   0        0        0     7320 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/otp/load.py
+-rw-r--r--   0        0        0     2962 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/otp/oaep.py
+-rw-r--r--   0        0        0    11574 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/otp/otp.py
+-rw-r--r--   0        0        0      876 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/otp/tokenizer.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/setup/__init__.py
+-rw-r--r--   0        0        0     2416 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/setup/apk_parser.py
+-rwxr-xr-x   0        0        0     4485 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/setup/app_decoder.py
+-rw-r--r--   0        0        0     1810 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psa/setup/github.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/application/__init__.py
+-rw-r--r--   0        0        0     2533 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/application/abrp.py
+-rw-r--r--   0        0        0     2624 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/application/battery_charge_curve.py
+-rw-r--r--   0        0        0     5321 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/application/car_controller.py
+-rw-r--r--   0        0        0     7216 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/application/charge_control.py
+-rw-r--r--   0        0        0     4213 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/application/charging.py
+-rw-r--r--   0        0        0     4991 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/application/ecomix.py
+-rw-r--r--   0        0        0    10395 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/application/psa_client.py
+-rw-r--r--   0        0        0     2747 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/application/trip_parser.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/model/__init__.py
+-rw-r--r--   0        0        0      186 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/model/battery_curve.py
+-rw-r--r--   0        0        0     4435 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/model/car.py
+-rw-r--r--   0        0        0     1178 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/model/car_model.py
+-rw-r--r--   0        0        0     2806 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/model/car_status.py
+-rw-r--r--   0        0        0      809 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/model/charge.py
+-rw-r--r--   0        0        0     3746 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/model/trip.py
+-rw-r--r--   0        0        0     1349 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/repository/car_model.py
+-rw-r--r--   0        0        0     6844 2023-04-13 07:09:29.052944 psa_car_controller-3.0.9/psa_car_controller/psacc/repository/config_repository.py
+-rw-r--r--   0        0        0    13186 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/psacc/repository/db.py
+-rw-r--r--   0        0        0     7012 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/psacc/repository/trips.py
+-rw-r--r--   0        0        0     6630 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/psacc/resources/car_models.yml
+-rw-r--r--   0        0        0     1372 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/psacc/utils/utils.py
+-rw-r--r--   0        0        0       18 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/__init__.py
+-rw-r--r--   0        0        0     3281 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/app.py
+-rw-r--r--   0        0        0     8418 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/clientside.js
+-rw-r--r--   0        0        0     3588 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/images/battery-charge-line.svg
+-rw-r--r--   0        0        0      295 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/images/battery-charge.svg
+-rw-r--r--   0        0        0     3577 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/images/consumption.svg
+-rw-r--r--   0        0        0     7480 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/images/electricity bill.svg
+-rw-r--r--   0        0        0     2040 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/images/mileage.svg
+-rw-r--r--   0        0        0     3094 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/images/pollution.svg
+-rw-r--r--   0        0        0     1070 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/images/settings.svg
+-rw-r--r--   0        0        0      582 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/images/sync.svg
+-rw-r--r--   0        0        0    26505 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/sprites/osm-liberty.json
+-rw-r--r--   0        0        0   103877 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/sprites/osm-liberty.png
+-rw-r--r--   0        0        0    26581 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/sprites/osm-liberty@2x.json
+-rw-r--r--   0        0        0   202875 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/sprites/osm-liberty@2x.png
+-rw-r--r--   0        0        0      908 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/assets/style.json
+-rw-r--r--   0        0        0     1238 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/dash_custom.py
+-rw-r--r--   0        0        0     8787 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/figures.py
+-rw-r--r--   0        0        0     1568 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/tools/Button.py
+-rw-r--r--   0        0        0     1030 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/tools/Switch.py
+-rw-r--r--   0        0        0     4876 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/tools/figurefilter.py
+-rw-r--r--   0        0        0     3030 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/tools/utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/view/__init__.py
+-rw-r--r--   0        0        0     6793 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/view/config_views.py
+-rw-r--r--   0        0        0     3233 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/view/control.py
+-rw-r--r--   0        0        0    17501 2023-04-13 07:09:29.056944 psa_car_controller-3.0.9/psa_car_controller/web/view/views.py
+-rw-r--r--   0        0        0     1455 2023-04-13 07:09:49.767215 psa_car_controller-3.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 psa_car_controller-3.0.9/PKG-INFO
```

### Comparing `psa_car_controller-3.0.8/LICENSE` & `psa_car_controller-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/__main__.py` & `psa_car_controller-3.0.9/psa_car_controller/__main__.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/common/mylogger.py` & `psa_car_controller-3.0.9/psa_car_controller/common/mylogger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/common/utils.py` & `psa_car_controller-3.0.9/psa_car_controller/common/utils.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/RemoteClient.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/RemoteClient.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/RemoteCredentials.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/RemoteCredentials.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/__init__.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/__init__.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/api/trips_api.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/api/trips_api.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/api/user_api.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/api/user_api.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/api/vehicles_api.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/api/vehicles_api.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/api_client.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/api_client.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/configuration.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/configuration.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/__init__.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/adas.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/adas.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/adas_park_assist.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/adas_park_assist.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alert.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alert.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alert_end_position.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alert_end_position.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alert_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alert_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alert_msg_enum.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alert_msg_enum.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alerts.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alerts.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/alerts_embedded.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/alerts_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/battery.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/battery.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/bounded_program.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/bounded_program.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/charging_status_enum.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/charging_status_enum.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/circle_zone.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/circle_zone.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/circle_zone_coordinates.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/circle_zone_coordinates.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collection_result.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collection_result.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collision.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collision.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collision_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collision_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collision_obj.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collision_obj.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collision_obj_front.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collision_obj_front.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collisions.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collisions.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/collisions_embedded.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/collisions_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/created_at_field.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/created_at_field.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/data_monitor_trigger.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/data_monitor_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/data_trigger.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/data_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/default_alert_push.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/default_alert_push.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/default_alert_push_attributes.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/default_alert_push_attributes.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/doors_state.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/doors_state.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/doors_state_opening.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/doors_state_opening.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/e_coaching.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/e_coaching.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/e_coaching_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/e_coaching_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/e_coaching_scores.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/e_coaching_scores.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/energy.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/energy.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/energy_battery.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/energy_battery.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/energy_battery_health.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/energy_battery_health.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/energy_charging.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/energy_charging.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/engine.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/engine.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/engine_oil.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/engine_oil.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/environment.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/environment.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/environment_luminosity.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/environment_luminosity.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/event.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/event.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/event_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/event_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/extension.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/extension.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/extension_type.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/extension_type.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/geometry.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/geometry.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/ignition.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/ignition.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/index_range.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/index_range.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/kinetic.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/kinetic.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/lighting.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/lighting.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/link.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/link.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/maintenance.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/maintenance.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/maintenance_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/maintenance_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/maintenance_obj.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/maintenance_obj.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_id.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_id.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_parameter.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_parameter.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_parameter_trigger_param.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_parameter_trigger_param.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_ref.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_ref.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_ref_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_ref_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_status.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_status.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_status_setter.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_status_setter.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_subscribe.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_subscribe.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_batch_notify.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_batch_notify.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_retry_policy.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_retry_policy.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_trigger.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_webhook.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_webhook.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitor_webhook_attributes.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitor_webhook_attributes.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitors.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitors.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/monitors_embedded.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/monitors_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/overall_autonomy.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/overall_autonomy.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/point.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/point.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/polygon_zone.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/polygon_zone.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/position.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/position.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/position_properties.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/position_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     def type(self, type):
         """Sets the type of this PositionProperties.
 
 
         :param type: The type of this PositionProperties.  # noqa: E501
         :type: str
         """
-        allowed_values = ["Estimated", "Acquired", "Estimate", "Aquire"]  # noqa: E501
+        allowed_values = ["Estimated", "Acquired", "Estimate", "Acquire"]  # noqa: E501
         if type not in allowed_values:
             raise ValueError(
                 "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
                 .format(type, allowed_values)
             )
 
         self._type = type
```

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/preconditioning.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/preconditioning.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/preconditioning_air_conditioning.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/preconditioning_air_conditioning.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/preconditioning_program.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/preconditioning_program.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/privacy.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/privacy.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/program.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/program.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/program_occurence.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/program_occurence.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/safety.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/safety.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/service_type.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/service_type.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/status.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/status.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/status_embedded.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/status_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/status_extension_type.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/status_extension_type.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/status_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/status_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/tab_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/tab_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_embedded.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_enum.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_enum.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_extension.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_extension.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_extension_type.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_extension_type.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_embedded.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_braking_system.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_braking_system.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_gear.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_gear.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_mode.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_mode.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_monitor_trigger.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_monitor_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_range.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_range.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_stamped.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_stamped.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_trigger.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_zone_monitor_trigger.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_zone_monitor_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/time_zone_trigger.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/time_zone_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/trip.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/trip.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/trip_avg_consumption.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/trip_avg_consumption.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/trip_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/trip_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/trips.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/trips.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/trips_embedded.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/trips_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/updated_field.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/updated_field.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/url.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/url.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/user.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/user.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/user_embedded.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/user_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/user_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/user_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vect2_d.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vect2_d.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicle.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicle.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicle_engine.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicle_engine.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicle_links.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicle_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicle_odometer.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicle_odometer.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicles.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicles.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/vehicles_embedded.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/vehicles_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/way_points.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/way_points.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/way_points_embedded.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/way_points_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/x_error.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/x_error.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/zone_monitor_trigger.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/zone_monitor_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/zone_trigger.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/zone_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/zone_trigger_place.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/zone_trigger_place.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/models/zone_trigger_place_center.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/models/zone_trigger_place_center.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/connected_car_api/rest.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/connected_car_api/rest.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/constants.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/constants.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/mqtt_request.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/mqtt_request.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/oauth.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/oauth.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/otp/load.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/otp/load.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/otp/oaep.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/otp/oaep.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/otp/otp.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/otp/otp.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/otp/tokenizer.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/otp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/setup/apk_parser.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/setup/apk_parser.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/setup/app_decoder.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/setup/app_decoder.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psa/setup/github.py` & `psa_car_controller-3.0.9/psa_car_controller/psa/setup/github.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/application/abrp.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/application/abrp.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/application/battery_charge_curve.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/application/battery_charge_curve.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/application/car_controller.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/application/car_controller.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/application/charge_control.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/application/charge_control.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/application/charging.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/application/charging.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/application/ecomix.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/application/ecomix.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/application/psa_client.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/application/psa_client.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/application/trip_parser.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/application/trip_parser.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/model/car.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/model/car.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/model/car_model.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/model/car_model.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/model/car_status.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/model/car_status.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/model/charge.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/model/charge.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/model/trip.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/model/trip.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/repository/car_model.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/repository/car_model.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/repository/config_repository.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/repository/config_repository.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/repository/db.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/repository/db.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/repository/trips.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/repository/trips.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/resources/car_models.yml` & `psa_car_controller-3.0.9/psa_car_controller/psacc/resources/car_models.yml`

 * *Files 9% similar despite different names*

```diff
@@ -78,14 +78,21 @@
 - !ElecModel
   name: e-Rifter
   battery_power: 45
   fuel_capacity: 0
   abrp_name: opel:comboe:22:50:peugeot
   reg: VR3EZZKXZ.*
   max_elec_consumption: 70
+- !ElecModel
+  name: ION
+  battery_power: 14.5
+  fuel_capacity: 0
+  abrp_name: peugeot:ion:12:14:other
+  reg: VF31NZKY.*
+  max_elec_consumption: 70
 - !CarModel
   name: SUV 3008 Hybrid 225
   battery_power: 13.2
   fuel_capacity: 43
   abrp_name:
   reg: VF3M4DGZ.*
   max_elec_consumption: 70
@@ -111,22 +118,38 @@
   battery_power: 0
   fuel_capacity: 44
   abrp_name:
   reg: VR3UPHN[SEK].*
   max_elec_consumption: 70
   max_fuel_consumption: 30
 - !CarModel
+  name: '208'
+  battery_power: 0
+  fuel_capacity: 44
+  abrp_name:
+  reg: VF3CCBHY6H.*
+  max_elec_consumption: 70
+  max_fuel_consumption: 30
+- !CarModel
   name: '2008'
   battery_power: 0
   fuel_capacity: 44
   abrp_name:
   reg: VR3USHNS.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
 - !CarModel
+  name: '2008'
+  battery_power: 0
+  fuel_capacity: 44
+  abrp_name:
+  reg: VF3CU9HP.*
+  max_elec_consumption: 70
+  max_fuel_consumption: 30
+- !CarModel
   name: 2008 II
   battery_power: 0
   fuel_capacity: 45
   abrp_name:
   reg: VR3USHNK.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
@@ -139,15 +162,23 @@
   max_elec_consumption: 70
   max_fuel_consumption: 30
 - !CarModel
   name: SUV 5008 II 2018
   battery_power: 0
   fuel_capacity: 56
   abrp_name:
-  reg: VF3MRHNY.*
+  reg: VF3MRHNYHH.*
+  max_elec_consumption: 70
+  max_fuel_consumption: 30
+- !CarModel
+  name: SUV 3008 II
+  battery_power: 0
+  fuel_capacity: 53
+  abrp_name:
+  reg: VF3MRHNYHJ.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
 - !CarModel
   name: N5008 GT-LINE 1.6L
   battery_power: 0
   fuel_capacity: 60
   abrp_name:
@@ -223,14 +254,22 @@
   battery_power: 0
   fuel_capacity: 45
   abrp_name:
   reg: VF72RHNPXK.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
 - !CarModel
+  name: 308 Hybrid
+  battery_power: 12.4
+  fuel_capacity: 40
+  abrp_name:
+  reg: VR3F3DGYT.*
+  max_elec_consumption: 70
+  max_fuel_consumption: 30
+- !CarModel
   name: 308 SW Hybrid
   battery_power: 12.4
   fuel_capacity: 40
   abrp_name:
   reg: VR3F4DGYTN.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
@@ -261,7 +300,23 @@
   name: Astra L Hybrid
   battery_power: 12.4
   fuel_capacity: 42
   abrp_name:
   reg: VXKF3DGXTN.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
+- !CarModel
+  name: 308 SW Hybrid
+  battery_power: 12.4
+  fuel_capacity: 40
+  abrp_name:
+  reg: VR3F4DGXTN.*
+  max_elec_consumption: 70
+  max_fuel_consumption: 30
+- !CarModel
+  name: DS4 E-Tense
+  battery_power: 12.4
+  fuel_capacity: 40
+  abrp_name:
+  reg: VR1F4DGYTM.*
+  max_elec_consumption: 70
+  max_fuel_consumption: 30
```

### Comparing `psa_car_controller-3.0.8/psa_car_controller/psacc/utils/utils.py` & `psa_car_controller-3.0.9/psa_car_controller/psacc/utils/utils.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/app.py` & `psa_car_controller-3.0.9/psa_car_controller/web/app.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/clientside.js` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/clientside.js`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/images/battery-charge-line.svg` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/images/battery-charge-line.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/images/consumption.svg` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/images/consumption.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/images/electricity bill.svg` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/images/electricity bill.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/images/mileage.svg` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/images/mileage.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/images/pollution.svg` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/images/pollution.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/images/settings.svg` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/images/settings.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/images/sync.svg` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/images/sync.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/sprites/osm-liberty.json` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/sprites/osm-liberty.json`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/sprites/osm-liberty.png` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/sprites/osm-liberty.png`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/sprites/osm-liberty@2x.json` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/sprites/osm-liberty@2x.json`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/sprites/osm-liberty@2x.png` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/sprites/osm-liberty@2x.png`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/assets/style.json` & `psa_car_controller-3.0.9/psa_car_controller/web/assets/style.json`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/dash_custom.py` & `psa_car_controller-3.0.9/psa_car_controller/web/dash_custom.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/figures.py` & `psa_car_controller-3.0.9/psa_car_controller/web/figures.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/tools/Button.py` & `psa_car_controller-3.0.9/psa_car_controller/web/tools/Button.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/tools/Switch.py` & `psa_car_controller-3.0.9/psa_car_controller/web/tools/Switch.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/tools/figurefilter.py` & `psa_car_controller-3.0.9/psa_car_controller/web/tools/figurefilter.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/tools/utils.py` & `psa_car_controller-3.0.9/psa_car_controller/web/tools/utils.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/view/config_views.py` & `psa_car_controller-3.0.9/psa_car_controller/web/view/config_views.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/view/control.py` & `psa_car_controller-3.0.9/psa_car_controller/web/view/control.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/psa_car_controller/web/view/views.py` & `psa_car_controller-3.0.9/psa_car_controller/web/view/views.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.0.8/pyproject.toml` & `psa_car_controller-3.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psa-car-controller"
-version = "v3.0.8"
+version = "v3.0.9"
 description = "This is a python program to control a psa car with connected_car v4 api."
 authors = ["Florian Bezannier <florian.bezannier@hotmail.fr>"]
 license = "GPL-3.0"
 homepage = "https://github.com/flobz/psa_car_controller"
 repository = "https://github.com/flobz/psa_car_controller"
 include = [
     "LICENSE",
```

### Comparing `psa_car_controller-3.0.8/PKG-INFO` & `psa_car_controller-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psa-car-controller
-Version: 3.0.8
+Version: 3.0.9
 Summary: This is a python program to control a psa car with connected_car v4 api.
 Home-page: https://github.com/flobz/psa_car_controller
 License: GPL-3.0
 Author: Florian Bezannier
 Author-email: florian.bezannier@hotmail.fr
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

