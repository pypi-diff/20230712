# Comparing `tmp/aiovantage-0.7.0.tar.gz` & `tmp/aiovantage-0.8.0.tar.gz`

## Comparing `aiovantage-0.7.0.tar` & `aiovantage-0.8.0.tar`

### file list

```diff
@@ -1,158 +1,164 @@
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.pylintrc
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 aiovantage-0.7.0/TODO
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.vscode/settings.json
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/dump_system.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/monitor_all.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/anemo_sensors/dump_anemo_sensors.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/anemo_sensors/monitor_anemo_sensors.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/areas/dump_areas.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/blind_groups/dump_blind_groups.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/blinds/dump_blinds.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/blinds/monitor_blinds.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/buttons/dump_buttons.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/buttons/monitor_buttons.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/command_client/event_log.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/command_client/status_load.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/config_client/dump_objects.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/config_client/get_version.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/gmem/dump_gmem.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/gmem/monitor_gmem.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/gmem/set_gmem.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/light_sensors/dump_light_sensors.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/light_sensors/monitor_light_sensors.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/load_groups/dump_load_groups.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/load_groups/monitor_load_groups.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/loads/control_load.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/loads/dump_loads.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/loads/monitor_loads.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/loads/poll_on_loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/loads/toggle_load.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/masters/dump_masters.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/masters/monitor_masters.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/omni_sensors/monitor_omni_sensors.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/rgb_loads/monitor_rgb_loads.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/stations/dump_stations.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/stations/jingle_bells.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/tasks/dump_tasks.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/tasks/run_task.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/temperature_sensors/dump_temperature_sensors.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aiovantage-0.7.0/examples/temperature_sensors/monitor_temperature_sensors.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/__about__.py
--rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/__init__.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/connection.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/discovery.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/errors.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/py.typed
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/query.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/__init__.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/commands.py
--rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/events.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/utils.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/light_sensor.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/sounder.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/command_client/interfaces/temperature.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/README.md
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/__init__.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/helpers.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/xml_dataclass.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/types.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/open_filter.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/introspection/get_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/methods/login/login.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/module.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/module_gen2.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/somfy/rs485_group.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/somfy/rs485_shade.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/somfy/urtsi_2_group.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/config_client/objects/somfy/urtsi_2_shade.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/anemo_sensors.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/areas.py
--rw-r--r--   0        0        0    13315 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/base.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/blinds.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/buttons.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/gmem.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/light_sensors.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/loads.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/masters.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/modules.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/stations.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/tasks.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 aiovantage-0.7.0/src/aiovantage/controllers/temperature_sensors.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.7.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.7.0/LICENSE
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 aiovantage-0.7.0/README.md
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 aiovantage-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 aiovantage-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.pylintrc
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 aiovantage-0.8.0/TODO
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.vscode/settings.json
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/dump_system.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/monitor_all.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/anemo_sensors/dump_anemo_sensors.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/anemo_sensors/monitor_anemo_sensors.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/light_sensors/dump_light_sensors.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/light_sensors/monitor_light_sensors.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/load_groups/monitor_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/masters/dump_masters.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/masters/monitor_masters.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/stations/jingle_bells.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/tasks/run_task.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/temperature_sensors/dump_temperature_sensors.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 aiovantage-0.8.0/examples/temperature_sensors/monitor_temperature_sensors.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     9185 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/connection.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/discovery.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/errors.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/events.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/commands.py
+-rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/light_sensor.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/sounder.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/command_client/interfaces/temperature.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/requests.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/close_filter.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/get_object.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/introspection/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/login/__init__.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/interfaces/login/login.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/area.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/blind.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/blind_base.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/blind_group.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/blind_group_base.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/button.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/child_device.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/child_object.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/custom_device.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/dc_power_profile.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/dimmer.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/eq_ux.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/gmem.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/keypad.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/light_sensor.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/load.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/load_group.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/location_object.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/master.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/module.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/module_gen2.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/omni_sensor.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/pwm_power_profile.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/qis_blind.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/qube_blind.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/relay_blind.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/rgb_load_base.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/scene_point_relay.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/sensor.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/somfy_rs_485_group_child.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/somfy_rs_485_shade_child.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/somfy_urtsi_2_group_child.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/somfy_urtsi_2_shade_child.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/station_bus.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/station_object.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/system_object.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/task.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/temperature.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/vantage_ddg_color_load.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/vantage_dg_color_load.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/config_client/models/vantage_dmx_dali_gateway.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/anemo_sensors.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/light_sensors.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/modules.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aiovantage-0.8.0/src/aiovantage/controllers/temperature_sensors.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.8.0/LICENSE
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 aiovantage-0.8.0/README.md
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 aiovantage-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 aiovantage-0.8.0/PKG-INFO
```

### Comparing `aiovantage-0.7.0/.pre-commit-config.yaml` & `aiovantage-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/CONTRIBUTING.md` & `aiovantage-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/TODO` & `aiovantage-0.8.0/TODO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # TODO
 
 - Add `Vantage.DmxDaliGateway` as a Station
 - Cleanup "ELAGG", etc subscriptions on shutdown to avoid memory leaks on the controller
 - Look into pointing xsdata to a module to parse objects
   - <https://xsdata.readthedocs.io/en/latest/models.html#type-wildcard>
-- Consider moving system objects to a top-level "models" module
 - Consider grouping like-objects into a single file, eg all stations into station.py
 - Consider grouped controllers like aiohue, eg. for sensors, loads, etc.
-- Consider renaming config_client/methods to config_client/interfaces and flattening
 - Consider renaming GMemController to VariablesController, MastersController to ControllersController
-- Consider retiring xml_dataclass.py in favor of pure dataclasses
 - Sphinx docs / readthedocs
 - Smarter fetching of objects?
   - Eg. combine multiple requests into one
   - Eg. If we request 50 and get < 50 don't make another request
 - Consider "ctypes" style rpc for command_client INVOKE methods
   - Potentially move calls back into controllers
