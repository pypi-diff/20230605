# Comparing `tmp/pht-station-0.1.tar.gz` & `tmp/pht_station-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pht-station-0.1.tar", last modified: Mon May  2 10:13:47 2022, max compression
+gzip compressed data, was "pht_station-0.2.0.tar", max compression
```

## Comparing `pht-station-0.1.tar` & `pht_station-0.2.0.tar`

### file list

```diff
@@ -1,165 +1,180 @@
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.233716 pht-station-0.1/
--rw-rw-rw-   0        0        0     5547 2022-05-02 10:13:47.233716 pht-station-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4708 2022-05-02 10:13:25.000000 pht-station-0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.111545 pht-station-0.1/pht_station.egg-info/
--rw-rw-rw-   0        0        0     5547 2022-05-02 10:13:46.000000 pht-station-0.1/pht_station.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4373 2022-05-02 10:13:47.000000 pht-station-0.1/pht_station.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-02 10:13:46.000000 pht-station-0.1/pht_station.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2022-05-02 10:13:46.000000 pht-station-0.1/pht_station.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      182 2022-05-02 10:13:46.000000 pht-station-0.1/pht_station.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-05-02 10:13:47.000000 pht-station-0.1/pht_station.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      467 2022-05-02 10:13:47.234715 pht-station-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1659 2022-05-02 10:13:36.000000 pht-station-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.112545 pht-station-0.1/station/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.118564 pht-station-0.1/station/app/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.121929 pht-station-0.1/station/app/api/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/api/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.123529 pht-station-0.1/station/app/api/api_v1/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/api/api_v1/__init__.py
--rw-rw-rw-   0        0        0      981 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/api/api_v1/api.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.131557 pht-station-0.1/station/app/api/api_v1/endpoints/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/api/api_v1/endpoints/__init__.py
--rw-rw-rw-   0        0        0     3685 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/api/api_v1/endpoints/airflow.py
--rw-rw-rw-   0        0        0     2371 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/api/api_v1/endpoints/datasets.py
--rw-rw-rw-   0        0        0     6704 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/api/api_v1/endpoints/docker_trains.py
--rw-rw-rw-   0        0        0     2076 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/api/api_v1/endpoints/fhir.py
--rw-rw-rw-   0        0        0     9165 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/api/api_v1/endpoints/local_trains.py
--rw-rw-rw-   0        0        0     1796 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/api/api_v1/endpoints/notifications.py
--rw-rw-rw-   0        0        0      669 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/api/api_v1/endpoints/station.py
--rw-rw-rw-   0        0        0     3058 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/api/api_v1/endpoints/station_status.py
--rw-rw-rw-   0        0        0      704 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/api/dependencies.py
--rw-rw-rw-   0        0        0     4382 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/auth.py
--rw-rw-rw-   0        0        0     1855 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/cache.py
--rw-rw-rw-   0        0        0    31246 2022-05-02 09:28:09.000000 pht-station-0.1/station/app/config.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.140432 pht-station-0.1/station/app/crud/
--rw-rw-rw-   0        0        0      261 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/crud/__init__.py
--rw-rw-rw-   0        0        0     2244 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/crud/base.py
--rw-rw-rw-   0        0        0     1752 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/crud/crud_datasets.py
--rw-rw-rw-   0        0        0     4654 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/crud/crud_docker_trains.py
--rw-rw-rw-   0        0        0     1720 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/crud/crud_fhir_servers.py
--rw-rw-rw-   0        0        0    10001 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/crud/crud_local_train.py
--rw-rw-rw-   0        0        0      616 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/crud/crud_notifications.py
--rw-rw-rw-   0        0        0     1927 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/crud/crud_train_configs.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.144169 pht-station-0.1/station/app/db/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/db/__init__.py
--rw-rw-rw-   0        0        0      615 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/db/base.py
--rw-rw-rw-   0        0        0      303 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/db/base_class.py
--rw-rw-rw-   0        0        0      602 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/db/session.py
--rw-rw-rw-   0        0        0     1407 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/db/setup_db.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.146784 pht-station-0.1/station/app/docker_trains/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/docker_trains/__init__.py
--rw-rw-rw-   0        0        0      813 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/docker_trains/update.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.147791 pht-station-0.1/station/app/fhir/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/fhir/__init__.py
--rw-rw-rw-   0        0        0     1529 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/fhir/server.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.149790 pht-station-0.1/station/app/local_train_minio/
--rw-rw-rw-   0        0        0     3149 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/local_train_minio/LocalTrainMinIO.py
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/local_train_minio/__init__.py
--rw-rw-rw-   0        0        0     3458 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/logger.py
--rw-rw-rw-   0        0        0      847 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/main.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.155856 pht-station-0.1/station/app/models/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/models/__init__.py
--rw-rw-rw-   0        0        0      980 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/models/datasets.py
--rw-rw-rw-   0        0        0     2532 2022-04-14 13:39:59.000000 pht-station-0.1/station/app/models/docker_trains.py
--rw-rw-rw-   0        0        0      809 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/models/fhir_server.py
--rw-rw-rw-   0        0        0     2124 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/models/local_trains.py
--rw-rw-rw-   0        0        0      498 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/models/notification.py
--rw-rw-rw-   0        0        0     1066 2022-05-02 09:28:09.000000 pht-station-0.1/station/app/run_station.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.168861 pht-station-0.1/station/app/schemas/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/__init__.py
--rw-rw-rw-   0        0        0     1174 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/airflow.py
--rw-rw-rw-   0        0        0      855 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/datasets.py
--rw-rw-rw-   0        0        0     1062 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/schemas/dl_models.py
--rw-rw-rw-   0        0        0     2716 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/docker_trains.py
--rw-rw-rw-   0        0        0     1977 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/fhir.py
--rw-rw-rw-   0        0        0      936 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/local_trains.py
--rw-rw-rw-   0        0        0      555 2022-04-14 13:39:33.000000 pht-station-0.1/station/app/schemas/notifications.py
--rw-rw-rw-   0        0        0      447 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/protocol.py
--rw-rw-rw-   0        0        0      465 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/station.py
--rw-rw-rw-   0        0        0      828 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/station_status.py
--rw-rw-rw-   0        0        0     1011 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/trains.py
--rw-rw-rw-   0        0        0     1103 2022-03-29 13:08:18.000000 pht-station-0.1/station/app/schemas/users.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.170945 pht-station-0.1/station/clients/
--rw-rw-rw-   0        0        0       56 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.173944 pht-station-0.1/station/clients/airflow/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/airflow/__init__.py
--rw-rw-rw-   0        0        0     4956 2022-05-02 09:28:09.000000 pht-station-0.1/station/clients/airflow/client.py
--rw-rw-rw-   0        0        0     4903 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/airflow/docker_trains.py
--rw-rw-rw-   0        0        0      613 2022-04-14 13:39:33.000000 pht-station-0.1/station/clients/airflow/utils.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.175944 pht-station-0.1/station/clients/central/
--rw-rw-rw-   0        0        0        0 2022-04-14 13:39:59.000000 pht-station-0.1/station/clients/central/__init__.py
--rw-rw-rw-   0        0        0     1984 2022-04-14 13:39:59.000000 pht-station-0.1/station/clients/central/central_client.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.177945 pht-station-0.1/station/clients/conductor/
--rw-rw-rw-   0        0        0       46 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/conductor/__init__.py
--rw-rw-rw-   0        0        0     1460 2022-05-02 09:28:09.000000 pht-station-0.1/station/clients/conductor/rest_client.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.179944 pht-station-0.1/station/clients/docker/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/docker/__init__.py
--rw-rw-rw-   0        0        0     3631 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/docker/client.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.180944 pht-station-0.1/station/clients/fhir/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/fhir/__init__.py
--rw-rw-rw-   0        0        0     5274 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/fhir/client.py
--rw-rw-rw-   0        0        0     3006 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/harbor_client.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.182944 pht-station-0.1/station/clients/minio/
--rw-rw-rw-   0        0        0       33 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/minio/__init__.py
--rw-rw-rw-   0        0        0     7261 2022-03-29 13:08:18.000000 pht-station-0.1/station/clients/minio/client.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.186945 pht-station-0.1/station/ctl/
--rw-rw-rw-   0        0        0        0 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/__init__.py
--rw-rw-rw-   0        0        0     1274 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/cli.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.194947 pht-station-0.1/station/ctl/config/
--rw-rw-rw-   0        0        0      110 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/config/__init__.py
--rw-rw-rw-   0        0        0     2729 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/config/command.py
--rw-rw-rw-   0        0        0      238 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/config/config.py
--rw-rw-rw-   0        0        0     6146 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/config/fix.py
--rw-rw-rw-   0        0        0     1065 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/config/fs.py
--rw-rw-rw-   0        0        0     1603 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/config/generators.py
--rw-rw-rw-   0        0        0     2692 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/config/validate.py
--rw-rw-rw-   0        0        0    25896 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/config/validators.py
--rw-rw-rw-   0        0        0     1465 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/constants.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.200517 pht-station-0.1/station/ctl/install/
--rw-rw-rw-   0        0        0        0 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/install/__init__.py
--rw-rw-rw-   0        0        0     2053 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/install/certs.py
--rw-rw-rw-   0        0        0     5367 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/install/command.py
--rw-rw-rw-   0        0        0     2614 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/install/docker.py
--rw-rw-rw-   0        0        0     1623 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/install/fs.py
--rw-rw-rw-   0        0        0     5269 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/install/templates.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.205523 pht-station-0.1/station/ctl/tests/
--rw-rw-rw-   0        0        0        0 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/tests/__init__.py
--rw-rw-rw-   0        0        0     1370 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/tests/test_config.py
--rw-rw-rw-   0        0        0     2616 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/tests/test_install.py
--rw-rw-rw-   0        0        0     2443 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/tests/test_validators.py
--rw-rw-rw-   0        0        0      150 2022-05-02 09:28:09.000000 pht-station-0.1/station/ctl/util.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.217619 pht-station-0.1/station/tests/
--rw-rw-rw-   0        0        0        0 2022-03-29 13:08:18.000000 pht-station-0.1/station/tests/__init__.py
--rw-rw-rw-   0        0        0     4278 2022-03-29 13:08:18.000000 pht-station-0.1/station/tests/test_api_airflow.py
--rw-rw-rw-   0        0        0      984 2022-03-29 13:08:18.000000 pht-station-0.1/station/tests/test_api_datasets.py
--rw-rw-rw-   0        0        0    13496 2022-03-29 13:08:18.000000 pht-station-0.1/station/tests/test_api_docker_trains.py
--rw-rw-rw-   0        0        0     3114 2022-03-29 13:08:18.000000 pht-station-0.1/station/tests/test_api_fhir_servers.py
--rw-rw-rw-   0        0        0     7182 2022-03-29 13:08:18.000000 pht-station-0.1/station/tests/test_api_local_trains.py
--rw-rw-rw-   0        0        0     2751 2022-04-14 13:39:33.000000 pht-station-0.1/station/tests/test_api_notifications.py
--rw-rw-rw-   0        0        0     1401 2022-03-29 13:08:18.000000 pht-station-0.1/station/tests/test_auth.py
--rw-rw-rw-   0        0        0      992 2022-04-28 07:02:17.000000 pht-station-0.1/station/tests/test_central_client.py
--rw-rw-rw-   0        0        0      604 2022-04-14 13:39:33.000000 pht-station-0.1/station/tests/test_db.py
--rw-rw-rw-   0        0        0     7975 2022-05-02 09:28:09.000000 pht-station-0.1/station/tests/test_settings.py
--rw-rw-rw-   0        0        0      494 2022-03-29 13:08:18.000000 pht-station-0.1/station/tests/test_status.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.219616 pht-station-0.1/station/worker/
--rw-rw-rw-   0        0        0        0 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.221614 pht-station-0.1/station/worker/discovery/
--rw-rw-rw-   0        0        0       47 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/discovery/__init__.py
--rw-rw-rw-   0        0        0      831 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/discovery/data_discovery.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.225615 pht-station-0.1/station/worker/loader/
--rw-rw-rw-   0        0        0      112 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/loader/__init__.py
--rw-rw-rw-   0        0        0     2090 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/loader/base_loader.py
--rw-rw-rw-   0        0        0     4467 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/loader/dataset.py
--rw-rw-rw-   0        0        0     3832 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/loader/model_loader.py
--rw-rw-rw-   0        0        0     2416 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/pht_worker.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.228615 pht-station-0.1/station/worker/testing/
--rw-rw-rw-   0        0        0        0 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/testing/__init__.py
--rw-rw-rw-   0        0        0      405 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/testing/db.py
--rw-rw-rw-   0        0        0     2320 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/testing/populate_minio.py
--rw-rw-rw-   0        0        0     1334 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/testing/train_lightning_model.py
-drwxrwxrwx   0        0        0        0 2022-05-02 10:13:47.232713 pht-station-0.1/station/worker/trainer/
--rw-rw-rw-   0        0        0       89 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/trainer/__init__.py
--rw-rw-rw-   0        0        0     2844 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/trainer/base_trainer.py
--rw-rw-rw-   0        0        0     6686 2022-05-02 09:28:09.000000 pht-station-0.1/station/worker/trainer/federated_trainer.py
+-rw-r--r--   0        0        0     1927 2023-06-05 07:01:36.971701 pht_station-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2652 2023-02-06 09:52:28.229709 pht_station-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/.dockerignore
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.847591 pht_station-0.2.0/station/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.568252 pht_station-0.2.0/station/app/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.305183 pht_station-0.2.0/station/app/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.288975 pht_station-0.2.0/station/app/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     1150 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/api/api_v1/api.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.263471 pht_station-0.2.0/station/app/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     3612 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/api/api_v1/endpoints/airflow.py
+-rw-r--r--   0        0        0     7514 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/api/api_v1/endpoints/datasets.py
+-rw-r--r--   0        0        0     6235 2023-02-06 09:52:28.247709 pht_station-0.2.0/station/app/api/api_v1/endpoints/docker_trains.py
+-rw-r--r--   0        0        0     2075 2023-02-06 09:52:28.248714 pht_station-0.2.0/station/app/api/api_v1/endpoints/fhir.py
+-rw-r--r--   0        0        0     5162 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/api/api_v1/endpoints/local_trains.py
+-rw-r--r--   0        0        0     2470 2023-02-06 09:52:28.250721 pht_station-0.2.0/station/app/api/api_v1/endpoints/master_images.py
+-rw-r--r--   0        0        0     1808 2023-02-06 09:52:28.251708 pht_station-0.2.0/station/app/api/api_v1/endpoints/notifications.py
+-rw-r--r--   0        0        0      587 2023-02-06 09:52:28.252711 pht_station-0.2.0/station/app/api/api_v1/endpoints/station.py
+-rw-r--r--   0        0        0     2342 2023-02-06 09:52:28.253712 pht_station-0.2.0/station/app/api/api_v1/endpoints/station_status.py
+-rw-r--r--   0        0        0      679 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/api/dependencies.py
+-rw-r--r--   0        0        0     5122 2023-02-06 09:52:28.257709 pht_station-0.2.0/station/app/auth.py
+-rw-r--r--   0        0        0     1747 2023-02-06 09:52:28.258710 pht_station-0.2.0/station/app/cache.py
+-rw-r--r--   0        0        0     3739 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/clients.py
+-rw-r--r--   0        0        0      277 2023-02-06 09:52:28.260830 pht_station-0.2.0/station/app/config.py
+-rw-r--r--   0        0        0      298 2023-02-06 09:52:28.261841 pht_station-0.2.0/station/app/crud/__init__.py
+-rw-r--r--   0        0        0     2533 2023-02-06 09:52:28.262840 pht_station-0.2.0/station/app/crud/base.py
+-rw-r--r--   0        0        0     2479 2023-02-06 09:52:28.265857 pht_station-0.2.0/station/app/crud/crud_datasets.py
+-rw-r--r--   0        0        0      675 2023-02-06 09:52:28.266866 pht_station-0.2.0/station/app/crud/crud_discovery.py
+-rw-r--r--   0        0        0     8668 2023-02-06 09:52:28.267868 pht_station-0.2.0/station/app/crud/crud_docker_trains.py
+-rw-r--r--   0        0        0     1773 2023-02-06 09:52:28.268868 pht_station-0.2.0/station/app/crud/crud_fhir_servers.py
+-rw-r--r--   0        0        0     3648 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/crud/crud_local_train.py
+-rw-r--r--   0        0        0      546 2023-02-06 09:52:28.271866 pht_station-0.2.0/station/app/crud/crud_notifications.py
+-rw-r--r--   0        0        0     1997 2023-02-06 09:52:28.272866 pht_station-0.2.0/station/app/crud/crud_train_configs.py
+-rw-r--r--   0        0        0     1503 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/crud/local_train_master_image.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.545965 pht_station-0.2.0/station/app/datasets/__init__.py
+-rw-r--r--   0        0        0     1799 2023-02-06 09:52:28.274865 pht_station-0.2.0/station/app/datasets/filesystem.py
+-rw-r--r--   0        0        0     7734 2023-02-06 09:52:28.275865 pht_station-0.2.0/station/app/datasets/statistics.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.224536 pht_station-0.2.0/station/app/db/__init__.py
+-rw-r--r--   0        0        0      750 2023-02-06 14:20:00.310226 pht_station-0.2.0/station/app/db/base.py
+-rw-r--r--   0        0        0      289 2022-08-01 10:19:24.230970 pht_station-0.2.0/station/app/db/base_class.py
+-rw-r--r--   0        0        0      459 2023-02-06 09:52:28.277962 pht_station-0.2.0/station/app/db/session.py
+-rw-r--r--   0        0        0     1345 2023-02-06 09:52:28.278872 pht_station-0.2.0/station/app/db/setup_db.py
+-rw-r--r--   0        0        0     1459 2022-08-01 10:19:24.403753 pht_station-0.2.0/station/app/env.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.345748 pht_station-0.2.0/station/app/fhir/__init__.py
+-rw-r--r--   0        0        0     2595 2023-02-06 09:52:28.280868 pht_station-0.2.0/station/app/fhir/server.py
+-rw-r--r--   0        0        0     2895 2023-05-24 10:01:24.509203 pht_station-0.2.0/station/app/logger.py
+-rw-r--r--   0        0        0      933 2023-05-09 10:32:59.163014 pht_station-0.2.0/station/app/main.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.406771 pht_station-0.2.0/station/app/models/__init__.py
+-rw-r--r--   0        0        0      784 2023-02-06 09:52:28.292149 pht_station-0.2.0/station/app/models/datasets.py
+-rw-r--r--   0        0        0      345 2023-02-06 09:52:28.294158 pht_station-0.2.0/station/app/models/discovery.py
+-rw-r--r--   0        0        0     2808 2023-02-06 14:16:52.531459 pht_station-0.2.0/station/app/models/docker_trains.py
+-rw-r--r--   0        0        0      963 2023-02-06 09:52:28.296161 pht_station-0.2.0/station/app/models/fhir_server.py
+-rw-r--r--   0        0        0     3225 2023-02-06 09:52:28.298158 pht_station-0.2.0/station/app/models/local_trains.py
+-rw-r--r--   0        0        0      569 2023-02-06 09:52:28.298158 pht_station-0.2.0/station/app/models/notification.py
+-rw-r--r--   0        0        0     1502 2023-05-24 10:01:24.524827 pht_station-0.2.0/station/app/run_station.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.493050 pht_station-0.2.0/station/app/schemas/__init__.py
+-rw-r--r--   0        0        0     1114 2023-02-06 09:52:28.300235 pht_station-0.2.0/station/app/schemas/airflow.py
+-rw-r--r--   0        0        0     2651 2023-02-06 09:52:28.302162 pht_station-0.2.0/station/app/schemas/datasets.py
+-rw-r--r--   0        0        0     1038 2023-02-06 09:52:28.302162 pht_station-0.2.0/station/app/schemas/discovery.py
+-rw-r--r--   0        0        0     1004 2023-02-06 09:52:28.304512 pht_station-0.2.0/station/app/schemas/dl_models.py
+-rw-r--r--   0        0        0     2888 2023-02-06 09:52:28.305506 pht_station-0.2.0/station/app/schemas/docker_trains.py
+-rw-r--r--   0        0        0     2194 2023-02-06 09:52:28.306505 pht_station-0.2.0/station/app/schemas/fhir.py
+-rw-r--r--   0        0        0     3149 2023-02-06 09:52:28.308508 pht_station-0.2.0/station/app/schemas/local_trains.py
+-rw-r--r--   0        0        0      708 2023-02-06 09:52:28.309506 pht_station-0.2.0/station/app/schemas/notifications.py
+-rw-r--r--   0        0        0      425 2023-02-06 09:52:28.310505 pht_station-0.2.0/station/app/schemas/protocol.py
+-rw-r--r--   0        0        0      448 2023-02-06 09:52:28.311507 pht_station-0.2.0/station/app/schemas/station.py
+-rw-r--r--   0        0        0      781 2023-02-06 09:52:28.312514 pht_station-0.2.0/station/app/schemas/station_status.py
+-rw-r--r--   0        0        0      966 2023-02-06 09:52:28.312514 pht_station-0.2.0/station/app/schemas/trains.py
+-rw-r--r--   0        0        0     1094 2023-02-06 09:52:28.313524 pht_station-0.2.0/station/app/schemas/users.py
+-rw-r--r--   0        0        0    43179 2023-05-24 10:01:24.525938 pht_station-0.2.0/station/app/settings.py
+-rw-r--r--   0        0        0    12288 2023-05-24 10:01:24.525938 pht_station-0.2.0/station/app/test.db
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.354010 pht_station-0.2.0/station/app/tests/__init__.py
+-rw-r--r--   0        0        0     4184 2023-02-06 09:52:28.321353 pht_station-0.2.0/station/app/tests/test_api_airflow.py
+-rw-r--r--   0        0        0      933 2023-02-06 09:52:28.322369 pht_station-0.2.0/station/app/tests/test_api_datasets.py
+-rw-r--r--   0        0        0    13153 2023-02-06 09:52:28.323363 pht_station-0.2.0/station/app/tests/test_api_docker_trains.py
+-rw-r--r--   0        0        0     3132 2023-02-06 09:52:28.324368 pht_station-0.2.0/station/app/tests/test_api_fhir_servers.py
+-rw-r--r--   0        0        0     1585 2023-02-06 09:52:28.325364 pht_station-0.2.0/station/app/tests/test_api_local_trains.py
+-rw-r--r--   0        0        0     2539 2023-02-06 09:52:28.325364 pht_station-0.2.0/station/app/tests/test_api_notifications.py
+-rw-r--r--   0        0        0     1177 2023-02-06 09:52:28.326365 pht_station-0.2.0/station/app/tests/test_auth.py
+-rw-r--r--   0        0        0     1188 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/app/tests/test_central_client.py
+-rw-r--r--   0        0        0      826 2023-02-06 09:52:28.328370 pht_station-0.2.0/station/app/tests/test_db.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.351668 pht_station-0.2.0/station/app/tests/test_files/entrypoint.py
+-rw-r--r--   0        0        0     1340 2023-02-06 09:52:28.329431 pht_station-0.2.0/station/app/tests/test_local_trains.py
+-rw-r--r--   0        0        0     7944 2023-02-06 09:52:28.330453 pht_station-0.2.0/station/app/tests/test_settings.py
+-rw-r--r--   0        0        0      420 2023-02-06 09:52:28.331363 pht_station-0.2.0/station/app/tests/test_status.py
+-rw-r--r--   0        0        0        0 2022-08-11 07:11:09.946932 pht_station-0.2.0/station/app/trains/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-11 07:11:09.947785 pht_station-0.2.0/station/app/trains/docker/__init__.py
+-rw-r--r--   0        0        0     6584 2023-02-06 09:52:28.333493 pht_station-0.2.0/station/app/trains/docker/airflow.py
+-rw-r--r--   0        0        0      822 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/app/trains/docker/update.py
+-rw-r--r--   0        0        0        0 2022-08-11 07:11:09.949200 pht_station-0.2.0/station/app/trains/local/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/airflow/__init__.py
+-rw-r--r--   0        0        0     5057 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/airflow/client.py
+-rw-r--r--   0        0        0     6616 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/airflow/docker_trains.py
+-rw-r--r--   0        0        0     2394 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/base.py
+-rw-r--r--   0        0        0       45 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/central/__init__.py
+-rw-r--r--   0        0        0     3293 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/central/central_client.py
+-rw-r--r--   0        0        0      137 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/central/schemas.py
+-rw-r--r--   0        0        0       45 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/conductor/__init__.py
+-rw-r--r--   0        0        0     1436 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/conductor/rest_client.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/docker/__init__.py
+-rw-r--r--   0        0        0     3740 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/docker/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/fhir/__init__.py
+-rw-r--r--   0        0        0     5243 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/fhir/client.py
+-rw-r--r--   0        0        0     3507 2023-05-24 10:01:24.527771 pht_station-0.2.0/station/common/clients/harbor_client.py
+-rw-r--r--   0        0        0       32 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/minio/__init__.py
+-rw-r--r--   0        0        0    11455 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/minio/client.py
+-rw-r--r--   0        0        0     2712 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/resource_client.py
+-rw-r--r--   0        0        0       37 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/station/__init__.py
+-rw-r--r--   0        0        0     1355 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/station/client.py
+-rw-r--r--   0        0        0     1584 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/station/local_trains.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/tests/__init__.py
+-rw-r--r--   0        0        0      853 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/tests/test_central_client.py
+-rw-r--r--   0        0        0     1631 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/clients/tests/test_station_client.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/__init__.py
+-rw-r--r--   0        0        0     2519 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/fix.py
+-rw-r--r--   0        0        0     2406 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/generators.py
+-rw-r--r--   0        0        0    13204 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/station_config.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/tests/__init__.py
+-rw-r--r--   0        0        0     1265 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/tests/cert.pem
+-rw-r--r--   0        0        0     1679 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/tests/key.pem
+-rw-r--r--   0        0        0     3505 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/tests/test_station_config.py
+-rw-r--r--   0        0        0     2518 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/tests/test_station_config.yml
+-rw-r--r--   0        0        0     3668 2023-05-24 10:01:24.540779 pht_station-0.2.0/station/common/config/validators.py
+-rw-r--r--   0        0        0     1721 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/common/constants.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.710500 pht_station-0.2.0/station/ctl/__init__.py
+-rw-r--r--   0        0        0     1562 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/cli.py
+-rw-r--r--   0        0        0      107 2023-02-06 09:52:28.355911 pht_station-0.2.0/station/ctl/config/__init__.py
+-rw-r--r--   0        0        0     2542 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/config/command.py
+-rw-r--r--   0        0        0    10104 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/config/fix.py
+-rw-r--r--   0        0        0     1075 2023-02-06 09:52:28.363917 pht_station-0.2.0/station/ctl/config/fs.py
+-rw-r--r--   0        0        0     1816 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/config/validate.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.615591 pht_station-0.2.0/station/ctl/fhir/__init__.py
+-rw-r--r--   0        0        0      774 2023-02-06 09:52:28.368916 pht_station-0.2.0/station/ctl/fhir/command.py
+-rw-r--r--   0        0        0     1572 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/fhir/manage.py
+-rw-r--r--   0        0        0     2411 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/fhir/setup.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.677002 pht_station-0.2.0/station/ctl/install/__init__.py
+-rw-r--r--   0        0        0     2853 2023-02-06 09:52:28.371914 pht_station-0.2.0/station/ctl/install/certs.py
+-rw-r--r--   0        0        0    12998 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/install/command.py
+-rw-r--r--   0        0        0     3013 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/install/docker.py
+-rw-r--r--   0        0        0     1837 2023-05-24 10:01:24.556432 pht_station-0.2.0/station/ctl/install/fs.py
+-rw-r--r--   0        0        0    13076 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/install/templates.py
+-rw-r--r--   0        0        0    38914 2022-11-16 14:46:10.023598 pht_station-0.2.0/station/ctl/templates/airflow.cfg.tmpl
+-rw-r--r--   0        0        0      296 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/templates/authup/authup.api.conf.tmpl
+-rw-r--r--   0        0        0     3693 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/templates/docker-compose.yml.tmpl
+-rw-r--r--   0        0        0      257 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/templates/init.sql.tmpl
+-rw-r--r--   0        0        0     3288 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/templates/station_config.yml.tmpl
+-rw-r--r--   0        0        0      382 2022-08-01 10:19:24.690599 pht_station-0.2.0/station/ctl/templates/traefik/config.yml.tmpl
+-rw-r--r--   0        0        0      628 2022-11-16 13:15:51.913906 pht_station-0.2.0/station/ctl/templates/traefik/traefik.yml.tmpl
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.618548 pht_station-0.2.0/station/ctl/tests/__init__.py
+-rw-r--r--   0        0        0     3010 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/tests/test_config.py
+-rw-r--r--   0        0        0     2707 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/ctl/tests/test_install.py
+-rw-r--r--   0        0        0     2465 2023-02-06 09:52:28.382289 pht_station-0.2.0/station/ctl/tests/test_validators.py
+-rw-r--r--   0        0        0      338 2023-02-06 09:52:28.383299 pht_station-0.2.0/station/ctl/util.py
+-rw-r--r--   0        0        0        0 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/scripts/__init__.py
+-rw-r--r--   0        0        0      440 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/scripts/run_dev.py
+-rw-r--r--   0        0        0        0 2023-01-31 12:11:18.164891 pht_station-0.2.0/station/trains/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-31 12:11:18.169904 pht_station-0.2.0/station/trains/local/__init__.py
+-rw-r--r--   0        0        0     2803 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/trains/local/airflow.py
+-rw-r--r--   0        0        0     2357 2023-02-06 09:52:28.385301 pht_station-0.2.0/station/trains/local/build.py
+-rw-r--r--   0        0        0     1637 2023-02-06 09:52:28.386299 pht_station-0.2.0/station/trains/local/docker.py
+-rw-r--r--   0        0        0      922 2023-02-06 09:52:28.387302 pht_station-0.2.0/station/trains/local/update.py
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.764517 pht_station-0.2.0/station/worker/__init__.py
+-rw-r--r--   0        0        0       46 2022-08-01 10:19:24.757813 pht_station-0.2.0/station/worker/discovery/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/discovery/data_discovery.py
+-rw-r--r--   0        0        0      109 2022-08-01 10:19:24.719800 pht_station-0.2.0/station/worker/loader/__init__.py
+-rw-r--r--   0        0        0     2019 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/loader/base_loader.py
+-rw-r--r--   0        0        0     4434 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/loader/dataset.py
+-rw-r--r--   0        0        0     3797 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/loader/model_loader.py
+-rw-r--r--   0        0        0     2387 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/pht_worker.py
+-rw-r--r--   0        0        0       64 2022-08-01 10:19:24.771945 pht_station-0.2.0/station/worker/requirements.txt
+-rw-r--r--   0        0        0        0 2022-08-01 10:19:24.730047 pht_station-0.2.0/station/worker/testing/__init__.py
+-rw-r--r--   0        0        0      393 2023-02-06 09:52:28.392304 pht_station-0.2.0/station/worker/testing/db.py
+-rw-r--r--   0        0        0     2304 2023-02-06 09:52:28.393306 pht_station-0.2.0/station/worker/testing/populate_minio.py
+-rw-r--r--   0        0        0     1333 2023-02-06 09:52:28.393306 pht_station-0.2.0/station/worker/testing/train_lightning_model.py
+-rw-r--r--   0        0        0       87 2022-08-01 10:19:24.738767 pht_station-0.2.0/station/worker/trainer/__init__.py
+-rw-r--r--   0        0        0     2709 2023-05-24 10:01:24.572056 pht_station-0.2.0/station/worker/trainer/base_trainer.py
+-rw-r--r--   0        0        0     7008 2023-02-06 09:52:28.396298 pht_station-0.2.0/station/worker/trainer/federated_trainer.py
+-rw-r--r--   0        0        0     5018 1970-01-01 00:00:00.000000 pht_station-0.2.0/setup.py
+-rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 pht_station-0.2.0/PKG-INFO
```

### Comparing `pht-station-0.1/station/app/api/api_v1/endpoints/airflow.py` & `pht_station-0.2.0/station/app/api/api_v1/endpoints/airflow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,123 @@
-from fastapi import APIRouter, Depends, HTTPException
-from sqlalchemy.orm import Session
-from datetime import datetime
-
-from station.app.api import dependencies
-from station.clients.airflow.client import airflow_client
-from station.clients.airflow import docker_trains as airflow_docker_train
-from station.app.schemas.airflow import AirflowInformation, AirflowTaskLog, AirflowRun, AirflowRunMsg
-from station.app.schemas.local_trains import LocalTrainRun
-from station.app.schemas.docker_trains import DockerTrainExecution
-from station.app.crud.crud_local_train import local_train
-from station.app.crud.crud_docker_trains import docker_trains
-
-
-router = APIRouter()
-
-
-@router.post("/{dag_id}/run", response_model=AirflowRun)
-def run(run_msg: AirflowRunMsg, dag_id: str, db: Session = Depends(dependencies.get_db)):
-    """
-    Trigger a dag run and return the run_id of the run
-    @param dag_id: ID of the DAG e.G. "run_local" , "run_pht_train" etc.
-    @param run_msg: UID of the train
-    @param db:  reference to the postgres database
-    """
-
-    if dag_id == "run_local":
-        config = local_train.get_train_config(db, run_msg.train_id)
-        run_id = airflow_client.trigger_dag("run_local", config)
-        run_information = LocalTrainRun(train_id=run_msg.train_id, run_id=run_id)
-        local_train.create_run(db, obj_in=run_information)
-
-    elif dag_id == "run_pht_train":
-        train = docker_trains.get_by_train_id(db, run_msg.train_id)
-        if not train.config_id:
-            run_config = None
-            config_id = "default"
-        else:
-            run_config = DockerTrainExecution(config_id=train.config_id)
-            config_id = train.config_id
-        execution = airflow_docker_train.run_train(db, run_msg.train_id, run_config)
-        run_id = execution.airflow_dag_run
-
-    else:
-        raise HTTPException(status_code=404, detail=f"DAG with id '{dag_id}' not found.")
-
-    return {"run_id": run_id,
-            "config_id": config_id,
-            "dag_id": dag_id,
-            "train_id": run_msg.train_id,
-            "start_date": datetime.now()
-            }
-
-
-@router.get("/logs/{dag_id}/{run_id}", response_model=AirflowInformation)
-def get_airflow_run_information(run_id: str, dag_id: str):
-    """
-    Get information about one airflow DAG execution.
-    @param dag_id: ID of the DAG e.G. "run_local" , "run_pht_train" etc.
-    @param run_id: Airflow run ID
-    @return:
-    """
-
-    run_info = airflow_client.get_run_information(dag_id, run_id)
-    for instance in run_info["tasklist"]["task_instances"][:]:
-        try:
-            instance.pop("sla_miss")
-        except KeyError:
-            pass
-        try:
-            instance.pop("pool_slots")
-        except KeyError:
-            pass
-        try:
-            instance.pop("pool")
-        except KeyError:
-            pass
-
-    print(run_info["tasklist"]["task_instances"][:])
-    return run_info
-
-
-@router.get("/logs/{dag_id}/{run_id}/{task_id}", response_model=AirflowTaskLog)
-def get_airflow_task_log(dag_id: str, run_id: str, task_id: str, task_try_number: int = None):
-    """
-    Get log of a task in a DAG execution.
-    @param dag_id: ID of the DAG e.G. "run_local" , "run_pht_train" etc.
-    @param task_id: id of teh task
-    @param run_id: Airflow run ID
-    @param task_try_number: specific try number for log request
-    @return:
-    """
-    run_info_data = airflow_client.get_task_log(dag_id, run_id, task_id, task_try_number)
-    if not run_info_data:
-        raise HTTPException(status_code=404, detail=f"{task_id} not found.")
-    return {"run_info": run_info_data}
+from datetime import datetime
+
+from fastapi import APIRouter, Depends, HTTPException
+from sqlalchemy.orm import Session
+
+from station.app.api import dependencies
+from station.app.auth import authorized_user
+
+# from station.common.clients.airflow.client import airflow_client
+from station.app.config import clients
+from station.app.crud.crud_docker_trains import docker_trains
+from station.app.schemas.airflow import (
+    AirflowInformation,
+    AirflowRun,
+    AirflowRunMsg,
+    AirflowTaskLog,
+)
+from station.app.schemas.docker_trains import DockerTrainExecution
+from station.app.schemas.users import User
+from station.common.clients.airflow import docker_trains as airflow_docker_train
+
+router = APIRouter()
+
+
+@router.post("/{dag_id}/run", response_model=AirflowRun)
+def run(
+    run_msg: AirflowRunMsg,
+    dag_id: str,
+    db: Session = Depends(dependencies.get_db),
+    user: User = Depends(authorized_user),
+):
+    """
+    Trigger a dag run and return the run_id of the run
+    @param dag_id: ID of the DAG e.G. "run_local" , "run_pht_train" etc.
+    @param run_msg: UID of the train
+    @param db:  reference to the postgres database
+
+    Args:
+        user:
+    """
+
+    if dag_id == "run_local":
+        raise NotImplementedError("run_local is not implemented yet")
+
+    elif dag_id == "run_pht_train":
+        train = docker_trains.get_by_train_id(db, run_msg.train_id)
+        if not train.config_id:
+            run_config = None
+            config_id = "default"
+        else:
+            run_config = DockerTrainExecution(config_id=train.config_id)
+            config_id = train.config_id
+        execution = airflow_docker_train.run_train(db, run_msg.train_id, run_config)
+        run_id = execution.airflow_dag_run
+
+    else:
+        raise HTTPException(
+            status_code=404, detail=f"DAG with id '{dag_id}' not found."
+        )
+
+    return {
+        "run_id": run_id,
+        "config_id": config_id,
+        "dag_id": dag_id,
+        "train_id": run_msg.train_id,
+        "start_date": datetime.now(),
+    }
+
+
+@router.get("/logs/{dag_id}/{run_id}", response_model=AirflowInformation)
+def get_airflow_run_information(
+    dag_id: str, run_id: str, user: User = Depends(authorized_user)
+):
+    """
+    Get information about one airflow DAG execution.
+    @param dag_id: ID of the DAG e.G. "run_local" , "run_pht_train" etc.
+    @param run_id: Airflow run ID
+    @return:
+    """
+
+    run_info = clients.airflow.get_run_information(dag_id, run_id)
+
+    for instance in run_info["tasklist"]["task_instances"][:]:
+        try:
+            instance.pop("sla_miss")
+        except KeyError:
+            pass
+        try:
+            instance.pop("pool_slots")
+        except KeyError:
+            pass
+        try:
+            instance.pop("pool")
+        except KeyError:
+            pass
+
+    return run_info
+
+
+@router.get(
+    "/logs/{dag_id}/{run_id}/{task_id}/{task_try_number}", response_model=AirflowTaskLog
+)
+def get_airflow_task_log(
+    dag_id: str,
+    run_id: str,
+    task_id: str,
+    task_try_number: int,
+    user: User = Depends(authorized_user),
+):
+    """
+    Get log of a task in a DAG execution.
+    @param dag_id: ID of the DAG e.G. "run_local" , "run_pht_train" etc.
+    @param task_id: id of teh task
+    @param run_id: Airflow run ID
+    @param task_try_number: specific try number for log request
+    @return:
+    """
+    run_info_data = clients.airflow.get_task_log(
+        dag_id, run_id, task_id, task_try_number
+    )
+    if not run_info_data:
+        raise HTTPException(status_code=404, detail=f"{task_id} not found.")
+    return {"run_info": run_info_data}
```

### Comparing `pht-station-0.1/station/app/api/api_v1/endpoints/docker_trains.py` & `pht_station-0.2.0/station/app/api/api_v1/endpoints/docker_trains.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,144 +1,190 @@
-import json
-from typing import List
-from sqlalchemy.orm import Session
-from fastapi import APIRouter, Depends, HTTPException
-
-from station.app.api import dependencies
-from station.clients.airflow import docker_trains as airflow_docker_train
-from station.app.schemas.docker_trains import DockerTrain, DockerTrainCreate, DockerTrainConfig, \
-    DockerTrainConfigCreate, DockerTrainConfigUpdate, DockerTrainExecution, DockerTrainState, DockerTrainSavedExecution
-from station.app.crud.crud_docker_trains import docker_trains
-from station.app.crud.crud_train_configs import docker_train_config
-from station.clients.harbor_client import harbor_client
-
-router = APIRouter()
-
-@router.get("/sync", response_model=List[DockerTrain])
-def synchronize_database(station_id: int = None, db: Session = Depends(dependencies.get_db)):
-    artifacts = harbor_client.get_artifacts_for_station(station_id=station_id)
-    if isinstance(artifacts, dict):
-        error = artifacts.get("errors")
-        if error:
-            raise HTTPException(status_code=404, detail=f"Station {station_id} not found.")
-    elif isinstance(artifacts, list):
-        train_list = []
-        if len(artifacts) == 0:
-            print(f"No train registered at station {station_id}.")
-        else:
-            for train in artifacts:
-                id = train["name"].split("/")[1]
-                created_at = train["creation_time"][:-1]
-                updated_at = train["update_time"][:-1]
-                if created_at == updated_at:
-                    updated_at = None
-                new_train = docker_trains.add_if_not_exists(db, train_id=id, created_at=created_at, updated_at=updated_at)
-                if new_train:
-                    train_list.append(new_train)
-        return train_list
-    else:
-        raise HTTPException(status_code=500, detail="Invalid response.")
-
-
-@router.get("", response_model=List[DockerTrain])
-def get_available_trains(limit: int = 0, db: Session = Depends(dependencies.get_db)):
-    if limit != 0:
-        db_trains = docker_trains.get_multi(db, limit=limit)
-    else:
-        db_trains = docker_trains.get_multi(db)
-    return db_trains
-
-
-@router.post("", response_model=DockerTrain)
-def register_train(create_msg: DockerTrainCreate, db: Session = Depends(dependencies.get_db)):
-    if docker_trains.get_by_train_id(db, train_id=create_msg.train_id):
-        raise HTTPException(status_code=400, detail=f"Train with id '{create_msg.train_id}' already exists.")
-    db_train = docker_trains.create(db, obj_in=create_msg)
-    return db_train
-
-
-@router.get("/{train_id}", response_model=DockerTrain)
-def get_train_by_train_id(train_id: str, db: Session = Depends(dependencies.get_db)):
-    db_train = docker_trains.get_by_train_id(db, train_id)
-    if not db_train:
-        raise HTTPException(status_code=404, detail=f"Train with id '{train_id}' not found.")
-    return db_train
-
-
-@router.post("/{train_id}/run", response_model=DockerTrainSavedExecution)
-def run_docker_train(train_id: str, run_config: DockerTrainExecution = None, db: Session = Depends(dependencies.get_db)):
-    execution = airflow_docker_train.run_train(db, train_id, run_config)
-    return execution
-
-
-@router.get("/{train_id}/config", response_model=DockerTrainConfig)
-def get_config_for_train(train_id: str, db: Session = Depends(dependencies.get_db)):
-    train = docker_trains.get_by_train_id(db, train_id)
-    if not train.config_id:
-        raise HTTPException(status_code=404, detail=f"Train '{train_id}' does not have an assigned config.")
-    config = docker_train_config.get(db, train.config_id)
-    return config
-
-
-@router.post("/{train_id}/config/{config_id}", response_model=DockerTrain)
-def assign_config_to_docker_train(train_id: str, config_id: int, db: Session = Depends(dependencies.get_db)):
-    train = docker_trains.get_by_train_id(db, train_id=train_id)
-    if not train:
-        raise HTTPException(status_code=404, detail=f"Train with id '{train_id}' not found.")
-
-    config = docker_train_config.get(db, config_id)
-    if not config:
-        raise HTTPException(status_code=404, detail=f"Config with id '{config_id}' not found.")
-
-    train = docker_train_config.assign_to_train(db, train_id, config.id)
-    return train
-
-
-@router.get("/{train_id}/state", response_model=DockerTrainState)
-def get_state_for_train(train_id: str, db: Session = Depends(dependencies.get_db)):
-    state = docker_trains.read_train_state(db, train_id)
-    return state
-
-
-@router.put("/{train_id}/state", response_model=DockerTrainState)
-def update_state_for_train(train_id: str, state: DockerTrainState, db: Session = Depends(dependencies.get_db)):
-    state = docker_trains.update_train_state(db, train_id, state)
-    return state
-
-
-@router.get("/configs/all", response_model=List[DockerTrainConfig])
-def get_all_docker_train_configs(db: Session = Depends(dependencies.get_db), skip: int = 0, limit: int = 100):
-    db_configs = docker_train_config.get_multi(db, skip=skip, limit=limit)
-    return db_configs
-
-
-@router.post("/config", response_model=DockerTrainConfig)
-def add_docker_train_configuration(config_in: DockerTrainConfigCreate, db: Session = Depends(dependencies.get_db)):
-    if docker_train_config.get_by_name(db, name=config_in.name):
-        raise HTTPException(status_code=400, detail="A config with the given name already exists.")
-    config = docker_train_config.create(db, obj_in=config_in)
-    return config
-
-
-@router.put("/config/{config_id}", response_model=DockerTrainConfig)
-def update_docker_train_configuration(update_config: DockerTrainConfigUpdate, config_id: int,
-                                      db: Session = Depends(dependencies.get_db)):
-    old_config = docker_train_config.get(db, config_id)
-    if not old_config:
-        raise HTTPException(status_code=404, detail=f"Config with id '{config_id}' not found.")
-    config = docker_train_config.update(db, db_obj=old_config, obj_in=update_config)
-    return config
-
-
-@router.get("/config/{config_id}", response_model=DockerTrainConfig)
-def get_docker_train_configuration(config_id: int, db: Session = Depends(dependencies.get_db)):
-    config = docker_train_config.get(db, config_id)
-    if not config:
-        raise HTTPException(status_code=404, detail=f"Config with id '{config_id}' not found.")
-
-    return config
-
-
-@router.get("/{train_id}/executions", response_model=List[DockerTrainSavedExecution])
-def get_docker_train_executions(train_id: str, db: Session = Depends(dependencies.get_db)):
-    executions = docker_trains.get_train_executions(db, train_id)
-    return executions
+from typing import List, Union
+
+from fastapi import APIRouter, Depends, HTTPException
+from sqlalchemy.orm import Session
+
+from station.app.api import dependencies
+from station.app.crud.crud_docker_trains import docker_trains
+from station.app.crud.crud_train_configs import docker_train_config
+from station.app.schemas.docker_trains import (
+    DockerTrain,
+    DockerTrainConfig,
+    DockerTrainConfigCreate,
+    DockerTrainConfigUpdate,
+    DockerTrainCreate,
+    DockerTrainExecution,
+    DockerTrainSavedExecution,
+    DockerTrainState,
+)
+from station.app.trains.docker import airflow
+
+router = APIRouter()
+
+
+@router.post("/sync", response_model=List[DockerTrain])
+def synchronize_database(db: Session = Depends(dependencies.get_db)):
+    return docker_trains.synchronize_central(db)
+
+
+@router.get("", response_model=List[DockerTrain])
+def get_available_trains(limit: int = 0, db: Session = Depends(dependencies.get_db)):
+    if limit != 0:
+        db_trains = docker_trains.get_multi(db, limit=limit)
+    else:
+        db_trains = docker_trains.get_multi(db)
+    return db_trains
+
+
+@router.post("", response_model=DockerTrain)
+def register_train(
+    create_msg: DockerTrainCreate, db: Session = Depends(dependencies.get_db)
+):
+    if docker_trains.get_by_train_id(db, train_id=create_msg.train_id):
+        raise HTTPException(
+            status_code=400,
+            detail=f"Train with id '{create_msg.train_id}' already exists.",
+        )
+    db_train = docker_trains.create(db, obj_in=create_msg)
+    return db_train
+
+
+@router.get("/{train_id}", response_model=DockerTrain)
+def get_train_by_train_id(
+    train_id: Union[int, str], db: Session = Depends(dependencies.get_db)
+):
+    if isinstance(train_id, str):
+        db_train = docker_trains.get_by_train_id(db, train_id)
+    else:
+        db_train = docker_trains.get(db, id=train_id)
+    if not db_train:
+        raise HTTPException(
+            status_code=404, detail=f"Train with id '{train_id}' not found."
+        )
+    return db_train
+
+
+@router.post("/{train_id}/run", response_model=DockerTrainSavedExecution)
+def run_docker_train(
+    train_id: str,
+    run_config: DockerTrainExecution = None,
+    db: Session = Depends(dependencies.get_db),
+):
+    execution = airflow.run_train(db, train_id, run_config)
+    return execution
+
+
+@router.get("/{train_id}/config", response_model=DockerTrainConfig)
+def get_config_for_train(train_id: str, db: Session = Depends(dependencies.get_db)):
+    train = docker_trains.get_by_train_id(db, train_id)
+    if not train.config_id:
+        raise HTTPException(
+            status_code=404,
+            detail=f"Train '{train_id}' does not have an assigned config.",
+        )
+    config = docker_train_config.get(db, train.config_id)
+    return config
+
+
+@router.post("/{train_id}/config/{config_id}", response_model=DockerTrain)
+def assign_config_to_docker_train(
+    train_id: str, config_id: int, db: Session = Depends(dependencies.get_db)
+):
+    train = docker_trains.get_by_train_id(db, train_id=train_id)
+    if not train:
+        raise HTTPException(
+            status_code=404, detail=f"Train with id '{train_id}' not found."
+        )
+
+    config = docker_train_config.get(db, config_id)
+    if not config:
+        raise HTTPException(
+            status_code=404, detail=f"Config with id '{config_id}' not found."
+        )
+
+    train = docker_train_config.assign_to_train(db, train_id, config.id)
+    return train
+
+
+@router.get("/{train_id}/state", response_model=DockerTrainState)
+def get_state_for_train(train_id: str, db: Session = Depends(dependencies.get_db)):
+    state = docker_trains.read_train_state(db, train_id)
+    return state
+
+
+@router.put("/{train_id}/state", response_model=DockerTrainState)
+def update_state_for_train(
+    train_id: str, state: DockerTrainState, db: Session = Depends(dependencies.get_db)
+):
+    state = docker_trains.update_train_state(db, train_id, state)
+    return state
+
+
+@router.get("/configs/all", response_model=List[DockerTrainConfig])
+def get_all_docker_train_configs(
+    db: Session = Depends(dependencies.get_db), skip: int = 0, limit: int = 100
+):
+    db_configs = docker_train_config.get_multi(db, skip=skip, limit=limit)
+    return db_configs
+
+
+@router.post("/config", response_model=DockerTrainConfig)
+def add_docker_train_configuration(
+    config_in: DockerTrainConfigCreate, db: Session = Depends(dependencies.get_db)
+):
+    print(config_in)
+    if docker_train_config.get_by_name(db, name=config_in.name):
+        raise HTTPException(
+            status_code=400, detail="A config with the given name already exists."
+        )
+    config = docker_train_config.create(db, obj_in=config_in)
+    return config
+
+
+@router.put("/config/{config_id}", response_model=DockerTrainConfig)
+def update_docker_train_configuration(
+    update_config: DockerTrainConfigUpdate,
+    config_id: int,
+    db: Session = Depends(dependencies.get_db),
+):
+    old_config = docker_train_config.get(db, config_id)
+    if not old_config:
+        raise HTTPException(
+            status_code=404, detail=f"Config with id '{config_id}' not found."
+        )
+    config = docker_train_config.update(db, db_obj=old_config, obj_in=update_config)
+    return config
+
+
+@router.get("/config/{config_id}", response_model=DockerTrainConfig)
+def get_docker_train_configuration(
+    config_id: int, db: Session = Depends(dependencies.get_db)
+):
+    config = docker_train_config.get(db, config_id)
+    if not config:
+        raise HTTPException(
+            status_code=404, detail=f"Config with id '{config_id}' not found."
+        )
+
+    return config
+
+
+@router.get("/executions/all", response_model=List[DockerTrainSavedExecution])
+def get_all_docker_train_executions(
+    skip: int = 0, limit: int = 100, db: Session = Depends(dependencies.get_db)
+):
+    db_executions = docker_trains.get_executions(db, skip=skip, limit=limit)
+    return db_executions
+
+
+@router.get("/{train_id}/executions", response_model=List[DockerTrainSavedExecution])
+def get_docker_train_executions(
+    train_id: str,
+    skip: int = 0,
+    limit: int = 100,
+    db: Session = Depends(dependencies.get_db),
+):
+    executions = docker_trains.get_train_executions(
+        db,
+        train_id,
+    )
+    return executions
```

### Comparing `pht-station-0.1/station/app/auth.py` & `pht_station-0.2.0/station/app/auth.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,158 @@
-from fastapi.security import HTTPBearer, HTTPAuthorizationCredentials
-import requests
-from loguru import logger
-from fastapi import Depends, HTTPException
-from requests import HTTPError
-from enum import Enum
-
-from station.app.config import settings
-from station.app.schemas.users import User
-from station.app.cache import redis_cache
-
-
-class TokenCacheKeys(str, Enum):
-    robot_token = "robot-token"
-    user_token_prefix = "user-token-"
-
-
-def get_robot_token(robot_id: str = None, robot_secret: str = None, token_url: str = None) -> str:
-    """
-    Get robot token from auth server.
-    """
-    # todo token caching
-
-    if not token_url:
-        token_url = settings.config.auth.token_url
-    if not robot_id:
-        robot_id = settings.config.auth.robot_id
-    if not robot_secret:
-        robot_secret = settings.config.auth.robot_secret.get_secret_value()
-
-    # try to read the token from cache and return it if it exists
-    cached_token = redis_cache.get(TokenCacheKeys.robot_token.value)
-    if cached_token:
-        logger.debug(f"Found cached robot token")
-        return cached_token
-    else:
-        # get a new token from the auth server
-        logger.debug(f"Requesting new robot token from {token_url}")
-        data = {
-            "id": robot_id,
-            "secret": robot_secret,
-            "grant_type": "robot_credentials"
-        }
-
-        response = requests.post(token_url, data=data).json()
-
-        # parse values from response and set cache
-        token = response.get("access_token")
-        ttl = response.get("expires_in")
-        redis_cache.set(TokenCacheKeys.robot_token.value, token, ttl)
-
-        return token
-
-
-def validate_user_token(token: str, robot_token: str, token_url: str = None) -> User:
-    """
-    Validate a user token against the auth server and parse a user object from the response.
-    Args:
-        token: token to validate
-        robot_token: the robot token to request token validation
-        token_url: token url of the auth server
-
-    Returns:
-        User object parsed from the auth server response
-    """
-    # todo token caching
-    if token_url is None:
-        token_url = settings.config.auth.token_url
-    url = f"{token_url}/{token}"
-    headers = {"Authorization": f"Bearer {robot_token}"}
-    r = requests.get(url, headers=headers)
-    print(headers)
-    print(r.text)
-    r.raise_for_status()
-    response = r.json()
-    if response.get("target").get("kind") == "user":
-        user = User(**response.get("target").get("entity"),
-                    permissions=response.get("target").get("permissions"))
-        return user
-    else:
-        raise NotImplementedError("Only user entities are supported.")
-
-
-def get_current_user(token: HTTPAuthorizationCredentials = Depends(HTTPBearer()),
-                     robot_token: str = Depends(get_robot_token),
-                     token_url: str = None) -> User:
-    """
-    Validate a user token against the auth server and parse a user object from the response.
-    Args:
-        token: token to validate
-        robot_token: the robot token to request token validation
-        token_url: token url of the auth server
-
-    Returns:
-        User object parsed from the auth server response
-    """
-
-    logger.debug(f"Validating user token {token.credentials}")
-    if token_url is None:
-        token_url = settings.config.auth.token_url
-    try:
-        user = validate_user_token(token=token.credentials, robot_token=robot_token, token_url=token_url)
-        return user
-    except HTTPError as e:
-        if e.response.status_code == 401:
-            raise HTTPException(status_code=401, detail="Invalid token")
-        elif e.response.status_code == 400:
-            # attempt refresh robot token
-            try:
-                robot_token = get_robot_token(robot_id=settings.config.auth.robot_id,
-                                              robot_secret=settings.config.auth.robot_secret.get_secret_value(),
-                                              token_url=token_url)
-
-                user = validate_user_token(token=token.credentials, robot_token=robot_token, token_url=token_url)
-                return user
-            except HTTPError:
-                raise HTTPException(status_code=401, detail="Invalid token")
+from enum import Enum
+from typing import List
+
+import requests
+from fastapi import Depends, HTTPException
+from fastapi.security import HTTPAuthorizationCredentials, HTTPBearer
+from loguru import logger
+from requests import HTTPError
+
+from station.app.cache import redis_cache
+from station.app.config import settings
+from station.app.schemas.users import User, UserPermission
+
+
+class TokenCacheKeys(str, Enum):
+    robot_token = "robot-token"
+    user_token_prefix = "user-token-"
+
+
+def get_robot_token(
+    robot_id: str = None, robot_secret: str = None, token_url: str = None
+) -> str:
+    """
+    Get robot token from auth server.
+    """
+    # todo token caching
+
+    logger.debug("Getting robot token")
+
+    if not token_url:
+        token_url = settings.config.auth.token_url
+    if not robot_id:
+        robot_id = settings.config.auth.robot_id
+    if not robot_secret:
+        robot_secret = settings.config.auth.robot_secret.get_secret_value()
+
+    # try to read the token from cache and return it if it exists
+    cached_token = redis_cache.get(TokenCacheKeys.robot_token.value)
+    if cached_token:
+        logger.debug("Found cached robot token")
+        return cached_token
+    else:
+        # get a new token from the auth server
+        logger.debug(f"Requesting new robot token from {token_url}")
+        data = {
+            "id": robot_id,
+            "secret": robot_secret,
+            "grant_type": "robot_credentials",
+        }
+
+        response = requests.post(token_url, data=data).json()
+
+        # parse values from response and set cache
+        token = response.get("access_token")
+        ttl = response.get("expires_in")
+
+        redis_cache.set(TokenCacheKeys.robot_token.value, token, ttl)
+
+        return token
+
+
+def validate_user_token(token: str, user_url: str = None) -> User:
+    """
+    Validate a user token against the auth server and parse a user object from the response.
+    Args:
+        token: token to validate
+        user_url: user url of the auth server
+
+    Returns:
+        User object parsed from the auth server response
+    """
+    # todo token caching
+    if user_url is None:
+        user_url = settings.config.auth.user_url
+    url = f"{user_url}/@me"
+    logger.debug(f"Validating user token against {url}")
+    headers = {"Authorization": f"Bearer {token}"}
+    r = requests.get(url, headers=headers)
+    r.raise_for_status()
+    user = User(**r.json())
+    return user
+
+
+def get_current_user(token: str, token_url: str = None) -> User:
+    """
+    Validate a user token against the auth server and parse a user object from the response.
+    Args:
+        token: token to validate
+        robot_token: the robot token to request token validation
+        token_url: token url of the auth server
+
+    Returns:
+        User object parsed from the auth server response
+    """
+
+    logger.debug("Validating bearer token")
+    if not settings.is_initialized:
+        logger.error("Found uninitialized setting.... Initializing settings")
+        settings.setup()
+    if token_url is None:
+        token_url = settings.config.auth.token_url
+    try:
+        user = validate_user_token(token=token)
+
+        return user
+    except HTTPError as e:
+        logger.error(f"Error validating user token: {e}")
+        if e.response.status_code == 401:
+            raise HTTPException(status_code=401, detail="Invalid token")
+        elif e.response.status_code == 400:
+            # attempt refresh robot token
+            try:
+
+                get_robot_token(
+                    robot_id=settings.config.auth.robot_id,
+                    robot_secret=settings.config.auth.robot_secret.get_secret_value(),
+                    token_url=token_url,
+                )
+
+                user = validate_user_token(token=token)
+                return user
+            except HTTPError:
+                raise HTTPException(status_code=401, detail="Invalid token")
+
+
+def get_user_permissions(user: User, token_url: str = None) -> List[UserPermission]:
+    # todo token caching
+    logger.debug(f"Getting user permissions for {user.name}")
+    if token_url is None:
+        token_url = settings.config.auth.token_url
+    url = f"{token_url}/introspect"
+    headers = {"Authorization": f"Bearer {user.token}"}
+    r = requests.get(url, headers=headers)
+    r.raise_for_status()
+    permissions = [UserPermission(**p) for p in r.json().get("permissions")]
+    return permissions
+
+
+# def authorized_user(token: HTTPAuthorizationCredentials = Depends(HTTPBearer()),
+#                     permissions: List[UserPermission] = None) -> User:
+def authorized_user(token: HTTPAuthorizationCredentials = Depends(HTTPBearer())):
+    """
+    Authorize a user by checking if they are in the allowed users list.
+    Args:
+        token: Bearer token from http header
+        permissions: list of permissions to check
+
+    Returns:
+        User object if authorized
+
+    """
+    logger.debug("Authorizing user")
+    user = get_current_user(token=token.credentials)
+    # if permissions:
+    #     user.permissions = get_user_permissions(user)
+    #     # todo validate permissions
+
+    return user
```

### Comparing `pht-station-0.1/station/app/crud/base.py` & `pht_station-0.2.0/station/app/crud/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,78 @@
-from typing import Any, Dict, Generic, List, Optional, Type, TypeVar, Union
-
-from fastapi.encoders import jsonable_encoder
-from pydantic import BaseModel
-from sqlalchemy.orm import Session
-
-from station.app.db.base_class import Base
-
-ModelType = TypeVar("ModelType", bound=Base)
-CreateSchemaType = TypeVar("CreateSchemaType", bound=BaseModel)
-UpdateSchemaType = TypeVar("UpdateSchemaType", bound=BaseModel)
-
-
-class CRUDBase(Generic[ModelType, CreateSchemaType, UpdateSchemaType]):
-    def __init__(self, model: Type[ModelType]):
-        """
-        CRUD object with default methods to Create, Read, Update, Delete (CRUD).
-
-        **Parameters**
-
-        * `model`: A SQLAlchemy model class
-        * `schema`: A Pydantic model (schema) class
-        """
-        self.model = model
-
-    def get(self, db: Session, id: Any) -> Optional[ModelType]:
-        return db.query(self.model).filter(self.model.id == id).first()
-
-    def get_multi(
-        self, db: Session, *, skip: int = 0, limit: int = 100
-    ) -> List[ModelType]:
-        return db.query(self.model).offset(skip).limit(limit).all()
-
-    def create(self, db: Session, *, obj_in: CreateSchemaType) -> ModelType:
-        obj_in_data = jsonable_encoder(obj_in)
-        db_obj = self.model(**obj_in_data)  # type: ignore
-        db.add(db_obj)
-        db.commit()
-        db.refresh(db_obj)
-        return db_obj
-
-    def update(
-        self,
-        db: Session,
-        *,
-        db_obj: ModelType,
-        obj_in: Union[UpdateSchemaType, Dict[str, Any]]
-    ) -> ModelType:
-
-        # todo check if automatic update of updated_at makes sense
-        obj_data = jsonable_encoder(db_obj)
-        if isinstance(obj_in, dict):
-            update_data = obj_in
-        else:
-            update_data = obj_in.dict(exclude_unset=True)
-        for field in obj_data:
-            if field in update_data:
-                setattr(db_obj, field, update_data[field])
-        db.add(db_obj)
-        db.commit()
-        db.refresh(db_obj)
-        return db_obj
-
-    def remove(self, db: Session, *, id: int) -> ModelType:
-        obj = db.query(self.model).get(id)
-        db.delete(obj)
-        db.commit()
-        return obj
+from typing import Any, Dict, Generic, List, Optional, Type, TypeVar, Union
+
+from fastapi.encoders import jsonable_encoder
+from pydantic import BaseModel
+from sqlalchemy.orm import Session
+from sqlalchemy.sql.schema import Column
+
+from station.app.db.base_class import Base
+
+ModelType = TypeVar("ModelType", bound=Base)
+CreateSchemaType = TypeVar("CreateSchemaType", bound=BaseModel)
+UpdateSchemaType = TypeVar("UpdateSchemaType", bound=BaseModel)
+
+
+class CRUDBase(Generic[ModelType, CreateSchemaType, UpdateSchemaType]):
+    def __init__(self, model: Type[ModelType]):
+        """
+        CRUD object with default methods to Create, Read, Update, Delete (CRUD).
+
+        **Parameters**
+
+        * `model`: A SQLAlchemy model class
+        * `schema`: A Pydantic model (schema) class
+        """
+        self.model = model
+
+    def get(self, db: Session, id: Any) -> Optional[ModelType]:
+        return db.query(self.model).filter(self.model.id == id).first()
+
+    def get_multi(
+        self, db: Session, *, skip: int = 0, limit: int = 100
+    ) -> List[ModelType]:
+        if isinstance(self.model.__table__.columns.get("created_at", None), Column):
+            return (
+                db.query(self.model)
+                .order_by(self.model.created_at.desc())
+                .offset(skip)
+                .limit(limit)
+                .all()
+            )
+
+        return db.query(self.model).offset(skip).limit(limit).all()
+
+    def create(self, db: Session, *, obj_in: CreateSchemaType) -> ModelType:
+        obj_in_data = jsonable_encoder(obj_in, exclude_none=True)
+        db_obj = self.model(**obj_in_data)  # type: ignore
+        db.add(db_obj)
+        db.commit()
+        db.refresh(db_obj)
+        return db_obj
+
+    def update(
+        self,
+        db: Session,
+        *,
+        db_obj: ModelType,
+        obj_in: Union[UpdateSchemaType, Dict[str, Any]]
+    ) -> ModelType:
+
+        # todo check if automatic update of updated_at makes sense
+        obj_data = jsonable_encoder(db_obj)
+        if isinstance(obj_in, dict):
+            update_data = obj_in
+        else:
+            update_data = obj_in.dict(exclude_unset=True)
+        for field in obj_data:
+            if field in update_data:
+                setattr(db_obj, field, update_data[field])
+        db.add(db_obj)
+        db.commit()
+        db.refresh(db_obj)
+        return db_obj
+
+    def remove(self, db: Session, *, id: int) -> ModelType:
+        obj = db.query(self.model).get(id)
+        db.delete(obj)
+        db.commit()
+        return obj
```

### Comparing `pht-station-0.1/station/app/crud/crud_fhir_servers.py` & `pht_station-0.2.0/station/app/crud/crud_fhir_servers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,55 @@
-from typing import Any, Union, Dict, List
-from sqlalchemy.orm import Session
-
-from .base import CRUDBase, CreateSchemaType, ModelType, UpdateSchemaType
-from station.app.schemas.fhir import FHIRServerCreate, FHIRServerUpdate
-from station.app.models.fhir_server import FHIRServer
-from station.app.config import settings
-
-
-class CRUDFHIRServers(CRUDBase[FHIRServer, FHIRServerCreate, FHIRServerUpdate]):
-
-    def create(self, db: Session, *, obj_in: CreateSchemaType) -> ModelType:
-        # Encrypt sensitive values
-        encrypted_in = self.encrypt_sensitive_values(obj_in)
-        # Add encrypted values to the db
-        return super().create(db, obj_in=encrypted_in)
-
-    def update(self, db: Session, *, db_obj: ModelType, obj_in: Union[UpdateSchemaType, Dict[str, Any]]) -> ModelType:
-        obj_in = self.encrypt_sensitive_values(obj_in)
-        return super().update(db, db_obj=db_obj, obj_in=obj_in)
-
-    def encrypt_sensitive_values(self, obj_in: Union[FHIRServerCreate, FHIRServerUpdate]) -> FHIRServerCreate:
-        """
-        Encrypt sensitive values in the FHIRServerCreate/FHIRServerUpdate object
-        Args:
-            obj_in:
-
-        Returns:
-            the same object with encrypted sensitive values
-        """
-        fernet = settings.get_fernet()
-
-        if obj_in.client_secret:
-            obj_in.client_secret = fernet.encrypt(obj_in.client_secret.encode()).decode()
-        if obj_in.password:
-            obj_in.password = fernet.encrypt(obj_in.password.encode()).decode()
-        if obj_in.token:
-            obj_in.token = fernet.encrypt(obj_in.token.encode()).decode()
-
-        return obj_in
-
-
-fhir_servers = CRUDFHIRServers(FHIRServer)
+from typing import Any, Dict, Union
+
+from sqlalchemy.orm import Session
+
+from station.app.models.fhir_server import FHIRServer
+from station.app.schemas.fhir import FHIRServerCreate, FHIRServerUpdate
+
+from .base import CreateSchemaType, CRUDBase, ModelType, UpdateSchemaType
+
+
+class CRUDFHIRServers(CRUDBase[FHIRServer, FHIRServerCreate, FHIRServerUpdate]):
+    def create(self, db: Session, *, obj_in: CreateSchemaType) -> ModelType:
+        # Encrypt sensitive values
+        encrypted_in = self.encrypt_sensitive_values(obj_in)
+        # Add encrypted values to the db
+        return super().create(db, obj_in=encrypted_in)
+
+    def update(
+        self,
+        db: Session,
+        *,
+        db_obj: ModelType,
+        obj_in: Union[UpdateSchemaType, Dict[str, Any]]
+    ) -> ModelType:
+        obj_in = self.encrypt_sensitive_values(obj_in)
+        return super().update(db, db_obj=db_obj, obj_in=obj_in)
+
+    def encrypt_sensitive_values(
+        self, obj_in: Union[FHIRServerCreate, FHIRServerUpdate]
+    ) -> FHIRServerCreate:
+        """
+        Encrypt sensitive values in the FHIRServerCreate/FHIRServerUpdate object
+        Args:
+            obj_in:
+        Returns:
+            the same object with encrypted sensitive values
+        """
+
+        from station.app.settings import settings
+
+        fernet = settings.get_fernet()
+
+        if obj_in.client_secret:
+            obj_in.client_secret = fernet.encrypt(
+                obj_in.client_secret.encode()
+            ).decode()
+        if obj_in.password:
+            obj_in.password = fernet.encrypt(obj_in.password.encode()).decode()
+        if obj_in.token:
+            obj_in.token = fernet.encrypt(obj_in.token.encode()).decode()
+
+        return obj_in
+
+
+fhir_servers = CRUDFHIRServers(FHIRServer)
```

### Comparing `pht-station-0.1/station/app/crud/crud_notifications.py` & `pht_station-0.2.0/station/app/crud/crud_notifications.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from sqlalchemy.orm import Session
-from typing import Any, Dict, Generic, List, Optional, Type, TypeVar, Union
-from .base import CRUDBase
-
-from station.app.models.notification import Notification
-from station.app.schemas.notifications import NotificationCreate, NotificationUpdate
-
-
-
-class CRUDNotifications(CRUDBase[Notification, NotificationCreate, NotificationUpdate]):
-
-    def read_notifications_for_user(self, db: Session, user: str) -> List[Notification]:
-        return db.query(Notification).filter(Notification.target_user == user).all()
-
-
-
-notifications = CRUDNotifications(Notification)
+from typing import List
+
+from sqlalchemy.orm import Session
+
+from station.app.models.notification import Notification
+from station.app.schemas.notifications import NotificationCreate, NotificationUpdate
+
+from .base import CRUDBase
+
+
+class CRUDNotifications(CRUDBase[Notification, NotificationCreate, NotificationUpdate]):
+    def read_notifications_for_user(self, db: Session, user: str) -> List[Notification]:
+        return db.query(Notification).filter(Notification.target_user == user).all()
+
+
+notifications = CRUDNotifications(Notification)
```

### Comparing `pht-station-0.1/station/app/db/setup_db.py` & `pht_station-0.2.0/station/app/db/setup_db.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,59 @@
-import uuid
-
-from station.app.db.session import engine, SessionLocal
-from station.app.db.base import Base
-
-from station.app.models import docker_trains
-
-
-# TODO use alembic
-def setup_db(dev=False):
-    Base.metadata.create_all(bind=engine)
-    if dev:
-        seed_db_for_testing()
-
-
-def reset_db(dev=False):
-    Base.metadata.drop_all(bind=engine)
-    Base.metadata.create_all(bind=engine)
-
-    if dev:
-        seed_db_for_testing()
-
-
-def seed_db_for_testing():
-    session = SessionLocal()
-    # create docker trains
-    if not session.query(docker_trains.DockerTrain).all():
-
-        dts = []
-        for _ in range(3):
-            dt = docker_trains.DockerTrain(
-                train_id=str(uuid.uuid4()),
-
-            )
-            dts.append(dt)
-        session.add_all(dts)
-        session.commit()
-
-        # Create states for the created trains
-        states = []
-        for dt in dts:
-            state = docker_trains.DockerTrainState(
-                train_id=dt.id,
-                status="inactive"
-            )
-            states.append(state)
-
-        session.add_all(states)
-
-        config = docker_trains.DockerTrainConfig(
-            name="default"
-        )
-
-        session.add(config)
-        session.commit()
-
-    session.close()
-
-
-if __name__ == '__main__':
-    # Base.metadata.drop_all(bind=engine)
-    setup_db()
+import uuid
+
+from station.app.db.base import Base
+from station.app.db.session import SessionLocal, engine
+from station.app.models import docker_trains
+
+
+# TODO use alembic
+def setup_db(dev=False, reset=False):
+
+    if reset:
+        reset_db(dev=False)
+    else:
+        Base.metadata.create_all(bind=engine)
+    if dev:
+        seed_db_for_testing()
+
+
+def reset_db(dev=False):
+    Base.metadata.drop_all(bind=engine)
+    Base.metadata.create_all(bind=engine)
+
+    if dev:
+        seed_db_for_testing()
+
+
+def seed_db_for_testing():
+    session = SessionLocal()
+    # create docker trains
+    if not session.query(docker_trains.DockerTrain).all():
+
+        dts = []
+        for _ in range(3):
+            dt = docker_trains.DockerTrain(
+                train_id=str(uuid.uuid4()),
+            )
+            dts.append(dt)
+        session.add_all(dts)
+        session.commit()
+
+        # Create states for the created trains
+        states = []
+        for dt in dts:
+            state = docker_trains.DockerTrainState(train_id=dt.id, status="inactive")
+            states.append(state)
+
+        session.add_all(states)
+
+        config = docker_trains.DockerTrainConfig(name="default")
+
+        session.add(config)
+        session.commit()
+
+    session.close()
+
+
+if __name__ == "__main__":
+    # Base.metadata.drop_all(bind=engine)
+    setup_db()
```

### Comparing `pht-station-0.1/station/app/logger.py` & `pht_station-0.2.0/station/app/logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,86 @@
-"""Configure handlers and formats for application loggers."""
-import logging
-import sys
-from pprint import pformat
-
-# if you dont like imports of private modules
-# you can move it to typing.py module
-from loguru import logger
-from loguru._defaults import LOGURU_FORMAT
-
-
-class InterceptHandler(logging.Handler):
-    """
-    Default handler from examples in loguru documentaion.
-    See https://loguru.readthedocs.io/en/stable/overview.html#entirely-compatible-with-standard-logging
-    """
-
-    def emit(self, record: logging.LogRecord):
-        # Get corresponding Loguru level if it exists
-        try:
-            level = logger.level(record.levelname).name
-        except ValueError:
-            level = record.levelno
-
-        # Find caller from where originated the logged message
-        frame, depth = logging.currentframe(), 2
-        while frame.f_code.co_filename == logging.__file__:
-            frame = frame.f_back
-            depth += 1
-
-        logger.opt(depth=depth, exception=record.exc_info).log(
-            level, record.getMessage()
-        )
-
-
-def format_record(record: dict) -> str:
-    """
-    Custom format for loguru loggers.
-    Uses pformat for log any data like request/response body during debug.
-    Works with logging if loguru handler it.
-
-    Example:
-    >>> payload = [{"users":[{"name": "Nick", "age": 87, "is_active": True}, {"name": "Alex", "age": 27, "is_active": True}], "count": 2}]
-    >>> logger.bind(payload=).debug("users payload")
-    >>> [   {   'count': 2,
-    >>>         'users': [   {'age': 87, 'is_active': True, 'name': 'Nick'},
-    >>>                      {'age': 27, 'is_active': True, 'name': 'Alex'}]}]
-    """
-
-    format_string = LOGURU_FORMAT
-    if record["extra"].get("payload") is not None:
-        record["extra"]["payload"] = pformat(
-            record["extra"]["payload"], indent=4, compact=True, width=88
-        )
-        format_string += "\n<level>{extra[payload]}</level>"
-
-    format_string += "{exception}\n"
-    return format_string
-
-
-def init_logging():
-    """
-    Replaces logging handlers with a handler for using the custom handler.
-
-    WARNING!
-    if you call the init_logging in startup event function,
-    then the first logs before the application start will be in the old format
-
-    >>> app.add_event_handler("startup", init_logging)
-    stdout:
-    INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
-    INFO:     Started reloader process [11528] using statreload
-    INFO:     Started server process [6036]
-    INFO:     Waiting for application startup.
-    2020-07-25 02:19:21.357 | INFO     | uvicorn.lifespan.on:startup:34 - Application startup complete.
-
-    """
-
-    # disable handlers for specific uvicorn loggers
-    # to redirect their output to the default uvicorn logger
-    # works with uvicorn==0.11.6
-    loggers = (
-        logging.getLogger(name)
-        for name in logging.root.manager.loggerDict
-        if name.startswith("uvicorn.")
-    )
-    for uvicorn_logger in loggers:
-        uvicorn_logger.handlers = []
-
-    # change handler for default uvicorn logger
-    intercept_handler = InterceptHandler()
-    logging.getLogger("uvicorn").handlers = [intercept_handler]
-
-    # set logs output, level and format
-    logger.configure(
-        handlers=[{"sink": sys.stdout, "level": logging.DEBUG, "format": format_record}]
-    )
+import logging
+import sys
+from pprint import pformat
+
+from loguru import logger
+from loguru._defaults import LOGURU_FORMAT
+
+
+class InterceptHandler(logging.Handler):
+    """
+    Default handler from examples in loguru documentaion.
+    See https://loguru.readthedocs.io/en/stable/overview.html#entirely-compatible-with-standard-logging
+    """
+
+    def emit(self, record: logging.LogRecord):
+        # Get corresponding Loguru level if it exists
+        try:
+            level = logger.level(record.levelname).name
+        except ValueError:
+            level = record.levelno
+
+        # Find caller from where originated the logged message
+        frame, depth = logging.currentframe(), 2
+        while frame.f_code.co_filename == logging.__file__:
+            frame = frame.f_back
+            depth += 1
+
+        logger.opt(depth=depth, exception=record.exc_info).log(
+            level, record.getMessage()
+        )
+
+
+def format_record(record: dict) -> str:
+    """
+    Custom format for loguru loggers.
+    Uses pformat for log any data like request/response body during debug.
+    Works with logging if loguru handler it.
+    """
+
+    format_string = LOGURU_FORMAT
+    if record["extra"].get("payload") is not None:
+        record["extra"]["payload"] = pformat(
+            record["extra"]["payload"], indent=4, compact=True, width=88
+        )
+        format_string += "\n<level>{extra[payload]}</level>"
+
+    format_string += "{exception}\n"
+    return format_string
+
+
+def init_logging():
+    """
+    Replaces logging handlers with a handler for using the custom handler.
+
+    WARNING!
+    if you call the init_logging in startup event function,
+    then the first logs before the application start will be in the old format
+    >>> app.add_event_handler("startup", init_logging)
+    stdout:
+    INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
+    INFO:     Started reloader process [11528] using statreload
+    INFO:     Started server process [6036]
+    INFO:     Waiting for application startup.
+    2020-07-25 02:19:21.357 | INFO     | uvicorn.lifespan.on:startup:34 - Application startup complete.
+
+    """
+
+    # disable handlers for specific uvicorn loggers
+    # to redirect their output to the default uvicorn logger
+    # works with uvicorn==0.11.6
+    loggers = (
+        logging.getLogger(name)
+        for name in logging.root.manager.loggerDict
+        if name.startswith("uvicorn.")
+    )
+    for uvicorn_logger in loggers:
+        uvicorn_logger.handlers = []
+
+    # change handler for default uvicorn logger
+    intercept_handler = InterceptHandler()
+    logging.getLogger("uvicorn").handlers = [intercept_handler]
+    logging.getLogger("uvicorn.access").handlers = [InterceptHandler()]
+    # set logs output, level and format
+    logger.configure(
+        handlers=[{"sink": sys.stdout, "level": logging.DEBUG, "format": format_record}]
+    )
```

### Comparing `pht-station-0.1/station/app/models/docker_trains.py` & `pht_station-0.2.0/station/app/models/docker_trains.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,62 @@
-from sqlalchemy import Boolean, Column, ForeignKey, Integer, String, DateTime, JSON
-from sqlalchemy.orm import relationship, backref
-from datetime import datetime
-
-from station.app.db.base_class import Base
-
-
-class DockerTrainState(Base):
-    __tablename__ = "docker_train_states"
-    id = Column(Integer, primary_key=True, index=True)
-    train_id = Column(Integer, ForeignKey('docker_trains.id'))
-    #train = relationship("DockerTrain", backref=backref("state", uselist=False))
-    last_execution = Column(DateTime, nullable=True)
-    num_executions = Column(Integer, default=0)
-    status = Column(String, default="inactive")
-
-
-class DockerTrainExecution(Base):
-    __tablename__ = "docker_train_executions"
-    id = Column(Integer, primary_key=True, index=True)
-    train_id = Column(Integer, ForeignKey('docker_trains.id'))
-    #train_state_id = Column(Integer, ForeignKey('docker_train_states.id'), nullable=True)
-    start = Column(DateTime, default=datetime.now())
-    end = Column(DateTime, nullable=True)
-    airflow_dag_run = Column(String, nullable=True)
-    config = Column(Integer, ForeignKey('docker_train_configs.id'), nullable=True)
-
-
-class DockerTrainConfig(Base):
-    __tablename__ = "docker_train_configs"
-    id = Column(Integer, primary_key=True, index=True)
-    name = Column(String, unique=True)
-    created_at = Column(DateTime, default=datetime.now())
-    updated_at = Column(DateTime, nullable=True)
-    airflow_config = Column(JSON, nullable=True)
-    trains = relationship("DockerTrain")
-    cpu_requirements = Column(JSON, nullable=True)
-    gpu_requirements = Column(JSON, nullable=True)
-    auto_execute = Column(Boolean, default=False)
-    dataset_id = Column(Integer, ForeignKey('datasets.id'), nullable=True)
-
-
-class DockerTrain(Base):
-    __tablename__ = "docker_trains"
-    id = Column(Integer, primary_key=True, index=True)
-    train_id = Column(String, unique=True, index=True)
-    created_at = Column(DateTime, default=datetime.now())
-    updated_at = Column(DateTime, nullable=True)
-    proposal_id = Column(Integer, default=0)
-    config_id = Column(Integer, ForeignKey("docker_train_configs.id"), nullable=True)
-    #config = relationship("DockerTrainConfig", back_populates="trains")
-    is_active = Column(Boolean, default=False)
-    state = relationship("DockerTrainState", uselist=False)
-    #state = relationship("DockerTrainState", backref=backref('train', uselist=False))
-    executions = relationship("DockerTrainExecution")
+from datetime import datetime
+
+from sqlalchemy import JSON, Boolean, Column, DateTime, ForeignKey, Integer, String
+from sqlalchemy.dialects.postgresql import UUID
+from sqlalchemy.orm import relationship
+
+from station.app.db.base_class import Base
+
+
+class DockerTrainState(Base):
+    __tablename__ = "docker_train_states"
+    id = Column(Integer, primary_key=True, index=True)
+    train_id = Column(Integer, ForeignKey("docker_trains.id"))
+    # train = relationship("DockerTrain", backref=backref("state", uselist=False))
+    last_execution = Column(DateTime, nullable=True)
+    num_executions = Column(Integer, default=0)
+    status = Column(String, default="inactive")
+    central_status = Column(String, nullable=True)
+
+
+class DockerTrainExecution(Base):
+    __tablename__ = "docker_train_executions"
+    id = Column(Integer, primary_key=True, index=True)
+    train_id = Column(Integer, ForeignKey("docker_trains.id"))
+    # train_state_id = Column(Integer, ForeignKey('docker_train_states.id'), nullable=True)
+    start = Column(DateTime, default=datetime.now())
+    end = Column(DateTime, nullable=True)
+    airflow_dag_run = Column(String, nullable=True)
+    config = Column(Integer, ForeignKey("docker_train_configs.id"), nullable=True)
+    dataset_id = Column(UUID(as_uuid=True), ForeignKey("datasets.id"), nullable=True)
+
+
+class DockerTrainConfig(Base):
+    __tablename__ = "docker_train_configs"
+    id = Column(Integer, primary_key=True, index=True)
+    name = Column(String, unique=True)
+    created_at = Column(DateTime, default=datetime.now())
+    updated_at = Column(DateTime, nullable=True)
+    airflow_config = Column(JSON, nullable=True)
+    trains = relationship("DockerTrain")
+    cpu_requirements = Column(JSON, nullable=True)
+    gpu_requirements = Column(JSON, nullable=True)
+    auto_execute = Column(Boolean, default=False)
+    dataset_id = Column(UUID(as_uuid=True), ForeignKey("datasets.id"), nullable=True)
+
+
+class DockerTrain(Base):
+    __tablename__ = "docker_trains"
+    id = Column(Integer, primary_key=True, index=True)
+    train_id = Column(String, unique=True, index=True)
+    name = Column(String, nullable=True)
+    proposal = Column(String, nullable=True)
+    is_active = Column(Boolean, default=False)
+    image_name = Column(String, nullable=True)
+    type = Column(String, nullable=True)
+    created_at = Column(DateTime, default=datetime.now())
+    updated_at = Column(DateTime, nullable=True)
+    config_id = Column(Integer, ForeignKey("docker_train_configs.id"), nullable=True)
+    config = relationship("DockerTrainConfig", back_populates="trains")
+    state = relationship("DockerTrainState", uselist=False, cascade="all, delete")
+    executions = relationship("DockerTrainExecution", cascade="all, delete")
+    num_participants = Column(Integer, nullable=True)
```

### Comparing `pht-station-0.1/station/app/schemas/airflow.py` & `pht_station-0.2.0/station/app/schemas/airflow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-from pydantic import BaseModel
-from datetime import datetime
-from typing import Optional, Any, List
-
-
-class TaskInstances(BaseModel):
-    dag_id: str
-    duration: Optional[float]
-    end_date: Optional[datetime]
-    execution_date: datetime
-    executor_config: str
-    hostname: str
-    max_tries: int
-    operator: str
-    pid: Optional[int]
-    priority_weight: int
-    queue: str
-    queued_when: Optional[datetime]
-    start_date: Optional[datetime]
-    state: Optional[str]
-    task_id: str
-    try_number: int
-    unixname: str
-
-
-class Tasklist(BaseModel):
-    task_instances: List[TaskInstances]
-    total_entries: int
-
-
-class AirflowInformation(BaseModel):
-    conf: dict
-    dag_id: str
-    dag_run_id: str
-    end_date: Optional[datetime]
-    execution_date: datetime
-    external_trigger: bool
-    logical_date: datetime
-    start_date: Optional[datetime]
-    state: str
-    tasklist: Tasklist
-
-
-class AirflowTaskLog(BaseModel):
-    run_info: str
-
-
-class AirflowRunMsg(BaseModel):
-    train_id: str
-
-
-class AirflowRun(BaseModel):
-    run_id: str
-    dag_id: str
-    train_id: str
-    start_date: datetime
+from datetime import datetime
+from typing import List, Optional
+
+from pydantic import BaseModel
+
+
+class TaskInstances(BaseModel):
+    dag_id: str
+    duration: Optional[float]
+    end_date: Optional[datetime]
+    execution_date: datetime
+    executor_config: str
+    hostname: str
+    max_tries: int
+    operator: str
+    pid: Optional[int]
+    priority_weight: int
+    queue: str
+    queued_when: Optional[datetime]
+    start_date: Optional[datetime]
+    state: Optional[str]
+    task_id: str
+    try_number: int
+    unixname: str
+
+
+class Tasklist(BaseModel):
+    task_instances: List[TaskInstances]
+    total_entries: int
+
+
+class AirflowInformation(BaseModel):
+    conf: dict
+    dag_id: str
+    dag_run_id: str
+    end_date: Optional[datetime]
+    execution_date: datetime
+    external_trigger: bool
+    logical_date: datetime
+    start_date: Optional[datetime]
+    state: str
+    tasklist: Tasklist
+
+
+class AirflowTaskLog(BaseModel):
+    run_info: str
+
+
+class AirflowRunMsg(BaseModel):
+    train_id: str
+
+
+class AirflowRun(BaseModel):
+    run_id: str
+    dag_id: str
+    train_id: str
+    start_date: datetime
```

### Comparing `pht-station-0.1/station/app/schemas/dl_models.py` & `pht_station-0.2.0/station/app/schemas/dl_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-from pydantic import BaseModel
-from datetime import datetime
-from typing import Optional
-
-
-class TorchModelBase(BaseModel):
-    model_id: Optional[str] = None
-
-
-class TorchModelCreate(TorchModelBase):
-    pass
-
-
-class TorchModelUpdate(TorchModelBase):
-    pass
-
-
-class TorchModelCheckPoint(BaseModel):
-    id: int
-    created_at: datetime
-    updated_at: Optional[datetime]
-    checkpoint: Optional[bytes]
-
-    class Config:
-        orm_mode = True
-
-
-class TorchModel(TorchModelBase):
-    id: int
-    created_at: datetime
-    updated_at: Optional[datetime]
-
-    class Config:
-        orm_mode = True
-
-
-class DLModelBase(BaseModel):
-    model_type: str
-    model_name: str
-    model_src: str
-    train_id: Optional[str] = None
-
-
-class DLModelCreate(DLModelBase):
-    pass
-
-
-class DLModelUpdate(DLModelBase):
-    pass
-
-
-class DLModel(DLModelBase):
-    id: int
-    model_id: Optional[str] = None
-    created_at: datetime
-    updated_at: Optional[datetime] = None
-
-    class Config:
-        orm_mode = True
+from datetime import datetime
+from typing import Optional
+
+from pydantic import BaseModel
+
+
+class TorchModelBase(BaseModel):
+    model_id: Optional[str] = None
+
+
+class TorchModelCreate(TorchModelBase):
+    pass
+
+
+class TorchModelUpdate(TorchModelBase):
+    pass
+
+
+class TorchModelCheckPoint(BaseModel):
+    id: int
+    created_at: datetime
+    updated_at: Optional[datetime]
+    checkpoint: Optional[bytes]
+
+    class Config:
+        orm_mode = True
+
+
+class TorchModel(TorchModelBase):
+    id: int
+    created_at: datetime
+    updated_at: Optional[datetime]
+
+    class Config:
+        orm_mode = True
+
+
+class DLModelBase(BaseModel):
+    model_type: str
+    model_name: str
+    model_src: str
+    train_id: Optional[str] = None
+
+
+class DLModelCreate(DLModelBase):
+    pass
+
+
+class DLModelUpdate(DLModelBase):
+    pass
+
+
+class DLModel(DLModelBase):
+    id: int
+    model_id: Optional[str] = None
+    created_at: datetime
+    updated_at: Optional[datetime] = None
+
+    class Config:
+        orm_mode = True
```

### Comparing `pht-station-0.1/station/app/schemas/trains.py` & `pht_station-0.2.0/station/app/schemas/users.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-from pydantic import BaseModel
-from datetime import datetime
-from typing import Optional
-
-from station.app.schemas import datasets
-
-
-class DBSchema(BaseModel):
-    class Config:
-        orm_mode = True
-
-
-class TrainState(DBSchema):
-    id: int
-    iteration: int
-    round: int
-    updated_at: Optional[datetime] = None
-    signing_key: Optional[str] = None
-    sharing_key: Optional[str] = None
-    seed: Optional[int] = None
-    key_broadcast: Optional[str] = None
-
-
-class TrainCreate(BaseModel):
-    name: Optional[str] = None
-    proposal_id: Optional[str] = None
-
-
-class TrainUpdate(TrainCreate):
-    pass
-
-
-class Train(DBSchema):
-    id: int
-    name: Optional[str] = None
-    created_at: datetime
-    updated_at: Optional[datetime] = None
-    is_active: bool
-    proposal_id: Optional[str] = None
-    state: TrainState
-    token: Optional[str] = None
-    dataset: Optional[datasets.DataSet] = None
-
-
-class FederatedTrainConfigCreate(DBSchema):
-    name: str
+import datetime
+from typing import List, Optional
+
+from pydantic import BaseModel
+
+
+def to_camel(string: str) -> str:
+    split = string.split("_")
+    return split[0] + "".join(word.capitalize() for word in split[1:])
+
+
+class UserPermission(BaseModel):
+    id: str
+    negation: bool
+    power: int
+    condition: Optional[str] = None
+    fields: Optional[List[str]] = None
+
+
+class User(BaseModel):
+    id: str
+    name: str
+    email: Optional[str] = None
+    active: bool
+    token: Optional[str] = None
+    created_at: datetime.datetime
+    updated_at: Optional[datetime.datetime] = None
+    realm_id: str
+    display_name: str
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    name_locked: bool
+    permissions: Optional[List[UserPermission]] = None
+    status: Optional[str] = None
+    status_message: Optional[str] = None
+
+
+class Token(BaseModel):
+    exp: int
+    iat: int
+    iss: str
+    remote_address: str
+    sub: str
+    sub_kind: str
+
+    class Config:
+        alias_generator = to_camel
+
+
+class UserResponse(BaseModel):
+    user: User
+    token: dict
```

### Comparing `pht-station-0.1/station/clients/airflow/client.py` & `pht_station-0.2.0/station/common/clients/airflow/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,127 +1,148 @@
-import requests
-import os
-from dotenv import find_dotenv, load_dotenv
-from requests.auth import HTTPBasicAuth
-from loguru import logger
-
-from station.app.schemas.station_status import HealthStatus
-
-
-class AirflowClient:
-    def __init__(self, airflow_api_url: str = None, airflow_user: str = None, airflow_password: str = None):
-        self.airflow_url = airflow_api_url if airflow_api_url else os.getenv("AIRFLOW_API_URL", "localhost:8080/api/v1")
-        self.airflow_user = airflow_user if airflow_user else os.getenv("AIRFLOW_USER", "admin")
-        self.airflow_pw = airflow_password if airflow_password else os.getenv("AIRFLOW_PW", "admin")
-        self.auth = HTTPBasicAuth(self.airflow_user, self.airflow_pw)
-
-    def trigger_dag(self, dag_id: str, config: dict = None) -> str:
-        """
-        Execute a dag with the given configuration
-
-        :param dag_id: string identifier of the dag i.e. 'run_train'
-        :param config: dictionary containing configuration values passed to the dag
-        :return:
-        """
-
-        # create default empty config
-        config_msg = {
-            "conf": {},
-        }
-        if config:
-            config_msg["conf"] = config
-
-        url = self.airflow_url + f"dags/{dag_id}/dagRuns"
-        r = requests.post(url=url, auth=self.auth, json=config_msg)
-        try:
-            r.raise_for_status()
-
-        except Exception as e:
-            logger.error(f"Error triggering dag: \n{e}")
-            raise e
-        return r.json()["dag_run_id"]
-
-    def get_dag_run(self, dag_id: str):
-        pass
-
-    def get_all_dag_runs(self, dag_id: str):
-        url = self.airflow_url + f"dags/{dag_id}/dagRuns"
-        r = requests.get(url=url, auth=self.auth)
-        r.raise_for_status()
-        return r.json()
-
-    def get_dags(self):
-        url = self.airflow_url + "dags"
-        r = requests.get(url=url, auth=self.auth)
-        r.raise_for_status()
-
-        return r.json()
-
-    # TODO create arguments for individual connection options
-    def create_connection(self, connection_dict: dict):
-        url = self.airflow_url + "connections"
-        r = requests.post(url=url, json=connection_dict)
-        r.raise_for_status()
-
-    def health_check(self) -> HealthStatus:
-        """
-
-        @return: dict: Airflow Status
-        """
-        url = self.airflow_url + "/health"
-        r = requests.get(url=url)
-        try:
-            r.raise_for_status()
-            return HealthStatus.healthy
-        except Exception as e:
-            logger.error(f"Error checking airflow health: \n{e}")
-            return HealthStatus.error
-
-    def get_run_information(self, dag_id: str, run_id: str) -> dict:
-        """
-        requests the information about a dag run state from airflow.
-        @param dag_id: ID of the dag (e.g. "run_train" or "run_local")
-        @param run_id: Airflow ID of the run (has the form of e.g. " "manual__2021-11-09T14:12:24.622670+00:00")
-        @return: dict: information about the run
-        """
-        url = self.airflow_url + f"dags/{dag_id}/dagRuns/{run_id}/taskInstances"
-        task_list = requests.get(url=url, auth=self.auth)
-        task_list.raise_for_status()
-        task_list = task_list.json()
-        url = self.airflow_url + f"dags/{dag_id}/dagRuns/{run_id}"
-        information = requests.get(url=url, auth=self.auth)
-        information.raise_for_status()
-        information = information.json()
-        information["tasklist"] = task_list
-        return information
-
-    def get_task_log(self, dag_id: str, run_id: str, task_id: str, task_try_number: int = None) -> dict:
-        """
-        get the log of a task for a specific run
-        @param dag_id: dag under which the task is run
-        @param run_id: id for specific run
-        @param task_id: task for which the logs are requested
-        @param task_try_number: specific try number of the task, default is the last try
-        @return: logs of the task run
-        """
-
-        task_number_list = []
-        task_known = False
-        for task in self.get_run_information(dag_id, run_id)["tasklist"]["task_instances"]:
-            if task["task_id"] == task_id:
-                task_known = True
-                task_number_list.append(task["try_number"])
-        if task_known:
-            last_task_try_number = max(task_number_list)
-            if task_try_number and task_try_number <= last_task_try_number:
-                try_number = task_try_number
-            else:
-                try_number = last_task_try_number
-            url = self.airflow_url + f"dags/{dag_id}/dagRuns/{run_id}/taskInstances/{task_id}/logs/{try_number}"
-            log = requests.get(url=url, auth=self.auth)
-            log.raise_for_status()
-            return log.content.decode("utf-8")
-        else:
-            return None
-
-
-airflow_client = AirflowClient()
+import os
+
+import requests
+from loguru import logger
+from requests.auth import HTTPBasicAuth
+
+from station.app.schemas.station_status import HealthStatus
+
+
+class AirflowClient:
+    def __init__(
+        self,
+        airflow_api_url: str = None,
+        airflow_user: str = None,
+        airflow_password: str = None,
+    ):
+        self.airflow_url = (
+            airflow_api_url
+            if airflow_api_url
+            else os.getenv("AIRFLOW_API_URL", "localhost:8080/api/v1")
+        )
+        self.airflow_user = (
+            airflow_user if airflow_user else os.getenv("AIRFLOW_USER", "admin")
+        )
+        self.airflow_pw = (
+            airflow_password if airflow_password else os.getenv("AIRFLOW_PW", "admin")
+        )
+        self.auth = HTTPBasicAuth(self.airflow_user, self.airflow_pw)
+
+    def trigger_dag(self, dag_id: str, config: dict = None) -> str:
+        """
+        Execute a dag with the given configuration
+
+        :param dag_id: string identifier of the dag i.e. 'run_train'
+        :param config: dictionary containing configuration values passed to the dag
+        :return:
+        """
+
+        # create default empty config
+        config_msg = {
+            "conf": {},
+        }
+        if config:
+            config_msg["conf"] = config
+
+        url = self.airflow_url + f"dags/{dag_id}/dagRuns"
+        r = requests.post(url=url, auth=self.auth, json=config_msg)
+        try:
+            r.raise_for_status()
+
+        except Exception as e:
+            logger.error(f"Error triggering dag: \n{e}")
+            logger.error(f"Error message: \n{r.text}")
+            raise e
+        return r.json()["dag_run_id"]
+
+    def get_dag_run(self, dag_id: str):
+        pass
+
+    def get_all_dag_runs(self, dag_id: str):
+        url = self.airflow_url + f"dags/{dag_id}/dagRuns"
+        r = requests.get(url=url, auth=self.auth)
+        r.raise_for_status()
+        return r.json()
+
+    def get_dags(self):
+        url = self.airflow_url + "dags"
+        r = requests.get(url=url, auth=self.auth)
+        r.raise_for_status()
+
+        return r.json()
+
+    # TODO create arguments for individual connection options
+    def create_connection(self, connection_dict: dict):
+        url = self.airflow_url + "connections"
+        r = requests.post(url=url, json=connection_dict)
+        r.raise_for_status()
+
+    def health_check(self) -> HealthStatus:
+        """
+
+        @return: dict: Airflow Status
+        """
+        url = self.airflow_url + "/health"
+        r = requests.get(url=url)
+        try:
+            r.raise_for_status()
+            return HealthStatus.healthy
+        except Exception as e:
+            logger.error(f"Error checking airflow health: \n{e}")
+            return HealthStatus.error
+
+    def get_run_information(self, dag_id: str, run_id: str) -> dict:
+        """
+        requests the information about a dag run state from airflow.
+        @param dag_id: ID of the dag (e.g. "run_train" or "run_local")
+        @param run_id: Airflow ID of the run (has the form of e.g. " "manual__2021-11-09T14:12:24.622670+00:00")
+        @return: dict: information about the run
+        """
+        url = self.airflow_url + f"dags/{dag_id}/dagRuns/{run_id}/taskInstances"
+        task_list = requests.get(url=url, auth=self.auth)
+        task_list.raise_for_status()
+        task_list = task_list.json()
+        url = self.airflow_url + f"dags/{dag_id}/dagRuns/{run_id}"
+        information = requests.get(url=url, auth=self.auth)
+        information.raise_for_status()
+        information = information.json()
+        information["tasklist"] = task_list
+        return information
+
+    def get_task_log(
+        self, dag_id: str, run_id: str, task_id: str, task_try_number: int = None
+    ) -> str:
+        """
+        get the log of a task for a specific run
+        @param dag_id: dag under which the task is run
+        @param run_id: id for specific run
+        @param task_id: task for which the logs are requested
+        @param task_try_number: specific try number of the task, default is the last try
+        @return: logs of the task run
+        """
+
+        task_number_list = []
+        task_known = False
+        for task in self.get_run_information(dag_id, run_id)["tasklist"][
+            "task_instances"
+        ]:
+            if task["task_id"] == task_id:
+                task_known = True
+                task_number_list.append(task["try_number"])
+        if task_known:
+            last_task_try_number = max(task_number_list)
+            if task_try_number and task_try_number <= last_task_try_number:
+                try_number = task_try_number
+            else:
+                try_number = last_task_try_number
+            url = (
+                self.airflow_url
+                + f"dags/{dag_id}/dagRuns/{run_id}/taskInstances/{task_id}/logs/{try_number}"
+            )
+            log = requests.get(url=url, auth=self.auth)
+            log.raise_for_status()
+            return log.content.decode("utf-8")
+        else:
+            return ""
+
+
+airflow_client = AirflowClient()
```

### Comparing `pht-station-0.1/station/clients/central/central_client.py` & `pht_station-0.2.0/station/common/clients/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,81 @@
-from typing import Any
-import urllib.parse
-
-import requests
-import pendulum
-
-
-class CentralApiClient:
-
-    def __init__(self, api_url: str, robot_id: str, robot_secret: str):
-        self.api_url = api_url
-        self.robot_id = robot_id
-        self.robot_secret = robot_secret
-        self.token = None
-        self.token_expiration = None
-        self.setup()
-
-    def setup(self):
-        self._get_token()
-
-    @property
-    def headers(self) -> dict:
-        token = self._get_token()
-
-        return {"Authorization": f"Bearer {token}"}
-
-    def get_trains(self, station_id: Any) -> list:
-        pass
-
-    def get_registry_credentials(self, station_id: Any) -> dict:
-        url = self.api_url + f"/stations/{station_id}?"
-        filters = "fields[station]=+secure_id,+registry_project_account_name,+registry_project_account_token,+public_key"
-        safe_filters = urllib.parse.quote(filters, safe="=")
-        url = url + safe_filters
-        r = requests.get(url, headers=self.headers)
-        r.raise_for_status()
-        return r.json()
-
-    def update_public_key(self, station_id: Any, public_key: str) -> dict:
-        url = self.api_url + f"/stations/{station_id}"
-        payload = {
-            "public_key": public_key
-        }
-        r = requests.post(url, headers=self.headers, json=payload)
-        r.raise_for_status()
-        return r.json()
-
-    def _get_token(self) -> str:
-        if not self.token or self.token_expiration < pendulum.now():
-            r = requests.post(f"{self.api_url}/token", data={"id": self.robot_id, "secret": self.robot_secret})
-            try:
-                r.raise_for_status()
-            except requests.exceptions.HTTPError as e:
-                print(r.text)
-                raise e
-            r = r.json()
-            self.token = r["access_token"]
-            self.token_expiration = pendulum.now().add(seconds=r["expires_in"])
-
-        return self.token
+import urllib.parse
+
+import pendulum
+import requests
+from authup import Authup
+from pydantic import SecretStr
+
+
+class BaseClient:
+    def __init__(
+        self,
+        base_url: str,
+        auth_url: str = None,
+        username: str = None,
+        password: str = None,
+        robot_id: str = None,
+        robot_secret: str = None,
+        headers: dict = None,
+    ):
+        self.base_url = base_url
+        self.auth_url = auth_url
+        self.username = username
+        self.password = password
+        self.robot_id = robot_id
+        self.robot_secret = robot_secret
+        self.token = None
+        self.refresh_token = None
+        self.token_expiration = None
+        self._headers = headers
+
+        self.auth = Authup(
+            url=self.auth_url,
+            username=self.username,
+            password=self.password,
+            robot_id=self.robot_id,
+            robot_secret=self.robot_secret,
+        )
+
+        if not self.auth_url:
+            self.auth_url = f"{self.base_url}/auth"
+
+        # self.setup()
+
+    @property
+    def headers(self) -> dict:
+        return self.auth.get_authorization_header()
+
+    # def setup(self):
+    #     self._get_token()
+
+    def _get_token(self) -> str:
+        if not self.token or self.token_expiration < pendulum.now():
+            if self.username and self.password:
+                r = requests.post(
+                    self.auth_url,
+                    data={"username": self.username, "password": self.password},
+                )
+            elif self.robot_id and self.robot_secret:
+                if isinstance(self.robot_secret, SecretStr):
+                    self.robot_secret = self.robot_secret.get_secret_value()
+                r = requests.post(
+                    self.auth_url,
+                    data={"id": self.robot_id, "secret": self.robot_secret},
+                )
+            else:
+                raise Exception("No credentials provided")
+
+            try:
+                r.raise_for_status()
+            except requests.exceptions.HTTPError as e:
+                print(r.text)
+                raise e
+            r = r.json()
+            self.token = r["access_token"]
+            self.token_expiration = pendulum.now().add(seconds=r["expires_in"])
+
+        return self.token
+
+    @staticmethod
+    def _make_url_safe(url: str) -> str:
+        return urllib.parse.quote(url, safe="=&?")
```

### Comparing `pht-station-0.1/station/clients/conductor/rest_client.py` & `pht_station-0.2.0/station/common/clients/conductor/rest_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-from typing import Any, Dict
-
-import requests
-from sqlalchemy.orm import Session
-import os
-
-
-class ConductorRESTClient:
-
-    def __init__(self, conductor_url: str = None, station_id: int = None):
-        self.conductor_url = conductor_url if conductor_url else os.getenv("CONDUCTOR_URL")
-        self.station_id = station_id if station_id else os.getenv("STATION_ID")
-
-        assert self.conductor_url
-        assert self.station_id
-
-    def get_model_for_train(self, train_id: Any, db: Session):
-        """
-        Obtain the model definition for the train given by the id from the conductor
-
-        :param train_id:
-        :param db:
-        :return:
-        """
-
-        url = self.conductor_url + f"/api/trains/{train_id}/model"
-        r = requests.get(url=url)
-        return r.json()
-
-    def upload_model_parameters(self, train_id: Any):
-        pass
-
-    def get_aggregated_model(self, train_id: Any):
-        pass
-
-    def get_available_trains(self):
-        url = self.conductor_url + f"/api/stations/{self.station_id}/trains"
-        r = requests.get(url)
-        r.raise_for_status()
-        return r.json()
-
-    def post_discovery_results(self, train_id: Any, discovery_results: Dict):
-        url = self.conductor_url + f"/api/trains/{train_id}/discovery"
-        r = requests.post(url, json=discovery_results)
-        print(r.request.body)
-        r.raise_for_status()
-        return r.json()
+import os
+from typing import Any, Dict
+
+import requests
+from sqlalchemy.orm import Session
+
+
+class ConductorRESTClient:
+    def __init__(self, conductor_url: str = None, station_id: int = None):
+        self.conductor_url = (
+            conductor_url if conductor_url else os.getenv("CONDUCTOR_URL")
+        )
+        self.station_id = station_id if station_id else os.getenv("STATION_ID")
+
+        assert self.conductor_url
+        assert self.station_id
+
+    def get_model_for_train(self, train_id: Any, db: Session):
+        """
+        Obtain the model definition for the train given by the id from the conductor
+
+        :param train_id:
+        :param db:
+        :return:
+        """
+
+        url = self.conductor_url + f"/api/trains/{train_id}/model"
+        r = requests.get(url=url)
+        return r.json()
+
+    def upload_model_parameters(self, train_id: Any):
+        pass
+
+    def get_aggregated_model(self, train_id: Any):
+        pass
+
+    def get_available_trains(self):
+        url = self.conductor_url + f"/api/stations/{self.station_id}/trains"
+        r = requests.get(url)
+        r.raise_for_status()
+        return r.json()
+
+    def post_discovery_results(self, train_id: Any, discovery_results: Dict):
+        url = self.conductor_url + f"/api/trains/{train_id}/discovery"
+        r = requests.post(url, json=discovery_results)
+        print(r.request.body)
+        r.raise_for_status()
+        return r.json()
```

### Comparing `pht-station-0.1/station/clients/docker/client.py` & `pht_station-0.2.0/station/common/clients/docker/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,101 @@
-import docker
-import time
-import os
-
-
-class DockerClient:
-    """
-    Get Information for the local docker instances
-    """
-
-    def __init__(self):
-        # TODO os env and add trys around the rest when wassetn posible to create a docker client
-
-        try:
-            self.client = docker.APIClient(base_url='unix://var/run/docker.sock')
-            self.containers = self.client.containers()
-        except docker.errors.DockerException as e:
-            print(e)
-            self.client = None
-            self.containers = None
-        self.container_statuses = []
-        self.sleep_time_for_cpu_usage_check = 3
-
-    def get_stats_all(self):
-        """
-        Returns a list of dicts, of  all the memory usage and the cpu utilization for all locally running docker
-        containers
-        """
-        container_statuses_start = self._get_all_stats_all_container()
-        time.sleep(self.sleep_time_for_cpu_usage_check)
-        container_statuses_end = self._get_all_stats_all_container()
-        return self._calculate_usage_statistics(container_statuses_start, container_statuses_end)
-
-    def get_stats_container(self, container_id):
-        """
-         Returns a list of dicts, with one element of the container with the id container_id the memory usage and
-         the cpu utilization for all locally running docker containers
-        """
-        container_status_start = self._get_all_stats_container(container_id)
-        time.sleep(self.sleep_time_for_cpu_usage_check)
-        container_status_end = self._get_all_stats_container(container_id)
-        return self._calculate_usage_statistics([container_status_start], [container_status_end])
-
-    def get_information_all_containers(self):
-        return self.containers
-
-    def get_master_images(self, masterImage):
-        # pull master image
-        registry = os.getenv("HARBOR_URL").split("//")[-1]
-        master_image_source = f"{registry}/{masterImage}"
-        self.docker_client.images.pull(master_image_source, tag="latest")
-
-    def _get_all_stats_all_container(self):
-        """
-        returns all the stats for all containers using the APIClient
-        """
-        container_statuses = []
-        for container in self.containers:
-            container_statuses.append(self.client.stats(container["Id"], stream=False))
-        return container_statuses
-
-    def _get_all_stats_container(self, container_id):
-        return self.client.stats(container_id, stream=True)
-
-    def _calculate_usage_statistics(self, start_measurements, end_measurements):
-        stats = []
-        for i in range(len(start_measurements)):
-            cpu_usage = self._calculate_cpu_usage(start_measurements[i], end_measurements[i])
-            name_container = start_measurements[i]["name"]
-            memory_usage = start_measurements[i]["memory_stats"]["usage"] / start_measurements[i]["memory_stats"][
-                "limit"]
-            status_dict = {"cpu_percent": cpu_usage, "memory_percent": memory_usage, "name": name_container}
-            stats.append(status_dict)
-        return stats
-
-    def _calculate_cpu_usage(self, start_measurement, end_measurement):
-        cpu_cycles_container = start_measurement["cpu_stats"]["cpu_usage"]["total_usage"] - \
-                               end_measurement["cpu_stats"]["cpu_usage"]["total_usage"]
-        total_cycles = start_measurement["cpu_stats"]["system_cpu_usage"] - end_measurement["cpu_stats"][
-            "system_cpu_usage"]
-        return cpu_cycles_container / total_cycles
-
-
-dockerClient = DockerClient()
+import os
+import time
+
+import docker
+
+
+class DockerClient:
+    """
+    Get Information for the local docker instances
+    """
+
+    def __init__(self):
+        # TODO os env and add trys around the rest when wassetn posible to create a docker client
+
+        try:
+            self.client = docker.APIClient(base_url="unix://var/run/docker.sock")
+            self.containers = self.client.containers()
+        except docker.errors.DockerException as e:
+            print(e)
+            self.client = None
+            self.containers = None
+        self.container_statuses = []
+        self.sleep_time_for_cpu_usage_check = 3
+
+    def get_stats_all(self):
+        """
+        Returns a list of dicts, of  all the memory usage and the cpu utilization for all locally running docker
+        containers
+        """
+        container_statuses_start = self._get_all_stats_all_container()
+        time.sleep(self.sleep_time_for_cpu_usage_check)
+        container_statuses_end = self._get_all_stats_all_container()
+        return self._calculate_usage_statistics(
+            container_statuses_start, container_statuses_end
+        )
+
+    def get_stats_container(self, container_id):
+        """
+        Returns a list of dicts, with one element of the container with the id container_id the memory usage and
+        the cpu utilization for all locally running docker containers
+        """
+        container_status_start = self._get_all_stats_container(container_id)
+        time.sleep(self.sleep_time_for_cpu_usage_check)
+        container_status_end = self._get_all_stats_container(container_id)
+        return self._calculate_usage_statistics(
+            [container_status_start], [container_status_end]
+        )
+
+    def get_information_all_containers(self):
+        return self.containers
+
+    def get_master_images(self, masterImage):
+        # pull master image
+        registry = os.getenv("HARBOR_URL").split("//")[-1]
+        master_image_source = f"{registry}/{masterImage}"
+        self.docker_client.images.pull(master_image_source, tag="latest")
+
+    def _get_all_stats_all_container(self):
+        """
+        returns all the stats for all containers using the APIClient
+        """
+        container_statuses = []
+        for container in self.containers:
+            container_statuses.append(self.client.stats(container["Id"], stream=False))
+        return container_statuses
+
+    def _get_all_stats_container(self, container_id):
+        return self.client.stats(container_id, stream=True)
+
+    def _calculate_usage_statistics(self, start_measurements, end_measurements):
+        stats = []
+        for i in range(len(start_measurements)):
+            cpu_usage = self._calculate_cpu_usage(
+                start_measurements[i], end_measurements[i]
+            )
+            name_container = start_measurements[i]["name"]
+            memory_usage = (
+                start_measurements[i]["memory_stats"]["usage"]
+                / start_measurements[i]["memory_stats"]["limit"]
+            )
+            status_dict = {
+                "cpu_percent": cpu_usage,
+                "memory_percent": memory_usage,
+                "name": name_container,
+            }
+            stats.append(status_dict)
+        return stats
+
+    def _calculate_cpu_usage(self, start_measurement, end_measurement):
+        cpu_cycles_container = (
+            start_measurement["cpu_stats"]["cpu_usage"]["total_usage"]
+            - end_measurement["cpu_stats"]["cpu_usage"]["total_usage"]
+        )
+        total_cycles = (
+            start_measurement["cpu_stats"]["system_cpu_usage"]
+            - end_measurement["cpu_stats"]["system_cpu_usage"]
+        )
+        return cpu_cycles_container / total_cycles
+
+
+dockerClient = DockerClient()
```

### Comparing `pht-station-0.1/station/clients/fhir/client.py` & `pht_station-0.2.0/station/common/clients/fhir/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,114 +1,127 @@
-from requests.auth import HTTPBasicAuth
-import requests
-import os
-
-from train_lib.clients.fhir import build_query_string
-from train_lib.clients.fhir.fhir_client import BearerAuth
-
-
-class FhirClient:
-    def __init__(self, server_url: str = None, username: str = None, password: str = None, token: str = None,
-                 server_type: str = None, disable_auth: bool = False):
-        """
-        Fhir client for station internal / health check / how many data points are in a fhir server
-        The code in hear is mostly copied from the train libary fhir client .
-
-        :param server_url: base url of the FHIR server to execute the query against
-        :param username: username for use in basic auth authentication against the fhir server
-        :param password: password for use in basic auth
-        :param token: token to use for authenticating against a FHIR server using a bearer token
-        :param server_type: the type of the server one of ["blaze", "hapi", "ibm"]
-        """
-        self.server_url = server_url if server_url else os.getenv("FHIR_ADDRESS")
-        self.username = username if username else os.getenv("FHIR_USER")
-        self.password = password if password else os.getenv("FHIR_PW")
-        self.token = token if token else os.getenv("FHIR_TOKEN")
-        self.server_type = server_type if server_type else os.getenv("FHIR_SERVER_TYPE")
-        self.output_format = None
-        # Check for correct initialization based on env vars or constructor parameters
-        if not (self.username and self.password) and self.token:
-            raise ValueError("Only one of username:pw or token auth can be selected")
-        if not ((self.username and self.password) or self.token) and disable_auth:
-            raise ValueError("Insufficient login information, either token or username and password need to be set.")
-        if not self.server_url:
-            raise ValueError("No FHIR server address available")
-
-    def health_check(self):
-        api_url = self._generate_api_url() + "/metadata"
-        auth = self._generate_auth()
-
-        response = {"status": None,
-                    "date": None,
-                    "name": None}
-        try:
-            # TODO remove verify false only for thesting becouse of verificaion problems with the ibm fhir server
-            r = requests.get(api_url, auth=auth, verify=False)
-            r.raise_for_status()
-            r_json = r.json()
-
-            # This is hear to make the response the same for all health check
-            if r_json["status"] == "active":
-                response["status"] = "healthy"
-                response["date"] = r_json["date"]
-        except requests.exceptions.ConnectionError as e:
-            print(e)
-            pass
-        except requests.exceptions.HTTPError as e:
-            print(e)
-            pass
-        return response
-
-    def get_number_of_resource(self):
-        api_url = self._generate_api_url() + "/Resource?_count=0"
-        auth = self._generate_auth()
-        r = requests.get(api_url, auth=auth, verify=False).json()
-        return r["total"]
-
-    def _generate_url(self, query: dict = None, query_string: str = None, return_format="json", limit=1000):
-        """
-        Generates the fhir search url to request from the server based. Either based on a previously given query string
-        or based on a dictionary containing the query definition in the query.json file.
-
-        :param query: dictionary containing the content of the query definition in the query.json file
-        :param query_string: Predefined Fhir url query string to append to base server url
-        :param return_format: the format in which the server should return the data.
-        :param limit: the max number of entries in a paginated response
-        :return: url string to perform a request against a fhir server with
-        """
-        url = self._generate_api_url() + "/"
-        if query:
-            url += build_query_string(query_dict=query)
-        elif query_string:
-            url += query_string
-        else:
-            raise ValueError("Either query dictionary or string need to be given")
-        # add formatting configuration
-        url += f"&_format={return_format}&_limit={limit}"
-
-        return url
-
-    def _generate_auth(self) -> requests.auth.AuthBase:
-        """
-        Generate authoriation for the request to be sent to server. Either based on a given bearer token or using basic
-        auth with username and password.
-
-        :return: Auth object to pass to a requests call.
-        """
-        if self.username and self.password:
-            return HTTPBasicAuth(username=self.username, password=self.password)
-        # TODO request token from id provider if configured
-        elif self.token:
-            return BearerAuth(token=self.token)
-
-    def _generate_api_url(self) -> str:
-        url = self.server_url
-        if self.server_type == "ibm":
-            url += "/fhir-server/api/v4"
-
-        elif self.server_type in ["blaze", "hapi"]:
-            url += "/fhir"
-
-        else:
-            raise ValueError(f"Unsupported FHIR server type: {self.server_type}")
-
-        return url
+import os
+
+import requests
+from requests.auth import HTTPBasicAuth
+from train_lib.clients.fhir import build_query_string
+from train_lib.clients.fhir.fhir_client import BearerAuth
+
+
+class FhirClient:
+    def __init__(
+        self,
+        server_url: str = None,
+        username: str = None,
+        password: str = None,
+        token: str = None,
+        server_type: str = None,
+        disable_auth: bool = False,
+    ):
+        """
+        Fhir client for station internal / health check / how many data points are in a fhir server
+        The code in hear is mostly copied from the train libary fhir client .
+
+        :param server_url: base url of the FHIR server to execute the query against
+        :param username: username for use in basic auth authentication against the fhir server
+        :param password: password for use in basic auth
+        :param token: token to use for authenticating against a FHIR server using a bearer token
+        :param server_type: the type of the server one of ["blaze", "hapi", "ibm"]
+        """
+        self.server_url = server_url if server_url else os.getenv("FHIR_ADDRESS")
+        self.username = username if username else os.getenv("FHIR_USER")
+        self.password = password if password else os.getenv("FHIR_PW")
+        self.token = token if token else os.getenv("FHIR_TOKEN")
+        self.server_type = server_type if server_type else os.getenv("FHIR_SERVER_TYPE")
+        self.output_format = None
+        # Check for correct initialization based on env vars or constructor parameters
+        if not (self.username and self.password) and self.token:
+            raise ValueError("Only one of username:pw or token auth can be selected")
+        if not ((self.username and self.password) or self.token) and disable_auth:
+            raise ValueError(
+                "Insufficient login information, either token or username and password need to be set."
+            )
+        if not self.server_url:
+            raise ValueError("No FHIR server address available")
+
+    def health_check(self):
+        api_url = self._generate_api_url() + "/metadata"
+        auth = self._generate_auth()
+
+        response = {"status": None, "date": None, "name": None}
+        try:
+            # TODO remove verify false only for thesting becouse of verificaion problems with the ibm fhir server
+            r = requests.get(api_url, auth=auth, verify=False)
+            r.raise_for_status()
+            r_json = r.json()
+
+            # This is hear to make the response the same for all health check
+            if r_json["status"] == "active":
+                response["status"] = "healthy"
+                response["date"] = r_json["date"]
+        except requests.exceptions.ConnectionError as e:
+            print(e)
+            pass
+        except requests.exceptions.HTTPError as e:
+            print(e)
+            pass
+        return response
+
+    def get_number_of_resource(self):
+        api_url = self._generate_api_url() + "/Resource?_count=0"
+        auth = self._generate_auth()
+        r = requests.get(api_url, auth=auth, verify=False).json()
+        return r["total"]
+
+    def _generate_url(
+        self,
+        query: dict = None,
+        query_string: str = None,
+        return_format="json",
+        limit=1000,
+    ):
+        """
+        Generates the fhir search url to request from the server based. Either based on a previously given query string
+        or based on a dictionary containing the query definition in the query.json file.
+
+        :param query: dictionary containing the content of the query definition in the query.json file
+        :param query_string: Predefined Fhir url query string to append to base server url
+        :param return_format: the format in which the server should return the data.
+        :param limit: the max number of entries in a paginated response
+        :return: url string to perform a request against a fhir server with
+        """
+        url = self._generate_api_url() + "/"
+        if query:
+            url += build_query_string(query_dict=query)
+        elif query_string:
+            url += query_string
+        else:
+            raise ValueError("Either query dictionary or string need to be given")
+        # add formatting configuration
+        url += f"&_format={return_format}&_limit={limit}"
+
+        return url
+
+    def _generate_auth(self) -> requests.auth.AuthBase:
+        """
+        Generate authoriation for the request to be sent to server. Either based on a given bearer token or using basic
+        auth with username and password.
+
+        :return: Auth object to pass to a requests call.
+        """
+        if self.username and self.password:
+            return HTTPBasicAuth(username=self.username, password=self.password)
+        # TODO request token from id provider if configured
+        elif self.token:
+            return BearerAuth(token=self.token)
+
+    def _generate_api_url(self) -> str:
+        url = self.server_url
+        if self.server_type == "ibm":
+            url += "/fhir-server/api/v4"
+
+        elif self.server_type in ["blaze", "hapi"]:
+            url += "/fhir"
+
+        else:
+            raise ValueError(f"Unsupported FHIR server type: {self.server_type}")
+
+        return url
```

### Comparing `pht-station-0.1/station/ctl/config/command.py` & `pht_station-0.2.0/station/ctl/config/command.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-import os
-import pprint
-from typing import List
-
-import click
-from rich.console import Console
-from rich.table import Table
-
-from station.ctl.config import load_config, find_config, validate_config, fix_config
-from station.ctl.config.validators import ConfigItemValidationStatus, ConfigIssueLevel, ConfigItemValidationResult
-from station.ctl.constants import Icons
-from station.ctl.util import get_template_env
-
-
-@click.command(help="Validate and/or fix a station configuration file")
-@click.option('-f', '--file', help="Path to the configuration file to validate/fix")
-@click.pass_context
-def config(ctx, file):
-    """Validate and/or fix the configuration file"""
-
-    if not file:
-        click.echo("No configuration file specified. Looking for a config file in the current directory...", nl=False)
-        station_config, file = find_config(os.getcwd())
-        click.echo(f"{Icons.CHECKMARK.value}")
-    else:
-        station_config = load_config(file)
-
-    click.echo(f"Validating configuration file...")
-    results, table = validate_config(station_config)
-    issues = [result for result in results if result.status != ConfigItemValidationStatus.VALID]
-    if issues:
-        _display_issues(issues, table)
-        click.confirm('Fix issues now?', abort=True)
-        fixed_config = fix_config(ctx.obj, station_config, results)
-        render_config(fixed_config, file)
-        click.echo(f"Fixed configuration file written to: {file}")
-
-    else:
-        click.echo('Configuration file is valid.')
-
-
-def _display_issues(issues: List[ConfigItemValidationResult], table: Table):
-    console = Console()
-    console.print(table)
-    num_warnings = len([result for result in issues if result.level == ConfigIssueLevel.WARN])
-    num_errors = len([result for result in issues if result.level == ConfigIssueLevel.ERROR])
-    warning_styled = click.style(f"{num_warnings}", fg="yellow")
-    errors_styled = click.style(f"{num_errors}", fg="red")
-    click.echo(f"Found {warning_styled} warnings and {errors_styled} errors")
-
-
-def render_config(config: dict, path: str):
-
-    env = get_template_env()
-    template = env.get_template('station_config.yml.tmpl')
-
-    pprint.pp(config)
-
-    out_config = template.render(
-        station_id=config['station_id'],
-        version=config['version'],
-        environment=config['environment'],
-        central=config['central'],
-        http=config['http'],
-        https=config['https'],
-        registry=config['registry'],
-        db=config['db'],
-        api=config['api'],
-        airflow=config['airflow'],
-        minio=config['minio'],
-    )
-
-    with open(path, 'w') as f:
-        f.write(out_config)
+import os
+
+import click
+from rich.console import Console
+
+from station.common.constants import Icons
+from station.ctl.config import find_config, fix_config, load_config
+from station.ctl.config.validate import validate_config
+from station.ctl.util import get_template_env
+
+
+@click.command(help="Validate and/or fix a station configuration file")
+@click.option("-f", "--file", help="Path to the configuration file to validate/fix")
+@click.option(
+    "--dry-run",
+    is_flag=True,
+    help="Do not write the fixed config to disk. But print it instead.",
+)
+@click.pass_context
+def settings(ctx, file, dry_run):
+    """Validate and/or fix the configuration file"""
+
+    if not file:
+        click.echo(
+            "No configuration file specified. Looking for a config file in the current directory... ",
+            nl=False,
+        )
+        station_config, file = find_config(os.getcwd())
+        click.echo(f"{Icons.CHECKMARK.value}")
+    else:
+        station_config = load_config(file)
+
+    click.echo("Validating configuration file...")
+
+    results = validate_config(station_config)
+
+    if results is not None:
+        table, results = results
+        console = Console()
+        console.print(table)
+        click.confirm("Fix issues now?", abort=True)
+        fixed_config = fix_config(ctx.obj, station_config, results)
+        render_config(fixed_config, file)
+        if not dry_run:
+            click.echo(f"Fixed configuration file written to: {file}")
+
+    else:
+        click.echo("Configuration file is valid.")
+
+
+def render_config(config: dict, path: str, dry_run: bool = False) -> str | None:
+    env = get_template_env()
+    template = env.get_template("station_config.yml.tmpl")
+    # write out the correct path to key file on host when rendering the template from docker container
+
+    # todo check and improve this
+    if config["station_config"].get("host_path"):
+        key_name = config["station_config"]["central"]["private_key"].split("/")[-1]
+        key_path = os.path.join(config["host_path"], key_name)
+        config["station_config"]["central"]["private_key"] = key_path
+
+    # todo fix this hack
+    # extract https certs from config
+    certs = config["station_config"]["https"].pop("certificate")
+
+    out_config = template.render(certificate=certs, **config["station_config"])
+
+    # print the rendered config to stdout and return it if dry_run is True
+    if dry_run:
+        click.echo(out_config)
+        return out_config
+    else:
+        with open(path, "w") as f:
+            f.write(out_config)
```

### Comparing `pht-station-0.1/station/ctl/config/fs.py` & `pht_station-0.2.0/station/ctl/config/fs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-from enum import Enum
-import os
-from typing import Tuple
-
-import yaml
-
-
-class ConfigFiles(Enum):
-    """
-    Enum for config file names
-    """
-    STATION_CONFIG = 'station_config.yml'
-    STATION_CONFIG_SHORT = 'config.yml'
-    STATION = 'station.yml'
-
-
-def load_config(file_name) -> dict:
-    """
-    Loads a config file and returns a dict with the content
-    """
-    with open(file_name, 'r') as stream:
-        try:
-            return yaml.safe_load(stream)
-        except yaml.YAMLError as exc:
-            print(exc)
-
-        except FileNotFoundError:
-            FileNotFoundError(f'Config file {file_name} not found')
-
-
-def find_config(directory) -> Tuple[dict, str]:
-    """
-    Finds a config file in a directory and returns a dict with the content
-    """
-    for file_name in ConfigFiles:
-        try:
-            return load_config(os.path.join(directory, file_name.value)), file_name.value
-        except FileNotFoundError:
-            pass
-    raise FileNotFoundError(f'No config file found in {directory}')
+import os
+from enum import Enum
+from typing import Tuple
+
+import yaml
+
+
+class ConfigFiles(Enum):
+    """
+    Enum for config file names
+    """
+
+    STATION_CONFIG = "station_config.yml"
+    STATION_CONFIG_SHORT = "config.yml"
+    STATION = "station.yml"
+
+
+def load_config(file_name) -> dict:
+    """
+    Loads a config file and returns a dict with the content
+    """
+    with open(file_name, "r") as stream:
+        try:
+            return yaml.safe_load(stream)
+        except yaml.YAMLError as exc:
+            print(exc)
+
+        except FileNotFoundError:
+            FileNotFoundError(f"Config file {file_name} not found")
+
+
+def find_config(directory) -> Tuple[dict, str]:
+    """
+    Finds a config file in a directory and returns a dict with the content
+    """
+    for file_name in ConfigFiles:
+        try:
+            return (
+                load_config(os.path.join(directory, file_name.value)),
+                file_name.value,
+            )
+        except FileNotFoundError:
+            pass
+    raise FileNotFoundError(f"No config file found in {directory}")
```

### Comparing `pht-station-0.1/station/ctl/constants.py` & `pht_station-0.2.0/station/common/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,79 @@
-from enum import Enum
-
-CERTS_REGEX = r'https\.certs\[([0-9]*)\]'
-
-
-class DockerVolumes(Enum):
-    POSTGRES = "pg_pht_station"
-
-
-class DockerNetworks(Enum):
-    STATION = "pht-station"
-
-
-class PHTImages(Enum):
-    API = "ghcr.io/pht-medic/station-api"
-    UI = "ghcr.io/pht-medic/station-ui"
-    AUTH = "ghcr.io/pht-medic/station-ui"
-    AIRFLOW = "ghcr.io/pht-medic/station-airflow"
-
-
-class ServiceImages(Enum):
-    MINIO = "minio/minio:latest"
-    POSTGRES = "postgres:13"
-    REDIS = "redislabs/rejson:latest"
-    TRAEFIK = "traefik:v2.6"
-
-
-class DefaultValues(Enum):
-    """
-    Default values for the station configuration
-    """
-    FERNET_KEY = "your_fernet_key"
-    ADMIN = "admin"
-    PRIVATE_KEY = "/path/to/private_key.pem"
-    STATION_DOMAIN = "example-station.com"
-    CERT = "example-cert.pem"
-    KEY = "example-key.pem"
-    DOMAIN = "station.localhost"
-    ROBOT_ID = "central-robot-id"
-    ROBOT_SECRET = "central-robot-secret"
-    HTTP_PORT = 80
-    HTTPS_PORT = 443
-
-
-class PHTDirectories(Enum):
-    SERVICE_DATA_DIR = "service_data"
-    SERVICE_LOG_DIR = "logs"
-    CONFIG_DIR = "configs"
-    CERTS_DIR = "certs"
-    STATION_DATA_DIR = "data"
-    SETUP_SCRIPT_DIR = "setup_scripts"
-
-
-class ServiceDirectories(Enum):
-    AUTH = "auth"
-    MINIO = "minio"
-    POSTGRES = "postgres"
-    REDIS = "redis"
-
-
-class Icons(Enum):
-    CHECKMARK = "✔"
-    CROSS = "✖"
-    WARNING = "⚠"
+from enum import Enum
+
+CERTS_REGEX = r"https\.certs\[([0-9]*)\]"
+
+
+class ApplicationEnvironment(str, Enum):
+    DEVELOPMENT = "development"
+    PRODUCTION = "production"
+
+
+class DockerVolumes(Enum):
+    POSTGRES = "pg_pht_station"
+
+
+class DockerNetworks(Enum):
+    STATION = "pht-station"
+
+
+class PHTImages(Enum):
+    API = "ghcr.io/pht-medic/station-api"
+    UI = "ghcr.io/pht-medic/station-ui"
+    AUTH = "ghcr.io/authup/authup"
+    AIRFLOW = "ghcr.io/pht-medic/airflow"
+
+
+class ServiceImages(Enum):
+    MINIO = "minio/minio:RELEASE.2022-11-11T03-44-20Z"
+    POSTGRES = "postgres:14"
+    REDIS = "redislabs/rejson:latest"
+    TRAEFIK = "traefik:v2.8"
+    BLAZE = "samply/blaze:latest"
+
+
+class DefaultValues(Enum):
+    """
+    Default values for the station configuration
+    """
+
+    FERNET_KEY = "your_fernet_key"
+    ADMIN = "admin"
+    ADMIN_PASSWORD = "password"
+    PRIVATE_KEY = "/path/to/private_key.pem"
+    STATION_DOMAIN = "example-station.com"
+    CERT = "example-cert.pem"
+    KEY = "example-key.pem"
+    DOMAIN = "station.localhost"
+    ROBOT_ID = "central-robot-id"
+    ROBOT_SECRET = "central-robot-secret"
+    HTTP_PORT = 80
+    HTTPS_PORT = 443
+
+
+class PHTDirectories(Enum):
+    SERVICE_DATA_DIR = "service_data"
+    SERVICE_LOG_DIR = "logs"
+    CONFIG_DIR = "configs"
+    CERTS_DIR = "certs"
+    STATION_DATA_DIR = "station_data"
+    SETUP_SCRIPT_DIR = "setup_scripts"
+
+
+class DataDirectories(str, Enum):
+    MODELS = "models"
+    TRAINS = "trains"
+    DATASETS = "datasets"
+    LOCAL_TRAINS = "localtrains"
+
+
+class ServiceNames(Enum):
+    AUTH = "auth"
+    POSTGRES = "postgres"
+    REDIS = "redis"
+    MINIO = "minio"
+
+
+class Icons(Enum):
+    CHECKMARK = "✓"
+    CROSS = "❌"
+    WARNING = "⚠"
```

### Comparing `pht-station-0.1/station/ctl/install/docker.py` & `pht_station-0.2.0/station/ctl/install/docker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,98 @@
-from docker import DockerClient
-import docker
-import docker.errors
-import click
-
-from station.ctl import constants
-
-
-def setup_docker():
-    client = _get_docker_client()
-    click.echo('Creating docker volumes... ', nl=False)
-    for vol in constants.DockerVolumes:
-
-        try:
-            volume = client.volumes.get(vol.value)
-        except docker.errors.NotFound:
-            try:
-                client.volumes.create(name=vol.value)
-
-            except Exception as e:
-                click.echo(f"{constants.Icons.CROSS.value} Failed to create volume: \n {e}")
-                raise e
-
-        except Exception as e:
-            click.echo(f"{constants.Icons.CROSS.value} Failed to create volume: \n {e}")
-            raise e
-
-    click.echo(constants.Icons.CHECKMARK.value)
-
-    click.echo('Creating docker networks... ', nl=False)
-    for net in constants.DockerNetworks:
-        try:
-            network = client.networks.get(net.value)
-        except docker.errors.NotFound:
-            try:
-                client.networks.create(name=net.value)
-
-
-            except Exception as e:
-                click.echo(f"{constants.Icons.CROSS.value} Failed to create network: \n {e}")
-                raise e
-        except Exception as e:
-            click.echo(f"{constants.Icons.CROSS.value} Failed to create network: \n {e}")
-            raise e
-    click.echo(constants.Icons.CHECKMARK.value)
-
-
-def download_docker_images(ctx):
-    client = _get_docker_client()
-
-    click.echo('Downloading PHT Station images:')
-    version = ctx.obj['version']
-    # download pht images
-    for image in constants.PHTImages:
-        _download_image(client, image.value, version)
-    click.echo('Downloading service images:')
-    for image in constants.ServiceImages:
-        _download_image(client, image.value)
-
-
-def _download_image(client, image: str, tag=None):
-    if not tag:
-        image_tag = image.split(':')
-        if len(image_tag) == 2:
-            image = image_tag[0]
-            tag = image_tag[1]
-
-    click.echo(f"\tDownloading {image}:{tag}... ", nl=False)
-    try:
-        client.images.pull(image, tag=tag)
-        click.echo(constants.Icons.CHECKMARK.value)
-
-    except Exception as e:
-        click.echo(f"{constants.Icons.CROSS.value} Failed to download image: \n {e}")
-
-
-def _get_docker_client() -> DockerClient:
-    try:
-        client = docker.from_env()
-    except Exception as e:
-        click.echo(f"{constants.Icons.CROSS.value} Failed to connect to docker: \n {e}")
-        raise e
-
-    return client
+import click
+
+import docker
+import docker.errors
+from docker import DockerClient
+from station.common import constants
+
+
+def setup_docker():
+    client = _get_docker_client()
+    click.echo("Creating docker volumes... ", nl=False)
+    for vol in constants.DockerVolumes:
+        try:
+            volume = client.volumes.get(vol.value)
+            if (
+                click.prompt(
+                    f"\nVolume {vol.value} already exists. Do you want to reset it? [y/N]",
+                    default="N",
+                )
+                == "y"
+            ):
+                volume.remove()
+                client.volumes.create(name=vol.value)
+                click.echo(f"Volume was reset {vol.value}")
+
+        except docker.errors.NotFound:
+            try:
+                client.volumes.create(name=vol.value)
+                click.echo(constants.Icons.CHECKMARK.value)
+
+            except Exception as e:
+                click.echo(
+                    f"{constants.Icons.CROSS.value} Failed to create volume: \n {e}"
+                )
+                raise e
+
+        except Exception as e:
+            click.echo(f"{constants.Icons.CROSS.value} Failed to create volume: \n {e}")
+            raise e
+
+    click.echo("Creating docker networks... ", nl=False)
+    for net in constants.DockerNetworks:
+        try:
+            client.networks.get(net.value)
+        except docker.errors.NotFound:
+            try:
+                client.networks.create(name=net.value)
+
+            except Exception as e:
+                click.echo(
+                    f"{constants.Icons.CROSS.value} Failed to create network: \n {e}"
+                )
+                raise e
+        except Exception as e:
+            click.echo(
+                f"{constants.Icons.CROSS.value} Failed to create network: \n {e}"
+            )
+            raise e
+    click.echo(constants.Icons.CHECKMARK.value)
+
+
+def download_docker_images(ctx):
+    client = _get_docker_client()
+
+    click.echo("Downloading PHT Station images:")
+    version = ctx.obj["version"]
+    # download pht images
+    for image in constants.PHTImages:
+        _download_image(client, image.value, version)
+    click.echo("Downloading service images:")
+    for image in constants.ServiceImages:
+        _download_image(client, image.value)
+
+
+def _download_image(client, image: str, tag=None):
+    if not tag:
+        image_tag = image.split(":")
+        if len(image_tag) == 2:
+            image = image_tag[0]
+            tag = image_tag[1]
+
+    click.echo(f"\tDownloading {image}:{tag}... ", nl=False)
+    try:
+        client.images.pull(image, tag=tag)
+        click.echo(constants.Icons.CHECKMARK.value)
+
+    except Exception as e:
+        click.echo(f"{constants.Icons.CROSS.value} Failed to download image: \n {e}")
+
+
+def _get_docker_client() -> DockerClient:
+    try:
+        client = docker.from_env()
+    except Exception as e:
+        click.echo(f"{constants.Icons.CROSS.value} Failed to connect to docker: \n {e}")
+        raise e
+
+    return client
```

### Comparing `pht-station-0.1/station/ctl/tests/test_install.py` & `pht_station-0.2.0/station/ctl/tests/test_install.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,98 @@
-import os
-
-import pytest
-from dotenv import load_dotenv, find_dotenv
-import yaml
-
-from station.clients.central.central_client import CentralApiClient
-from station.ctl.install.fs import create_pht_dirs
-
-from station.ctl.util import get_template_env
-from station.ctl.install import templates
-from station.ctl.constants import PHTDirectories
-from station.ctl.install import docker
-from station.ctl.install import certs
-
-
-@pytest.fixture
-def central_client():
-    load_dotenv(find_dotenv())
-    url = os.getenv("CENTRAL_API_URL")
-    client_id = os.getenv("STATION_ROBOT_ID")
-    client_secret = os.getenv("STATION_ROBOT_SECRET")
-    return CentralApiClient(url, client_id, client_secret)
-
-
-def test_ensure_directory_structure(tmp_path):
-    p = tmp_path / "station"
-    create_pht_dirs(p)
-    for dir in PHTDirectories:
-        assert p.joinpath(dir.value).exists()
-
-
-def test_get_template_env():
-    env = get_template_env()
-    assert env
-
-    template = env.get_template("init.sql.tmpl")
-    assert template
-
-
-def test_render_init_sql():
-    sql = templates.render_init_sql("test_db_user")
-    assert sql
-    print(sql)
-    lines = sql.splitlines()
-    assert len(lines) == 4
-    assert lines[-1].endswith("test_db_user;")
-    assert lines[-2].endswith("test_db_user;")
-
-
-def test_render_traefik_configs():
-    traefik_config, router_config = templates.render_traefik_configs(
-        http_port=80,
-        https_port=443,
-        domain="test.com",
-        https_enabled=True,
-        certs=[{"cert": "test", "key": "test"}],
-    )
-    assert traefik_config
-    assert router_config
-
-    print(traefik_config)
-    print(router_config)
-
-    traefik_dict = yaml.safe_load(traefik_config)
-    router_dict = yaml.safe_load(router_config)
-    print(traefik_dict)
-    print(router_dict)
-
-    assert traefik_dict["entryPoints"]["http"]["address"] == ":80"
-    assert traefik_dict["entryPoints"]["https"]["address"] == ":443"
-
-    assert router_dict["http"]["routers"]["traefik"]["tls"]["domains"][0]["main"] == "test.com"
-    assert router_dict["tls"]["certificates"][0]["certFile"] == "test"
-    assert router_dict["tls"]["certificates"][0]["keyFile"] == "test"
-
-
-def test_setup_volumes():
-    docker.setup_docker()
-
-
-def test_generate_certs(tmp_path):
-    key_path = tmp_path / "key.pem"
-    cert_path = tmp_path / "cert.pem"
-    certs.generate_certificates("test.com", str(key_path), str(cert_path))
-    assert key_path.exists()
-    assert key_path.read_bytes()
-    assert cert_path.exists()
-    assert cert_path.read_bytes()
-
-
+import os
+from collections import namedtuple
+
+import pytest
+import yaml
+from dotenv import find_dotenv, load_dotenv
+
+from station.common.clients.central.central_client import CentralApiClient
+from station.common.constants import PHTDirectories
+from station.ctl.install import certs, docker, templates
+from station.ctl.install.command import _setup_auth_server
+from station.ctl.install.fs import create_pht_dirs
+from station.ctl.util import get_template_env
+
+
+@pytest.fixture
+def central_client():
+    load_dotenv(find_dotenv())
+    url = os.getenv("CENTRAL_API_URL")
+    client_id = os.getenv("STATION_ROBOT_ID")
+    client_secret = os.getenv("STATION_ROBOT_SECRET")
+    return CentralApiClient(url, client_id, client_secret)
+
+
+def test_ensure_directory_structure(tmp_path):
+    p = tmp_path / "station"
+    create_pht_dirs(p)
+    for dir in PHTDirectories:
+        assert p.joinpath(dir.value).exists()
+
+
+def test_get_template_env():
+    env = get_template_env()
+    assert env
+
+
+def test_setup_auth():
+    ctx = {
+        "obj": {
+            "version": "latest",
+        }
+    }
+    ctx = namedtuple("Struct", ctx.keys())(*ctx.values())
+    _setup_auth_server(ctx)
+
+
+def test_render_init_sql():
+    sql = templates.render_init_sql("test_db_user")
+    assert sql
+    print(sql)
+    lines = sql.splitlines()
+    assert len(lines) == 4
+    assert lines[-1].endswith("test_db_user;")
+    assert lines[-2].endswith("test_db_user;")
+
+
+def test_render_traefik_configs():
+    traefik_config, router_config = templates.render_traefik_configs(
+        http_port=80,
+        https_port=443,
+        domain="test.com",
+        https_enabled=True,
+        certs=[{"cert": "test", "key": "test"}],
+    )
+    assert traefik_config
+    assert router_config
+
+    print(traefik_config)
+    print(router_config)
+
+    traefik_dict = yaml.safe_load(traefik_config)
+    router_dict = yaml.safe_load(router_config)
+    print(traefik_dict)
+    print(router_dict)
+
+    assert traefik_dict["entryPoints"]["http"]["address"] == ":80"
+    assert traefik_dict["entryPoints"]["https"]["address"] == ":443"
+
+    assert (
+        router_dict["http"]["routers"]["traefik"]["tls"]["domains"][0]["main"]
+        == "test.com"
+    )
+    assert router_dict["tls"]["certificates"][0]["certFile"] == "test"
+    assert router_dict["tls"]["certificates"][0]["keyFile"] == "test"
+
+
+def test_setup_volumes():
+    docker.setup_docker()
+
+
+def test_generate_certs(tmp_path):
+    key_path = tmp_path / "key.pem"
+    cert_path = tmp_path / "cert.pem"
+    certs.generate_certificates("test.com", str(key_path), str(cert_path))
+    assert key_path.exists()
+    assert key_path.read_bytes()
+    assert cert_path.exists()
+    assert cert_path.read_bytes()
```

### Comparing `pht-station-0.1/station/ctl/tests/test_validators.py` & `pht_station-0.2.0/station/ctl/tests/test_validators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,95 @@
-from cryptography.fernet import Fernet
-
-from station.ctl.config import validators
-
-
-def test_validate_db_config():
-    # invalid password
-    db_config = {
-        "admin_user": "admin",
-        "admin_password": "admin"
-    }
-
-    result = validators.validate_db_config(db_config)
-    issues = [issue for issue in result if issue.status != validators.ConfigItemValidationStatus.VALID]
-    assert len(issues) == 1
-    assert issues[0].display_field == "db.admin_password"
-
-    # invalid username and password
-    db_config = {
-        "admin_user": "",
-        "admin_password": "admin"
-    }
-
-    result = validators.validate_db_config(db_config)
-    issues = [issue for issue in result if issue.status != validators.ConfigItemValidationStatus.VALID]
-    assert len(issues) == 2
-
-    # valid config
-    db_config = {
-        "admin_user": "admin",
-        "admin_password": "valid_password"
-    }
-
-    result = validators.validate_db_config(db_config)
-    issues = [issue for issue in result if issue.status != validators.ConfigItemValidationStatus.VALID]
-    assert len(issues) == 0
-
-    # no config given
-    db_config = None
-
-    result = validators.validate_db_config(db_config)
-    issues = [issue for issue in result if issue.status != validators.ConfigItemValidationStatus.VALID]
-    assert len(issues) == 1
-
-
-def test_validate_api_config():
-    api_config = {
-        "fernet_key": "your_fernet_key"
-    }
-
-    result = validators.validate_api_config(api_config)
-    issues = [issue for issue in result if issue.status != validators.ConfigItemValidationStatus.VALID]
-    assert len(issues) == 1
-    assert issues[0].display_field == "api.fernet_key"
-
-    api_config = {
-        "fernet_key": "dsa"
-    }
-
-    result = validators.validate_api_config(api_config)
-    issues = [issue for issue in result if issue.status != validators.ConfigItemValidationStatus.VALID]
-    assert len(issues) == 1
-    assert issues[0].display_field == "api.fernet_key"
-
-    api_config = {
-        "fernet_key": Fernet.generate_key().decode()
-    }
-    result = validators.validate_api_config(api_config)
-    issues = [issue for issue in result if issue.status != validators.ConfigItemValidationStatus.VALID]
-    assert len(issues) == 0
-
-
-def test_validate_minio_config():
-    pass
-
-
-def test_validate_airflow_config():
-    pass
-
-def test_validate_central_config():
-    pass
+from cryptography.fernet import Fernet
+
+from station.ctl.config import validators
+
+
+def test_validate_db_config():
+    # invalid password
+    db_config = {"admin_user": "admin", "admin_password": "admin"}
+
+    result = validators.validate_db_config(db_config)
+    issues = [
+        issue
+        for issue in result
+        if issue.status != validators.ConfigItemValidationStatus.VALID
+    ]
+    assert len(issues) == 1
+    assert issues[0].display_field == "db.admin_password"
+
+    # invalid username and password
+    db_config = {"admin_user": "", "admin_password": "admin"}
+
+    result = validators.validate_db_config(db_config)
+    issues = [
+        issue
+        for issue in result
+        if issue.status != validators.ConfigItemValidationStatus.VALID
+    ]
+    assert len(issues) == 2
+
+    # valid config
+    db_config = {"admin_user": "admin", "admin_password": "valid_password"}
+
+    result = validators.validate_db_config(db_config)
+    issues = [
+        issue
+        for issue in result
+        if issue.status != validators.ConfigItemValidationStatus.VALID
+    ]
+    assert len(issues) == 0
+
+    # no config given
+    db_config = None
+
+    result = validators.validate_db_config(db_config)
+    issues = [
+        issue
+        for issue in result
+        if issue.status != validators.ConfigItemValidationStatus.VALID
+    ]
+    assert len(issues) == 1
+
+
+def test_validate_api_config():
+    api_config = {"fernet_key": "your_fernet_key"}
+
+    result = validators.validate_api_config(api_config)
+    issues = [
+        issue
+        for issue in result
+        if issue.status != validators.ConfigItemValidationStatus.VALID
+    ]
+    assert len(issues) == 1
+    assert issues[0].display_field == "api.fernet_key"
+
+    api_config = {"fernet_key": "dsa"}
+
+    result = validators.validate_api_config(api_config)
+    issues = [
+        issue
+        for issue in result
+        if issue.status != validators.ConfigItemValidationStatus.VALID
+    ]
+    assert len(issues) == 1
+    assert issues[0].display_field == "api.fernet_key"
+
+    api_config = {"fernet_key": Fernet.generate_key().decode()}
+    result = validators.validate_api_config(api_config)
+    issues = [
+        issue
+        for issue in result
+        if issue.status != validators.ConfigItemValidationStatus.VALID
+    ]
+    assert len(issues) == 0
+
+
+def test_validate_minio_config():
+    pass
+
+
+def test_validate_airflow_config():
+    pass
+
+
+def test_validate_central_config():
+    pass
```

### Comparing `pht-station-0.1/station/tests/test_api_airflow.py` & `pht_station-0.2.0/station/app/tests/test_api_airflow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,120 @@
-import pytest
-import os
-from fastapi.testclient import TestClient
-
-from station.app.main import app
-from station.app.api.dependencies import get_db
-
-from .test_db import override_get_db
-
-app.dependency_overrides[get_db] = override_get_db
-
-client = TestClient(app)
-
-@pytest.fixture()
-def train_id():
-    return "airflow_test"
-
-
-def test_run(train_id):
-    if os.getenv("ENVIRONMENT") == "testing":
-        response = client.post("/api/trains/docker",
-                               json={"train_id": train_id,
-                                     "config": {"name": "testconfig",
-                                                "airflow_config": {
-                                                    "repository": f"dev-harbor.grafm.de/station_1/{train_id}",
-                                                    "tag": "latest"
-                                                }}})
-        if response.status_code == 200:
-
-            run_pht_train = client.post("/api/airflow/run_pht_train/run",
-                                        json={"train_id": train_id})
-            response_pht_train = run_pht_train.json()
-
-            assert run_pht_train.status_code == 200
-            assert response_pht_train["dag_id"] == "run_pht_train"
-            assert response_pht_train["train_id"] == "airflow_test"
-            assert response_pht_train["start_date"]
-
-            execution = client.get(f"/api/trains/docker/{train_id}/executions")
-            assert execution.json()[-1]["airflow_dag_run"] == response_pht_train["run_id"]
-
-
-def test_run_fails(train_id):
-    if os.getenv("ENVIRONMENT") == "testing":
-        run_wrong_dag = client.post("/api/airflow/dag_not_there/run",
-                                    json={"train_id": train_id})
-        assert run_wrong_dag.status_code == 404, run_wrong_dag.text
-
-
-def test_get_airflow_run_information(train_id):
-    if os.getenv("ENVIRONMENT") == "testing":
-        response = client.get(f"/api/trains/docker/{train_id}/executions")
-        executions = response.json()
-        assert len(executions) > 0
-        run_id = executions[-1]["airflow_dag_run"]
-
-        run_info_response = client.get(f"/api/airflow/logs/run_pht_train/{run_id}")
-        print(run_info_response.json())
-        assert run_info_response.status_code == 200
-
-
-def test_get_airflow_run_information_fails():
-    if os.getenv("ENVIRONMENT") == "testing":
-        with pytest.raises(Exception):
-            run_id_fail = client.get(f"/api/airflow/logs/run_pht_train/no_run_id")
-            assert run_id_fail.status_code == 404
-
-        with pytest.raises(Exception):
-            dag_id_fail = client.get(f"/api/airflow/logs/dag_not_there/no_run_id")
-            assert dag_id_fail.status_code == 404
-
-
-def test_get_airflow_task_log(train_id):
-    if os.getenv("ENVIRONMENT") == "testing":
-        response = client.get(f"/api/trains/docker/{train_id}/executions")
-        executions = response.json()
-        assert len(executions) > 0
-        run_id = executions[-1]["airflow_dag_run"]
-
-        run_info_response = client.get(f"/api/airflow/logs/run_pht_train/{run_id}")
-        tasklist = run_info_response.json()["tasklist"]
-        for task in tasklist["task_instances"]:
-            task_id = task["task_id"]
-            task_info = client.get(f"/api/airflow/logs/run_pht_train/{run_id}/{task_id}")
-            assert task_info.json()["run_info"]
-            assert task_info.status_code == 200
-
-        # with given task try number
-        for task in tasklist["task_instances"]:
-            task_id = task["task_id"]
-            task_info = client.get(f"/api/airflow/logs/run_pht_train/{run_id}/{task_id}/?task_try_number=0")
-            assert task_info.json()["run_info"]
-            assert task_info.status_code == 200
-
-
-def test_get_airflow_task_log_fails(train_id):
-    if os.getenv("ENVIRONMENT") == "testing":
-        response = client.get(f"/api/trains/docker/{train_id}/executions")
-        executions = response.json()
-        assert len(executions) > 0
-        run_id = executions[-1]["airflow_dag_run"]
-
-        task_info = client.get(f"/api/airflow/logs/run_pht_train/{run_id}/no_task_id")
-        assert task_info.status_code == 404
+import os
+
+import pytest
+from fastapi.testclient import TestClient
+
+from station.app.api.dependencies import get_db
+from station.app.main import app
+
+from .test_db import override_get_db
+
+app.dependency_overrides[get_db] = override_get_db
+
+client = TestClient(app)
+
+
+@pytest.fixture()
+def train_id():
+    return "airflow_test"
+
+
+def test_run(train_id):
+    if os.getenv("ENVIRONMENT") == "testing":
+        response = client.post(
+            "/api/trains/docker",
+            json={
+                "train_id": train_id,
+                "config": {
+                    "name": "testconfig",
+                    "airflow_config": {
+                        "repository": f"dev-harbor.grafm.de/station_1/{train_id}",
+                        "tag": "latest",
+                    },
+                },
+            },
+        )
+        if response.status_code == 200:
+
+            run_pht_train = client.post(
+                "/api/airflow/run_pht_train/run", json={"train_id": train_id}
+            )
+            response_pht_train = run_pht_train.json()
+
+            assert run_pht_train.status_code == 200
+            assert response_pht_train["dag_id"] == "run_pht_train"
+            assert response_pht_train["train_id"] == "airflow_test"
+            assert response_pht_train["start_date"]
+
+            execution = client.get(f"/api/trains/docker/{train_id}/executions")
+            assert (
+                execution.json()[-1]["airflow_dag_run"] == response_pht_train["run_id"]
+            )
+
+
+def test_run_fails(train_id):
+    if os.getenv("ENVIRONMENT") == "testing":
+        run_wrong_dag = client.post(
+            "/api/airflow/dag_not_there/run", json={"train_id": train_id}
+        )
+        assert run_wrong_dag.status_code == 404, run_wrong_dag.text
+
+
+def test_get_airflow_run_information(train_id):
+    if os.getenv("ENVIRONMENT") == "testing":
+        response = client.get(f"/api/trains/docker/{train_id}/executions")
+        executions = response.json()
+        assert len(executions) > 0
+        run_id = executions[-1]["airflow_dag_run"]
+
+        run_info_response = client.get(f"/api/airflow/logs/run_pht_train/{run_id}")
+        print(run_info_response.json())
+        assert run_info_response.status_code == 200
+
+
+def test_get_airflow_run_information_fails():
+    if os.getenv("ENVIRONMENT") == "testing":
+        with pytest.raises(Exception):
+            run_id_fail = client.get("/api/airflow/logs/run_pht_train/no_run_id")
+            assert run_id_fail.status_code == 404
+
+        with pytest.raises(Exception):
+            dag_id_fail = client.get("/api/airflow/logs/dag_not_there/no_run_id")
+            assert dag_id_fail.status_code == 404
+
+
+def test_get_airflow_task_log(train_id):
+    if os.getenv("ENVIRONMENT") == "testing":
+        response = client.get(f"/api/trains/docker/{train_id}/executions")
+        executions = response.json()
+        assert len(executions) > 0
+        run_id = executions[-1]["airflow_dag_run"]
+
+        run_info_response = client.get(f"/api/airflow/logs/run_pht_train/{run_id}")
+        tasklist = run_info_response.json()["tasklist"]
+        for task in tasklist["task_instances"]:
+            task_id = task["task_id"]
+            task_info = client.get(
+                f"/api/airflow/logs/run_pht_train/{run_id}/{task_id}"
+            )
+            assert task_info.json()["run_info"]
+            assert task_info.status_code == 200
+
+        # with given task try number
+        for task in tasklist["task_instances"]:
+            task_id = task["task_id"]
+            task_info = client.get(
+                f"/api/airflow/logs/run_pht_train/{run_id}/{task_id}/?task_try_number=0"
+            )
+            assert task_info.json()["run_info"]
+            assert task_info.status_code == 200
+
+
+def test_get_airflow_task_log_fails(train_id):
+    if os.getenv("ENVIRONMENT") == "testing":
+        response = client.get(f"/api/trains/docker/{train_id}/executions")
+        executions = response.json()
+        assert len(executions) > 0
+        run_id = executions[-1]["airflow_dag_run"]
+
+        task_info = client.get(f"/api/airflow/logs/run_pht_train/{run_id}/no_task_id")
+        assert task_info.status_code == 404
```

### Comparing `pht-station-0.1/station/tests/test_api_datasets.py` & `pht_station-0.2.0/station/app/tests/test_api_datasets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-from fastapi.testclient import TestClient
-
-
-from station.app.main import app
-from station.app.api.dependencies import get_db
-
-from .test_db import override_get_db
-
-app.dependency_overrides[get_db] = override_get_db
-
-client = TestClient(app)
-
-
-def test_data_set_create():
-    response = client.post("/api/datasets", json={
-        "name": "test data set",
-        "data_type": "tabular",
-        "storage_type": "fhir"
-
-    })
-
-    assert response.status_code == 200, response.text
-
-    data = response.json()
-    dataset_id = data["id"]
-    assert dataset_id
-
-
-def test_data_set_get():
-    response = client.get(f"/api/datasets/{1}")
-    assert response.status_code == 200, response.text
-
-    data = response.json()
-    assert data["name"] == "test data set"
-
-
-def test_get_all_data_sets():
-    response = client.get("/api/datasets")
-    assert response.status_code == 200, response.text
-    data = response.json()
-
-    assert len(data) >= 1
+from fastapi.testclient import TestClient
+
+from station.app.api.dependencies import get_db
+from station.app.main import app
+
+from .test_db import override_get_db
+
+app.dependency_overrides[get_db] = override_get_db
+
+client = TestClient(app)
+
+
+def test_data_set_create():
+    response = client.post(
+        "/api/datasets",
+        json={"name": "test data set", "data_type": "tabular", "storage_type": "fhir"},
+    )
+
+    assert response.status_code == 200, response.text
+
+    data = response.json()
+    dataset_id = data["id"]
+    assert dataset_id
+
+
+def test_data_set_get():
+    response = client.get(f"/api/datasets/{1}")
+    assert response.status_code == 200, response.text
+
+    data = response.json()
+    assert data["name"] == "test data set"
+
+
+def test_get_all_data_sets():
+    response = client.get("/api/datasets")
+    assert response.status_code == 200, response.text
+    data = response.json()
+
+    assert len(data) >= 1
```

### Comparing `pht-station-0.1/station/tests/test_api_docker_trains.py` & `pht_station-0.2.0/station/app/tests/test_api_docker_trains.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,381 +1,377 @@
-import pytest
-import os
-from fastapi.testclient import TestClient
-
-from station.app.main import app
-from station.app.api.dependencies import get_db
-from dotenv import load_dotenv, find_dotenv
-
-from .test_db import override_get_db
-
-app.dependency_overrides[get_db] = override_get_db
-
-client = TestClient(app)
-
-
-@pytest.fixture
-def train_id():
-    load_dotenv(find_dotenv())
-    return "testTrain"
-
-
-@pytest.fixture(scope='session')
-def docker_train_config():
-    config = {
-        "name": "test_config",
-        "airflow_config": {
-            "env": [{
-                "key": "FHIR_ADDRESS",
-                "value": "test_address"
-            }
-            ],
-            "volumes": [{
-                "host_path": "path/on/host",
-                "container_path": "path/in/container",
-                "mode": "ro"
-            }],
-            "repository": "example/repository",
-            "tag": "latest"
-        },
-
-        "auto_execute": True
-    }
-
-    return config
-
-
-@pytest.fixture(scope='session')
-def config_id(docker_train_config):
-    response = client.post(
-        "/api/trains/docker/config",
-        json=docker_train_config
-    )
-    return response.json()["id"]
-
-
-@pytest.fixture(scope='session', autouse=True)
-def train_list_length():
-    response = client.get("/api/trains/docker")
-    length = len(response.json())
-    return length
-
-
-def test_config_create(docker_train_config, config_id):
-    response = client.get(f"/api/trains/docker/config/{config_id}")
-    assert response.status_code == 200, response.text
-
-    assert response.json()["name"] == docker_train_config["name"]
-    assert response.json()["auto_execute"]
-
-
-def test_docker_train_create(train_id):
-    response = client.get("/api/trains/docker/configs/all")
-    print(response.json())
-    response = client.post("/api/trains/docker", json={
-        "train_id": train_id
-
-    })
-
-    assert response.status_code == 200, response.text
-
-    json_response = response.json()
-    assert json_response["train_id"] == train_id
-    print(json_response)
-    assert json_response["state"]["num_executions"] == 0
-    assert json_response["state"]["status"] == "inactive"
-
-
-def test_docker_train_create_fails(train_id):
-    response = client.post(
-        "/api/trains/docker",
-        json={
-            "train_id": train_id
-
-        }
-    )
-
-    assert response.status_code == 400, response.text
-
-
-def test_get_train_by_id(train_id):
-    response = client.get(f"/api/trains/docker/{train_id}")
-    assert response.status_code == 200, response.text
-
-
-def test_get_train_by_id_fails():
-    response = client.get("/api/trains/docker/notthere")
-    assert response.status_code == 404, response.text
-
-
-def test_list_docker_trains(train_list_length):
-    response = client.get("/api/trains/docker")
-
-    assert response.status_code == 200, response.text
-    print(response.json())
-
-    assert len(response.json()) == train_list_length+1
-
-
-def test_docker_train_config_create_fails(docker_train_config):
-    response = client.post(
-        "/api/trains/docker/config",
-        json=docker_train_config
-    )
-    assert response.status_code == 400
-
-
-def test_get_docker_train_configs():
-    response = client.get("/api/trains/docker/configs/all")
-    assert response.status_code == 200, response.text
-    assert len(response.json()) >= 1
-
-
-def test_get_docker_train_config_by_id(config_id):
-    response = client.get("/api/trains/docker/config/1")
-    assert response.status_code == 200, response.text
-
-
-def test_get_docker_train_config_by_id_fails():
-    response = client.get("/api/trains/docker/config/234")
-    assert response.status_code == 404, response.text
-
-
-def test_update_docker_train_config(docker_train_config, config_id):
-    docker_train_config["name"] = "updated name"
-    response = client.put(f"/api/trains/docker/config/{config_id}",
-                          json=docker_train_config)
-
-    assert response.status_code == 200, response.text
-    response = client.get(f"/api/trains/docker/config/{config_id}")
-
-    assert response.json()["name"] == "updated name"
-
-
-def test_update_docker_train_config_fails(docker_train_config):
-    docker_train_config["name"] = "updated name"
-    response = client.put("/api/trains/docker/config/234",
-                          json=docker_train_config)
-    assert response.status_code == 404, response.text
-
-
-def test_assign_docker_train_config(train_id, config_id):
-    response = client.post(f"/api/trains/docker/{train_id}/config/{config_id}")
-    assert response.status_code == 200, response.text
-    response = client.get(f"/api/trains/docker/{train_id}")
-
-    assert response.json()["config_id"] == config_id
-
-    # test non existing config error
-    response = client.post(f"/api/trains/docker/{train_id}/config/321")
-
-    assert response.status_code == 404
-
-    # test non existing train error
-
-    response = client.post("/api/trains/docker/no_train/config/1")
-    assert response.status_code == 404
-
-
-def test_get_config_for_train(train_id):
-    response = client.get(f"/api/trains/docker/{train_id}/config")
-    assert response.status_code == 200, response.text
-    assert len(response.json()["trains"]) == 1
-    print(response.json())
-
-    new_train_id = "no_config_train"
-    response = client.post(
-        "/api/trains/docker",
-        json={
-            "train_id": new_train_id
-
-        }
-    )
-    assert response.status_code == 200
-    response = client.get(f"/api/trains/docker/{new_train_id}/config")
-
-    assert response.status_code == 404
-
-
-def test_create_train_with_config(docker_train_config, config_id):
-    # assign existing config
-    response = client.post(
-        "/api/trains/docker",
-        json={
-            "train_id": "with_existing_config",
-            "config": config_id
-        }
-    )
-    assert response.status_code == 200, response.text
-    config_response = client.get(f"/api/trains/docker/with_existing_config/config")
-    assert config_response.json()["name"] == "updated name"
-    assert len(config_response.json()["trains"]) == 2
-
-    # fails with unknown config id
-    response = client.post(
-        "/api/trains/docker",
-        json={
-            "train_id": "config does not exist",
-            "config": 3213
-        }
-    )
-    assert response.status_code == 404, response.text
-
-    new_config = {
-        "name": "new config",
-        "airflow_config": {
-            "env": [{
-                "key": "FHIR_ADDRESS",
-                "value": "test_address"
-            }
-            ],
-            "volumes": [{
-                "host_path": "path/on/host",
-                "container_path": "path/in/container",
-                "mode": "ro"
-            }]
-
-        },
-
-        "auto_execute": False
-    }
-
-    response = client.post(
-        "/api/trains/docker",
-        json={
-            "train_id": "with_new_config",
-            "name": "train with new config",
-            "config": new_config
-        }
-    )
-    assert response.status_code == 200
-    print(response.json())
-
-    config_response = client.get(f"/api/trains/docker/with_new_config/config")
-    assert config_response.json()["name"] == "new config"
-
-
-def test_get_train_state():
-    train_id = "test_train_state"
-    response = client.post(
-        "/api/trains/docker",
-        json={
-            "train_id": train_id,
-        }
-    )
-    assert response.status_code == 200, response.text
-
-    response = client.get(f"/api/trains/docker/{train_id}/state")
-    assert response.status_code == 200, response.text
-    assert response.json()["status"] == "inactive"
-
-
-def test_update_train_state(train_id):
-    response = client.put(f"/api/trains/docker/{train_id}/state", json={"status": "active", "num_executions": 1})
-    assert response.status_code == 200, response.text
-    assert response.json()["status"] == "active"
-    assert response.json()["num_executions"] == 1
-
-
-def test_synchronize_database():
-    if os.getenv("ENVIRONMENT") == "testing":
-        response_nostation = client.get("/api/trains/docker/sync")
-        assert response_nostation.status_code == 200, response_nostation.text
-
-        response = client.get("/api/trains/docker/sync/?station_id=1")
-        if os.getenv("STATION_ID") == 1:
-            assert len(response.json()) == 0
-        assert response.status_code == 200, response.text
-
-
-def test_synchronize_database_fails():
-    if os.getenv("ENVIRONMENT") == "testing":
-        response = client.get("/api/trains/docker/sync/?station_id=123")
-        assert response.status_code == 404, response.text
-
-
-def test_run_docker_train(train_id, docker_train_config, config_id):
-    if os.getenv("ENVIRONMENT") == "testing":
-        old_state = client.get(f"/api/trains/docker/{train_id}/state")
-
-        # run with given config id
-        response = client.post(f"/api/trains/docker/{train_id}/run", json={"config_id": 1})
-        assert response.json()["airflow_dag_run"]
-        assert response.json()["config"] == 1
-        assert response.status_code == 200, response.text
-
-        state_response = client.get(f"/api/trains/docker/{train_id}/state")
-        assert old_state.json() != state_response.json()
-        assert old_state.json()["num_executions"] + 1 == state_response.json()["num_executions"]
-
-        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
-        assert execution_response.json()[-1]["airflow_dag_run"] == response.json()["airflow_dag_run"]
-
-        # run with default config
-        response = client.post(f"/api/trains/docker/{train_id}/run",
-                               json={"config_id": "default"})
-        assert response.json()["airflow_dag_run"]
-        assert response.json()["config"] is None
-        assert response.status_code == 200, response.text
-
-        state_response = client.get(f"/api/trains/docker/{train_id}/state")
-        assert old_state.json()["num_executions"] + 2 == state_response.json()["num_executions"]
-
-        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
-        assert execution_response.json()[-1]["airflow_dag_run"] == response.json()["airflow_dag_run"]
-
-        # run with config assigned to train
-        response = client.post(f"/api/trains/docker/{train_id}/run")
-        assert response.json()["airflow_dag_run"]
-        assert response.json()["config"] == config_id
-        assert response.status_code == 200, response.text
-
-        state_response = client.get(f"/api/trains/docker/{train_id}/state")
-        assert old_state.json()["num_executions"] + 3 == state_response.json()["num_executions"]
-
-        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
-        assert execution_response.json()[-1]["airflow_dag_run"] == response.json()["airflow_dag_run"]
-
-
-def test_run_docker_train_fails(train_id, docker_train_config, config_id):
-    old_state = client.get(f"/api/trains/docker/{train_id}/state")
-    old_executions = client.get(f"/api/trains/docker/{train_id}/executions")
-
-    if os.getenv("ENVIRONMENT") == "testing":
-
-        # no config with id given
-        response = client.post(f"/api/trains/docker/{train_id}/run", json={"config_id": 3213})
-        state_response = client.get(f"/api/trains/docker/{train_id}/state")
-        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
-        assert old_state.json() == state_response.json()
-        assert old_executions.json() == execution_response.json()
-        assert response.status_code == 400, response.text
-
-        # no tag and no repository given
-        specific_id = config_id+1
-        response = client.post(f"/api/trains/docker/{train_id}/run", json={"config_id": specific_id})
-        response_conf = client.get(f"/api/trains/docker/config/{specific_id}")
-        print(response_conf.json())
-        state_response = client.get(f"/api/trains/docker/{train_id}/state")
-        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
-        assert old_state.json() == state_response.json()
-        assert old_executions.json() == execution_response.json()
-        assert response.status_code == 400, response.text
-
-        # train not defined
-        response = client.post(f"/api/trains/docker/no_train/run", json={"config_id": 1})
-        assert response.status_code == 404, response.text
-
-    else:
-        response = client.post(f"/api/trains/docker/{train_id}/run", json={"config_id": "default"})
-        state_response = client.get(f"/api/trains/docker/{train_id}/state")
-        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
-        assert old_state.json() == state_response.json()
-        assert old_executions.json() == execution_response.json()
-        assert response.status_code == 503, response.text
-
-        response = client.post(f"/api/trains/docker/{train_id}/run")
-        state_response = client.get(f"/api/trains/docker/{train_id}/state")
-        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
-        assert old_state.json() == state_response.json()
-        assert old_executions.json() == execution_response.json()
-        assert response.status_code == 503, response.text
+import os
+
+import pytest
+from dotenv import find_dotenv, load_dotenv
+from fastapi.testclient import TestClient
+
+from station.app.api.dependencies import get_db
+from station.app.main import app
+
+from .test_db import override_get_db
+
+app.dependency_overrides[get_db] = override_get_db
+
+client = TestClient(app)
+
+
+@pytest.fixture
+def train_id():
+    load_dotenv(find_dotenv())
+    return "testTrain"
+
+
+@pytest.fixture(scope="session")
+def docker_train_config():
+    config = {
+        "name": "test_config",
+        "airflow_config": {
+            "env": [{"key": "FHIR_ADDRESS", "value": "test_address"}],
+            "volumes": [
+                {
+                    "host_path": "path/on/host",
+                    "container_path": "path/in/container",
+                    "mode": "ro",
+                }
+            ],
+            "repository": "example/repository",
+            "tag": "latest",
+        },
+        "auto_execute": True,
+    }
+
+    return config
+
+
+@pytest.fixture(scope="session")
+def config_id(docker_train_config):
+    response = client.post("/api/trains/docker/config", json=docker_train_config)
+    return response.json()["id"]
+
+
+@pytest.fixture(scope="session", autouse=True)
+def train_list_length():
+    response = client.get("/api/trains/docker")
+    length = len(response.json())
+    return length
+
+
+def test_config_create(docker_train_config, config_id):
+    response = client.get(f"/api/trains/docker/config/{config_id}")
+    assert response.status_code == 200, response.text
+
+    assert response.json()["name"] == docker_train_config["name"]
+    assert response.json()["auto_execute"]
+
+
+def test_docker_train_create(train_id):
+    response = client.get("/api/trains/docker/configs/all")
+    print(response.json())
+    response = client.post("/api/trains/docker", json={"train_id": train_id})
+
+    assert response.status_code == 200, response.text
+
+    json_response = response.json()
+    assert json_response["train_id"] == train_id
+    print(json_response)
+    assert json_response["state"]["num_executions"] == 0
+    assert json_response["state"]["status"] == "inactive"
+
+
+def test_docker_train_create_fails(train_id):
+    response = client.post("/api/trains/docker", json={"train_id": train_id})
+
+    assert response.status_code == 400, response.text
+
+
+def test_get_train_by_id(train_id):
+    response = client.get(f"/api/trains/docker/{train_id}")
+    assert response.status_code == 200, response.text
+
+
+def test_get_train_by_id_fails():
+    response = client.get("/api/trains/docker/notthere")
+    assert response.status_code == 404, response.text
+
+
+def test_list_docker_trains(train_list_length):
+    response = client.get("/api/trains/docker")
+
+    assert response.status_code == 200, response.text
+    print(response.json())
+
+    assert len(response.json()) == train_list_length + 1
+
+
+def test_docker_train_config_create_fails(docker_train_config):
+    response = client.post("/api/trains/docker/config", json=docker_train_config)
+    assert response.status_code == 400
+
+
+def test_get_docker_train_configs():
+    response = client.get("/api/trains/docker/configs/all")
+    assert response.status_code == 200, response.text
+    assert len(response.json()) >= 1
+
+
+def test_get_docker_train_config_by_id(config_id):
+    response = client.get("/api/trains/docker/config/1")
+    assert response.status_code == 200, response.text
+
+
+def test_get_docker_train_config_by_id_fails():
+    response = client.get("/api/trains/docker/config/234")
+    assert response.status_code == 404, response.text
+
+
+def test_update_docker_train_config(docker_train_config, config_id):
+    docker_train_config["name"] = "updated name"
+    response = client.put(
+        f"/api/trains/docker/config/{config_id}", json=docker_train_config
+    )
+
+    assert response.status_code == 200, response.text
+    response = client.get(f"/api/trains/docker/config/{config_id}")
+
+    assert response.json()["name"] == "updated name"
+
+
+def test_update_docker_train_config_fails(docker_train_config):
+    docker_train_config["name"] = "updated name"
+    response = client.put("/api/trains/docker/config/234", json=docker_train_config)
+    assert response.status_code == 404, response.text
+
+
+def test_assign_docker_train_config(train_id, config_id):
+    response = client.post(f"/api/trains/docker/{train_id}/config/{config_id}")
+    assert response.status_code == 200, response.text
+    response = client.get(f"/api/trains/docker/{train_id}")
+
+    assert response.json()["config_id"] == config_id
+
+    # test non existing config error
+    response = client.post(f"/api/trains/docker/{train_id}/config/321")
+
+    assert response.status_code == 404
+
+    # test non existing train error
+
+    response = client.post("/api/trains/docker/no_train/config/1")
+    assert response.status_code == 404
+
+
+def test_get_config_for_train(train_id):
+    response = client.get(f"/api/trains/docker/{train_id}/config")
+    assert response.status_code == 200, response.text
+    assert len(response.json()["trains"]) == 1
+    print(response.json())
+
+    new_train_id = "no_config_train"
+    response = client.post("/api/trains/docker", json={"train_id": new_train_id})
+    assert response.status_code == 200
+    response = client.get(f"/api/trains/docker/{new_train_id}/config")
+
+    assert response.status_code == 404
+
+
+def test_create_train_with_config(docker_train_config, config_id):
+    # assign existing config
+    response = client.post(
+        "/api/trains/docker",
+        json={"train_id": "with_existing_config", "config": config_id},
+    )
+    assert response.status_code == 200, response.text
+    config_response = client.get("/api/trains/docker/with_existing_config/config")
+    assert config_response.json()["name"] == "updated name"
+    assert len(config_response.json()["trains"]) == 2
+
+    # fails with unknown config id
+    response = client.post(
+        "/api/trains/docker", json={"train_id": "config does not exist", "config": 3213}
+    )
+    assert response.status_code == 404, response.text
+
+    new_config = {
+        "name": "new config",
+        "airflow_config": {
+            "env": [{"key": "FHIR_ADDRESS", "value": "test_address"}],
+            "volumes": [
+                {
+                    "host_path": "path/on/host",
+                    "container_path": "path/in/container",
+                    "mode": "ro",
+                }
+            ],
+        },
+        "auto_execute": False,
+    }
+
+    response = client.post(
+        "/api/trains/docker",
+        json={
+            "train_id": "with_new_config",
+            "name": "train with new config",
+            "config": new_config,
+        },
+    )
+    assert response.status_code == 200
+    print(response.json())
+
+    config_response = client.get("/api/trains/docker/with_new_config/config")
+    assert config_response.json()["name"] == "new config"
+
+
+def test_get_train_state():
+    train_id = "test_train_state"
+    response = client.post(
+        "/api/trains/docker",
+        json={
+            "train_id": train_id,
+        },
+    )
+    assert response.status_code == 200, response.text
+
+    response = client.get(f"/api/trains/docker/{train_id}/state")
+    assert response.status_code == 200, response.text
+    assert response.json()["status"] == "inactive"
+
+
+def test_update_train_state(train_id):
+    response = client.put(
+        f"/api/trains/docker/{train_id}/state",
+        json={"status": "active", "num_executions": 1},
+    )
+    assert response.status_code == 200, response.text
+    assert response.json()["status"] == "active"
+    assert response.json()["num_executions"] == 1
+
+
+def test_synchronize_database():
+    if os.getenv("ENVIRONMENT") == "testing":
+        response_nostation = client.get("/api/trains/docker/sync")
+        assert response_nostation.status_code == 200, response_nostation.text
+
+        response = client.get("/api/trains/docker/sync/?station_id=1")
+        if os.getenv("STATION_ID") == 1:
+            assert len(response.json()) == 0
+        assert response.status_code == 200, response.text
+
+
+def test_synchronize_database_fails():
+    if os.getenv("ENVIRONMENT") == "testing":
+        response = client.get("/api/trains/docker/sync/?station_id=123")
+        assert response.status_code == 404, response.text
+
+
+def test_run_docker_train(train_id, docker_train_config, config_id):
+    if os.getenv("ENVIRONMENT") == "testing":
+        old_state = client.get(f"/api/trains/docker/{train_id}/state")
+
+        # run with given config id
+        response = client.post(
+            f"/api/trains/docker/{train_id}/run", json={"config_id": 1}
+        )
+        assert response.json()["airflow_dag_run"]
+        assert response.json()["config"] == 1
+        assert response.status_code == 200, response.text
+
+        state_response = client.get(f"/api/trains/docker/{train_id}/state")
+        assert old_state.json() != state_response.json()
+        assert (
+            old_state.json()["num_executions"] + 1
+            == state_response.json()["num_executions"]
+        )
+
+        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
+        assert (
+            execution_response.json()[-1]["airflow_dag_run"]
+            == response.json()["airflow_dag_run"]
+        )
+
+        # run with default config
+        response = client.post(
+            f"/api/trains/docker/{train_id}/run", json={"config_id": "default"}
+        )
+        assert response.json()["airflow_dag_run"]
+        assert response.json()["config"] is None
+        assert response.status_code == 200, response.text
+
+        state_response = client.get(f"/api/trains/docker/{train_id}/state")
+        assert (
+            old_state.json()["num_executions"] + 2
+            == state_response.json()["num_executions"]
+        )
+
+        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
+        assert (
+            execution_response.json()[-1]["airflow_dag_run"]
+            == response.json()["airflow_dag_run"]
+        )
+
+        # run with config assigned to train
+        response = client.post(f"/api/trains/docker/{train_id}/run")
+        assert response.json()["airflow_dag_run"]
+        assert response.json()["config"] == config_id
+        assert response.status_code == 200, response.text
+
+        state_response = client.get(f"/api/trains/docker/{train_id}/state")
+        assert (
+            old_state.json()["num_executions"] + 3
+            == state_response.json()["num_executions"]
+        )
+
+        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
+        assert (
+            execution_response.json()[-1]["airflow_dag_run"]
+            == response.json()["airflow_dag_run"]
+        )
+
+
+def test_run_docker_train_fails(train_id, docker_train_config, config_id):
+    old_state = client.get(f"/api/trains/docker/{train_id}/state")
+    old_executions = client.get(f"/api/trains/docker/{train_id}/executions")
+
+    if os.getenv("ENVIRONMENT") == "testing":
+
+        # no config with id given
+        response = client.post(
+            f"/api/trains/docker/{train_id}/run", json={"config_id": 3213}
+        )
+        state_response = client.get(f"/api/trains/docker/{train_id}/state")
+        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
+        assert old_state.json() == state_response.json()
+        assert old_executions.json() == execution_response.json()
+        assert response.status_code == 400, response.text
+
+        # no tag and no repository given
+        specific_id = config_id + 1
+        response = client.post(
+            f"/api/trains/docker/{train_id}/run", json={"config_id": specific_id}
+        )
+        response_conf = client.get(f"/api/trains/docker/config/{specific_id}")
+        print(response_conf.json())
+        state_response = client.get(f"/api/trains/docker/{train_id}/state")
+        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
+        assert old_state.json() == state_response.json()
+        assert old_executions.json() == execution_response.json()
+        assert response.status_code == 400, response.text
+
+        # train not defined
+        response = client.post("/api/trains/docker/no_train/run", json={"config_id": 1})
+        assert response.status_code == 404, response.text
+
+    else:
+        response = client.post(
+            f"/api/trains/docker/{train_id}/run", json={"config_id": "default"}
+        )
+        state_response = client.get(f"/api/trains/docker/{train_id}/state")
+        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
+        assert old_state.json() == state_response.json()
+        assert old_executions.json() == execution_response.json()
+        assert response.status_code == 503, response.text
+
+        response = client.post(f"/api/trains/docker/{train_id}/run")
+        state_response = client.get(f"/api/trains/docker/{train_id}/state")
+        execution_response = client.get(f"/api/trains/docker/{train_id}/executions")
+        assert old_state.json() == state_response.json()
+        assert old_executions.json() == execution_response.json()
+        assert response.status_code == 503, response.text
```

### Comparing `pht-station-0.1/station/tests/test_api_fhir_servers.py` & `pht_station-0.2.0/station/app/tests/test_api_fhir_servers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,110 @@
-import pytest
-from fastapi.testclient import TestClient
-from dotenv import load_dotenv, find_dotenv
-
-from station.app.main import app
-from station.app.api.dependencies import get_db
-from station.app.crud.crud_fhir_servers import fhir_servers
-from station.app.schemas.fhir import FHIRServerCreate
-from station.app.config import settings
-
-from .test_db import override_get_db, TestingSessionLocal
-
-app.dependency_overrides[get_db] = override_get_db
-
-client = TestClient(app)
-
-
-@pytest.fixture()
-def station_settings():
-    load_dotenv(find_dotenv())
-    settings.setup()
-    return settings
-
-
-def test_fhir_server_encrypted_storage(station_settings):
-    load_dotenv(find_dotenv())
-
-    db = TestingSessionLocal()
-
-    obj_in = {"name": "Test Server", "api_address": "http://test.com", "username": "user", "password": "password"}
-    obj_in = FHIRServerCreate(**obj_in)
-    fhir_server = fhir_servers.create(db, obj_in=obj_in)
-
-    station_fernet = station_settings.get_fernet()
-    assert fhir_server.name == "Test Server"
-    assert fhir_server.password != "password"
-    assert station_fernet.decrypt(fhir_server.password.encode()) == b"password"
-
-    db.close()
-
-
-def test_fhir_server_create():
-    """
-    Test the creation of a FHIR server
-    """
-    response = client.post("/api/fhir/server", json={"name": "Test Server", "api_address": "http://test.com"})
-    assert response.status_code == 201
-    assert response.json()["name"] == "Test Server"
-    assert response.json()["api_address"] == "http://test.com"
-
-
-def test_fhir_server_get():
-    """
-    Test the retrieval of a FHIR server
-    """
-    response = client.get("/api/fhir/server/1")
-    assert response.status_code == 200
-    assert response.json()["name"] == "Test Server"
-    assert response.json()["api_address"] == "http://test.com"
-
-
-def test_list_fhir_servers():
-    """
-    Test the retrieval of a list of FHIR servers
-    """
-    response = client.post("/api/fhir/server", json={"name": "Test Server", "api_address": "http://test.com"})
-    assert response.status_code == 201
-    assert response.json()["name"] == "Test Server"
-    assert response.json()["api_address"] == "http://test.com"
-    response = client.get("/api/fhir/server")
-    assert response.status_code == 200
-    assert response.json()[0]["name"] == "Test Server"
-    assert response.json()[0]["api_address"] == "http://test.com"
-
-
-def test_update_fhir_server():
-    """
-    Test the update of a FHIR server
-    """
-    response = client.put("/api/fhir/server/1",
-                          json={"name": "Test Server Updated", "api_address": "http://test.com", "username": "user",
-                                "password": "password"})
-    assert response.status_code == 200
-    assert response.json()["name"] == "Test Server Updated"
-    assert response.json()["api_address"] == "http://test.com"
-
-
-def test_delete_fhir_server():
-    """
-    Test the deletion of a FHIR server
-    """
-    response = client.delete("/api/fhir/server/1")
-    assert response.status_code == 202
+import pytest
+from dotenv import find_dotenv, load_dotenv
+from fastapi.testclient import TestClient
+
+from station.app.api.dependencies import get_db
+from station.app.crud.crud_fhir_servers import fhir_servers
+from station.app.main import app
+from station.app.schemas.fhir import FHIRServerCreate
+from station.app.settings import settings
+
+from .test_db import TestingSessionLocal, override_get_db
+
+app.dependency_overrides[get_db] = override_get_db
+
+client = TestClient(app)
+
+
+@pytest.fixture()
+def station_settings():
+    load_dotenv(find_dotenv())
+    settings.setup()
+    return settings
+
+
+def test_fhir_server_encrypted_storage(station_settings):
+    load_dotenv(find_dotenv())
+
+    db = TestingSessionLocal()
+
+    obj_in = {
+        "name": "Test Server",
+        "api_address": "http://test.com",
+        "username": "user",
+        "password": "password",
+    }
+    obj_in = FHIRServerCreate(**obj_in)
+    fhir_server = fhir_servers.create(db, obj_in=obj_in)
+
+    station_fernet = station_settings.get_fernet()
+    assert fhir_server.name == "Test Server"
+    assert fhir_server.password != "password"
+    assert station_fernet.decrypt(fhir_server.password.encode()) == b"password"
+
+    db.close()
+
+
+def test_fhir_server_create():
+    """
+    Test the creation of a FHIR server
+    """
+    response = client.post(
+        "/api/fhir/server",
+        json={"name": "Test Server", "api_address": "http://test.com"},
+    )
+    assert response.status_code == 201
+    assert response.json()["name"] == "Test Server"
+    assert response.json()["api_address"] == "http://test.com"
+
+
+def test_fhir_server_get():
+    """
+    Test the retrieval of a FHIR server
+    """
+    response = client.get("/api/fhir/server/1")
+    assert response.status_code == 200
+    assert response.json()["name"] == "Test Server"
+    assert response.json()["api_address"] == "http://test.com"
+
+
+def test_list_fhir_servers():
+    """
+    Test the retrieval of a list of FHIR servers
+    """
+    response = client.post(
+        "/api/fhir/server",
+        json={"name": "Test Server", "api_address": "http://test.com"},
+    )
+    assert response.status_code == 201
+    assert response.json()["name"] == "Test Server"
+    assert response.json()["api_address"] == "http://test.com"
+    response = client.get("/api/fhir/server")
+    assert response.status_code == 200
+    assert response.json()[0]["name"] == "Test Server"
+    assert response.json()[0]["api_address"] == "http://test.com"
+
+
+def test_update_fhir_server():
+    """
+    Test the update of a FHIR server
+    """
+    response = client.put(
+        "/api/fhir/server/1",
+        json={
+            "name": "Test Server Updated",
+            "api_address": "http://test.com",
+            "username": "user",
+            "password": "password",
+        },
+    )
+    assert response.status_code == 200
+    assert response.json()["name"] == "Test Server Updated"
+    assert response.json()["api_address"] == "http://test.com"
+
+
+def test_delete_fhir_server():
+    """
+    Test the deletion of a FHIR server
+    """
+    response = client.delete("/api/fhir/server/1")
+    assert response.status_code == 202
```

### Comparing `pht-station-0.1/station/tests/test_api_notifications.py` & `pht_station-0.2.0/station/app/tests/test_api_notifications.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,91 @@
-import pytest
-from fastapi.testclient import TestClient
-from dotenv import load_dotenv, find_dotenv
-
-from station.app.main import app
-from station.app.api.dependencies import get_db
-from station.app.crud.crud_notifications import notifications
-from station.app.schemas.notifications import NotificationCreate
-from station.app.config import settings
-
-from .test_db import override_get_db, TestingSessionLocal
-
-app.dependency_overrides[get_db] = override_get_db
-
-client = TestClient(app)
-
-
-def test_notification_create():
-    """
-    Test the creation of a Notification
-    """
-    response = client.post("/api/notifications", json={"topic": "Test Notification", "message": "testing"})
-    assert response.status_code == 201
-    assert response.json()["topic"] == "Test Notification"
-    assert response.json()["message"] == "testing"
-
-
-def test_notification_create_fail():
-    """
-    Test the creation of a Notification --fail
-    """
-    response = client.post("/api/notification/x", json={"topic": "Test Notification", "message": "testing"})
-    assert response.status_code == 404, response.text
-
-
-def test_notification_get_by_id():
-    """
-    Test the retrieval of a Notification
-    """
-    response = client.get(f"/api/notifications/1")
-    assert response.status_code == 200
-    assert response.json()["topic"] == "Test Notification"
-    assert response.json()["message"] == "testing"
-
-
-def test_notification_get_by_id_fail():
-    """
-    Test the retrieval of a Notification --fail
-    """
-    response = client.get(f"/api/notification/x")
-    assert response.status_code == 404, response.text
-
-def test_notification_update():
-    """
-    Test the update of a Notification
-    """
-    response = client.put("/api/notifications/1", json={'message': 'testing', 'topic': 'Test Notification Updated', 'is_read': True})
-    assert response.status_code == 200
-    assert response.json()["topic"] == "Test Notification Updated"
-    assert response.json()["message"] == "testing"
-
-
-def test_get_list_notifications():
-    """
-    Test the retrieval of a list of Notifications
-    """
-    response = client.post("/api/notifications", json={"topic": "Test Notification 2", "message": "testing"})
-    assert response.status_code == 201
-    assert response.json()["topic"] == "Test Notification 2"
-    assert response.json()["message"] == "testing"
-    response = client.get(f"/api/notifications")
-    assert response.status_code == 200
-    assert len(response.json()) >= 1
-
-
-
-def test_notification_delete():
-    """
-    Test the deletion of a Notification
-    """
-    response = client.delete("/api/notifications/1")
-    assert response.status_code == 202, response.text
-
+from fastapi.testclient import TestClient
+
+from station.app.api.dependencies import get_db
+from station.app.main import app
+
+from .test_db import override_get_db
+
+app.dependency_overrides[get_db] = override_get_db
+
+client = TestClient(app)
+
+
+def test_notification_create():
+    """
+    Test the creation of a Notification
+    """
+    response = client.post(
+        "/api/notifications", json={"topic": "Test Notification", "message": "testing"}
+    )
+    assert response.status_code == 201
+    assert response.json()["topic"] == "Test Notification"
+    assert response.json()["message"] == "testing"
+
+
+def test_notification_create_fail():
+    """
+    Test the creation of a Notification --fail
+    """
+    response = client.post(
+        "/api/notification/x", json={"topic": "Test Notification", "message": "testing"}
+    )
+    assert response.status_code == 404, response.text
+
+
+def test_notification_get_by_id():
+    """
+    Test the retrieval of a Notification
+    """
+    response = client.get("/api/notifications/1")
+    assert response.status_code == 200
+    assert response.json()["topic"] == "Test Notification"
+    assert response.json()["message"] == "testing"
+
+
+def test_notification_get_by_id_fail():
+    """
+    Test the retrieval of a Notification --fail
+    """
+    response = client.get("/api/notification/x")
+    assert response.status_code == 404, response.text
+
+
+def test_notification_update():
+    """
+    Test the update of a Notification
+    """
+    response = client.put(
+        "/api/notifications/1",
+        json={
+            "message": "testing",
+            "topic": "Test Notification Updated",
+            "is_read": True,
+        },
+    )
+    assert response.status_code == 200
+    assert response.json()["topic"] == "Test Notification Updated"
+    assert response.json()["message"] == "testing"
+
+
+def test_get_list_notifications():
+    """
+    Test the retrieval of a list of Notifications
+    """
+    response = client.post(
+        "/api/notifications",
+        json={"topic": "Test Notification 2", "message": "testing"},
+    )
+    assert response.status_code == 201
+    assert response.json()["topic"] == "Test Notification 2"
+    assert response.json()["message"] == "testing"
+    response = client.get("/api/notifications")
+    assert response.status_code == 200
+    assert len(response.json()) >= 1
+
+
+def test_notification_delete():
+    """
+    Test the deletion of a Notification
+    """
+    response = client.delete("/api/notifications/1")
+    assert response.status_code == 202, response.text
```

### Comparing `pht-station-0.1/station/tests/test_central_client.py` & `pht_station-0.2.0/station/app/tests/test_central_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,44 @@
-import os
-
-from station.clients.central.central_client import CentralApiClient
-import pytest
-from dotenv import load_dotenv, find_dotenv
-
-
-@pytest.fixture
-def central_client():
-    load_dotenv(find_dotenv())
-    url = os.getenv("CENTRAL_API_URL")
-    client_id = os.getenv("STATION_ROBOT_ID")
-    client_secret = os.getenv("STATION_ROBOT_SECRET")
-    return CentralApiClient(url, client_id, client_secret)
-
-
-def test_get_token(central_client):
-    token = central_client._get_token()
-
-    assert token is not None
-
-
-def test_get_registry_credentials(central_client):
-    registry_credentials = central_client.get_registry_credentials(os.getenv("STATION_ID"))
-    print(registry_credentials)
-    assert registry_credentials
-
-
-def test_update_public_key(central_client):
-    public_key = "test_public_key".encode("utf-8").hex()
-    station_id = os.getenv("STATION_ID")
-    response = central_client.update_public_key(station_id, public_key)
-    print(response)
+import os
+import pprint
+
+import pytest
+from dotenv import find_dotenv, load_dotenv
+
+from station.common.clients.central.central_client import CentralApiClient
+
+
+@pytest.fixture
+def central_client():
+    load_dotenv(find_dotenv())
+    url = os.getenv("CENTRAL_API_URL")
+    client_id = os.getenv("STATION_ROBOT_ID")
+    client_secret = os.getenv("STATION_ROBOT_SECRET")
+    return CentralApiClient(url, client_id, client_secret)
+
+
+def test_get_token(central_client):
+    token = central_client._get_token()
+
+    assert token is not None
+
+
+def test_get_registry_credentials(central_client):
+    registry_credentials = central_client.get_registry_credentials(
+        os.getenv("STATION_ID")
+    )
+    pprint.pprint(registry_credentials)
+    assert registry_credentials
+
+
+def test_update_public_key(central_client):
+    public_key = "test_public_key".encode("utf-8").hex()
+    station_id = os.getenv("STATION_ID")
+    response = central_client.update_public_key(station_id, public_key)
+    print(response)
+
+
+def test_get_trains_for_station(central_client):
+    station_id = os.getenv("STATION_ID")
+    response = central_client.get_trains(station_id)
+    assert response
+    print(response)
```

### Comparing `pht-station-0.1/station/tests/test_db.py` & `pht_station-0.2.0/station/app/tests/test_db.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,34 @@
-from sqlalchemy import create_engine
-from sqlalchemy.orm import sessionmaker
-
-from station.app.db.base import Base
-# Create new sqlite database for testing
-
-SQLALCHEMY_DATABASE_URL = "sqlite:///./test.db"
-
-engine = create_engine(
-    SQLALCHEMY_DATABASE_URL, connect_args={"check_same_thread": False}
-)
-TestingSessionLocal = sessionmaker(autocommit=False, autoflush=False, bind=engine)
-
-Base.metadata.drop_all(bind=engine)
-Base.metadata.create_all(bind=engine)
-
-
-def override_get_db():
-    try:
-        db = TestingSessionLocal()
-        yield db
-    finally:
-        db.close()
-
+import os
+
+from dotenv import find_dotenv, load_dotenv
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker
+
+from station.app.db.base import Base
+
+# Create new sqlite database for testing
+
+# load the .env file
+load_dotenv(find_dotenv())
+
+SQLALCHEMY_DATABASE_URL = os.getenv("TEST_DB", "sqlite:///./test.db")
+
+if SQLALCHEMY_DATABASE_URL.startswith("sqlite"):
+    engine = create_engine(
+        SQLALCHEMY_DATABASE_URL, connect_args={"check_same_thread": False}
+    )
+else:
+    engine = create_engine(SQLALCHEMY_DATABASE_URL)
+
+TestingSessionLocal = sessionmaker(autocommit=False, autoflush=False, bind=engine)
+
+Base.metadata.drop_all(bind=engine)
+Base.metadata.create_all(bind=engine)
+
+
+def override_get_db():
+    try:
+        db = TestingSessionLocal()
+        yield db
+    finally:
+        db.close()
```

### Comparing `pht-station-0.1/station/worker/loader/base_loader.py` & `pht_station-0.2.0/station/worker/loader/base_loader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,65 @@
-import os
-from typing import Union
-import pytorch_lightning as pl
-
-from torch.utils.data import DataLoader, Dataset
-
-from station.clients.minio import MinioClient
-from station.worker.loader.dataset import MinioFolderDS
-from torchvision.transforms import Compose, ToTensor
-
-
-class BaseLoader:
-    def __init__(self,
-                 data_set: Union[Dataset, str] = None,
-                 station_api: str = None,
-                 config: dict = None,
-                 transform: Compose = None):
-
-        self.station_api = station_api if station_api else os.getenv("STATION_API_URL")
-        self.data_set = data_set
-        self.transform = transform
-        self.config = config
-        # TODO fix minio
-        self.minio_client = MinioClient()
-
-    def make_data_loader(self) -> DataLoader:
-        """
-        Create a pytorch data loder based on this instance's fields, either takes a data set directly passed
-        to the constructor or loads the data set from Minio if the given data set is specified as a string identifier
-
-        :return: pytorch Dataloader to be used in model training
-        """
-        if isinstance(self.data_set, str):
-            # Get data from db
-            self.data_set = self.get_data_set()
-        if self.config:
-            return DataLoader(self.data_set, **self.config)
-        return DataLoader(self.data_set)
-
-    def make_lightning_data_module(self) -> pl.LightningDataModule:
-        pass
-
-    def get_data_set(self):
-        # TODO enable different data set types
-        dataset = MinioFolderDS(client=self.minio_client, data_set_id=self.data_set, transform=self.transform)
-        return dataset
-
-
-if __name__ == '__main__':
-
-    transform = Compose([ToTensor()])
-
-    loader = BaseLoader(data_set="cifar/batch_1",
-                        transform=transform,
-                        config={"batch_size": 6, "num_workers": 0}
-                        ).make_data_loader()
-    for i, batch in enumerate(loader):
-        print(batch.size())
-        if i > 3:
-            break
+import os
+from typing import Union
+
+import pytorch_lightning as pl
+from torch.utils.data import DataLoader, Dataset
+from torchvision.transforms import Compose, ToTensor
+
+from station.common.clients.minio import MinioClient
+from station.worker.loader.dataset import MinioFolderDS
+
+
+class BaseLoader:
+    def __init__(
+        self,
+        data_set: Union[Dataset, str] = None,
+        station_api: str = None,
+        config: dict = None,
+        transform: Compose = None,
+    ):
+        self.station_api = station_api if station_api else os.getenv("STATION_API_URL")
+        self.data_set = data_set
+        self.transform = transform
+        self.config = config
+        # TODO fix minio
+        self.minio_client = MinioClient()
+
+    def make_data_loader(self) -> DataLoader:
+        """
+        Create a pytorch data loder based on this instance's fields, either takes a data set directly passed
+        to the constructor or loads the data set from Minio if the given data set is specified as a string identifier
+
+        :return: pytorch Dataloader to be used in model training
+        """
+        if isinstance(self.data_set, str):
+            # Get data from db
+            self.data_set = self.get_data_set()
+        if self.config:
+            return DataLoader(self.data_set, **self.config)
+        return DataLoader(self.data_set)
+
+    def make_lightning_data_module(self) -> pl.LightningDataModule:
+        pass
+
+    def get_data_set(self):
+        # TODO enable different data set types
+        dataset = MinioFolderDS(
+            client=self.minio_client,
+            data_set_id=self.data_set,
+            transform=self.transform,
+        )
+        return dataset
+
+
+if __name__ == "__main__":
+    transform = Compose([ToTensor()])
+
+    loader = BaseLoader(
+        data_set="cifar/batch_1",
+        transform=transform,
+        config={"batch_size": 6, "num_workers": 0},
+    ).make_data_loader()
+    for i, batch in enumerate(loader):
+        print(batch.size())
+        if i > 3:
+            break
```

### Comparing `pht-station-0.1/station/worker/loader/dataset.py` & `pht_station-0.2.0/station/worker/loader/dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,134 +1,150 @@
-from abc import ABC
-from typing import Iterator, Generator, List
-import torch
-from torch.utils.data import Dataset, IterableDataset, DataLoader
-from torch.utils.data.dataset import T_co
-from minio import datatypes
-from PIL import Image
-from torchvision.transforms import Compose, ToTensor, CenterCrop
-import numpy as np
-
-from station.clients.minio import MinioClient
-
-
-class BaseDataSet(Dataset, ABC):
-    id: str
-
-
-class MinioFolderDataSet(IterableDataset):
-
-    def __init__(self, minio_client: MinioClient, id: str = None, transform: Compose = None):
-        super(MinioFolderDataSet, self).__init__()
-        self.id = id
-        self.client = minio_client
-        self.transform = transform
-
-    def __iter__(self) -> Iterator[T_co]:
-        worker_info = torch.utils.data.get_worker_info()
-
-        if worker_info is None:
-            return self._make_generator()
-
-        else:
-            print(worker_info.num_workers)
-            # TODO
-            raise NotImplementedError("Implement sliced generators for multiworker loading")
-
-    def _make_generator(self, id: str = None):
-        if id:
-            self.id = id
-        minio_items = self._get_minio_items()
-
-        tensor_generator = self._make_image_generator(minio_items)
-        return tensor_generator
-
-    def _get_minio_items(self) -> Generator[datatypes.Object, None, None]:
-        items = self.client.get_data_set_items(self.id)
-        return items
-
-    def _make_image_generator(self,
-                              minio_items: Generator[datatypes.Object, None, None]
-                              ) -> Generator[torch.Tensor, None, None]:
-        for i, object in enumerate(minio_items):
-            minio_object = self.client.client.get_object("data-sets", object.object_name)
-            np_img = np.array(Image.open(minio_object))
-
-            print(object.object_name)
-
-            if self.transform:
-                yield self.transform(np_img)
-            else:
-                yield np_img
-
-
-class MinioFolderDS(Dataset):
-
-    # TODO generalized target creation
-
-    def __init__(self, client: MinioClient, data_set_id: str = None, transform: Compose = None,
-                 target_classes: List[str] = None):
-        super().__init__()
-        self.data_set_id = data_set_id
-        self.minio_client = client
-        self.transform = transform
-        self.items = None
-
-        self.get_minio_items()
-
-        if target_classes:
-            self.classes = np.asarray(target_classes)
-        else:
-            self.classes = self.get_classes_from_folders()
-
-    def __getitem__(self, index) -> T_co:
-        minio_object = self.minio_client.client.get_object("datasets", self.items[index])
-        np_img = np.array(Image.open(minio_object))
-        np_img = np.transpose(np_img.astype(float), (2, 1, 0))
-        label = self.get_label(self.items[index])
-        if self.transform:
-            return self.transform(np_img), label
-        return torch.Tensor(np_img), label
-
-    def __len__(self):
-        return len(list(self.items))
-
-    def get_label(self, item_name: str):
-        folder = item_name[len(self.data_set_id):].split("/")[0]
-        label = self.classes == folder
-        return torch.tensor(label, dtype=torch.long)
-
-    def get_minio_items(self):
-        minio_items = self.minio_client.get_data_set_items(self.data_set_id)
-        item_list = []
-        for item in minio_items:
-            item_list.append(item.object_name)
-
-        self.items = item_list
-
-    def save(self):
-
-        # TODO Save the full data set to disk somewhere to enable fast loading
-        pass
-
-    def get_classes_from_folders(self):
-        classes = self.minio_client.get_classes_by_folders(self.data_set_id)
-        print(classes)
-        return np.asarray(classes)
-
-
-if __name__ == '__main__':
-    minio_client = MinioClient(minio_server="localhost:9000",
-                               secret_key="minio_admin", access_key="minio_admin")
-
-    transform = Compose([ToTensor(), CenterCrop(size=24)])
-    minio_ds = MinioFolderDS(client=minio_client, data_set_id="cifar/batch_2", transform=transform)
-    minio_ds.get_minio_items()
-    print(len(minio_ds))
-
-    dl = DataLoader(minio_ds, batch_size=6, num_workers=0, shuffle=True)
-
-    for i, batch in enumerate(dl):
-        x, y = batch
-        print(y)
-        if i > 3:
-            break
+from abc import ABC
+from typing import Generator, Iterator, List
+
+import numpy as np
+import torch
+from minio import datatypes
+from PIL import Image
+from torch.utils.data import DataLoader, Dataset, IterableDataset
+from torch.utils.data.dataset import T_co
+from torchvision.transforms import CenterCrop, Compose, ToTensor
+
+from station.common.clients.minio import MinioClient
+
+
+class BaseDataSet(Dataset, ABC):
+    id: str
+
+
+class MinioFolderDataSet(IterableDataset):
+    def __init__(
+        self, minio_client: MinioClient, id: str = None, transform: Compose = None
+    ):
+        super(MinioFolderDataSet, self).__init__()
+        self.id = id
+        self.client = minio_client
+        self.transform = transform
+
+    def __iter__(self) -> Iterator[T_co]:
+        worker_info = torch.utils.data.get_worker_info()
+
+        if worker_info is None:
+            return self._make_generator()
+
+        else:
+            print(worker_info.num_workers)
+            # TODO
+            raise NotImplementedError(
+                "Implement sliced generators for multiworker loading"
+            )
+
+    def _make_generator(self, id: str = None):
+        if id:
+            self.id = id
+        minio_items = self._get_minio_items()
+
+        tensor_generator = self._make_image_generator(minio_items)
+        return tensor_generator
+
+    def _get_minio_items(self) -> Generator[datatypes.Object, None, None]:
+        items = self.client.get_minio_dir_items(self.id)
+        return items
+
+    def _make_image_generator(
+        self, minio_items: Generator[datatypes.Object, None, None]
+    ) -> Generator[torch.Tensor, None, None]:
+        for i, object in enumerate(minio_items):
+            minio_object = self.client.client.get_object(
+                "data-sets", object.object_name
+            )
+            np_img = np.array(Image.open(minio_object))
+
+            print(object.object_name)
+
+            if self.transform:
+                yield self.transform(np_img)
+            else:
+                yield np_img
+
+
+class MinioFolderDS(Dataset):
+    # TODO generalized target creation
+
+    def __init__(
+        self,
+        client: MinioClient,
+        data_set_id: str = None,
+        transform: Compose = None,
+        target_classes: List[str] = None,
+    ):
+        super().__init__()
+        self.data_set_id = data_set_id
+        self.minio_client = client
+        self.transform = transform
+        self.items = None
+
+        self.get_minio_items()
+
+        if target_classes:
+            self.classes = np.asarray(target_classes)
+        else:
+            self.classes = self.get_classes_from_folders()
+
+    def __getitem__(self, index) -> T_co:
+        minio_object = self.minio_client.client.get_object(
+            "datasets", self.items[index]
+        )
+        np_img = np.array(Image.open(minio_object))
+        np_img = np.transpose(np_img.astype(float), (2, 1, 0))
+        label = self.get_label(self.items[index])
+        if self.transform:
+            return self.transform(np_img), label
+        return torch.Tensor(np_img), label
+
+    def __len__(self):
+        return len(list(self.items))
+
+    def get_label(self, item_name: str):
+        folder = item_name[len(self.data_set_id) :].split("/")[0]
+        label = self.classes == folder
+        return torch.tensor(label, dtype=torch.long)
+
+    def get_minio_items(self):
+        minio_items = self.minio_client.get_minio_dir_items(self.data_set_id)
+        item_list = []
+        for item in minio_items:
+            item_list.append(item.object_name)
+
+        self.items = item_list
+
+    def save(self):
+        # TODO Save the full data set to disk somewhere to enable fast loading
+        pass
+
+    def get_classes_from_folders(self):
+        classes = self.minio_client.get_classes_by_folders(self.data_set_id)
+        print(classes)
+        return np.asarray(classes)
+
+
+if __name__ == "__main__":
+    minio_client = MinioClient(
+        minio_server="localhost:9000",
+        secret_key="minio_admin",
+        access_key="minio_admin",
+    )
+
+    transform = Compose([ToTensor(), CenterCrop(size=24)])
+    minio_ds = MinioFolderDS(
+        client=minio_client, data_set_id="cifar/batch_2", transform=transform
+    )
+    minio_ds.get_minio_items()
+    print(len(minio_ds))
+
+    dl = DataLoader(minio_ds, batch_size=6, num_workers=0, shuffle=True)
+
+    for i, batch in enumerate(dl):
+        x, y = batch
+        print(y)
+        if i > 3:
+            break
```

### Comparing `pht-station-0.1/station/worker/loader/model_loader.py` & `pht_station-0.2.0/station/worker/loader/model_loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,106 @@
-from typing import Any
-import requests
-from sqlalchemy.orm import Session
-import importlib.util
-import importlib.machinery
-import os
-import tempfile
-
-from station.clients.minio import MinioClient
-from conductor_lib.src.torch import LightningTrainModel
-from station.app.crud import federated_trains
-
-
-class ModelLoader:
-
-    def __init__(self, station_url: str = None):
-        self.station_url = station_url if station_url else os.getenv("STATION_API_URL")
-        assert self.station_url
-        self.minio_client = MinioClient()
-
-    def get_model_from_station(self, model_id: str = None) -> LightningTrainModel:
-        """
-        Use the station api to get a model registered under the specified model_id and return the initialized model
-
-        :param model_id: identifier of model registered at a station
-        :return: initialized model instance stored in the db with model_id
-        """
-
-        if not model_id:
-            model_id = self.model_id
-
-        # Get the model from the station api
-        url = self.station_url + f"/api/station/models/{model_id}"
-
-        r = requests.get(url=url)
-
-        r.raise_for_status()
-        model = r.json()
-        # initialize the model based on the received src code and name
-        model = self._make_lightning_module(model["model_src"], model["model_name"])
-        return model
-
-    def load_train_model(self, db: Session, train_id: Any):
-        db_train = federated_trains.get_by_train_id(db=db, train_id=train_id)
-
-        model = db_train.model
-        assert model
-
-        lightning_module = self._make_lightning_module(model.model_src, module_name=model.model_name)
-        return lightning_module
-
-    def save_model_checkpoint(self):
-        # TODO
-        pass
-
-    def load_torch_model_from_json(self, model_json: dict = None) -> LightningTrainModel:
-        """
-        Parse the content relevant for initializing a model from the given dictionary containing a user submitted
-        json file defining the module.
-        Initialize the model based on the found definitions.
-
-        :param model_json: submitted json object
-        :return: initialized instance of a LightningTrainModel
-        """
-        lightning_model_name = model_json["objects"]["lightning_model"]
-        lightning_model_src = model_json["src"]["lightning_model"]
-
-        ligntning_module = self._make_lightning_module(lightning_model_src, lightning_model_name)
-        return ligntning_module
-
-    @staticmethod
-    def _make_lightning_module(src: str, module_name: str) -> LightningTrainModel:
-        """
-        Creates a temporary python file based on the src code string submitted using a client library.
-        The lightning train model specified by module_name is imported and initialized from the created module and
-        returned as an in memory object.
-
-        :param src: String containing the source definition of the model
-        :param module_name: the name of the model to be imported from src
-        :return: an initialized LightningTrainModel instance based on the submitted source code
-        """
-
-        # intialize a tempfile with the model source code
-        tmp_mod = tempfile.NamedTemporaryFile("w+b", suffix=".py", delete=False)
-        tmp_mod.write(src.encode())
-        tmp_mod.read()
-
-        # initialize the temp file as a python module
-        spec = importlib.util.spec_from_file_location("lightning_model", tmp_mod.name)
-        foo = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(foo)
-
-        # Get the model by its name and initialize it
-        model: LightningTrainModel = foo.__getattribute__(module_name)()
-
-        # cleanup
-        tmp_mod.close()
-        os.unlink(tmp_mod.name)
-
-        return model
+import importlib.machinery
+import importlib.util
+import os
+import tempfile
+from typing import Any
+
+import requests
+from conductor_lib.src.torch import LightningTrainModel
+from sqlalchemy.orm import Session
+
+from station.app.crud import federated_trains
+from station.common.clients.minio import MinioClient
+
+
+class ModelLoader:
+    def __init__(self, station_url: str = None):
+        self.station_url = station_url if station_url else os.getenv("STATION_API_URL")
+        assert self.station_url
+        self.minio_client = MinioClient()
+
+    def get_model_from_station(self, model_id: str = None) -> LightningTrainModel:
+        """
+        Use the station api to get a model registered under the specified model_id and return the initialized model
+
+        :param model_id: identifier of model registered at a station
+        :return: initialized model instance stored in the db with model_id
+        """
+
+        if not model_id:
+            model_id = self.model_id
+
+        # Get the model from the station api
+        url = self.station_url + f"/api/station/models/{model_id}"
+
+        r = requests.get(url=url)
+
+        r.raise_for_status()
+        model = r.json()
+        # initialize the model based on the received src code and name
+        model = self._make_lightning_module(model["model_src"], model["model_name"])
+        return model
+
+    def load_train_model(self, db: Session, train_id: Any):
+        db_train = federated_trains.get_by_train_id(db=db, train_id=train_id)
+
+        model = db_train.model
+        assert model
+
+        lightning_module = self._make_lightning_module(
+            model.model_src, module_name=model.model_name
+        )
+        return lightning_module
+
+    def save_model_checkpoint(self):
+        # TODO
+        pass
+
+    def load_torch_model_from_json(
+        self, model_json: dict = None
+    ) -> LightningTrainModel:
+        """
+        Parse the content relevant for initializing a model from the given dictionary containing a user submitted
+        json file defining the module.
+        Initialize the model based on the found definitions.
+
+        :param model_json: submitted json object
+        :return: initialized instance of a LightningTrainModel
+        """
+        lightning_model_name = model_json["objects"]["lightning_model"]
+        lightning_model_src = model_json["src"]["lightning_model"]
+
+        ligntning_module = self._make_lightning_module(
+            lightning_model_src, lightning_model_name
+        )
+        return ligntning_module
+
+    @staticmethod
+    def _make_lightning_module(src: str, module_name: str) -> LightningTrainModel:
+        """
+        Creates a temporary python file based on the src code string submitted using a client library.
+        The lightning train model specified by module_name is imported and initialized from the created module and
+        returned as an in memory object.
+
+        :param src: String containing the source definition of the model
+        :param module_name: the name of the model to be imported from src
+        :return: an initialized LightningTrainModel instance based on the submitted source code
+        """
+
+        # intialize a tempfile with the model source code
+        tmp_mod = tempfile.NamedTemporaryFile("w+b", suffix=".py", delete=False)
+        tmp_mod.write(src.encode())
+        tmp_mod.read()
+
+        # initialize the temp file as a python module
+        spec = importlib.util.spec_from_file_location("lightning_model", tmp_mod.name)
+        foo = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(foo)
+
+        # Get the model by its name and initialize it
+        model: LightningTrainModel = foo.__getattribute__(module_name)()
+
+        # cleanup
+        tmp_mod.close()
+        os.unlink(tmp_mod.name)
+
+        return model
```

### Comparing `pht-station-0.1/station/worker/pht_worker.py` & `pht_station-0.2.0/station/worker/pht_worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,68 @@
-from typing import Any
-from sqlalchemy.orm import Session
-from dotenv import load_dotenv, find_dotenv
-import os
-
-from station.app.crud import federated_trains
-from station.worker import SessionLocal
-from station.clients.conductor import ConductorRESTClient
-from station.clients.minio import MinioClient
-from station.worker.discovery import perform_discovery
-from station.worker.loader import MinioFolderDS, BaseLoader, ModelLoader
-from station.worker.trainer import FederatedTrainer
-
-
-class PHTWorker:
-
-    def __init__(self):
-        self.conductor_client = ConductorRESTClient()
-        self.minio_client = MinioClient()
-
-    def perform_discovery(self, db: Session, train_id: Any):
-        db_train = federated_trains.get_by_train_id(db=db, train_id=train_id)
-        assert db_train.dataset
-        discovery_result = perform_discovery(db_train.dataset)
-
-        discovery_post = {
-            "station_id": os.getenv("STATION_ID"),
-            "results": discovery_result
-        }
-        self.conductor_client.post_discovery_results(train_id=train_id, discovery_results=discovery_post)
-
-    def make_data_loader(self, db: Session, train_id: Any):
-        db_train = federated_trains.get_by_train_id(db=db, train_id=train_id)
-        assert db_train.dataset
-        # TODO get configuration setting on whether to load and store the data set/loader
-        ds = MinioFolderDS(self.minio_client, data_set_id=db_train.dataset.access_path)
-        loader = BaseLoader(data_set=ds).make_data_loader()
-
-        return loader
-
-    def train_model(self, db: Session, train_id: Any):
-        model = ModelLoader().load_train_model(db, train_id)
-        print(model)
-        data_loader = self.make_data_loader(db, train_id)
-        trainer = FederatedTrainer(gpus=1, max_epochs=1)
-        trainer.fit(model=model, train_dataloader=data_loader)
-
-    def distribute_model(self, db: Session, train_id: Any):
-        pass
-
-
-if __name__ == '__main__':
-    load_dotenv(find_dotenv())
-    session = SessionLocal()
-    TRAIN_ID = "1"
-    worker = PHTWorker()
-    # worker.perform_discovery(session, TRAIN_ID)
-    # loader = worker.make_data_loader(session, TRAIN_ID)
-    worker.train_model(session, TRAIN_ID)
-
-    # for i, batch in enumerate(loader):
-    #     x, y = batch
-    #     print(y, x)
-    #     print(x.shape)
-    #     if i > 3:
-    #         break
+import os
+from typing import Any
+
+from dotenv import find_dotenv, load_dotenv
+from sqlalchemy.orm import Session
+
+from station.app.crud import federated_trains
+from station.common.clients.conductor import ConductorRESTClient
+from station.common.clients.minio import MinioClient
+from station.worker import SessionLocal
+from station.worker.discovery import perform_discovery
+from station.worker.loader import BaseLoader, MinioFolderDS, ModelLoader
+from station.worker.trainer import FederatedTrainer
+
+
+class PHTWorker:
+    def __init__(self):
+        self.conductor_client = ConductorRESTClient()
+        self.minio_client = MinioClient()
+
+    def perform_discovery(self, db: Session, train_id: Any):
+        db_train = federated_trains.get_by_train_id(db=db, train_id=train_id)
+        assert db_train.dataset
+        discovery_result = perform_discovery(db_train.dataset)
+
+        discovery_post = {
+            "station_id": os.getenv("STATION_ID"),
+            "results": discovery_result,
+        }
+        self.conductor_client.post_discovery_results(
+            train_id=train_id, discovery_results=discovery_post
+        )
+
+    def make_data_loader(self, db: Session, train_id: Any):
+        db_train = federated_trains.get_by_train_id(db=db, train_id=train_id)
+        assert db_train.dataset
+        # TODO get configuration setting on whether to load and store the data set/loader
+        ds = MinioFolderDS(self.minio_client, data_set_id=db_train.dataset.access_path)
+        loader = BaseLoader(data_set=ds).make_data_loader()
+
+        return loader
+
+    def train_model(self, db: Session, train_id: Any):
+        model = ModelLoader().load_train_model(db, train_id)
+        print(model)
+        data_loader = self.make_data_loader(db, train_id)
+        trainer = FederatedTrainer(gpus=1, max_epochs=1)
+        trainer.fit(model=model, train_dataloader=data_loader)
+
+    def distribute_model(self, db: Session, train_id: Any):
+        pass
+
+
+if __name__ == "__main__":
+    load_dotenv(find_dotenv())
+    session = SessionLocal()
+    TRAIN_ID = "1"
+    worker = PHTWorker()
+    # worker.perform_discovery(session, TRAIN_ID)
+    # loader = worker.make_data_loader(session, TRAIN_ID)
+    worker.train_model(session, TRAIN_ID)
+
+    # for i, batch in enumerate(loader):
+    #     x, y = batch
+    #     print(y, x)
+    #     print(x.shape)
+    #     if i > 3:
+    #         break
```

### Comparing `pht-station-0.1/station/worker/testing/populate_minio.py` & `pht_station-0.2.0/station/worker/testing/populate_minio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,68 @@
-import torchvision
-import os
-import pickle
-import numpy as np
-from PIL import Image as pimg
-from tqdm import tqdm
-
-MINIO_PATH = "../../../data"
-CIFAR_PATH = "../../data/cifar10/cifar-10-batches-py"
-
-
-def load_cifar_10(download=True):
-    cifar_path = os.path.join(MINIO_PATH, "cifar10")
-    batch_path = os.path.join(cifar_path, "cifar-10-batches-py")
-
-    # Download the torchvision cifar 10 dataset
-    if download:
-        torchvision.datasets.CIFAR10(cifar_path, download=True)
-
-    # Extract image data and labels from the batches
-    extract_cifar_10_batches(batch_path, cifar_path)
-
-
-def extract_cifar_10_batches(batch_path: str, out_path: str):
-    # load metadata
-    categories = pickle.load(open(os.path.join(batch_path, "batches.meta"), "rb"))["label_names"]
-    # Extract the 5 data batches
-    for i in range(5):
-
-        # create directory for batch if it doesn't exist
-        if not os.path.isdir(os.path.join(out_path, f"batch_{i + 1}")):
-            os.mkdir(os.path.join(out_path, f"batch_{i + 1}"))
-        # load batch file
-        file = f"data_batch_{i + 1}"
-        images, labels, filenames = load_cifar_pickle(batch_path, file)
-        # save images as png files
-        print(f"Extracting images for batch {i}")
-        for j, image in enumerate(tqdm(images)):
-
-            string_label = str(categories[labels[j]])
-            # Create class directory if it does not exist
-            class_dir = os.path.join(out_path, f"batch_{i + 1}", string_label)
-            if not os.path.isdir(class_dir):
-                os.mkdir(class_dir)
-            outfile = out_path + f"/batch_{i + 1}/" + string_label + "/" + str(filenames[j])
-            # Transpose image to fit regular image dimensions
-            img_array = image.transpose(1, 2, 0)
-            img = pimg.fromarray(img_array, mode="RGB")
-            img.save(outfile)
-
-
-def load_cifar_pickle(path, file):
-    f = open(os.path.join(path, file), 'rb')
-    dict = pickle.load(f, encoding="bytes")
-    images = dict[b'data']
-    images = np.reshape(images, (10000, 3, 32, 32))
-    labels = np.array(dict[b'labels'])
-    filenames = np.array((dict[b'filenames'])).astype("str")
-    return images, labels, filenames
-
-
-if __name__ == '__main__':
-    load_cifar_10(download=False)
+import os
+import pickle
+
+import numpy as np
+import torchvision
+from PIL import Image as pimg
+from tqdm import tqdm
+
+MINIO_PATH = "../../../data"
+CIFAR_PATH = "../../data/cifar10/cifar-10-batches-py"
+
+
+def load_cifar_10(download=True):
+    cifar_path = os.path.join(MINIO_PATH, "cifar10")
+    batch_path = os.path.join(cifar_path, "cifar-10-batches-py")
+
+    # Download the torchvision cifar 10 dataset
+    if download:
+        torchvision.datasets.CIFAR10(cifar_path, download=True)
+
+    # Extract image data and labels from the batches
+    extract_cifar_10_batches(batch_path, cifar_path)
+
+
+def extract_cifar_10_batches(batch_path: str, out_path: str):
+    # load metadata
+    categories = pickle.load(open(os.path.join(batch_path, "batches.meta"), "rb"))[
+        "label_names"
+    ]
+    # Extract the 5 data batches
+    for i in range(5):
+
+        # create directory for batch if it doesn't exist
+        if not os.path.isdir(os.path.join(out_path, f"batch_{i + 1}")):
+            os.mkdir(os.path.join(out_path, f"batch_{i + 1}"))
+        # load batch file
+        file = f"data_batch_{i + 1}"
+        images, labels, filenames = load_cifar_pickle(batch_path, file)
+        # save images as png files
+        print(f"Extracting images for batch {i}")
+        for j, image in enumerate(tqdm(images)):
+
+            string_label = str(categories[labels[j]])
+            # Create class directory if it does not exist
+            class_dir = os.path.join(out_path, f"batch_{i + 1}", string_label)
+            if not os.path.isdir(class_dir):
+                os.mkdir(class_dir)
+            outfile = (
+                out_path + f"/batch_{i + 1}/" + string_label + "/" + str(filenames[j])
+            )
+            # Transpose image to fit regular image dimensions
+            img_array = image.transpose(1, 2, 0)
+            img = pimg.fromarray(img_array, mode="RGB")
+            img.save(outfile)
+
+
+def load_cifar_pickle(path, file):
+    f = open(os.path.join(path, file), "rb")
+    dict = pickle.load(f, encoding="bytes")
+    images = dict[b"data"]
+    images = np.reshape(images, (10000, 3, 32, 32))
+    labels = np.array(dict[b"labels"])
+    filenames = np.array((dict[b"filenames"])).astype("str")
+    return images, labels, filenames
+
+
+if __name__ == "__main__":
+    load_cifar_10(download=False)
```

### Comparing `pht-station-0.1/station/worker/testing/train_lightning_model.py` & `pht_station-0.2.0/station/worker/testing/train_lightning_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-from conductor_lib.src.torch import LightningTrainModel
-import torch.nn as nn
-import torch.nn.functional as F
-import torch.optim as optim
-
-from torchvision import transforms
-
-
-class Cifar10Model(LightningTrainModel):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.conv1 = nn.Conv2d(3, 6, 5)
-        self.pool = nn.MaxPool2d(2, 2)
-        self.conv2 = nn.Conv2d(6, 16, 5)
-        self.fc1 = nn.Linear(16 * 5 * 5, 120)
-        self.fc2 = nn.Linear(120, 84)
-        self.fc3 = nn.Linear(84, 10)
-
-    def forward(self, x):
-        x = self.pool(F.relu(self.conv1(x)))
-        x = self.pool(F.relu(self.conv2(x)))
-        x = x.view(-1, 16 * 5 * 5)
-        x = F.relu(self.fc1(x))
-        x = F.relu(self.fc2(x))
-        x = self.fc3(x)
-        return x
-
-    def training_step(self, batch, batch_idx):
-        x, y = batch
-        y_hat = self.forward(x)
-
-        loss = F.cross_entropy(y_hat, y)
-        return loss
-
-    def configure_optimizers(self):
-        return optim.SGD(self.parameters(), lr=0.001, momentum=0.9)
-
-    def make_transform(self) -> transforms.Compose:
-        transform = transforms.Compose(
-            [transforms.ToTensor(),
-             transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))])
-
-        return transform
+import torch.nn as nn
+import torch.nn.functional as F
+import torch.optim as optim
+from conductor_lib.src.torch import LightningTrainModel
+from torchvision import transforms
+
+
+class Cifar10Model(LightningTrainModel):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.conv1 = nn.Conv2d(3, 6, 5)
+        self.pool = nn.MaxPool2d(2, 2)
+        self.conv2 = nn.Conv2d(6, 16, 5)
+        self.fc1 = nn.Linear(16 * 5 * 5, 120)
+        self.fc2 = nn.Linear(120, 84)
+        self.fc3 = nn.Linear(84, 10)
+
+    def forward(self, x):
+        x = self.pool(F.relu(self.conv1(x)))
+        x = self.pool(F.relu(self.conv2(x)))
+        x = x.view(-1, 16 * 5 * 5)
+        x = F.relu(self.fc1(x))
+        x = F.relu(self.fc2(x))
+        x = self.fc3(x)
+        return x
+
+    def training_step(self, batch, batch_idx):
+        x, y = batch
+        y_hat = self.forward(x)
+
+        loss = F.cross_entropy(y_hat, y)
+        return loss
+
+    def configure_optimizers(self):
+        return optim.SGD(self.parameters(), lr=0.001, momentum=0.9)
+
+    def make_transform(self) -> transforms.Compose:
+        transform = transforms.Compose(
+            [
+                transforms.ToTensor(),
+                transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5)),
+            ]
+        )
+
+        return transform
```

### Comparing `pht-station-0.1/station/worker/trainer/base_trainer.py` & `pht_station-0.2.0/station/worker/trainer/base_trainer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,75 @@
-from station.clients.minio import MinioClient
-from conductor_lib.src.torch import LightningTrainModel
-from typing import Union
-import os
-from torch.utils.data import DataLoader
-
-from station.worker.loader import BaseLoader
-
-
-class ModelTrainer:
-
-    def __init__(self, model_id: str = None, data_set_id: str = None, station_url: str = None):
-        """
-        Initialize a model trainer instance with a model and data set id
-
-        :param model_id:
-        :param data_set_id:
-        :param station_url:
-        """
-        self.model_id = model_id
-        self.station_url = station_url if station_url else os.getenv("STATION_API_URL")
-        assert self.station_url
-        self.model: LightningTrainModel = None
-        # TODO fix minio
-        self.data_set_id = data_set_id
-        self.minio_client = MinioClient(minio_server="localhost:9000",
-                                        secret_key="minio_admin", access_key="minio_admin")
-
-    def train_model(self, train_args: dict = None):
-        pass
-
-    def prepare_torch_data_loader(self,
-                                  data_set_id: str = None,
-                                  path: Union[str, os.PathLike] = None,
-                                  data_config: dict = None) -> DataLoader:
-        """
-        Create a pytorch data loader based on a specified data set id or path, applies the transforms specified
-        in the lightning model to the created data set
-
-        :param data_set_id: identifier for a data set registered at the station
-        :param path: path to directory accessible to the trainer where the raw data for the data set is stored
-        :param data_config: dictionary containing additional configuration parameters for the data set
-        :return:
-        """
-        if path:
-            # TODO Load data from file system
-            raise NotImplementedError("Only Minio based data sets available")
-        else:
-
-            # TODO use station api to get the relevant information for a data set from the db
-            if data_set_id:
-                self.data_set_id = data_set_id
-            # create a loader that will handle loading and preparing the data from Minio
-            base_loader = BaseLoader(data_set=data_set_id,
-                                     station_api=self.station_url,
-                                     config=data_config,
-                                     transform=self.model.make_transform())
-            data_loader = base_loader.make_data_loader()
-            return data_loader
-
-
-if __name__ == '__main__':
-    model_id = "af8c8b1e-3d89-4500-bc7d-7888e13381bd"
-
-    trainer = ModelTrainer(model_id=model_id, station_url="http://localhost:8001")
-    db_model = trainer.get_model_from_station(model_id=model_id)
-    print(db_model)
+import os
+from typing import Union
+
+from conductor_lib.src.torch import LightningTrainModel
+from torch.utils.data import DataLoader
+
+from station.common.clients.minio import MinioClient
+from station.worker.loader import BaseLoader
+
+
+class ModelTrainer:
+    def __init__(
+        self, model_id: str = None, data_set_id: str = None, station_url: str = None
+    ):
+        """
+        Initialize a model trainer instance with a model and data set id
+
+        :param model_id:
+        :param data_set_id:
+        :param station_url:
+        """
+        self.model_id = model_id
+        self.station_url = station_url if station_url else os.getenv("STATION_API_URL")
+        assert self.station_url
+        self.model: LightningTrainModel = None
+        # TODO fix minio
+        self.data_set_id = data_set_id
+        self.minio_client = MinioClient(
+            minio_server="localhost:9000",
+            secret_key="minio_admin",
+            access_key="minio_admin",
+        )
+
+    def train_model(self, train_args: dict = None):
+        pass
+
+    def prepare_torch_data_loader(
+        self,
+        data_set_id: str = None,
+        path: Union[str, os.PathLike] = None,
+        data_config: dict = None,
+    ) -> DataLoader:
+        """
+        Create a pytorch data loader based on a specified data set id or path, applies the transforms specified
+        in the lightning model to the created data set
+
+        :param data_set_id: identifier for a data set registered at the station
+        :param path: path to directory accessible to the trainer where the raw data for the data set is stored
+        :param data_config: dictionary containing additional configuration parameters for the data set
+        :return:
+        """
+        if path:
+            # TODO Load data from file system
+            raise NotImplementedError("Only Minio based data sets available")
+        else:
+            # TODO use station api to get the relevant information for a data set from the db
+            if data_set_id:
+                self.data_set_id = data_set_id
+            # create a loader that will handle loading and preparing the data from Minio
+            base_loader = BaseLoader(
+                data_set=data_set_id,
+                station_api=self.station_url,
+                config=data_config,
+                transform=self.model.make_transform(),
+            )
+            data_loader = base_loader.make_data_loader()
+            return data_loader
+
+
+if __name__ == "__main__":
+    model_id = "af8c8b1e-3d89-4500-bc7d-7888e13381bd"
+
+    trainer = ModelTrainer(model_id=model_id, station_url="http://localhost:8001")
+    db_model = trainer.get_model_from_station(model_id=model_id)
+    print(db_model)
```

