# Comparing `tmp/spacetraders-0.5.0.tar.gz` & `tmp/spacetraders-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetraders-0.5.0.tar", max compression
+gzip compressed data, was "spacetraders-0.6.0.tar", max compression
```

## Comparing `spacetraders-0.5.0.tar` & `spacetraders-0.6.0.tar`

### file list

```diff
@@ -1,220 +1,231 @@
--rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.5.0/README.md
--rw-r--r--   0        0        0      664 2023-05-24 19:24:39.688239 spacetraders-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      250 2023-05-24 19:22:46.258239 spacetraders-0.5.0/spacetraders/__init__.py
--rw-r--r--   0        0        0       47 2023-05-24 19:22:45.628239 spacetraders-0.5.0/spacetraders/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 19:22:45.688239 spacetraders-0.5.0/spacetraders/api/agents/__init__.py
--rw-r--r--   0        0        0     4139 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/agents/get_my_agent.py
--rw-r--r--   0        0        0        0 2023-05-24 19:22:45.688239 spacetraders-0.5.0/spacetraders/api/contracts/__init__.py
--rw-r--r--   0        0        0     4425 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/contracts/accept_contract.py
--rw-r--r--   0        0        0     5022 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/contracts/deliver_contract.py
--rw-r--r--   0        0        0     4437 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/contracts/fulfill_contract.py
--rw-r--r--   0        0        0     4420 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/contracts/get_contract.py
--rw-r--r--   0        0        0     4900 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/contracts/get_contracts.py
--rw-r--r--   0        0        0        0 2023-05-24 19:22:45.638239 spacetraders-0.5.0/spacetraders/api/default/__init__.py
--rw-r--r--   0        0        0     4069 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/default/get_status.py
--rw-r--r--   0        0        0     6960 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/default/register.py
--rw-r--r--   0        0        0        0 2023-05-24 19:22:45.688239 spacetraders-0.5.0/spacetraders/api/factions/__init__.py
--rw-r--r--   0        0        0     4427 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/factions/get_faction.py
--rw-r--r--   0        0        0     4853 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/factions/get_factions.py
--rw-r--r--   0        0        0        0 2023-05-24 19:22:45.688239 spacetraders-0.5.0/spacetraders/api/fleet/__init__.py
--rw-r--r--   0        0        0     4900 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/create_chart.py
--rw-r--r--   0        0        0     4550 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/create_ship_ship_scan.py
--rw-r--r--   0        0        0     4587 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/create_ship_system_scan.py
--rw-r--r--   0        0        0     4615 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
--rw-r--r--   0        0        0     5382 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/create_survey.py
--rw-r--r--   0        0        0     4961 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/fleet/dock_ship.py
--rw-r--r--   0        0        0     5217 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/fleet/extract_resources.py
--rw-r--r--   0        0        0     4373 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/fleet/get_my_ship.py
--rw-r--r--   0        0        0     4447 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/get_my_ship_cargo.py
--rw-r--r--   0        0        0     4871 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/get_my_ships.py
--rw-r--r--   0        0        0     5562 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/get_ship_cooldown.py
--rw-r--r--   0        0        0     4414 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/get_ship_nav.py
--rw-r--r--   0        0        0     4905 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/jettison.py
--rw-r--r--   0        0        0     5343 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/fleet/jump_ship.py
--rw-r--r--   0        0        0     5893 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/navigate_ship.py
--rw-r--r--   0        0        0     4905 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/negotiate_contract.py
--rw-r--r--   0        0        0     4954 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/orbit_ship.py
--rw-r--r--   0        0        0     5001 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/patch_ship_nav.py
--rw-r--r--   0        0        0     5192 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/purchase_cargo.py
--rw-r--r--   0        0        0     4680 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/purchase_ship.py
--rw-r--r--   0        0        0     4419 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/refuel_ship.py
--rw-r--r--   0        0        0     5010 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/sell_cargo.py
--rw-r--r--   0        0        0     5244 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/ship_refine.py
--rw-r--r--   0        0        0     5215 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/transfer_cargo.py
--rw-r--r--   0        0        0     5569 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/api/fleet/warp_ship.py
--rw-r--r--   0        0        0        0 2023-05-24 19:22:45.678239 spacetraders-0.5.0/spacetraders/api/systems/__init__.py
--rw-r--r--   0        0        0     4675 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/systems/get_jump_gate.py
--rw-r--r--   0        0        0     5061 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/systems/get_market.py
--rw-r--r--   0        0        0     4891 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/systems/get_shipyard.py
--rw-r--r--   0        0        0     4409 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/api/systems/get_system.py
--rw-r--r--   0        0        0     5421 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/systems/get_system_waypoints.py
--rw-r--r--   0        0        0     4817 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/systems/get_systems.py
--rw-r--r--   0        0        0     4650 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/api/systems/get_waypoint.py
--rw-r--r--   0        0        0     4384 2023-05-24 19:22:46.688239 spacetraders-0.5.0/spacetraders/client.py
--rw-r--r--   0        0        0      470 2023-05-24 19:22:46.578239 spacetraders-0.5.0/spacetraders/errors.py
--rw-r--r--   0        0        0    14521 2023-05-24 19:22:46.838239 spacetraders-0.5.0/spacetraders/models/__init__.py
--rw-r--r--   0        0        0     1269 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/accept_contract_response_200.py
--rw-r--r--   0        0        0     1299 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/accept_contract_response_200_data.py
--rw-r--r--   0        0        0     1587 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/agent.py
--rw-r--r--   0        0        0     1532 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/chart.py
--rw-r--r--   0        0        0     1709 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/connected_system.py
--rw-r--r--   0        0        0     2160 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/contract.py
--rw-r--r--   0        0        0     1712 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/contract_deliver_good.py
--rw-r--r--   0        0        0     1340 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/contract_payment.py
--rw-r--r--   0        0        0     1567 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/contract_terms.py
--rw-r--r--   0        0        0      201 2023-05-24 19:22:45.828239 spacetraders-0.5.0/spacetraders/models/contract_type.py
--rw-r--r--   0        0        0     1744 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/cooldown.py
--rw-r--r--   0        0        0     1251 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/create_chart_response_201.py
--rw-r--r--   0        0        0     1469 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/create_chart_response_201_data.py
--rw-r--r--   0        0        0     1304 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/create_ship_ship_scan_response_201.py
--rw-r--r--   0        0        0     1425 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
--rw-r--r--   0        0        0     1316 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/create_ship_system_scan_response_201.py
--rw-r--r--   0        0        0     1443 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/create_ship_system_scan_response_201_data.py
--rw-r--r--   0        0        0     1328 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
--rw-r--r--   0        0        0     1461 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
--rw-r--r--   0        0        0     1257 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/create_survey_response_201.py
--rw-r--r--   0        0        0     1398 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/create_survey_response_201_data.py
--rw-r--r--   0        0        0     1284 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/deliver_contract_json_body.py
--rw-r--r--   0        0        0     1275 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/deliver_contract_response_200.py
--rw-r--r--   0        0        0     1318 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/deliver_contract_response_200_data.py
--rw-r--r--   0        0        0     1292 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/dock_ship_dock_ship_200_response.py
--rw-r--r--   0        0        0     1227 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
--rw-r--r--   0        0        0     1368 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/extract_resources_json_body.py
--rw-r--r--   0        0        0     1281 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/extract_resources_response_201.py
--rw-r--r--   0        0        0     1532 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/extract_resources_response_201_data.py
--rw-r--r--   0        0        0     1261 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/extraction.py
--rw-r--r--   0        0        0     1250 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/extraction_yield.py
--rw-r--r--   0        0        0     1604 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/faction.py
--rw-r--r--   0        0        0     1421 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/faction_trait.py
--rw-r--r--   0        0        0     1869 2023-05-24 19:22:45.938239 spacetraders-0.5.0/spacetraders/models/faction_trait_symbol.py
--rw-r--r--   0        0        0     1275 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/fulfill_contract_response_200.py
--rw-r--r--   0        0        0     1301 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/fulfill_contract_response_200_data.py
--rw-r--r--   0        0        0     1175 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_contract_response_200.py
--rw-r--r--   0        0        0     1282 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_contracts_response_200.py
--rw-r--r--   0        0        0     1169 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/get_faction_response_200.py
--rw-r--r--   0        0        0     1276 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/get_factions_response_200.py
--rw-r--r--   0        0        0     1176 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_jump_gate_response_200.py
--rw-r--r--   0        0        0     1163 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_market_response_200.py
--rw-r--r--   0        0        0     1161 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_my_agent_response_200.py
--rw-r--r--   0        0        0     1186 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_my_ship_cargo_response_200.py
--rw-r--r--   0        0        0     1162 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/get_my_ship_response_200.py
--rw-r--r--   0        0        0     1262 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_my_ships_response_200.py
--rw-r--r--   0        0        0     1262 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_ship_cooldown_response_200.py
--rw-r--r--   0        0        0     1210 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_ship_nav_response_200.py
--rw-r--r--   0        0        0     1175 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_shipyard_response_200.py
--rw-r--r--   0        0        0     2640 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200.py
--rw-r--r--   0        0        0     1213 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_announcements_item.py
--rw-r--r--   0        0        0     1807 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards.py
--rw-r--r--   0        0        0     1264 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py
--rw-r--r--   0        0        0     1289 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py
--rw-r--r--   0        0        0     1191 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_links_item.py
--rw-r--r--   0        0        0     1314 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_server_resets.py
--rw-r--r--   0        0        0     1331 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_status_response_200_stats.py
--rw-r--r--   0        0        0     1163 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_system_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/get_system_waypoints_response_200.py
--rw-r--r--   0        0        0     1270 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/get_systems_response_200.py
--rw-r--r--   0        0        0     1266 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/get_waypoint_response_200.py
--rw-r--r--   0        0        0     1177 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/jettison_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/jettison_response_200.py
--rw-r--r--   0        0        0     1185 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/jettison_response_200_data.py
--rw-r--r--   0        0        0     1606 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/jump_gate.py
--rw-r--r--   0        0        0     1168 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/jump_ship_json_body.py
--rw-r--r--   0        0        0     1233 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/jump_ship_response_200.py
--rw-r--r--   0        0        0     1462 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/jump_ship_response_200_data.py
--rw-r--r--   0        0        0     2398 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/market.py
--rw-r--r--   0        0        0     1880 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/market_trade_good.py
--rw-r--r--   0        0        0      224 2023-05-24 19:22:45.828239 spacetraders-0.5.0/spacetraders/models/market_trade_good_supply.py
--rw-r--r--   0        0        0     2109 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/market_transaction.py
--rw-r--r--   0        0        0      170 2023-05-24 19:22:45.838239 spacetraders-0.5.0/spacetraders/models/market_transaction_type.py
--rw-r--r--   0        0        0     1206 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/meta.py
--rw-r--r--   0        0        0     1176 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/navigate_ship_json_body.py
--rw-r--r--   0        0        0     1257 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/navigate_ship_response_200.py
--rw-r--r--   0        0        0     1444 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/navigate_ship_response_200_data.py
--rw-r--r--   0        0        0     1400 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py
--rw-r--r--   0        0        0     1241 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py
--rw-r--r--   0        0        0     1304 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
--rw-r--r--   0        0        0     1231 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
--rw-r--r--   0        0        0     1420 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/patch_ship_nav_json_body.py
--rw-r--r--   0        0        0     1214 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/patch_ship_nav_response_200.py
--rw-r--r--   0        0        0     1352 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
--rw-r--r--   0        0        0     1484 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
--rw-r--r--   0        0        0     1211 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
--rw-r--r--   0        0        0     1333 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/purchase_ship_json_body.py
--rw-r--r--   0        0        0     1257 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/purchase_ship_response_201.py
--rw-r--r--   0        0        0     1447 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/purchase_ship_response_201_data.py
--rw-r--r--   0        0        0     1245 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/refuel_ship_response_200.py
--rw-r--r--   0        0        0     1562 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/refuel_ship_response_200_data.py
--rw-r--r--   0        0        0     1611 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/register_json_body.py
--rw-r--r--   0        0        0      244 2023-05-24 19:22:45.918239 spacetraders-0.5.0/spacetraders/models/register_json_body_faction.py
--rw-r--r--   0        0        0     1232 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/register_response_201.py
--rw-r--r--   0        0        0     1608 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/register_response_201_data.py
--rw-r--r--   0        0        0     2444 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/scanned_ship.py
--rw-r--r--   0        0        0     1144 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/scanned_ship_engine.py
--rw-r--r--   0        0        0     1141 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/scanned_ship_frame.py
--rw-r--r--   0        0        0     1149 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/scanned_ship_mounts_item.py
--rw-r--r--   0        0        0     1147 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/scanned_ship_reactor.py
--rw-r--r--   0        0        0     1492 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/scanned_system.py
--rw-r--r--   0        0        0     2293 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/scanned_waypoint.py
--rw-r--r--   0        0        0     1304 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
--rw-r--r--   0        0        0     1468 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
--rw-r--r--   0        0        0     1195 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_request.py
--rw-r--r--   0        0        0     3140 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship.py
--rw-r--r--   0        0        0     1484 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_cargo.py
--rw-r--r--   0        0        0     1510 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_cargo_item.py
--rw-r--r--   0        0        0     2248 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_crew.py
--rw-r--r--   0        0        0      167 2023-05-24 19:22:45.788239 spacetraders-0.5.0/spacetraders/models/ship_crew_rotation.py
--rw-r--r--   0        0        0     1879 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_engine.py
--rw-r--r--   0        0        0      319 2023-05-24 19:22:45.928239 spacetraders-0.5.0/spacetraders/models/ship_engine_symbol.py
--rw-r--r--   0        0        0     2278 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_frame.py
--rw-r--r--   0        0        0      694 2023-05-24 19:22:45.808239 spacetraders-0.5.0/spacetraders/models/ship_frame_symbol.py
--rw-r--r--   0        0        0     1586 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/ship_fuel.py
--rw-r--r--   0        0        0     1340 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/ship_fuel_consumed.py
--rw-r--r--   0        0        0     1965 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/ship_module.py
--rw-r--r--   0        0        0     1033 2023-05-24 19:22:45.848239 spacetraders-0.5.0/spacetraders/models/ship_module_symbol.py
--rw-r--r--   0        0        0     1947 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_mount.py
--rw-r--r--   0        0        0      572 2023-05-24 19:22:45.928239 spacetraders-0.5.0/spacetraders/models/ship_mount_deposits_item.py
--rw-r--r--   0        0        0      854 2023-05-24 19:22:45.928239 spacetraders-0.5.0/spacetraders/models/ship_mount_symbol.py
--rw-r--r--   0        0        0     2114 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/ship_nav.py
--rw-r--r--   0        0        0      206 2023-05-24 19:22:45.818239 spacetraders-0.5.0/spacetraders/models/ship_nav_flight_mode.py
--rw-r--r--   0        0        0     1891 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_nav_route.py
--rw-r--r--   0        0        0     1497 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_nav_route_waypoint.py
--rw-r--r--   0        0        0      196 2023-05-24 19:22:45.838239 spacetraders-0.5.0/spacetraders/models/ship_nav_status.py
--rw-r--r--   0        0        0     1934 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/ship_reactor.py
--rw-r--r--   0        0        0      344 2023-05-24 19:22:45.818239 spacetraders-0.5.0/spacetraders/models/ship_reactor_symbol.py
--rw-r--r--   0        0        0     1246 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/ship_refine_json_body.py
--rw-r--r--   0        0        0      330 2023-05-24 19:22:45.918239 spacetraders-0.5.0/spacetraders/models/ship_refine_json_body_produce.py
--rw-r--r--   0        0        0     1316 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response.py
--rw-r--r--   0        0        0     2047 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py
--rw-r--r--   0        0        0     1344 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
--rw-r--r--   0        0        0     1344 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
--rw-r--r--   0        0        0     1477 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/ship_registration.py
--rw-r--r--   0        0        0     1541 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/ship_requirements.py
--rw-r--r--   0        0        0      479 2023-05-24 19:22:45.898239 spacetraders-0.5.0/spacetraders/models/ship_role.py
--rw-r--r--   0        0        0      549 2023-05-24 19:22:45.798239 spacetraders-0.5.0/spacetraders/models/ship_type.py
--rw-r--r--   0        0        0     2009 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/shipyard.py
--rw-r--r--   0        0        0     2498 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/shipyard_ship.py
--rw-r--r--   0        0        0     1225 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/shipyard_ship_types_item.py
--rw-r--r--   0        0        0     1698 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/shipyard_transaction.py
--rw-r--r--   0        0        0     2228 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/survey.py
--rw-r--r--   0        0        0     1209 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/survey_deposit.py
--rw-r--r--   0        0        0      181 2023-05-24 19:22:45.818239 spacetraders-0.5.0/spacetraders/models/survey_size.py
--rw-r--r--   0        0        0     1725 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/system.py
--rw-r--r--   0        0        0     1112 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/system_faction.py
--rw-r--r--   0        0        0      405 2023-05-24 19:22:45.818239 spacetraders-0.5.0/spacetraders/models/system_type.py
--rw-r--r--   0        0        0     1352 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/system_waypoint.py
--rw-r--r--   0        0        0     1299 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/trade_good.py
--rw-r--r--   0        0        0     4422 2023-05-24 19:22:45.908239 spacetraders-0.5.0/spacetraders/models/trade_symbol.py
--rw-r--r--   0        0        0     1352 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
--rw-r--r--   0        0        0     1221 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
--rw-r--r--   0        0        0     1304 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
--rw-r--r--   0        0        0     1168 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/warp_ship_json_body.py
--rw-r--r--   0        0        0     1233 2023-05-24 19:22:47.228239 spacetraders-0.5.0/spacetraders/models/warp_ship_response_200.py
--rw-r--r--   0        0        0     1436 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/warp_ship_response_200_data.py
--rw-r--r--   0        0        0     2279 2023-05-24 19:22:47.238239 spacetraders-0.5.0/spacetraders/models/waypoint.py
--rw-r--r--   0        0        0     1116 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/waypoint_faction.py
--rw-r--r--   0        0        0     1178 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/waypoint_orbital.py
--rw-r--r--   0        0        0     1427 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/models/waypoint_trait.py
--rw-r--r--   0        0        0     2200 2023-05-24 19:22:45.938239 spacetraders-0.5.0/spacetraders/models/waypoint_trait_symbol.py
--rw-r--r--   0        0        0      381 2023-05-24 19:22:45.818239 spacetraders-0.5.0/spacetraders/models/waypoint_type.py
--rw-r--r--   0        0        0     1341 2023-05-24 19:22:47.248239 spacetraders-0.5.0/spacetraders/types.py
--rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 spacetraders-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.6.0/README.md
+-rw-r--r--   0        0        0      664 2023-06-05 13:55:27.670386 spacetraders-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      250 2023-06-05 13:53:26.330387 spacetraders-0.6.0/spacetraders/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-05 13:53:25.790387 spacetraders-0.6.0/spacetraders/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 13:53:25.840387 spacetraders-0.6.0/spacetraders/api/agents/__init__.py
+-rw-r--r--   0        0        0     4139 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/agents/get_my_agent.py
+-rw-r--r--   0        0        0        0 2023-06-05 13:53:25.840387 spacetraders-0.6.0/spacetraders/api/contracts/__init__.py
+-rw-r--r--   0        0        0     4425 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/contracts/accept_contract.py
+-rw-r--r--   0        0        0     5022 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/contracts/deliver_contract.py
+-rw-r--r--   0        0        0     4437 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/contracts/fulfill_contract.py
+-rw-r--r--   0        0        0     4420 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/contracts/get_contract.py
+-rw-r--r--   0        0        0     4900 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/contracts/get_contracts.py
+-rw-r--r--   0        0        0        0 2023-06-05 13:53:25.800387 spacetraders-0.6.0/spacetraders/api/default/__init__.py
+-rw-r--r--   0        0        0     4069 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/default/get_status.py
+-rw-r--r--   0        0        0     6960 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/default/register.py
+-rw-r--r--   0        0        0        0 2023-06-05 13:53:25.840387 spacetraders-0.6.0/spacetraders/api/factions/__init__.py
+-rw-r--r--   0        0        0     4427 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/factions/get_faction.py
+-rw-r--r--   0        0        0     4853 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/factions/get_factions.py
+-rw-r--r--   0        0        0        0 2023-06-05 13:53:25.850387 spacetraders-0.6.0/spacetraders/api/fleet/__init__.py
+-rw-r--r--   0        0        0     4900 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/create_chart.py
+-rw-r--r--   0        0        0     4550 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/create_ship_ship_scan.py
+-rw-r--r--   0        0        0     4587 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/create_ship_system_scan.py
+-rw-r--r--   0        0        0     4615 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
+-rw-r--r--   0        0        0     5382 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/create_survey.py
+-rw-r--r--   0        0        0     4961 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/dock_ship.py
+-rw-r--r--   0        0        0     5217 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/extract_resources.py
+-rw-r--r--   0        0        0     4462 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/get_mounts.py
+-rw-r--r--   0        0        0     4373 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/get_my_ship.py
+-rw-r--r--   0        0        0     4447 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/get_my_ship_cargo.py
+-rw-r--r--   0        0        0     4871 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/get_my_ships.py
+-rw-r--r--   0        0        0     5562 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/get_ship_cooldown.py
+-rw-r--r--   0        0        0     4414 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/get_ship_nav.py
+-rw-r--r--   0        0        0     5182 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/install_mount.py
+-rw-r--r--   0        0        0     4905 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/jettison.py
+-rw-r--r--   0        0        0     5343 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/jump_ship.py
+-rw-r--r--   0        0        0     5893 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/navigate_ship.py
+-rw-r--r--   0        0        0     4905 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/negotiate_contract.py
+-rw-r--r--   0        0        0     4954 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/orbit_ship.py
+-rw-r--r--   0        0        0     5001 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/patch_ship_nav.py
+-rw-r--r--   0        0        0     5192 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/purchase_cargo.py
+-rw-r--r--   0        0        0     4680 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/purchase_ship.py
+-rw-r--r--   0        0        0     4419 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/fleet/refuel_ship.py
+-rw-r--r--   0        0        0     5136 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/remove_mount.py
+-rw-r--r--   0        0        0     5010 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/sell_cargo.py
+-rw-r--r--   0        0        0     5244 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/ship_refine.py
+-rw-r--r--   0        0        0     5215 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/fleet/transfer_cargo.py
+-rw-r--r--   0        0        0     5569 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/fleet/warp_ship.py
+-rw-r--r--   0        0        0        0 2023-06-05 13:53:25.840387 spacetraders-0.6.0/spacetraders/api/systems/__init__.py
+-rw-r--r--   0        0        0     4735 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/systems/get_jump_gate.py
+-rw-r--r--   0        0        0     5121 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/api/systems/get_market.py
+-rw-r--r--   0        0        0     4951 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/systems/get_shipyard.py
+-rw-r--r--   0        0        0     4469 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/systems/get_system.py
+-rw-r--r--   0        0        0     5421 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/systems/get_system_waypoints.py
+-rw-r--r--   0        0        0     4877 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/api/systems/get_systems.py
+-rw-r--r--   0        0        0     4710 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/api/systems/get_waypoint.py
+-rw-r--r--   0        0        0     4384 2023-06-05 13:53:26.670387 spacetraders-0.6.0/spacetraders/client.py
+-rw-r--r--   0        0        0      470 2023-06-05 13:53:26.580387 spacetraders-0.6.0/spacetraders/errors.py
+-rw-r--r--   0        0        0    15720 2023-06-05 13:53:26.830387 spacetraders-0.6.0/spacetraders/models/__init__.py
+-rw-r--r--   0        0        0     1269 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/accept_contract_response_200.py
+-rw-r--r--   0        0        0     1299 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/accept_contract_response_200_data.py
+-rw-r--r--   0        0        0     1587 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/agent.py
+-rw-r--r--   0        0        0     1532 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/chart.py
+-rw-r--r--   0        0        0     1709 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/connected_system.py
+-rw-r--r--   0        0        0     2160 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/contract.py
+-rw-r--r--   0        0        0     1712 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/contract_deliver_good.py
+-rw-r--r--   0        0        0     1340 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/contract_payment.py
+-rw-r--r--   0        0        0     1567 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/contract_terms.py
+-rw-r--r--   0        0        0      201 2023-06-05 13:53:25.970387 spacetraders-0.6.0/spacetraders/models/contract_type.py
+-rw-r--r--   0        0        0     1744 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/cooldown.py
+-rw-r--r--   0        0        0     1251 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_chart_response_201.py
+-rw-r--r--   0        0        0     1469 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_chart_response_201_data.py
+-rw-r--r--   0        0        0     1304 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_ship_ship_scan_response_201.py
+-rw-r--r--   0        0        0     1425 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
+-rw-r--r--   0        0        0     1316 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_ship_system_scan_response_201.py
+-rw-r--r--   0        0        0     1443 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/create_ship_system_scan_response_201_data.py
+-rw-r--r--   0        0        0     1328 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
+-rw-r--r--   0        0        0     1461 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
+-rw-r--r--   0        0        0     1257 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/create_survey_response_201.py
+-rw-r--r--   0        0        0     1398 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/create_survey_response_201_data.py
+-rw-r--r--   0        0        0     1284 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/deliver_contract_json_body.py
+-rw-r--r--   0        0        0     1275 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/deliver_contract_response_200.py
+-rw-r--r--   0        0        0     1318 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/deliver_contract_response_200_data.py
+-rw-r--r--   0        0        0     1292 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/dock_ship_dock_ship_200_response.py
+-rw-r--r--   0        0        0     1227 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
+-rw-r--r--   0        0        0     1368 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/extract_resources_json_body.py
+-rw-r--r--   0        0        0     1281 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/extract_resources_response_201.py
+-rw-r--r--   0        0        0     1532 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/extract_resources_response_201_data.py
+-rw-r--r--   0        0        0     1261 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/extraction.py
+-rw-r--r--   0        0        0     1250 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/extraction_yield.py
+-rw-r--r--   0        0        0     1604 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/faction.py
+-rw-r--r--   0        0        0     1421 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/faction_trait.py
+-rw-r--r--   0        0        0     1869 2023-06-05 13:53:26.060387 spacetraders-0.6.0/spacetraders/models/faction_trait_symbol.py
+-rw-r--r--   0        0        0     1275 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/fulfill_contract_response_200.py
+-rw-r--r--   0        0        0     1301 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/fulfill_contract_response_200_data.py
+-rw-r--r--   0        0        0     1175 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_contract_response_200.py
+-rw-r--r--   0        0        0     1282 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_contracts_response_200.py
+-rw-r--r--   0        0        0     1169 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_faction_response_200.py
+-rw-r--r--   0        0        0     1276 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_factions_response_200.py
+-rw-r--r--   0        0        0     1176 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_jump_gate_response_200.py
+-rw-r--r--   0        0        0     1163 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_market_response_200.py
+-rw-r--r--   0        0        0     1208 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_mounts_get_mounts_200_response.py
+-rw-r--r--   0        0        0     1161 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_my_agent_response_200.py
+-rw-r--r--   0        0        0     1186 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/get_my_ship_cargo_response_200.py
+-rw-r--r--   0        0        0     1162 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_my_ship_response_200.py
+-rw-r--r--   0        0        0     1262 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_my_ships_response_200.py
+-rw-r--r--   0        0        0     1262 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_ship_cooldown_response_200.py
+-rw-r--r--   0        0        0     1210 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/get_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1175 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_shipyard_response_200.py
+-rw-r--r--   0        0        0     2640 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_status_response_200.py
+-rw-r--r--   0        0        0     1213 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_announcements_item.py
+-rw-r--r--   0        0        0     1807 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards.py
+-rw-r--r--   0        0        0     1264 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py
+-rw-r--r--   0        0        0     1289 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py
+-rw-r--r--   0        0        0     1191 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_links_item.py
+-rw-r--r--   0        0        0     1314 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_server_resets.py
+-rw-r--r--   0        0        0     1331 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_status_response_200_stats.py
+-rw-r--r--   0        0        0     1163 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/get_system_response_200.py
+-rw-r--r--   0        0        0     1294 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_system_waypoints_response_200.py
+-rw-r--r--   0        0        0     1270 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_systems_response_200.py
+-rw-r--r--   0        0        0     1266 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/get_waypoint_response_200.py
+-rw-r--r--   0        0        0     1340 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_201_response.py
+-rw-r--r--   0        0        0     1773 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_201_response_data.py
+-rw-r--r--   0        0        0     1385 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_201_response_data_transaction.py
+-rw-r--r--   0        0        0     1148 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/install_mount_install_mount_request.py
+-rw-r--r--   0        0        0     1177 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/jettison_json_body.py
+-rw-r--r--   0        0        0     1232 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/jettison_response_200.py
+-rw-r--r--   0        0        0     1185 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/jettison_response_200_data.py
+-rw-r--r--   0        0        0     1606 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/jump_gate.py
+-rw-r--r--   0        0        0     1168 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/jump_ship_json_body.py
+-rw-r--r--   0        0        0     1233 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/jump_ship_response_200.py
+-rw-r--r--   0        0        0     1462 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/jump_ship_response_200_data.py
+-rw-r--r--   0        0        0     2398 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/market.py
+-rw-r--r--   0        0        0     1880 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/market_trade_good.py
+-rw-r--r--   0        0        0      224 2023-06-05 13:53:25.980387 spacetraders-0.6.0/spacetraders/models/market_trade_good_supply.py
+-rw-r--r--   0        0        0     2109 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/market_transaction.py
+-rw-r--r--   0        0        0      170 2023-06-05 13:53:25.980387 spacetraders-0.6.0/spacetraders/models/market_transaction_type.py
+-rw-r--r--   0        0        0     1206 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/meta.py
+-rw-r--r--   0        0        0     1176 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/navigate_ship_json_body.py
+-rw-r--r--   0        0        0     1257 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/navigate_ship_response_200.py
+-rw-r--r--   0        0        0     1444 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/navigate_ship_response_200_data.py
+-rw-r--r--   0        0        0     1400 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py
+-rw-r--r--   0        0        0     1241 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py
+-rw-r--r--   0        0        0     1304 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
+-rw-r--r--   0        0        0     1231 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
+-rw-r--r--   0        0        0     1420 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/patch_ship_nav_json_body.py
+-rw-r--r--   0        0        0     1214 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/patch_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1352 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
+-rw-r--r--   0        0        0     1484 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1211 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
+-rw-r--r--   0        0        0     1333 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/purchase_ship_json_body.py
+-rw-r--r--   0        0        0     1257 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/purchase_ship_response_201.py
+-rw-r--r--   0        0        0     1447 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/purchase_ship_response_201_data.py
+-rw-r--r--   0        0        0     1245 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/refuel_ship_response_200.py
+-rw-r--r--   0        0        0     1562 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/refuel_ship_response_200_data.py
+-rw-r--r--   0        0        0     1516 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/register_json_body.py
+-rw-r--r--   0        0        0     1232 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/register_response_201.py
+-rw-r--r--   0        0        0     1608 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/register_response_201_data.py
+-rw-r--r--   0        0        0     1328 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_201_response.py
+-rw-r--r--   0        0        0     1761 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_201_response_data.py
+-rw-r--r--   0        0        0     1381 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_201_response_data_transaction.py
+-rw-r--r--   0        0        0     1144 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/remove_mount_remove_mount_request.py
+-rw-r--r--   0        0        0     2444 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/scanned_ship.py
+-rw-r--r--   0        0        0     1144 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/scanned_ship_engine.py
+-rw-r--r--   0        0        0     1141 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/scanned_ship_frame.py
+-rw-r--r--   0        0        0     1149 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/scanned_ship_mounts_item.py
+-rw-r--r--   0        0        0     1147 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/scanned_ship_reactor.py
+-rw-r--r--   0        0        0     1492 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/scanned_system.py
+-rw-r--r--   0        0        0     2293 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/scanned_waypoint.py
+-rw-r--r--   0        0        0     1304 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
+-rw-r--r--   0        0        0     1468 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1195 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_request.py
+-rw-r--r--   0        0        0     3140 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship.py
+-rw-r--r--   0        0        0     1484 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_cargo.py
+-rw-r--r--   0        0        0     1510 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_cargo_item.py
+-rw-r--r--   0        0        0     2248 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_crew.py
+-rw-r--r--   0        0        0      167 2023-06-05 13:53:25.940387 spacetraders-0.6.0/spacetraders/models/ship_crew_rotation.py
+-rw-r--r--   0        0        0     1879 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_engine.py
+-rw-r--r--   0        0        0      319 2023-06-05 13:53:26.040387 spacetraders-0.6.0/spacetraders/models/ship_engine_symbol.py
+-rw-r--r--   0        0        0     2278 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_frame.py
+-rw-r--r--   0        0        0      694 2023-06-05 13:53:25.960387 spacetraders-0.6.0/spacetraders/models/ship_frame_symbol.py
+-rw-r--r--   0        0        0     1586 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_fuel.py
+-rw-r--r--   0        0        0     1340 2023-06-05 13:53:27.170387 spacetraders-0.6.0/spacetraders/models/ship_fuel_consumed.py
+-rw-r--r--   0        0        0     1965 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_module.py
+-rw-r--r--   0        0        0     1033 2023-06-05 13:53:25.990387 spacetraders-0.6.0/spacetraders/models/ship_module_symbol.py
+-rw-r--r--   0        0        0     1947 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_mount.py
+-rw-r--r--   0        0        0      572 2023-06-05 13:53:26.050387 spacetraders-0.6.0/spacetraders/models/ship_mount_deposits_item.py
+-rw-r--r--   0        0        0      854 2023-06-05 13:53:26.050387 spacetraders-0.6.0/spacetraders/models/ship_mount_symbol.py
+-rw-r--r--   0        0        0     2114 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_nav.py
+-rw-r--r--   0        0        0      206 2023-06-05 13:53:25.960387 spacetraders-0.6.0/spacetraders/models/ship_nav_flight_mode.py
+-rw-r--r--   0        0        0     1891 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_nav_route.py
+-rw-r--r--   0        0        0     1497 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_nav_route_waypoint.py
+-rw-r--r--   0        0        0      196 2023-06-05 13:53:25.980387 spacetraders-0.6.0/spacetraders/models/ship_nav_status.py
+-rw-r--r--   0        0        0     1934 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_reactor.py
+-rw-r--r--   0        0        0      344 2023-06-05 13:53:25.960387 spacetraders-0.6.0/spacetraders/models/ship_reactor_symbol.py
+-rw-r--r--   0        0        0     1246 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_refine_json_body.py
+-rw-r--r--   0        0        0      330 2023-06-05 13:53:26.040387 spacetraders-0.6.0/spacetraders/models/ship_refine_json_body_produce.py
+-rw-r--r--   0        0        0     1316 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response.py
+-rw-r--r--   0        0        0     2047 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py
+-rw-r--r--   0        0        0     1344 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
+-rw-r--r--   0        0        0     1344 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
+-rw-r--r--   0        0        0     1477 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_registration.py
+-rw-r--r--   0        0        0     1541 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/ship_requirements.py
+-rw-r--r--   0        0        0      479 2023-06-05 13:53:26.030387 spacetraders-0.6.0/spacetraders/models/ship_role.py
+-rw-r--r--   0        0        0      549 2023-06-05 13:53:25.950387 spacetraders-0.6.0/spacetraders/models/ship_type.py
+-rw-r--r--   0        0        0     2009 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/shipyard.py
+-rw-r--r--   0        0        0     2498 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/shipyard_ship.py
+-rw-r--r--   0        0        0     1225 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/shipyard_ship_types_item.py
+-rw-r--r--   0        0        0     1698 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/shipyard_transaction.py
+-rw-r--r--   0        0        0     2228 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/survey.py
+-rw-r--r--   0        0        0     1209 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/survey_deposit.py
+-rw-r--r--   0        0        0      181 2023-06-05 13:53:25.970387 spacetraders-0.6.0/spacetraders/models/survey_size.py
+-rw-r--r--   0        0        0     1725 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/system.py
+-rw-r--r--   0        0        0     1112 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/system_faction.py
+-rw-r--r--   0        0        0      405 2023-06-05 13:53:25.960387 spacetraders-0.6.0/spacetraders/models/system_type.py
+-rw-r--r--   0        0        0     1352 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/system_waypoint.py
+-rw-r--r--   0        0        0     1299 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/trade_good.py
+-rw-r--r--   0        0        0     4422 2023-06-05 13:53:26.030387 spacetraders-0.6.0/spacetraders/models/trade_symbol.py
+-rw-r--r--   0        0        0     1352 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
+-rw-r--r--   0        0        0     1221 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
+-rw-r--r--   0        0        0     1304 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
+-rw-r--r--   0        0        0     1168 2023-06-05 13:53:27.140387 spacetraders-0.6.0/spacetraders/models/warp_ship_json_body.py
+-rw-r--r--   0        0        0     1233 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/warp_ship_response_200.py
+-rw-r--r--   0        0        0     1436 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/warp_ship_response_200_data.py
+-rw-r--r--   0        0        0     2279 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/waypoint.py
+-rw-r--r--   0        0        0     1116 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/waypoint_faction.py
+-rw-r--r--   0        0        0     1178 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/models/waypoint_orbital.py
+-rw-r--r--   0        0        0     1427 2023-06-05 13:53:27.150387 spacetraders-0.6.0/spacetraders/models/waypoint_trait.py
+-rw-r--r--   0        0        0     2200 2023-06-05 13:53:26.060387 spacetraders-0.6.0/spacetraders/models/waypoint_trait_symbol.py
+-rw-r--r--   0        0        0      381 2023-06-05 13:53:25.970387 spacetraders-0.6.0/spacetraders/models/waypoint_type.py
+-rw-r--r--   0        0        0     1341 2023-06-05 13:53:27.160387 spacetraders-0.6.0/spacetraders/types.py
+-rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 spacetraders-0.6.0/PKG-INFO
```

### Comparing `spacetraders-0.5.0/README.md` & `spacetraders-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/pyproject.toml` & `spacetraders-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacetraders"
-version = "0.5.0"
+version = "0.6.0"
 description = "Python API for Space Traders"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "spacetraders"}]
 
 [tool.poetry.dependencies]