```

### Comparing `aiovantage-0.7.0/.github/ISSUE_TEMPLATE/bug.yml` & `aiovantage-0.8.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `aiovantage-0.8.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/dump_system.py` & `aiovantage-0.8.0/examples/dump_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Optional
 
 from aiovantage import Vantage
-from aiovantage.config_client.objects import Area, Load
+from aiovantage.models import Area, Load
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/monitor_all.py` & `aiovantage-0.8.0/examples/monitor_all.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import SystemObject
+from aiovantage.models import SystemObject
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/anemo_sensors/dump_anemo_sensors.py` & `aiovantage-0.8.0/examples/anemo_sensors/dump_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/anemo_sensors/monitor_anemo_sensors.py` & `aiovantage-0.8.0/examples/anemo_sensors/monitor_anemo_sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import AnemoSensor
+from aiovantage.models import AnemoSensor
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/areas/dump_areas.py` & `aiovantage-0.8.0/examples/areas/dump_areas.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.8.0/examples/blind_groups/dump_blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/blinds/dump_blinds.py` & `aiovantage-0.8.0/examples/blinds/dump_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/blinds/monitor_blinds.py` & `aiovantage-0.8.0/examples/masters/monitor_masters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-"""Fetch all blinds from the Vantage controller, and print out any state changes."""
+"""Fetch all Vantage controllers, and print any state changes."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import SystemObject
+from aiovantage.models import Master
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: SystemObject, data: Dict[str, Any]) -> None:
+def callback(event: VantageEvent, obj: Master, data: Dict[str, Any]) -> None:
     """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
-        print(f"[Blind added] '{obj.name}' ({obj.id})")
+        print(f"[Master added] '{obj.name}' ({obj.id})")
 
     elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[Blind updated] '{obj.name}' ({obj.id})")
+        print(f"[Master updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
             print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to updates for all blinds
-        vantage.blinds.subscribe(callback)
+        # Subscribe to updates for all Vantage controllers
+        vantage.masters.subscribe(callback)
 
-        # Fetch all known blinds from the controller
-        await vantage.blinds.initialize()
+        # Fetch all known Vantage controllers
+        await vantage.masters.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.7.0/examples/buttons/dump_buttons.py` & `aiovantage-0.8.0/examples/buttons/dump_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/buttons/monitor_buttons.py` & `aiovantage-0.8.0/examples/buttons/monitor_buttons.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import Button
+from aiovantage.models import Button
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/command_client/event_log.py` & `aiovantage-0.8.0/examples/command_client/event_log.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/command_client/status_load.py` & `aiovantage-0.8.0/examples/command_client/status_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/config_client/dump_objects.py` & `aiovantage-0.8.0/examples/config_client/dump_objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import argparse
 import asyncio
 import contextlib
 import logging
 
 from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.helpers import get_objects
+from aiovantage.config_client.requests import get_objects
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/config_client/get_version.py` & `aiovantage-0.8.0/examples/config_client/get_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Example of using the ConfigClient to get the Vantage version."""
 import argparse
 import asyncio
 import contextlib
 import logging
 
 from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.methods.introspection import GetVersion
+from aiovantage.config_client.interfaces.introspection import GetVersion
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.8.0/examples/dry_contacts/dump_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.8.0/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import DryContact
+from aiovantage.models import DryContact
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/gmem/dump_gmem.py` & `aiovantage-0.8.0/examples/gmem/dump_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/gmem/monitor_gmem.py` & `aiovantage-0.8.0/examples/gmem/monitor_gmem.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import GMem
+from aiovantage.models import GMem
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/gmem/set_gmem.py` & `aiovantage-0.8.0/examples/gmem/set_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/light_sensors/dump_light_sensors.py` & `aiovantage-0.8.0/examples/light_sensors/dump_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/light_sensors/monitor_light_sensors.py` & `aiovantage-0.8.0/examples/light_sensors/monitor_light_sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import LightSensor
+from aiovantage.models import LightSensor
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/load_groups/dump_load_groups.py` & `aiovantage-0.8.0/examples/load_groups/dump_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/load_groups/monitor_load_groups.py` & `aiovantage-0.8.0/examples/load_groups/monitor_load_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import LoadGroup
+from aiovantage.models import LoadGroup
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/loads/control_load.py` & `aiovantage-0.8.0/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/loads/dump_loads.py` & `aiovantage-0.8.0/examples/loads/dump_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/loads/monitor_loads.py` & `aiovantage-0.8.0/examples/loads/monitor_loads.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import Load
+from aiovantage.models import Load
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/loads/poll_on_loads.py` & `aiovantage-0.8.0/examples/loads/poll_on_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/loads/toggle_load.py` & `aiovantage-0.8.0/examples/loads/toggle_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/masters/dump_masters.py` & `aiovantage-0.8.0/examples/masters/dump_masters.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/masters/monitor_masters.py` & `aiovantage-0.8.0/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""Fetch all Vantage controllers, and print any state changes."""
+"""Fetch all RGB loads from the Vantage controller, and print out any state changes."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import Master
+from aiovantage.models import RGBLoadBase
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: Master, data: Dict[str, Any]) -> None:
+def callback(event: VantageEvent, obj: RGBLoadBase, data: Dict[str, Any]) -> None:
     """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
-        print(f"[Master added] '{obj.name}' ({obj.id})")
-
+        print(f"[RGBLoad added] '{obj.name}' ({obj.id})")
     elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[Master updated] '{obj.name}' ({obj.id})")
+        print(f"[RGBLoad updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
             print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to updates for all Vantage controllers
-        vantage.masters.subscribe(callback)
+        # Subscribe to RGB load updates
+        vantage.rgb_loads.subscribe(callback)
 
-        # Fetch all known Vantage controllers
-        await vantage.masters.initialize()
+        # Fetch all known RGB loads from the controller
+        await vantage.rgb_loads.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.7.0/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.8.0/examples/omni_sensors/dump_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.8.0/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import OmniSensor
+from aiovantage.models import OmniSensor
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.8.0/examples/rgb_loads/dump_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.8.0/examples/blinds/monitor_blinds.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-"""Fetch all RGB loads from the Vantage controller, and print out any state changes."""
+"""Fetch all blinds from the Vantage controller, and print out any state changes."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import RGBLoad
+from aiovantage.models import SystemObject
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: RGBLoad, data: Dict[str, Any]) -> None:
+def callback(event: VantageEvent, obj: SystemObject, data: Dict[str, Any]) -> None:
     """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
-        print(f"[RGBLoad added] '{obj.name}' ({obj.id})")
+        print(f"[Blind added] '{obj.name}' ({obj.id})")
+
     elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[RGBLoad updated] '{obj.name}' ({obj.id})")
+        print(f"[Blind updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
             print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to RGB load updates
-        vantage.rgb_loads.subscribe(callback)
+        # Subscribe to updates for all blinds
+        vantage.blinds.subscribe(callback)
 
-        # Fetch all known RGB loads from the controller
-        await vantage.rgb_loads.initialize()
+        # Fetch all known blinds from the controller
+        await vantage.blinds.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.7.0/examples/stations/dump_stations.py` & `aiovantage-0.8.0/examples/stations/dump_stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/stations/jingle_bells.py` & `aiovantage-0.8.0/examples/stations/jingle_bells.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/tasks/dump_tasks.py` & `aiovantage-0.8.0/examples/tasks/dump_tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/tasks/run_task.py` & `aiovantage-0.8.0/examples/tasks/run_task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/temperature_sensors/dump_temperature_sensors.py` & `aiovantage-0.8.0/examples/temperature_sensors/dump_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/examples/temperature_sensors/monitor_temperature_sensors.py` & `aiovantage-0.8.0/examples/temperature_sensors/monitor_temperature_sensors.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import Temperature
+from aiovantage.models import Temperature
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
```

### Comparing `aiovantage-0.7.0/src/aiovantage/__init__.py` & `aiovantage-0.8.0/src/aiovantage/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,37 +4,38 @@
 
 import asyncio
 from types import TracebackType
 from typing import Any, Callable, Optional, Set, Type, TypeVar
 
 from typing_extensions import Self
 
-from aiovantage.command_client import CommandClient, Event, EventStream, EventType
-from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.objects import SystemObject
-from aiovantage.controllers.anemo_sensors import AnemoSensorsController
-from aiovantage.controllers.areas import AreasController
-from aiovantage.controllers.base import BaseController, EventCallback
-from aiovantage.controllers.blind_groups import BlindGroupsController
-from aiovantage.controllers.blinds import BlindsController
-from aiovantage.controllers.buttons import ButtonsController
-from aiovantage.controllers.dry_contacts import DryContactsController
-from aiovantage.controllers.gmem import GMemController
-from aiovantage.controllers.light_sensors import LightSensorsController
-from aiovantage.controllers.load_groups import LoadGroupsController
-from aiovantage.controllers.loads import LoadsController
-from aiovantage.controllers.masters import MastersController
-from aiovantage.controllers.modules import ModulesController
-from aiovantage.controllers.omni_sensors import OmniSensorsController
-from aiovantage.controllers.rgb_loads import RGBLoadsController
-from aiovantage.controllers.stations import StationsController
-from aiovantage.controllers.tasks import TasksController
-from aiovantage.controllers.temperature_sensors import TemperatureSensorsController
-
-from .events import VantageEvent
+from .command_client import CommandClient, Event, EventStream, EventType
+from .config_client import ConfigClient
+from .controllers import (
+    AnemoSensorsController,
+    AreasController,
+    BaseController,
+    BlindGroupsController,
+    BlindsController,
+    ButtonsController,
+    DryContactsController,
+    GMemController,
+    LightSensorsController,
+    LoadGroupsController,
+    LoadsController,
+    MastersController,
+    ModulesController,
+    OmniSensorsController,
+    RGBLoadsController,
+    StationsController,
+    TasksController,
+    TemperatureSensorsController,
+)
+from .events import EventCallback, VantageEvent
+from .models import SystemObject
 
 ControllerT = TypeVar("ControllerT", bound=BaseController[Any])
 
 
 class Vantage:
     """Control a Vantage InFusion controller."""
```

### Comparing `aiovantage-0.7.0/src/aiovantage/connection.py` & `aiovantage-0.8.0/src/aiovantage/connection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/discovery.py` & `aiovantage-0.8.0/src/aiovantage/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Helper utilities for discovering details about Vantage controllers."""
 import re
 from dataclasses import dataclass
 from typing import Optional
 
-from aiovantage import Vantage
-from aiovantage.command_client.commands import CommandClient
-from aiovantage.errors import (
+from . import Vantage
+from .command_client.commands import CommandClient
+from .errors import (
     ClientConnectionError,
     ClientError,
     LoginFailedError,
     LoginRequiredError,
 )
```

### Comparing `aiovantage-0.7.0/src/aiovantage/errors.py` & `aiovantage-0.8.0/src/aiovantage/errors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/query.py` & `aiovantage-0.8.0/src/aiovantage/query.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/README.md` & `aiovantage-0.8.0/src/aiovantage/command_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/__init__.py` & `aiovantage-0.8.0/src/aiovantage/command_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/commands.py` & `aiovantage-0.8.0/src/aiovantage/command_client/commands.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/events.py` & `aiovantage-0.8.0/src/aiovantage/command_client/events.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/utils.py` & `aiovantage-0.8.0/src/aiovantage/command_client/utils.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/anemo_sensor.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/anemo_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/base.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/introspection.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/introspection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/light_sensor.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/light_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/sounder.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/sounder.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,20 +50,20 @@
             frequency: The frequency to set.
         """
         # INVOKE <id> Sounder.SetFrequency <frequency>
         # -> R:INVOKE <id> <rcode> Sounder.SetFrequency
         await self.invoke(vid, "Sounder.SetFrequency", frequency)
 
     async def play_fx(
-        self, vid: int, fx: int, duration: float = 0, volume: float = 0
+        self, vid: int, effect: int, duration: float = 0, volume: float = 0
     ) -> None:
-        """Play an FX on the keypad speaker.
+        """Play a sound effect on the keypad speaker.
 
         Args:
             vid: The Vantage ID of the keypad.
-            fx: The FX to play.
+            effect: The effect to play.
             duration: The duration to play the FX for, in seconds, 0 for default.
             volume: The volume to play the FX at, as a percentage, 0 for default.
         """
         # INVOKE <id> Sounder.PlayFX <fx> <duration> <volume>
         # -> R:INVOKE <id> <rcode> Sounder.PlayFX
-        await self.invoke(vid, "Sounder.PlayFX", fx, duration, volume)
+        await self.invoke(vid, "Sounder.PlayFX", effect, duration, volume)
```

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/command_client/interfaces/temperature.py` & `aiovantage-0.8.0/src/aiovantage/command_client/interfaces/temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/src/aiovantage/config_client/README.md` & `aiovantage-0.8.0/src/aiovantage/config_client/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,63 +15,60 @@
 a particular interface.
 
 Since a common use case for interacting with the ACI service is to lookup system
 objects, this module also provides models to help with deserializing many of these
 object types, available in [`objects`](objects).
 
 Additionally, a few helper functions for fetching objects are provided by
-[`helpers.py`](helpers.py).
-
+[`requests.py`](requests.py).
 
 ## Examples
 
 ### Lookup objects by type, using a helper
 
 ```python
 from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.helpers import get_objects
+from aiovantage.config_client.requests import get_objects
 
 async with ConfigClient("hostname") as client:
     loads = get_objects(client, types=["Load", "Button"])
 ```
 
 ### Lookup objects by id, using a helper
 
 ```python
 from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.helpers import get_objects_by_id
+from aiovantage.config_client.requests import get_objects_by_id
 
 async with ConfigClient("hostname") as client:
     objects = get_objects_by_id(client, [118])
 ```
 
-
 ### Make a request using a method class
 
 ```python
 from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.methods.introspection import GetVersion
+from aiovantage.config_client.interfaces.introspection import GetVersion
 
 async with ConfigClient("hostname") as client:
     version = await client.request(GetVersion)
 ```
 
-
 ### Make a request using a method class, with params
 
 ```python
 from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.methods.login import Login
+from aiovantage.config_client.interfaces.login import Login
 
 async with ConfigClient("hostname") as client:
     await client.request(Login, Login.Params("username", "password"))
 ```
 
 ### Make a raw request
 
 ```python
 from aiovantage.config_client import ConfigClient
 
 async with ConfigClient("hostname") as client:
     response = await client.raw_request("IIntrospection", "<GetVersion></GetVersion>")
 
-```
+```
```

### Comparing `aiovantage-0.7.0/src/aiovantage/config_client/__init__.py` & `aiovantage-0.8.0/src/aiovantage/config_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,21 @@
 from typing_extensions import Self
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 from xsdata.formats.dataclass.parsers.handlers import XmlEventHandler
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
-from aiovantage.config_client.methods import Call, Method, Return
-from aiovantage.config_client.methods.introspection import GetVersion
-from aiovantage.config_client.methods.login import Login
 from aiovantage.connection import BaseConnection
 from aiovantage.errors import ClientResponseError, LoginFailedError, LoginRequiredError
 
+from .interfaces import Call, Method, Return
+from .interfaces.introspection import GetVersion
+from .interfaces.login import Login
+
 
 class ConfigConnection(BaseConnection):
     """Connection to a Vantage ACI server."""
 
     default_port = 2001
     default_ssl_port = 2010
     buffer_limit = 2**20
```

### Comparing `aiovantage-0.7.0/src/aiovantage/config_client/helpers.py` & `aiovantage-0.8.0/src/aiovantage/config_client/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Helper functions for fetching system objects."""
 
 from contextlib import suppress
 from typing import Any, AsyncIterator, Optional, Sequence
 