```

### Comparing `spacetraders-0.5.0/spacetraders/api/agents/get_my_agent.py` & `spacetraders-0.6.0/spacetraders/api/agents/get_my_agent.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/contracts/accept_contract.py` & `spacetraders-0.6.0/spacetraders/api/contracts/accept_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/contracts/deliver_contract.py` & `spacetraders-0.6.0/spacetraders/api/contracts/deliver_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/contracts/fulfill_contract.py` & `spacetraders-0.6.0/spacetraders/api/contracts/fulfill_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/contracts/get_contract.py` & `spacetraders-0.6.0/spacetraders/api/contracts/get_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/contracts/get_contracts.py` & `spacetraders-0.6.0/spacetraders/api/contracts/get_contracts.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/default/get_status.py` & `spacetraders-0.6.0/spacetraders/api/default/get_status.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/default/register.py` & `spacetraders-0.6.0/spacetraders/api/default/register.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/factions/get_faction.py` & `spacetraders-0.6.0/spacetraders/api/factions/get_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/factions/get_factions.py` & `spacetraders-0.6.0/spacetraders/api/factions/get_factions.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/create_chart.py` & `spacetraders-0.6.0/spacetraders/api/fleet/create_chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/create_ship_ship_scan.py` & `spacetraders-0.6.0/spacetraders/api/fleet/create_ship_ship_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/create_ship_system_scan.py` & `spacetraders-0.6.0/spacetraders/api/fleet/create_ship_system_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/create_ship_waypoint_scan.py` & `spacetraders-0.6.0/spacetraders/api/fleet/create_ship_waypoint_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/create_survey.py` & `spacetraders-0.6.0/spacetraders/api/fleet/create_survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/dock_ship.py` & `spacetraders-0.6.0/spacetraders/api/fleet/dock_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/extract_resources.py` & `spacetraders-0.6.0/spacetraders/api/fleet/extract_resources.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/get_my_ship.py` & `spacetraders-0.6.0/spacetraders/api/fleet/get_my_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/get_my_ship_cargo.py` & `spacetraders-0.6.0/spacetraders/api/fleet/get_my_ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/get_my_ships.py` & `spacetraders-0.6.0/spacetraders/api/fleet/get_my_ships.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/get_ship_cooldown.py` & `spacetraders-0.6.0/spacetraders/api/fleet/get_ship_cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/get_ship_nav.py` & `spacetraders-0.6.0/spacetraders/api/fleet/get_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/jettison.py` & `spacetraders-0.6.0/spacetraders/api/fleet/jettison.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/jump_ship.py` & `spacetraders-0.6.0/spacetraders/api/fleet/jump_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/navigate_ship.py` & `spacetraders-0.6.0/spacetraders/api/fleet/navigate_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/negotiate_contract.py` & `spacetraders-0.6.0/spacetraders/api/fleet/negotiate_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/orbit_ship.py` & `spacetraders-0.6.0/spacetraders/api/fleet/orbit_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/patch_ship_nav.py` & `spacetraders-0.6.0/spacetraders/api/fleet/patch_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/purchase_cargo.py` & `spacetraders-0.6.0/spacetraders/api/fleet/purchase_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/purchase_ship.py` & `spacetraders-0.6.0/spacetraders/api/fleet/purchase_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/refuel_ship.py` & `spacetraders-0.6.0/spacetraders/api/fleet/refuel_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/sell_cargo.py` & `spacetraders-0.6.0/spacetraders/api/fleet/sell_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/ship_refine.py` & `spacetraders-0.6.0/spacetraders/api/fleet/ship_refine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/transfer_cargo.py` & `spacetraders-0.6.0/spacetraders/api/fleet/transfer_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/fleet/warp_ship.py` & `spacetraders-0.6.0/spacetraders/api/fleet/warp_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/systems/get_jump_gate.py` & `spacetraders-0.6.0/spacetraders/api/systems/get_jump_gate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import Client
+from ...client import AuthenticatedClient, Client
 from ...models.get_jump_gate_response_200 import GetJumpGateResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/jump-gate".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -57,15 +57,15 @@
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetJumpGateResponse200]:
     """Get Jump Gate
 
      Get jump gate details for a waypoint.
 
     Args:
@@ -118,15 +118,15 @@
     )
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetJumpGateResponse200]:
     """Get Jump Gate
 
      Get jump gate details for a waypoint.
 
     Args:
```

### Comparing `spacetraders-0.5.0/spacetraders/api/systems/get_market.py` & `spacetraders-0.6.0/spacetraders/api/systems/get_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import Client
+from ...client import AuthenticatedClient, Client
 from ...models.get_market_response_200 import GetMarketResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/market".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -57,15 +57,15 @@
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetMarketResponse200]:
     """Get Market
 
      Retrieve imports, exports and exchange data from a marketplace. Imports can be sold, exports can be
     purchased, and exchange goods can be purchased or sold. Send a ship to the waypoint to access trade
     good prices and recent transactions.
@@ -120,15 +120,15 @@
     )
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetMarketResponse200]:
     """Get Market
 
      Retrieve imports, exports and exchange data from a marketplace. Imports can be sold, exports can be
     purchased, and exchange goods can be purchased or sold. Send a ship to the waypoint to access trade
     good prices and recent transactions.
```

### Comparing `spacetraders-0.5.0/spacetraders/api/systems/get_shipyard.py` & `spacetraders-0.6.0/spacetraders/api/systems/get_shipyard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import Client
+from ...client import AuthenticatedClient, Client
 from ...models.get_shipyard_response_200 import GetShipyardResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/shipyard".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -57,15 +57,15 @@
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetShipyardResponse200]:
     """Get Shipyard
 
      Get the shipyard for a waypoint. Send a ship to the waypoint to access ships that are currently
     available for purchase and recent transactions.
 
@@ -119,15 +119,15 @@
     )
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetShipyardResponse200]:
     """Get Shipyard
 
      Get the shipyard for a waypoint. Send a ship to the waypoint to access ships that are currently
     available for purchase and recent transactions.