-from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.methods.configuration import (
+from aiovantage.errors import ClientError, ClientResponseError
+
+from . import ConfigClient
+from .interfaces.configuration import (
     CloseFilter,
     GetFilterResults,
     GetObject,
     OpenFilter,
 )
-from aiovantage.errors import ClientError, ClientResponseError
 
 
 async def get_objects(
     client: ConfigClient,
     *,
     types: Optional[Sequence[str]] = None,
     xpath: Optional[str] = None,
```

### Comparing `aiovantage-0.7.0/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.8.0/src/aiovantage/config_client/interfaces/configuration/get_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 """IConfiguration.GetObject method definition."""
 
 from dataclasses import dataclass, field
 from typing import ClassVar, List, Optional
 
-from aiovantage.config_client.methods.types import ObjectChoice
+from aiovantage.config_client.interfaces.types import ObjectChoice
 
 
 @dataclass
 class GetObject:
     """IConfiguration.GetObject method definition."""
 
     interface: ClassVar[str] = "IConfiguration"
     call: Optional["GetObject.Params"] = field(default=None)
     return_value: Optional[List[ObjectChoice]] = field(
-        default=None, metadata={"name": "Object", "wrapper": "return"}
+        default=None,
+        metadata={
+            "name": "Object",
+            "wrapper": "return",
+        },
     )
 
     @dataclass
     class Params:
         """IConfiguration.GetObject method parameters."""
 
-        vids: List[int] = field(metadata={"name": "VID"})
+        vids: List[int] = field(
+            metadata={
+                "name": "VID",
+            }
+        )
```

### Comparing `aiovantage-0.7.0/src/aiovantage/config_client/methods/introspection/get_version.py` & `aiovantage-0.8.0/src/aiovantage/config_client/interfaces/introspection/get_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 @dataclass
 class GetVersion:
     """IIntrospection.GetVersion method definition."""
 
     interface: ClassVar[str] = "IIntrospection"
     call = None
     return_value: Optional["GetVersion.Return"] = field(
-        default=None, metadata={"name": "return"}
+        default=None,
+        metadata={
+            "name": "return",
+        },
     )
 
     @dataclass
     class Return:
         """IIntrospection.GetVersion method return value."""
 
         kernel: Optional[str] = field(default=None)
```

### Comparing `aiovantage-0.7.0/src/aiovantage/config_client/methods/login/login.py` & `aiovantage-0.8.0/src/aiovantage/config_client/interfaces/login/login.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,32 @@
 
 
 @dataclass
 class Login:
     """ILogin.Login method definition."""
 
     interface: ClassVar[str] = "ILogin"
+
     call: Optional["Login.Params"] = field(default=None)
-    return_value: Optional[bool] = field(default=None, metadata={"name": "return"})
+
+    return_value: Optional[bool] = field(
+        default=None,
+        metadata={
+            "name": "return",
+        },
+    )
 
     @dataclass
     class Params:
         """ILogin.Login method parameters."""
 
-        user: str = field(metadata={"name": "User"})
-        password: str = field(metadata={"name": "Password"})
+        user: str = field(
+            metadata={
+                "name": "User",
+            }
+        )
+
+        password: str = field(
+            metadata={
+                "name": "Password",
+            }
+        )
```

### Comparing `aiovantage-0.7.0/src/aiovantage/config_client/objects/__init__.py` & `aiovantage-0.8.0/src/aiovantage/config_client/models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Vantage object types."""
 
 from .anemo_sensor import AnemoSensor
 from .area import Area
 from .blind import Blind
+from .blind_base import BlindBase
 from .blind_group import BlindGroup
+from .blind_group_base import BlindGroupBase
 from .button import Button
+from .child_device import ChildDevice
+from .child_object import ChildObject
+from .custom_device import CustomDevice
 from .dc_power_profile import DCPowerProfile
-from .ddg_color_load import DDGColorLoad
-from .dg_color_load import DGColorLoad
 from .dimmer import Dimmer
 from .dry_contact import DryContact
 from .dual_relay_station import DualRelayStation
 from .eq_ctrl import EqCtrl
 from .eq_ux import EqUX
 from .gmem import GMem
 from .keypad import Keypad
@@ -24,36 +27,42 @@
 from .module_gen2 import ModuleGen2
 from .omni_sensor import OmniSensor
 from .power_profile import PowerProfile
 from .pwm_power_profile import PWMPowerProfile
 from .qis_blind import QISBlind
 from .qube_blind import QubeBlind
 from .relay_blind import RelayBlind
-from .rgb_load import RGBLoad
+from .rgb_load_base import RGBLoadBase
 from .scene_point_relay import ScenePointRelay
 from .sensor import Sensor
-from .somfy.rs485_group import RS485Group
-from .somfy.rs485_shade import RS485Shade
-from .somfy.urtsi_2_group import URTSI2Group
-from .somfy.urtsi_2_shade import URTSI2Shade
+from .somfy_rs_485_group_child import SomfyRS485GroupChild
+from .somfy_rs_485_shade_child import SomfyRS485ShadeChild
+from .somfy_urtsi_2_group_child import SomfyURTSI2GroupChild
+from .somfy_urtsi_2_shade_child import SomfyURTSI2ShadeChild
 from .station_bus import StationBus
 from .station_object import StationObject
 from .system_object import SystemObject
 from .task import Task
 from .temperature import Temperature
+from .vantage_ddg_color_load import VantageDDGColorLoad
+from .vantage_dg_color_load import VantageDGColorLoad
+from .vantage_dmx_dali_gateway import VantageDmxDaliGateway
 
 __all__ = [
     "AnemoSensor",
     "Area",
     "Blind",
+    "BlindBase",
     "BlindGroup",
+    "BlindGroupBase",
     "Button",
+    "ChildDevice",
+    "ChildObject",
+    "CustomDevice",
     "DCPowerProfile",
-    "DDGColorLoad",
-    "DGColorLoad",
     "Dimmer",
     "DryContact",
     "DualRelayStation",
     "EqCtrl",
     "EqUX",
     "GMem",
     "Keypad",
@@ -66,20 +75,23 @@
     "ModuleGen2",
     "OmniSensor",
     "PowerProfile",
     "PWMPowerProfile",
     "QISBlind",
     "QubeBlind",
     "RelayBlind",
-    "RGBLoad",
-    "RS485Group",
-    "RS485Shade",
+    "RGBLoadBase",
     "ScenePointRelay",
     "Sensor",
+    "SomfyRS485GroupChild",
+    "SomfyRS485ShadeChild",
+    "SomfyURTSI2GroupChild",
+    "SomfyURTSI2ShadeChild",
     "StationBus",
     "StationObject",
     "SystemObject",
     "Task",
     "Temperature",
-    "URTSI2Group",
-    "URTSI2Shade",
+    "VantageDDGColorLoad",
+    "VantageDGColorLoad",
+    "VantageDmxDaliGateway",
 ]
```

### Comparing `aiovantage-0.7.0/src/aiovantage/config_client/objects/gmem.py` & `aiovantage-0.8.0/src/aiovantage/config_client/models/gmem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,71 @@
 """GMem (variable) object."""
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Union
 
-from aiovantage.config_client.xml_dataclass import xml_attribute, xml_element, xml_text
-
 from .system_object import SystemObject
 
 
 @dataclass
+class Tag:
+    """GMem tag."""
+
+    type: str
+
+    object: bool = field(
+        default=False,
+        metadata={
+            "name": "object",
+            "type": "Attribute",
+        },
+    )
+
+
+@dataclass
+class Data:
+    """GMem data."""
+
+    fixed: bool = field(
+        default=False,
+        metadata={
+            "name": "Fixed",
+            "type": "Attribute",
+        },
+    )
+
+
+@dataclass
 class GMem(SystemObject):
     """GMem (variable) object."""
 
-    @dataclass
-    class Tag:
-        """GMem tag."""
-
-        type: str = xml_text()
-        object: bool = xml_attribute("object", default=False)
-
-    @dataclass
-    class Data:
-        """GMem data."""
-
-        fixed: bool = xml_attribute("Fixed", default=False)
-
-    data: Data = xml_element("data")
-    persistent: bool = xml_element("Persistent")
-    tag: Tag = xml_element("Tag")
-
-    def __post_init__(self) -> None:
-        """Declare state attributes in post init."""
-        self.value: Union[int, str, bool, None] = None
+    data: Data = field(
+        metadata={
+            "name": "data",
+        }
+    )
+
+    persistent: bool = field(
+        metadata={
+            "name": "Persistent",
+        }
+    )
+
+    tag: Tag = field(
+        metadata={
+            "name": "Tag",
+        }
+    )
+
+    value: Union[int, str, bool, None] = field(
+        default=None,
+        metadata={
+            "type": "Ignore",
+        },
+    )
 
     @property
     def is_bool(self) -> bool:
         """Return True if GMem is boolean type."""
         return self.tag.type == "bool"
 
     @property
```

### Comparing `aiovantage-0.7.0/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.8.0/src/aiovantage/config_client/models/omni_sensor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,75 @@
 """OmniSensor object."""
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from decimal import Decimal
 from typing import Union
 
-from aiovantage.config_client.xml_dataclass import xml_attribute, xml_element
-
+from .child_object import ChildObject
 from .sensor import Sensor
 
 
 @dataclass
-class OmniSensor(Sensor):
+class Formula:
+    """OmniSensor type conversion information."""
+
+    return_type: str = field(
+        metadata={
+            "name": "ReturnType",
+            "type": "Attribute",
+        }
+    )
+
+    level_type: str = field(
+        metadata={
+            "name": "LevelType",
+            "type": "Attribute",
+        }
+    )
+
+
+@dataclass
+class GetMethodType:
+    """Omnisensor method information."""
+
+    formula: Formula = field(
+        metadata={
+            "name": "Formula",
+        }
+    )
+
+    method: str = field(
+        metadata={
+            "name": "Method",
+        }
+    )
+
+    method_hw: str = field(
+        metadata={
+            "name": "MethodHW",
+        }
+    )
+
+
+@dataclass
+class OmniSensor(ChildObject, Sensor):
     """OmniSensor object."""
 
-    @dataclass
-    class GetMethodType:
-        """Omnisensor method information."""
-
-        @dataclass
-        class Formula:
-            """OmniSensor type conversion information."""
-
-            return_type: str = xml_attribute("ReturnType")
-            level_type: str = xml_attribute("LevelType")
-
-        formula: Formula = xml_element("Formula")
-        method: str = xml_element("Method")
-        method_hw: str = xml_element("MethodHW")
-
-    get: GetMethodType = xml_element("Get")
-    parent_id: int = xml_element("Parent")
-
-    def __post_init__(self) -> None:
-        """Declare state attributes in post init."""
-        self.level: Union[int, Decimal, None] = None
+    get: GetMethodType = field(
+        metadata={
+            "name": "Get",
+        }
+    )
+
+    level: Union[int, Decimal, None] = field(
+        default=None,
+        metadata={
+            "type": "Ignore",
+        },
+    )
 
     @property
     def is_current_sensor(self) -> bool:
         """Return True if the sensor is a current sensor."""
         return self.model == "Current"
 
     @property
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/anemo_sensors.py` & `aiovantage-0.8.0/src/aiovantage/controllers/anemo_sensors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Controller holding and managing Vantage anemo (wind) sensors."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import AnemoSensorInterface
-from aiovantage.config_client.objects import AnemoSensor
+from aiovantage.models import AnemoSensor
 
 from .base import BaseController, State
 
 
 class AnemoSensorsController(BaseController[AnemoSensor], AnemoSensorInterface):
     """Controller holding and managing Vantage anemo (wind) sensors."""
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/base.py` & `aiovantage-0.8.0/src/aiovantage/controllers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,30 +19,27 @@
     TypeVar,
     Union,
 )
 
 from aiovantage.command_client import CommandClient, Event, EventStream, EventType
 from aiovantage.command_client.utils import tokenize_response
 from aiovantage.config_client import ConfigClient
-from aiovantage.config_client.helpers import get_objects
-from aiovantage.config_client.objects import SystemObject
-from aiovantage.events import VantageEvent
+from aiovantage.config_client.requests import get_objects
+from aiovantage.events import EventCallback, VantageEvent
+from aiovantage.models import SystemObject
 from aiovantage.query import QuerySet
 
 if TYPE_CHECKING:
     from aiovantage import Vantage
 
 T = TypeVar("T", bound=SystemObject)
 
 
-# Types for callbacks for event subscriptions
-EventCallback = Callable[[VantageEvent, T, Dict[str, Any]], None]
+# Types for state and subscriptions
 EventSubscription = Tuple[EventCallback[T], Optional[Iterable[VantageEvent]]]
-
-# Type for state updates
 State = Optional[Dict[str, Any]]
 
 
 class BaseController(QuerySet[T]):
     """Base controller for Vantage objects."""
 
     vantage_types: Tuple[str, ...]
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/blinds.py` & `aiovantage-0.8.0/src/aiovantage/controllers/blinds.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Controller holding and managing Vantage blinds."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import BlindInterface
-from aiovantage.config_client.objects import Blind
+from aiovantage.models import BlindBase
 
 from .base import BaseController, State
 
 
-class BlindsController(BaseController[Blind], BlindInterface):
+class BlindsController(BaseController[BlindBase], BlindInterface):
     """Controller holding and managing Vantage blinds."""
 
     vantage_types = (
         "QISBlind",
         "QubeBlind",
         "RelayBlind",
         "Somfy.RS-485_Shade_CHILD",
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/buttons.py` & `aiovantage-0.8.0/src/aiovantage/controllers/buttons.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Controller holding and managing Vantage buttons."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import ButtonInterface
-from aiovantage.config_client.objects import Button
+from aiovantage.models import Button
 
 from .base import BaseController, State
 
 
 class ButtonsController(BaseController[Button], ButtonInterface):
     """Controller holding and managing Vantage buttons."""
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.8.0/src/aiovantage/controllers/dry_contacts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Controller holding and managing Vantage dry contacts."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import ButtonInterface
-from aiovantage.config_client.objects import DryContact
+from aiovantage.models import DryContact
 
 from .base import BaseController, State
 
 
 class DryContactsController(BaseController[DryContact], ButtonInterface):
     """Controller holding and managing Vantage dry contacts."""
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/gmem.py` & `aiovantage-0.8.0/src/aiovantage/controllers/gmem.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import re
 from typing import Sequence, Union
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import GMemInterface
 from aiovantage.command_client.utils import parse_byte_param
-from aiovantage.config_client.objects import GMem
-from aiovantage.controllers.base import BaseController, State
+from aiovantage.models import GMem
+
+from .base import BaseController, State
 
 
 class GMemController(BaseController[GMem], GMemInterface):
     """Controller holding and managing Vantage variables."""
 
     vantage_types = ("GMem",)
     """The Vantage object types that this controller will fetch."""
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/light_sensors.py` & `aiovantage-0.8.0/src/aiovantage/controllers/light_sensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Controller holding and managing Vantage light sensors."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import LightSensorInterface
-from aiovantage.config_client.objects import LightSensor
+from aiovantage.models import LightSensor
 
 from .base import BaseController, State
 
 
 class LightSensorsController(BaseController[LightSensor], LightSensorInterface):
     """Controller holding and managing Vantage light sensors."""
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/load_groups.py` & `aiovantage-0.8.0/src/aiovantage/controllers/load_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Controller holding and managing Vantage load groups."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces.load import LoadInterface
-from aiovantage.config_client.objects import Load, LoadGroup
+from aiovantage.models import Load, LoadGroup
 from aiovantage.query import QuerySet
 
 from .base import BaseController, State
 
 
 class LoadGroupsController(BaseController[LoadGroup], LoadInterface):
     """Controller holding and managing Vantage load groups."""
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/loads.py` & `aiovantage-0.8.0/src/aiovantage/controllers/loads.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Controller holding and managing Vantage loads."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import LoadInterface
-from aiovantage.config_client.objects import Load
+from aiovantage.models import Load
 from aiovantage.query import QuerySet
 
 from .base import BaseController, State
 
 
 class LoadsController(BaseController[Load], LoadInterface):
     """Controller holding and managing Vantage loads."""
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/masters.py` & `aiovantage-0.8.0/src/aiovantage/controllers/masters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Controller holding and managing Vantage controllers."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import IntrospectionInterface, ObjectInterface
-from aiovantage.config_client.objects import Master
-from aiovantage.controllers.base import BaseController, State
+from aiovantage.models import Master
+
+from .base import BaseController, State
 
 
 class MastersController(
     BaseController[Master],
     ObjectInterface,
     IntrospectionInterface,
 ):
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.8.0/src/aiovantage/controllers/omni_sensors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Controller holding and managing Vantage omni sensors."""
 
 from decimal import Decimal
 from typing import Sequence, Union
 
 from typing_extensions import override
 
-from aiovantage.config_client.objects import OmniSensor
-from aiovantage.controllers.base import BaseController, State
+from aiovantage.models import OmniSensor
+
+from .base import BaseController, State
 
 
 class OmniSensorsController(BaseController[OmniSensor]):
     """Controller holding and managing Vantage omni sensors."""
 
     vantage_types = ("OmniSensor",)
     """The Vantage object types that this controller will fetch."""
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.8.0/src/aiovantage/controllers/rgb_loads.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import (
     ColorTemperatureInterface,
     LoadInterface,
     RGBLoadInterface,
 )
-from aiovantage.config_client.objects import RGBLoad
+from aiovantage.models import RGBLoadBase
 from aiovantage.query import QuerySet
 
 from .base import BaseController, State
 
 
 class RGBLoadsController(
-    BaseController[RGBLoad],
+    BaseController[RGBLoadBase],
     LoadInterface,
     RGBLoadInterface,
     ColorTemperatureInterface,
 ):
     """Controller holding and managing Vantage RGB loads."""
 
     vantage_types = ("Vantage.DGColorLoad", "Vantage.DDGColorLoad")
@@ -42,15 +42,15 @@
     @override
     async def fetch_object_state(self, vid: int) -> State:
         """Fetch the state properties of an RGB load."""
         state: Dict[str, Any] = {
             "level": await LoadInterface.get_level(self, vid),
         }
 
-        rgb_load: RGBLoad = self[vid]
+        rgb_load: RGBLoadBase = self[vid]
         if rgb_load.is_rgb:
             state["hsl"] = await RGBLoadInterface.get_hsl(self, vid)
             state["rgb"] = await RGBLoadInterface.get_rgb(self, vid)
             state["rgbw"] = await RGBLoadInterface.get_rgbw(self, vid)
 
         if rgb_load.is_cct:
             state["color_temp"] = await ColorTemperatureInterface.get_color_temp(
@@ -58,15 +58,15 @@
             )
 
         return state
 
     @override
     def parse_object_update(self, vid: int, status: str, args: Sequence[str]) -> State:
         """Handle state changes for an RGB load."""
-        rgb_load: RGBLoad = self[vid]
+        rgb_load: RGBLoadBase = self[vid]
         if status == "Load.GetLevel":
             return {
                 "level": LoadInterface.parse_get_level_status(args),
             }
 
         if status == "RGBLoad.GetHSL" and rgb_load.is_rgb:
             channel, value = RGBLoadInterface.parse_color_channel_status(args)
@@ -90,20 +90,20 @@
             return {
                 "color_temp": ColorTemperatureInterface.parse_get_status(args),
             }
 
         return None
 
     @property
-    def is_on(self) -> QuerySet[RGBLoad]:
+    def is_on(self) -> QuerySet[RGBLoadBase]:
         """Return a queryset of all RGB loads that are turned on."""
         return self.filter(lambda load: load.is_on)
 
     @property
-    def is_off(self) -> QuerySet[RGBLoad]:
+    def is_off(self) -> QuerySet[RGBLoadBase]:
         """Return a queryset of all RGB loads that are turned off."""
         return self.filter(lambda load: not load.is_on)
 
     def _build_color_from_channels(
         self, vid: int, channel: int, value: int, num_channels: int
     ) -> Optional[Tuple[int, ...]]:
         # Build a color from a series of channel value events. We need to store
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/tasks.py` & `aiovantage-0.8.0/src/aiovantage/controllers/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Controller holding and managing Vantage tasks."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import TaskInterface
-from aiovantage.config_client.objects import Task
+from aiovantage.models import Task
 
 from .base import BaseController, State
 
 
 class TasksController(BaseController[Task], TaskInterface):
     """Controller holding and managing Vantage tasks."""
```

### Comparing `aiovantage-0.7.0/src/aiovantage/controllers/temperature_sensors.py` & `aiovantage-0.8.0/src/aiovantage/controllers/temperature_sensors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Controller holding and managing Vantage temperature sensors."""
 
 from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import TemperatureInterface
-from aiovantage.config_client.objects import Temperature
+from aiovantage.models import Temperature
 
 from .base import BaseController, State
 
 
 class TemperatureSensorsController(BaseController[Temperature], TemperatureInterface):
     """Controller holding and managing Vantage temperature sensors."""
```

### Comparing `aiovantage-0.7.0/LICENSE` & `aiovantage-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.7.0/README.md` & `aiovantage-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 | BlindGroups   | Groups of blinds      | `vantage.blind_groups`        | [Examples](examples/blind_groups)         |
 | Buttons       | Keypad buttons        | `vantage.buttons`             | [Examples](examples/buttons)              |
 | DryContacts   | Motion sensors, etc   | `vantage.dry_contacts`        | [Examples](examples/dry_contacts)         |
 | GMem          | Vantage variables     | `vantage.gmem`                | [Examples](examples/gmem)                 |
 | LightSensor   | Light sensors         | `vantage.light_sensors`       | [Examples](examples/light_sensors)        |
 | Load          | Lights, relays, etc   | `vantage.loads`               | [Examples](examples/loads)                |
 | LoadGroup     | Groups of loads       | `vantage.load_groups`         | [Examples](examples/load_groups)          |
+| Master        | Vantage controllers   | `vantage.masters`             | [Examples](examples/masters)              |
+| Module        | Dimmer modules        | `vantage.modules`             |                                           |
 | OmniSensor    | Power, current, etc   | `vantage.omni_sensors`        | [Examples](examples/omni_sensors)         |
 | RGBLoad       | RGB lights            | `vantage.rgb_loads`           | [Examples](examples/rgb_loads)            |
 | Stations      | Keypads, etc          | `vantage.stations`            | [Examples](examples/stations)             |
 | Tasks         | Vantage tasks         | `vantage.tasks`               | [Examples](examples/tasks)                |
 | Temperature   | Temperature sensors   | `vantage.temperature_sensors` | [Examples](examples/temperature_sensors)  |
 
 If you have an object that you expect to show up in one of these controllers, but it is missing, please let me know in an issue.
```

### Comparing `aiovantage-0.7.0/pyproject.toml` & `aiovantage-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,19 @@
     "Q",    # flake8-quotes
     "C90",  # mccabe
 ]
 ignore = [
     "E501",  # line too long, handled by black
 ]
 
+[tool.ruff.per-file-ignores]
+"src/aiovantage/config_client/models/**/*.py" = [
+    "D106"  # Missing docstring in public nested class
+]
+
 [tool.ruff.isort]
 known-first-party = ["aiovantage"]
 
 [tool.ruff.mccabe]
 max-complexity = 15
 
 [tool.ruff.pydocstyle]
```

### Comparing `aiovantage-0.7.0/PKG-INFO` & `aiovantage-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.7.0
+Version: 0.8.0
 Summary: Interact with and control Vantage InFusion home automation controllers.
 Project-URL: Documentation, https://github.com/loopj/aiovantage#readme
 Project-URL: Issues, https://github.com/loopj/aiovantage/issues
 Project-URL: Source, https://github.com/loopj/aiovantage
 Author-email: James Smith <james@loopj.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -76,14 +76,16 @@
 | BlindGroups   | Groups of blinds      | `vantage.blind_groups`        | [Examples](examples/blind_groups)         |
 | Buttons       | Keypad buttons        | `vantage.buttons`             | [Examples](examples/buttons)              |
 | DryContacts   | Motion sensors, etc   | `vantage.dry_contacts`        | [Examples](examples/dry_contacts)         |
 | GMem          | Vantage variables     | `vantage.gmem`                | [Examples](examples/gmem)                 |
 | LightSensor   | Light sensors         | `vantage.light_sensors`       | [Examples](examples/light_sensors)        |
 | Load          | Lights, relays, etc   | `vantage.loads`               | [Examples](examples/loads)                |
 | LoadGroup     | Groups of loads       | `vantage.load_groups`         | [Examples](examples/load_groups)          |
+| Master        | Vantage controllers   | `vantage.masters`             | [Examples](examples/masters)              |
+| Module        | Dimmer modules        | `vantage.modules`             |                                           |
 | OmniSensor    | Power, current, etc   | `vantage.omni_sensors`        | [Examples](examples/omni_sensors)         |
 | RGBLoad       | RGB lights            | `vantage.rgb_loads`           | [Examples](examples/rgb_loads)            |
 | Stations      | Keypads, etc          | `vantage.stations`            | [Examples](examples/stations)             |
 | Tasks         | Vantage tasks         | `vantage.tasks`               | [Examples](examples/tasks)                |
 | Temperature   | Temperature sensors   | `vantage.temperature_sensors` | [Examples](examples/temperature_sensors)  |
 
 If you have an object that you expect to show up in one of these controllers, but it is missing, please let me know in an issue.
```