```

### Comparing `spacetraders-0.5.0/spacetraders/api/systems/get_system.py` & `spacetraders-0.6.0/spacetraders/api/systems/get_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import Client
+from ...client import AuthenticatedClient, Client
 from ...models.get_system_response_200 import GetSystemResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str = "X1-OE",
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}".format(
         _client.base_url, systemSymbol=system_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -55,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     system_symbol: str = "X1-OE",
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetSystemResponse200]:
     """Get System
 
      Get the details of a system.
 
     Args:
@@ -113,15 +113,15 @@
         )
     )
 
 
 async def asyncio_detailed(
     system_symbol: str = "X1-OE",
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetSystemResponse200]:
     """Get System
 
      Get the details of a system.
 
     Args:
```

### Comparing `spacetraders-0.5.0/spacetraders/api/systems/get_system_waypoints.py` & `spacetraders-0.6.0/spacetraders/api/systems/get_system_waypoints.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/api/systems/get_systems.py` & `spacetraders-0.6.0/spacetraders/api/systems/get_systems.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import Client
+from ...client import AuthenticatedClient, Client
 from ...models.get_systems_response_200 import GetSystemsResponse200
 from ...types import UNSET, ApiError, Error, Response, Unset
 
 
 def _get_kwargs(
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Dict[str, Any]:
     url = "{}/systems".format(_client.base_url)
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -61,15 +61,15 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetSystemsResponse200]:
     """List Systems
 
      Return a list of all systems.
@@ -122,15 +122,15 @@
             headers=resp.headers,
         )
     )
 
 
 async def asyncio_detailed(
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetSystemsResponse200]:
     """List Systems
 
      Return a list of all systems.
```

### Comparing `spacetraders-0.5.0/spacetraders/api/systems/get_waypoint.py` & `spacetraders-0.6.0/spacetraders/api/systems/get_waypoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
-from ...client import Client
+from ...client import AuthenticatedClient, Client
 from ...models.get_waypoint_response_200 import GetWaypointResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
@@ -57,15 +57,15 @@
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetWaypointResponse200]:
     """Get Waypoint
 
      View the details of a waypoint.
 
     Args:
@@ -118,15 +118,15 @@
     )
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    _client: Client,
+    _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
 ) -> Response[GetWaypointResponse200]:
     """Get Waypoint
 
      View the details of a waypoint.
 
     Args:
```

### Comparing `spacetraders-0.5.0/spacetraders/client.py` & `spacetraders-0.6.0/spacetraders/client.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/__init__.py` & `spacetraders-0.6.0/spacetraders/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from .fulfill_contract_response_200_data import FulfillContractResponse200Data
 from .get_contract_response_200 import GetContractResponse200
 from .get_contracts_response_200 import GetContractsResponse200
 from .get_faction_response_200 import GetFactionResponse200
 from .get_factions_response_200 import GetFactionsResponse200
 from .get_jump_gate_response_200 import GetJumpGateResponse200
 from .get_market_response_200 import GetMarketResponse200
+from .get_mounts_get_mounts_200_response import GetMountsGetMounts200Response
 from .get_my_agent_response_200 import GetMyAgentResponse200
 from .get_my_ship_cargo_response_200 import GetMyShipCargoResponse200
 from .get_my_ship_response_200 import GetMyShipResponse200
 from .get_my_ships_response_200 import GetMyShipsResponse200
 from .get_ship_cooldown_response_200 import GetShipCooldownResponse200
 from .get_ship_nav_response_200 import GetShipNavResponse200
 from .get_shipyard_response_200 import GetShipyardResponse200
@@ -67,14 +68,24 @@
 from .get_status_response_200_links_item import GetStatusResponse200LinksItem
 from .get_status_response_200_server_resets import GetStatusResponse200ServerResets
 from .get_status_response_200_stats import GetStatusResponse200Stats
 from .get_system_response_200 import GetSystemResponse200
 from .get_system_waypoints_response_200 import GetSystemWaypointsResponse200
 from .get_systems_response_200 import GetSystemsResponse200
 from .get_waypoint_response_200 import GetWaypointResponse200
+from .install_mount_install_mount_201_response import (
+    InstallMountInstallMount201Response,
+)
+from .install_mount_install_mount_201_response_data import (
+    InstallMountInstallMount201ResponseData,
+)
+from .install_mount_install_mount_201_response_data_transaction import (
+    InstallMountInstallMount201ResponseDataTransaction,
+)
+from .install_mount_install_mount_request import InstallMountInstallMountRequest
 from .jettison_json_body import JettisonJsonBody
 from .jettison_response_200 import JettisonResponse200
 from .jettison_response_200_data import JettisonResponse200Data
 from .jump_gate import JumpGate
 from .jump_ship_json_body import JumpShipJsonBody
 from .jump_ship_response_200 import JumpShipResponse200
 from .jump_ship_response_200_data import JumpShipResponse200Data
@@ -106,17 +117,24 @@
 from .purchase_cargo_purchase_cargo_request import PurchaseCargoPurchaseCargoRequest
 from .purchase_ship_json_body import PurchaseShipJsonBody
 from .purchase_ship_response_201 import PurchaseShipResponse201
 from .purchase_ship_response_201_data import PurchaseShipResponse201Data
 from .refuel_ship_response_200 import RefuelShipResponse200
 from .refuel_ship_response_200_data import RefuelShipResponse200Data
 from .register_json_body import RegisterJsonBody
-from .register_json_body_faction import RegisterJsonBodyFaction
 from .register_response_201 import RegisterResponse201
 from .register_response_201_data import RegisterResponse201Data
+from .remove_mount_remove_mount_201_response import RemoveMountRemoveMount201Response
+from .remove_mount_remove_mount_201_response_data import (
+    RemoveMountRemoveMount201ResponseData,
+)
+from .remove_mount_remove_mount_201_response_data_transaction import (
+    RemoveMountRemoveMount201ResponseDataTransaction,
+)
+from .remove_mount_remove_mount_request import RemoveMountRemoveMountRequest
 from .scanned_ship import ScannedShip
 from .scanned_ship_engine import ScannedShipEngine
 from .scanned_ship_frame import ScannedShipFrame
 from .scanned_ship_mounts_item import ScannedShipMountsItem
 from .scanned_ship_reactor import ScannedShipReactor
 from .scanned_system import ScannedSystem
 from .scanned_waypoint import ScannedWaypoint
@@ -231,14 +249,15 @@
     "FulfillContractResponse200Data",
     "GetContractResponse200",
     "GetContractsResponse200",
     "GetFactionResponse200",
     "GetFactionsResponse200",
     "GetJumpGateResponse200",
     "GetMarketResponse200",
+    "GetMountsGetMounts200Response",
     "GetMyAgentResponse200",
     "GetMyShipCargoResponse200",
     "GetMyShipResponse200",
     "GetMyShipsResponse200",
     "GetShipCooldownResponse200",
     "GetShipNavResponse200",
     "GetShipyardResponse200",
@@ -250,14 +269,18 @@
     "GetStatusResponse200LinksItem",
     "GetStatusResponse200ServerResets",
     "GetStatusResponse200Stats",
     "GetSystemResponse200",
     "GetSystemsResponse200",
     "GetSystemWaypointsResponse200",
     "GetWaypointResponse200",
+    "InstallMountInstallMount201Response",
+    "InstallMountInstallMount201ResponseData",
+    "InstallMountInstallMount201ResponseDataTransaction",
+    "InstallMountInstallMountRequest",
     "JettisonJsonBody",
     "JettisonResponse200",
     "JettisonResponse200Data",
     "JumpGate",
     "JumpShipJsonBody",
     "JumpShipResponse200",
     "JumpShipResponse200Data",
@@ -281,17 +304,20 @@
     "PurchaseCargoPurchaseCargoRequest",
     "PurchaseShipJsonBody",
     "PurchaseShipResponse201",
     "PurchaseShipResponse201Data",
     "RefuelShipResponse200",
     "RefuelShipResponse200Data",
     "RegisterJsonBody",
-    "RegisterJsonBodyFaction",
     "RegisterResponse201",
     "RegisterResponse201Data",
+    "RemoveMountRemoveMount201Response",
+    "RemoveMountRemoveMount201ResponseData",
+    "RemoveMountRemoveMount201ResponseDataTransaction",
+    "RemoveMountRemoveMountRequest",
     "ScannedShip",
     "ScannedShipEngine",
     "ScannedShipFrame",
     "ScannedShipMountsItem",
     "ScannedShipReactor",
     "ScannedSystem",
     "ScannedWaypoint",
```

### Comparing `spacetraders-0.5.0/spacetraders/models/accept_contract_response_200.py` & `spacetraders-0.6.0/spacetraders/models/accept_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/accept_contract_response_200_data.py` & `spacetraders-0.6.0/spacetraders/models/accept_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/agent.py` & `spacetraders-0.6.0/spacetraders/models/agent.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/chart.py` & `spacetraders-0.6.0/spacetraders/models/chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/connected_system.py` & `spacetraders-0.6.0/spacetraders/models/connected_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/contract.py` & `spacetraders-0.6.0/spacetraders/models/contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/contract_deliver_good.py` & `spacetraders-0.6.0/spacetraders/models/contract_deliver_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/contract_payment.py` & `spacetraders-0.6.0/spacetraders/models/contract_payment.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/contract_terms.py` & `spacetraders-0.6.0/spacetraders/models/contract_terms.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/cooldown.py` & `spacetraders-0.6.0/spacetraders/models/cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/create_chart_response_201.py` & `spacetraders-0.6.0/spacetraders/models/create_chart_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/create_chart_response_201_data.py` & `spacetraders-0.6.0/spacetraders/models/create_chart_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/create_ship_ship_scan_response_201.py` & `spacetraders-0.6.0/spacetraders/models/create_ship_ship_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/create_ship_ship_scan_response_201_data.py` & `spacetraders-0.6.0/spacetraders/models/create_ship_ship_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/create_ship_system_scan_response_201.py` & `spacetraders-0.6.0/spacetraders/models/create_ship_system_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/create_ship_system_scan_response_201_data.py` & `spacetraders-0.6.0/spacetraders/models/create_ship_system_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/create_ship_waypoint_scan_response_201.py` & `spacetraders-0.6.0/spacetraders/models/create_ship_waypoint_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py` & `spacetraders-0.6.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/create_survey_response_201.py` & `spacetraders-0.6.0/spacetraders/models/create_survey_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/create_survey_response_201_data.py` & `spacetraders-0.6.0/spacetraders/models/create_survey_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/deliver_contract_json_body.py` & `spacetraders-0.6.0/spacetraders/models/deliver_contract_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/deliver_contract_response_200.py` & `spacetraders-0.6.0/spacetraders/models/deliver_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/deliver_contract_response_200_data.py` & `spacetraders-0.6.0/spacetraders/models/deliver_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/dock_ship_dock_ship_200_response.py` & `spacetraders-0.6.0/spacetraders/models/dock_ship_dock_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py` & `spacetraders-0.6.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/extract_resources_json_body.py` & `spacetraders-0.6.0/spacetraders/models/extract_resources_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/extract_resources_response_201.py` & `spacetraders-0.6.0/spacetraders/models/extract_resources_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/extract_resources_response_201_data.py` & `spacetraders-0.6.0/spacetraders/models/extract_resources_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/extraction.py` & `spacetraders-0.6.0/spacetraders/models/extraction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/extraction_yield.py` & `spacetraders-0.6.0/spacetraders/models/extraction_yield.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/faction.py` & `spacetraders-0.6.0/spacetraders/models/faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/faction_trait.py` & `spacetraders-0.6.0/spacetraders/models/faction_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/faction_trait_symbol.py` & `spacetraders-0.6.0/spacetraders/models/faction_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/fulfill_contract_response_200.py` & `spacetraders-0.6.0/spacetraders/models/fulfill_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/fulfill_contract_response_200_data.py` & `spacetraders-0.6.0/spacetraders/models/fulfill_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_contract_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_contracts_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_contracts_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_faction_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_faction_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_factions_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_factions_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_jump_gate_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_jump_gate_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_market_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_market_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_my_agent_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_my_agent_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_my_ship_cargo_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_my_ship_cargo_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_my_ship_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_my_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_my_ships_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_my_ships_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_ship_cooldown_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_ship_cooldown_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_ship_nav_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_shipyard_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_shipyard_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_status_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_status_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_status_response_200_announcements_item.py` & `spacetraders-0.6.0/spacetraders/models/get_status_response_200_announcements_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards.py` & `spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py` & `spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards_most_credits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py` & `spacetraders-0.6.0/spacetraders/models/get_status_response_200_leaderboards_most_submitted_charts_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_status_response_200_links_item.py` & `spacetraders-0.6.0/spacetraders/models/get_status_response_200_links_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_status_response_200_server_resets.py` & `spacetraders-0.6.0/spacetraders/models/get_status_response_200_server_resets.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_status_response_200_stats.py` & `spacetraders-0.6.0/spacetraders/models/get_status_response_200_stats.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_system_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_system_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_system_waypoints_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_system_waypoints_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_systems_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_systems_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/get_waypoint_response_200.py` & `spacetraders-0.6.0/spacetraders/models/get_waypoint_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/jettison_json_body.py` & `spacetraders-0.6.0/spacetraders/models/jettison_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/jettison_response_200.py` & `spacetraders-0.6.0/spacetraders/models/jettison_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/jettison_response_200_data.py` & `spacetraders-0.6.0/spacetraders/models/jettison_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/jump_gate.py` & `spacetraders-0.6.0/spacetraders/models/jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/jump_ship_json_body.py` & `spacetraders-0.6.0/spacetraders/models/jump_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/jump_ship_response_200.py` & `spacetraders-0.6.0/spacetraders/models/jump_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/jump_ship_response_200_data.py` & `spacetraders-0.6.0/spacetraders/models/jump_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/market.py` & `spacetraders-0.6.0/spacetraders/models/market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/market_trade_good.py` & `spacetraders-0.6.0/spacetraders/models/market_trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/market_transaction.py` & `spacetraders-0.6.0/spacetraders/models/market_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/meta.py` & `spacetraders-0.6.0/spacetraders/models/meta.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/navigate_ship_json_body.py` & `spacetraders-0.6.0/spacetraders/models/navigate_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/navigate_ship_response_200.py` & `spacetraders-0.6.0/spacetraders/models/navigate_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/navigate_ship_response_200_data.py` & `spacetraders-0.6.0/spacetraders/models/navigate_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py` & `spacetraders-0.6.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py` & `spacetraders-0.6.0/spacetraders/models/negotiate_contract_negotiate_contract_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py` & `spacetraders-0.6.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py` & `spacetraders-0.6.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/patch_ship_nav_json_body.py` & `spacetraders-0.6.0/spacetraders/models/patch_ship_nav_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/patch_ship_nav_response_200.py` & `spacetraders-0.6.0/spacetraders/models/patch_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py` & `spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py` & `spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py` & `spacetraders-0.6.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/purchase_ship_json_body.py` & `spacetraders-0.6.0/spacetraders/models/purchase_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/purchase_ship_response_201.py` & `spacetraders-0.6.0/spacetraders/models/purchase_ship_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/purchase_ship_response_201_data.py` & `spacetraders-0.6.0/spacetraders/models/purchase_ship_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/refuel_ship_response_200.py` & `spacetraders-0.6.0/spacetraders/models/refuel_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/refuel_ship_response_200_data.py` & `spacetraders-0.6.0/spacetraders/models/refuel_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/register_json_body.py` & `spacetraders-0.6.0/spacetraders/models/register_json_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,29 +4,28 @@
     List,
     TypeVar,
     Union,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.register_json_body_faction import RegisterJsonBodyFaction
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="RegisterJsonBody")
 
 
 class RegisterJsonBody(BaseModel):
     """
     Attributes:
-        faction (RegisterJsonBodyFaction): The faction you choose determines your headquarters.
+        faction (Any): The faction you choose determines your headquarters. Example: COSMIC.
         symbol (str): How other agents will see your ships and information. Example: BADGER.
         email (Union[Unset, str]): Your email address. This is used if you reserved your call sign between resets.
     """
 
-    faction: RegisterJsonBodyFaction = Field(alias="faction")
+    faction: Any = Field(alias="faction")
     symbol: str = Field(alias="symbol")
     email: Union[Unset, str] = Field(UNSET, alias="email")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.5.0/spacetraders/models/register_response_201.py` & `spacetraders-0.6.0/spacetraders/models/register_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/register_response_201_data.py` & `spacetraders-0.6.0/spacetraders/models/register_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/scanned_ship.py` & `spacetraders-0.6.0/spacetraders/models/scanned_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/scanned_ship_engine.py` & `spacetraders-0.6.0/spacetraders/models/scanned_ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/scanned_ship_frame.py` & `spacetraders-0.6.0/spacetraders/models/scanned_ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/scanned_ship_mounts_item.py` & `spacetraders-0.6.0/spacetraders/models/scanned_ship_mounts_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/scanned_ship_reactor.py` & `spacetraders-0.6.0/spacetraders/models/scanned_ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/scanned_system.py` & `spacetraders-0.6.0/spacetraders/models/scanned_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/scanned_waypoint.py` & `spacetraders-0.6.0/spacetraders/models/scanned_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py` & `spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py` & `spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/sell_cargo_sell_cargo_request.py` & `spacetraders-0.6.0/spacetraders/models/sell_cargo_sell_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship.py` & `spacetraders-0.6.0/spacetraders/models/ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_cargo.py` & `spacetraders-0.6.0/spacetraders/models/ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_cargo_item.py` & `spacetraders-0.6.0/spacetraders/models/ship_cargo_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_crew.py` & `spacetraders-0.6.0/spacetraders/models/ship_crew.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_engine.py` & `spacetraders-0.6.0/spacetraders/models/ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_frame.py` & `spacetraders-0.6.0/spacetraders/models/ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_frame_symbol.py` & `spacetraders-0.6.0/spacetraders/models/ship_frame_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_fuel.py` & `spacetraders-0.6.0/spacetraders/models/ship_fuel.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_fuel_consumed.py` & `spacetraders-0.6.0/spacetraders/models/ship_fuel_consumed.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_module.py` & `spacetraders-0.6.0/spacetraders/models/ship_module.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_module_symbol.py` & `spacetraders-0.6.0/spacetraders/models/ship_module_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_mount.py` & `spacetraders-0.6.0/spacetraders/models/ship_mount.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_mount_deposits_item.py` & `spacetraders-0.6.0/spacetraders/models/ship_mount_deposits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_mount_symbol.py` & `spacetraders-0.6.0/spacetraders/models/ship_mount_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_nav.py` & `spacetraders-0.6.0/spacetraders/models/ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_nav_route.py` & `spacetraders-0.6.0/spacetraders/models/ship_nav_route.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_nav_route_waypoint.py` & `spacetraders-0.6.0/spacetraders/models/ship_nav_route_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_reactor.py` & `spacetraders-0.6.0/spacetraders/models/ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_refine_json_body.py` & `spacetraders-0.6.0/spacetraders/models/ship_refine_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response.py` & `spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py` & `spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py` & `spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py` & `spacetraders-0.6.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_registration.py` & `spacetraders-0.6.0/spacetraders/models/ship_registration.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_requirements.py` & `spacetraders-0.6.0/spacetraders/models/ship_requirements.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/ship_type.py` & `spacetraders-0.6.0/spacetraders/models/ship_type.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/shipyard.py` & `spacetraders-0.6.0/spacetraders/models/shipyard.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/shipyard_ship.py` & `spacetraders-0.6.0/spacetraders/models/shipyard_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/shipyard_ship_types_item.py` & `spacetraders-0.6.0/spacetraders/models/shipyard_ship_types_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/shipyard_transaction.py` & `spacetraders-0.6.0/spacetraders/models/shipyard_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/survey.py` & `spacetraders-0.6.0/spacetraders/models/survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/survey_deposit.py` & `spacetraders-0.6.0/spacetraders/models/survey_deposit.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/system.py` & `spacetraders-0.6.0/spacetraders/models/system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/system_faction.py` & `spacetraders-0.6.0/spacetraders/models/system_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/system_waypoint.py` & `spacetraders-0.6.0/spacetraders/models/system_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/trade_good.py` & `spacetraders-0.6.0/spacetraders/models/trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/trade_symbol.py` & `spacetraders-0.6.0/spacetraders/models/trade_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py` & `spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py` & `spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py` & `spacetraders-0.6.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/warp_ship_json_body.py` & `spacetraders-0.6.0/spacetraders/models/warp_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/warp_ship_response_200.py` & `spacetraders-0.6.0/spacetraders/models/warp_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/warp_ship_response_200_data.py` & `spacetraders-0.6.0/spacetraders/models/warp_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/waypoint.py` & `spacetraders-0.6.0/spacetraders/models/waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/waypoint_faction.py` & `spacetraders-0.6.0/spacetraders/models/waypoint_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/waypoint_orbital.py` & `spacetraders-0.6.0/spacetraders/models/waypoint_orbital.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/waypoint_trait.py` & `spacetraders-0.6.0/spacetraders/models/waypoint_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/models/waypoint_trait_symbol.py` & `spacetraders-0.6.0/spacetraders/models/waypoint_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/spacetraders/types.py` & `spacetraders-0.6.0/spacetraders/types.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.5.0/PKG-INFO` & `spacetraders-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetraders
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python API for Space Traders
 License: Apache-2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

