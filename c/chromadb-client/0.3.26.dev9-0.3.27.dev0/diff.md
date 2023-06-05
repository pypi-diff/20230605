# Comparing `tmp/chromadb-client-0.3.26.dev9.tar.gz` & `tmp/chromadb-client-0.3.27.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-client-0.3.26.dev9.tar", last modified: Wed May 24 20:22:06 2023, max compression
+gzip compressed data, was "chromadb-client-0.3.27.dev0.tar", last modified: Mon Jun  5 18:02:18 2023, max compression
```

## Comparing `chromadb-client-0.3.26.dev9.tar` & `chromadb-client-0.3.27.dev0.tar`

### file list

```diff
@@ -1,194 +1,231 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.696671 chromadb-client-0.3.26.dev9/
--rw-r--r--   0 hammad     (501) staff       (20)       84 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.dockerignore
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.672731 chromadb-client-0.3.26.dev9/.github/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.678024 chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 hammad     (501) staff       (20)     1512 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 hammad     (501) staff       (20)     1520 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 hammad     (501) staff       (20)     1384 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.678737 chromadb-client-0.3.26.dev9/.github/workflows/
--rw-r--r--   0 hammad     (501) staff       (20)     1187 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 hammad     (501) staff       (20)     1321 2023-05-24 20:17:49.000000 chromadb-client-0.3.26.dev9/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 hammad     (501) staff       (20)     4169 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.github/workflows/chroma-release.yml
--rw-r--r--   0 hammad     (501) staff       (20)     1205 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.github/workflows/chroma-test.yml
--rw-r--r--   0 hammad     (501) staff       (20)     1734 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 hammad     (501) staff       (20)      228 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/.gitignore
--rw-r--r--   0 hammad     (501) staff       (20)     1030 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/.pre-commit-config.yaml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.678848 chromadb-client-0.3.26.dev9/.vscode/
--rw-r--r--   0 hammad     (501) staff       (20)      978 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/.vscode/settings.json
--rw-r--r--   0 hammad     (501) staff       (20)     3323 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/DEVELOP.md
--rw-r--r--   0 hammad     (501) staff       (20)      619 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/Dockerfile
--rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-02-13 21:59:42.000000 chromadb-client-0.3.26.dev9/LICENSE
--rw-r--r--   0 hammad     (501) staff       (20)     2109 2023-05-24 20:22:06.696530 chromadb-client-0.3.26.dev9/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)     1559 2023-05-24 20:22:04.000000 chromadb-client-0.3.26.dev9/README.md
--rw-r--r--   0 hammad     (501) staff       (20)      619 2023-03-30 18:05:39.000000 chromadb-client-0.3.26.dev9/RELEASE_PROCESS.md
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.680522 chromadb-client-0.3.26.dev9/bin/
--rw-r--r--   0 hammad     (501) staff       (20)     1610 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/backup.sh
--rwxr-xr-x   0 hammad     (501) staff       (20)      110 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev9/bin/build
--rwxr-xr-x   0 hammad     (501) staff       (20)      234 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev9/bin/docker_entrypoint.sh
--rw-r--r--   0 hammad     (501) staff       (20)     6462 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/generate_cloudformation.py
--rwxr-xr-x   0 hammad     (501) staff       (20)      463 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/integration-test
--rw-r--r--   0 hammad     (501) staff       (20)     1688 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/restore.sh
--rw-r--r--   0 hammad     (501) staff       (20)     1105 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/setup_linux.sh
--rw-r--r--   0 hammad     (501) staff       (20)      451 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/setup_mac.sh
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.680657 chromadb-client-0.3.26.dev9/bin/templates/
--rw-r--r--   0 hammad     (501) staff       (20)      985 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev9/bin/templates/docker-compose.yml
--rwxr-xr-x   0 hammad     (501) staff       (20)      451 2023-05-12 22:12:15.000000 chromadb-client-0.3.26.dev9/bin/test-package.sh
--rwxr-xr-x   0 hammad     (501) staff       (20)      297 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/test-remote
--rw-r--r--   0 hammad     (501) staff       (20)      205 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/test.py
--rwxr-xr-x   0 hammad     (501) staff       (20)      151 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/bin/version
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.681349 chromadb-client-0.3.26.dev9/chromadb/
--rw-r--r--   0 hammad     (501) staff       (20)      895 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.681899 chromadb-client-0.3.26.dev9/chromadb/api/
--rw-r--r--   0 hammad     (501) staff       (20)    10960 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/chromadb/api/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)    12141 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/chromadb/api/fastapi.py
--rw-r--r--   0 hammad     (501) staff       (20)    17500 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/chromadb/api/local.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.682050 chromadb-client-0.3.26.dev9/chromadb/api/models/
--rw-r--r--   0 hammad     (501) staff       (20)    15170 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/chromadb/api/models/Collection.py
--rw-r--r--   0 hammad     (501) staff       (20)    10780 2023-05-19 22:52:05.000000 chromadb-client-0.3.26.dev9/chromadb/api/types.py
--rw-r--r--   0 hammad     (501) staff       (20)      168 2023-03-24 17:22:43.000000 chromadb-client-0.3.26.dev9/chromadb/app.py
--rw-r--r--   0 hammad     (501) staff       (20)     4195 2023-05-24 20:12:36.000000 chromadb-client-0.3.26.dev9/chromadb/config.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.682700 chromadb-client-0.3.26.dev9/chromadb/db/
--rw-r--r--   0 hammad     (501) staff       (20)     3260 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/db/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     4816 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/chromadb/db/base.py
--rw-r--r--   0 hammad     (501) staff       (20)    21674 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/db/clickhouse.py
--rw-r--r--   0 hammad     (501) staff       (20)    17967 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/db/duckdb.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.682968 chromadb-client-0.3.26.dev9/chromadb/db/impl/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/db/impl/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     4766 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/db/impl/sqlite.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.683233 chromadb-client-0.3.26.dev9/chromadb/db/index/
--rw-r--r--   0 hammad     (501) staff       (20)      447 2023-03-30 18:05:39.000000 chromadb-client-0.3.26.dev9/chromadb/db/index/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)    11060 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/chromadb/db/index/hnswlib.py
--rw-r--r--   0 hammad     (501) staff       (20)     8090 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/db/migrations.py
--rw-r--r--   0 hammad     (501) staff       (20)     1293 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/chromadb/errors.py
--rw-r--r--   0 hammad     (501) staff       (20)       22 2023-05-24 20:22:04.000000 chromadb-client-0.3.26.dev9/chromadb/is_thin_client.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.683372 chromadb-client-0.3.26.dev9/chromadb/server/
--rw-r--r--   0 hammad     (501) staff       (20)      172 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/server/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.683618 chromadb-client-0.3.26.dev9/chromadb/server/fastapi/
--rw-r--r--   0 hammad     (501) staff       (20)     9064 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     2134 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.683982 chromadb-client-0.3.26.dev9/chromadb/telemetry/
--rw-r--r--   0 hammad     (501) staff       (20)     3165 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/telemetry/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)      591 2023-03-26 23:12:08.000000 chromadb-client-0.3.26.dev9/chromadb/telemetry/events.py
--rw-r--r--   0 hammad     (501) staff       (20)     1083 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.684399 chromadb-client-0.3.26.dev9/chromadb/test/
--rw-r--r--   0 hammad     (501) staff       (20)     3110 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/conftest.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.684654 chromadb-client-0.3.26.dev9/chromadb/test/db/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.685436 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 hammad     (501) staff       (20)       51 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 hammad     (501) staff       (20)     1168 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/test_base.py
--rw-r--r--   0 hammad     (501) staff       (20)     4999 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/test/db/test_migrations.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.685555 chromadb-client-0.3.26.dev9/chromadb/test/hnswlib/
--rw-r--r--   0 hammad     (501) staff       (20)     2337 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/hnswlib/test_hnswlib.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.686491 chromadb-client-0.3.26.dev9/chromadb/test/property/
--rw-r--r--   0 hammad     (501) staff       (20)     9698 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/invariants.py
--rw-r--r--   0 hammad     (501) staff       (20)    15532 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/strategies.py
--rw-r--r--   0 hammad     (501) staff       (20)     1942 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_add.py
--rw-r--r--   0 hammad     (501) staff       (20)     6211 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_collections.py
--rw-r--r--   0 hammad     (501) staff       (20)     8333 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 hammad     (501) staff       (20)     9590 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 hammad     (501) staff       (20)     6297 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_filtering.py
--rw-r--r--   0 hammad     (501) staff       (20)     4899 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/chromadb/test/property/test_persist.py
--rw-r--r--   0 hammad     (501) staff       (20)    40187 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/chromadb/test/test_api.py
--rw-r--r--   0 hammad     (501) staff       (20)     2195 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/chromadb/test/test_chroma.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.686711 chromadb-client-0.3.26.dev9/chromadb/utils/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2023-03-25 00:05:13.000000 chromadb-client-0.3.26.dev9/chromadb/utils/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)    16026 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/chromadb/utils/embedding_functions.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.687353 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)     2109 2023-05-24 20:22:06.000000 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)     4875 2023-05-24 20:22:06.000000 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2023-05-24 20:22:06.000000 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)      112 2023-05-24 20:22:06.000000 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        9 2023-05-24 20:22:06.000000 chromadb-client-0.3.26.dev9/chromadb_client.egg-info/top_level.txt
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.675142 chromadb-client-0.3.26.dev9/clients/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.689580 chromadb-client-0.3.26.dev9/clients/js/
--rw-r--r--   0 hammad     (501) staff       (20)       66 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/.gitignore
--rw-r--r--   0 hammad     (501) staff       (20)       32 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/.prettierignore
--rw-r--r--   0 hammad     (501) staff       (20)        3 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/.prettierrc.json
--rw-r--r--   0 hammad     (501) staff       (20)     1200 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/DEVELOP.md
--rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/LICENSE
--rw-r--r--   0 hammad     (501) staff       (20)     1266 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/README.md
--rw-r--r--   0 hammad     (501) staff       (20)      324 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/config.yml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.674574 chromadb-client-0.3.26.dev9/clients/js/examples/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.690307 chromadb-client-0.3.26.dev9/clients/js/examples/browser/
--rw-r--r--   0 hammad     (501) staff       (20)      358 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/examples/browser/README.md
--rw-r--r--   0 hammad     (501) staff       (20)     1690 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/examples/browser/app.ts
--rw-r--r--   0 hammad     (501) staff       (20)      834 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/examples/browser/index.html
--rw-r--r--   0 hammad     (501) staff       (20)      409 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/examples/browser/package.json
--rw-r--r--   0 hammad     (501) staff       (20)    71072 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.690946 chromadb-client-0.3.26.dev9/clients/js/examples/node/
--rw-r--r--   0 hammad     (501) staff       (20)       57 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/examples/node/README.md
--rw-r--r--   0 hammad     (501) staff       (20)     1191 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/examples/node/app.js
--rw-r--r--   0 hammad     (501) staff       (20)    46542 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/examples/node/package-lock.json
--rw-r--r--   0 hammad     (501) staff       (20)      503 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/examples/node/package.json
--rw-r--r--   0 hammad     (501) staff       (20)    17116 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 hammad     (501) staff       (20)     1075 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/genapi.sh
--rw-r--r--   0 hammad     (501) staff       (20)      469 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/jest.config.ts
--rw-r--r--   0 hammad     (501) staff       (20)      153 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/openapitools.json
--rw-r--r--   0 hammad     (501) staff       (20)   450648 2023-02-27 17:19:35.000000 chromadb-client-0.3.26.dev9/clients/js/package-lock.json
--rw-r--r--   0 hammad     (501) staff       (20)     1401 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/clients/js/package.json
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.691580 chromadb-client-0.3.26.dev9/clients/js/src/
--rw-r--r--   0 hammad     (501) staff       (20)     8084 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/ChromaClient.ts
--rw-r--r--   0 hammad     (501) staff       (20)    19403 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/clients/js/src/Collection.ts
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.692004 chromadb-client-0.3.26.dev9/clients/js/src/embeddings/
--rw-r--r--   0 hammad     (501) staff       (20)      937 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 hammad     (501) staff       (20)       91 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 hammad     (501) staff       (20)     1562 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.692839 chromadb-client-0.3.26.dev9/clients/js/src/generated/
--rw-r--r--   0 hammad     (501) staff       (20)      921 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/README.md
--rw-r--r--   0 hammad     (501) staff       (20)    56700 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/api.ts
--rw-r--r--   0 hammad     (501) staff       (20)     1478 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/configuration.ts
--rw-r--r--   0 hammad     (501) staff       (20)      429 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/index.ts
--rw-r--r--   0 hammad     (501) staff       (20)     5862 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/models.ts
--rw-r--r--   0 hammad     (501) staff       (20)     1307 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/src/generated/runtime.ts
--rw-r--r--   0 hammad     (501) staff       (20)      320 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/index.ts
--rw-r--r--   0 hammad     (501) staff       (20)     1719 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/types.ts
--rw-r--r--   0 hammad     (501) staff       (20)     2001 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/src/utils.ts
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.694569 chromadb-client-0.3.26.dev9/clients/js/test/
--rw-r--r--   0 hammad     (501) staff       (20)     2625 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/add.collections.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     7586 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/clients/js/test/client.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     3284 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/collection.client.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     2551 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)      451 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/test/data.ts
--rw-r--r--   0 hammad     (501) staff       (20)      711 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     2381 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/clients/js/test/get.collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)      206 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/initClient.ts
--rw-r--r--   0 hammad     (501) staff       (20)      577 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     1990 2023-05-19 21:55:12.000000 chromadb-client-0.3.26.dev9/clients/js/test/query.collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)     2160 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/update.collection.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)      802 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 hammad     (501) staff       (20)      367 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/clients/js/tsconfig.json
--rw-r--r--   0 hammad     (501) staff       (20)      110 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/tsconfig.module.json
--rw-r--r--   0 hammad     (501) staff       (20)   157735 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/clients/js/yarn.lock
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.695065 chromadb-client-0.3.26.dev9/clients/python/
--rw-r--r--   0 hammad     (501) staff       (20)     1559 2023-05-24 17:49:30.000000 chromadb-client-0.3.26.dev9/clients/python/README.md
--rwxr-xr-x   0 hammad     (501) staff       (20)     1203 2023-05-24 17:49:03.000000 chromadb-client-0.3.26.dev9/clients/python/build_python_thin_client.sh
--rw-r--r--   0 hammad     (501) staff       (20)       22 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/clients/python/is_thin_client.py
--rw-r--r--   0 hammad     (501) staff       (20)     1166 2023-05-23 22:03:26.000000 chromadb-client-0.3.26.dev9/clients/python/pyproject.toml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.695292 chromadb-client-0.3.26.dev9/config/
--rw-r--r--   0 hammad     (501) staff       (20)      385 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/config/backup_disk.xml
--rw-r--r--   0 hammad     (501) staff       (20)      233 2023-03-06 21:32:56.000000 chromadb-client-0.3.26.dev9/config/chroma_users.xml
--rw-r--r--   0 hammad     (501) staff       (20)     1080 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/docker-compose.server.example.yml
--rw-r--r--   0 hammad     (501) staff       (20)     1230 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/docker-compose.test.yml
--rw-r--r--   0 hammad     (501) staff       (20)     1226 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/docker-compose.yml
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.695694 chromadb-client-0.3.26.dev9/examples/
--rw-r--r--   0 hammad     (501) staff       (20)    10346 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/examples/alternative_embeddings.ipynb
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.675509 chromadb-client-0.3.26.dev9/examples/deployments/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-05-24 20:22:06.696348 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/
--rw-r--r--   0 hammad     (501) staff       (20)      611 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 hammad     (501) staff       (20)      444 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 hammad     (501) staff       (20)      125 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 hammad     (501) staff       (20)     2237 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 hammad     (501) staff       (20)      181 2023-03-30 18:55:40.000000 chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/variables.tf
--rw-r--r--   0 hammad     (501) staff       (20)     5830 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/examples/local_persistence.ipynb
--rw-r--r--   0 hammad     (501) staff       (20)     5493 2023-05-18 17:34:58.000000 chromadb-client-0.3.26.dev9/examples/where_filtering.ipynb
--rw-r--r--   0 hammad     (501) staff       (20)      495 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/log_config.yml
--rw-r--r--   0 hammad     (501) staff       (20)      372 2023-05-19 05:51:23.000000 chromadb-client-0.3.26.dev9/pull_request_template.md
--rw-r--r--   0 hammad     (501) staff       (20)     1166 2023-05-24 20:22:04.000000 chromadb-client-0.3.26.dev9/pyproject.toml
--rw-r--r--   0 hammad     (501) staff       (20)      312 2023-05-23 22:03:28.000000 chromadb-client-0.3.26.dev9/requirements.txt
--rw-r--r--   0 hammad     (501) staff       (20)      146 2023-05-19 05:51:31.000000 chromadb-client-0.3.26.dev9/requirements_dev.txt
--rw-r--r--   0 hammad     (501) staff       (20)       38 2023-05-24 20:22:06.696710 chromadb-client-0.3.26.dev9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.518897 chromadb-client-0.3.27.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.522897 chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/chroma-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/chroma-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-05 18:02:13.000000 chromadb-client-0.3.27.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/RELEASE_PROCESS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/backup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/docker_entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/generate_cloudformation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/integration-test
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/restore.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/setup_linux.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/setup_mac.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/bin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/test-package.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      297 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/test-remote
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/bin/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/chromadb/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/chromadb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12480 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/api/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/api/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.526897 chromadb-client-0.3.27.dev0/chromadb/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/api/models/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22262 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/db/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/impl/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/db/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/index/hnswlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/db/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/db/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/ingest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 18:02:13.000000 chromadb-client-0.3.27.dev0/chromadb/is_thin_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.518897 chromadb-client-0.3.27.dev0/chromadb/segment/impl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/segment/impl/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/segment/impl/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    17879 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/segment/impl/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/segment/impl/vector/local_hnsw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.530897 chromadb-client-0.3.27.dev0/chromadb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.534897 chromadb-client-0.3.27.dev0/chromadb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.534897 chromadb-client-0.3.27.dev0/chromadb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.534897 chromadb-client-0.3.27.dev0/chromadb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.534897 chromadb-client-0.3.27.dev0/chromadb/test/db/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.534897 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/db/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/test/hnswlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/hnswlib/test_hnswlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/test/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/test/property/
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/test/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15026 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/segment/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40112 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/test_chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.538897 chromadb-client-0.3.27.dev0/chromadb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/chromadb/utils/messageid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.542897 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-05 18:02:18.000000 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-05 18:02:18.000000 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:02:18.000000 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 18:02:18.000000 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 18:02:18.000000 chromadb-client-0.3.27.dev0/chromadb_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.522897 chromadb-client-0.3.27.dev0/clients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.546897 chromadb-client-0.3.27.dev0/clients/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/.prettierrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.522897 chromadb-client-0.3.27.dev0/clients/js/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.546897 chromadb-client-0.3.27.dev0/clients/js/examples/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/browser/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/browser/app.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/browser/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/browser/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71072 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.546897 chromadb-client-0.3.27.dev0/clients/js/examples/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/node/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)    46542 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/node/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/node/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1075 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/genapi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/jest.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/openapitools.json
+-rw-r--r--   0 runner    (1001) docker     (123)   450648 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.546897 chromadb-client-0.3.27.dev0/clients/js/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    19403 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/Collection.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/clients/js/src/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/clients/js/src/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    56700 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/api.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/models.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/types.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/src/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/clients/js/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/data.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/initClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/tsconfig.module.json
+-rw-r--r--   0 runner    (1001) docker     (123)   157735 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/js/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/clients/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/python/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/python/integration-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/python/is_thin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/clients/python/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/config/backup_disk.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/config/chroma_users.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/docker-compose.server.example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/docker-compose.test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/alternative_embeddings.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.522897 chromadb-client-0.3.27.dev0/examples/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.550897 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/variables.tf
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/local_persistence.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/examples/where_filtering.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/log_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.522897 chromadb-client-0.3.27.dev0/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/migrations/embeddings_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/migrations/metadb/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/migrations/metadb/00001-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/migrations/sysdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 18:02:13.000000 chromadb-client-0.3.27.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-05 18:02:02.000000 chromadb-client-0.3.27.dev0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 18:02:18.554897 chromadb-client-0.3.27.dev0/setup.cfg
```

### Comparing `chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/bug_report.yaml` & `chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/feature_request.yaml` & `chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `chromadb-client-0.3.27.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/.github/workflows/chroma-integration-test.yml` & `chromadb-client-0.3.27.dev0/.github/workflows/chroma-integration-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/.github/workflows/chroma-release-python-client.yml` & `chromadb-client-0.3.27.dev0/.github/workflows/chroma-release-python-client.yml`

 * *Files 5% similar despite different names*

```diff
@@ -38,8 +38,8 @@
       with:
         password: ${{ secrets.TEST_PYPI_PYTHON_CLIENT_PUBLISH_KEY }}
         repository_url: https://test.pypi.org/legacy/
     - name: Publish to PyPI
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
-        password: ${{ secrets.PYPI_API_TOKEN }}
+        password: ${{ secrets.PYPI_PYTHON_CLIENT_PUBLISH_KEY }}
```

### Comparing `chromadb-client-0.3.26.dev9/.github/workflows/chroma-release.yml` & `chromadb-client-0.3.27.dev0/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/.github/workflows/chroma-test.yml` & `chromadb-client-0.3.27.dev0/.github/workflows/chroma-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/.github/workflows/pr-review-checklist.yml` & `chromadb-client-0.3.27.dev0/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/.vscode/settings.json` & `chromadb-client-0.3.27.dev0/.vscode/settings.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666666%*

 * *Differences: {"'python.linting.mypyArgs'": "{insert: [(5, '--disable-error-code=type-abstract')]}"}*

```diff
@@ -22,15 +22,16 @@
     ],
     "python.linting.flake8Enabled": true,
     "python.linting.mypyArgs": [
         "--follow-imports=silent",
         "--ignore-missing-imports",
         "--show-column-numbers",
         "--no-pretty",
-        "--strict"
+        "--strict",
+        "--disable-error-code=type-abstract"
     ],
     "python.linting.mypyCategorySeverity.note": "Error",
     "python.linting.mypyEnabled": true,
     "python.testing.pytestArgs": [
         "."
     ],
     "python.testing.pytestEnabled": true,
```

### Comparing `chromadb-client-0.3.26.dev9/DEVELOP.md` & `chromadb-client-0.3.27.dev0/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/Dockerfile` & `chromadb-client-0.3.27.dev0/Dockerfile`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/LICENSE` & `chromadb-client-0.3.27.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/PKG-INFO` & `chromadb-client-0.3.27.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb-client
-Version: 0.3.26.dev9
+Version: 0.3.27.dev0
 Summary: Chroma Client.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,17 @@
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest", chroma_server_host="localhost", chroma_server_port=8000))
+client = chromadb.Client(Settings(chroma_api_impl="rest",
+                                  chroma_server_host="localhost",
+                                  chroma_server_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.26.dev9 Summary:
+Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.27.dev0 Summary:
 Chroma Client. Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-client-0.3.26.dev9/README.md` & `chromadb-client-0.3.27.dev0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest", chroma_server_host="localhost", chroma_server_port=8000))
+client = chromadb.Client(Settings(chroma_api_impl="rest",
+                                  chroma_server_host="localhost",
+                                  chroma_server_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

### Comparing `chromadb-client-0.3.26.dev9/RELEASE_PROCESS.md` & `chromadb-client-0.3.27.dev0/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/bin/backup.sh` & `chromadb-client-0.3.27.dev0/bin/backup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/bin/generate_cloudformation.py` & `chromadb-client-0.3.27.dev0/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/bin/restore.sh` & `chromadb-client-0.3.27.dev0/bin/restore.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/bin/setup_linux.sh` & `chromadb-client-0.3.27.dev0/bin/setup_linux.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/bin/templates/docker-compose.yml` & `chromadb-client-0.3.27.dev0/bin/templates/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb/__init__.py` & `chromadb-client-0.3.27.dev0/chromadb/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import chromadb.config
 import logging
 from chromadb.telemetry.events import ClientStartEvent
+from chromadb.telemetry import Telemetry
 from chromadb.config import Settings, System
 from chromadb.api import API
 
 logger = logging.getLogger(__name__)
 
 __settings = Settings()
 
-__version__ = "0.3.25"
+__version__ = "0.3.26"
 
 
 def configure(**kwargs) -> None:  # type: ignore
     """Override Chroma's default settings, environment variables or .env files"""
     global __settings
     __settings = chromadb.config.Settings(**kwargs)
 
 
 def get_settings() -> Settings:
     return __settings
 
 
 def Client(settings: Settings = __settings) -> API:
-    """Return a chroma.API instance based on the provided or environmental
-    settings, optionally overriding the DB instance."""
+    """Return a running chroma.API instance"""
 
     system = System(settings)
 
-    telemetry_client = system.get_telemetry()
+    telemetry_client = system.instance(Telemetry)
+    api = system.instance(API)
+
+    system.start()
 
     # Submit event for client start
     telemetry_client.capture(ClientStartEvent())
 
-    return system.get_api()
+    return api
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/api/__init__.py` & `chromadb-client-0.3.27.dev0/chromadb/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,20 @@
     Include,
     Metadatas,
     Where,
     QueryResult,
     GetResult,
     WhereDocument,
 )
+from chromadb.config import Component
 import chromadb.utils.embedding_functions as ef
-from chromadb.telemetry import Telemetry
+from overrides import override
 
 
-class API(ABC):
-    @abstractmethod
-    def __init__(self, telemetry_client: Telemetry):
-        pass
-
+class API(Component, ABC):
     @abstractmethod
     def heartbeat(self) -> int:
         """Returns the current server time in nanoseconds to check if the server is alive
 
         Args:
             None
 
@@ -285,23 +282,24 @@
         Args:
             embedding: The embedding to find the nearest neighbors of
             n_results: The number of nearest neighbors to return. Defaults to 10.
             where: A dictionary of key-value pairs to filter the embeddings by. Defaults to {}.
         """
         pass
 
+    @override
     @abstractmethod
-    def reset(self) -> bool:
+    def reset(self) -> None:
         """Resets the database
         ⚠️ This is destructive and will delete all data in the database.
         Args:
             None
 
         Returns:
-            True if the reset was successful
+            None
         """
         pass
 
     @abstractmethod
     def raw_sql(self, sql: str) -> pd.DataFrame:
         """Runs a raw SQL query against the database
         ⚠️ This method should not be used directly.
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/api/fastapi.py` & `chromadb-client-0.3.27.dev0/chromadb/api/fastapi.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,41 +18,47 @@
 import pandas as pd
 import requests
 import json
 from typing import Sequence
 from chromadb.api.models.Collection import Collection
 import chromadb.errors as errors
 from uuid import UUID
+from chromadb.telemetry import Telemetry
+from overrides import override
 
 
 class FastAPI(API):
     def __init__(self, system: System):
+        super().__init__(system)
         url_prefix = "https" if system.settings.chroma_server_ssl_enabled else "http"
         system.settings.require("chroma_server_host")
         system.settings.require("chroma_server_http_port")
         self._api_url = f"{url_prefix}://{system.settings.chroma_server_host}:{system.settings.chroma_server_http_port}/api/v1"
-        self._telemetry_client = system.get_telemetry()
+        self._telemetry_client = self.require(Telemetry)
 
+    @override
     def heartbeat(self) -> int:
         """Returns the current server time in nanoseconds to check if the server is alive"""
         resp = requests.get(self._api_url)
         raise_chroma_error(resp)
         return int(resp.json()["nanosecond heartbeat"])
 
+    @override
     def list_collections(self) -> Sequence[Collection]:
         """Returns a list of all collections"""
         resp = requests.get(self._api_url + "/collections")
         raise_chroma_error(resp)
         json_collections = resp.json()
         collections = []
         for json_collection in json_collections:
             collections.append(Collection(self, **json_collection))
 
         return collections
 
+    @override
     def create_collection(
         self,
         name: str,
         metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
         get_or_create: bool = False,
     ) -> Collection:
@@ -69,14 +75,15 @@
             client=self,
             id=resp_json["id"],
             name=resp_json["name"],
             embedding_function=embedding_function,
             metadata=resp_json["metadata"],
         )
 
+    @override
     def get_collection(
         self,
         name: str,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
         """Returns a collection"""
         resp = requests.get(self._api_url + "/collections/" + name)
@@ -86,59 +93,65 @@
             client=self,
             name=resp_json["name"],
             id=resp_json["id"],
             embedding_function=embedding_function,
             metadata=resp_json["metadata"],
         )
 
+    @override
     def get_or_create_collection(
         self,
         name: str,
         metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
         """Get a collection, or return it if it exists"""
 
         return self.create_collection(
             name, metadata, embedding_function, get_or_create=True
         )
 
+    @override
     def _modify(
         self,
         id: UUID,
         new_name: Optional[str] = None,
         new_metadata: Optional[CollectionMetadata] = None,
     ) -> None:
         """Updates a collection"""
         resp = requests.put(
             self._api_url + "/collections/" + str(id),
             data=json.dumps({"new_metadata": new_metadata, "new_name": new_name}),
         )
         raise_chroma_error(resp)
 
+    @override
     def delete_collection(self, name: str) -> None:
         """Deletes a collection"""
         resp = requests.delete(self._api_url + "/collections/" + name)
         raise_chroma_error(resp)
 
+    @override
     def _count(self, collection_id: UUID) -> int:
         """Returns the number of embeddings in the database"""
         resp = requests.get(
             self._api_url + "/collections/" + str(collection_id) + "/count"
         )
         raise_chroma_error(resp)
         return cast(int, resp.json())
 
-    def _peek(self, collection_id: UUID, limit: int = 10) -> GetResult:
+    @override
+    def _peek(self, collection_id: UUID, n: int = 10) -> GetResult:
         return self._get(
             collection_id,
-            limit=limit,
+            limit=n,
             include=["embeddings", "documents", "metadatas"],
         )
 
+    @override
     def _get(
         self,
         collection_id: UUID,
         ids: Optional[IDs] = None,
         where: Optional[Where] = {},
         sort: Optional[str] = None,
         limit: Optional[int] = None,
@@ -173,14 +186,15 @@
         return GetResult(
             ids=body["ids"],
             embeddings=body.get("embeddings", None),
             metadatas=body.get("metadatas", None),
             documents=body.get("documents", None),
         )
 
+    @override
     def _delete(
         self,
         collection_id: UUID,
         ids: Optional[IDs] = None,
         where: Optional[Where] = {},
         where_document: Optional[WhereDocument] = {},
     ) -> IDs:
@@ -192,14 +206,15 @@
                 {"where": where, "ids": ids, "where_document": where_document}
             ),
         )
 
         raise_chroma_error(resp)
         return cast(IDs, resp.json())
 
+    @override
     def _add(
         self,
         ids: IDs,
         collection_id: UUID,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
@@ -223,14 +238,15 @@
                 }
             ),
         )
 
         raise_chroma_error(resp)
         return True
 
+    @override
     def _update(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Optional[Embeddings] = None,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
@@ -251,14 +267,15 @@
                 }
             ),
         )
 
         resp.raise_for_status()
         return True
 
+    @override
     def _upsert(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
@@ -281,14 +298,15 @@
                 }
             ),
         )
 
         resp.raise_for_status()
         return True
 
+    @override
     def _query(
         self,
         collection_id: UUID,
         query_embeddings: Embeddings,
         n_results: int = 10,
         where: Optional[Where] = {},
         where_document: Optional[WhereDocument] = {},
@@ -316,42 +334,46 @@
             ids=body["ids"],
             distances=body.get("distances", None),
             embeddings=body.get("embeddings", None),
             metadatas=body.get("metadatas", None),
             documents=body.get("documents", None),
         )
 
-    def reset(self) -> bool:
+    @override
+    def reset(self) -> None:
         """Resets the database"""
         resp = requests.post(self._api_url + "/reset")
         raise_chroma_error(resp)
-        return cast(bool, resp.json())
 
+    @override
     def persist(self) -> bool:
         """Persists the database"""
         resp = requests.post(self._api_url + "/persist")
         raise_chroma_error(resp)
         return cast(bool, resp.json())
 
+    @override
     def raw_sql(self, sql: str) -> pd.DataFrame:
         """Runs a raw SQL query against the database"""
         resp = requests.post(
             self._api_url + "/raw_sql", data=json.dumps({"raw_sql": sql})
         )
         raise_chroma_error(resp)
         return pd.DataFrame.from_dict(resp.json())
 
+    @override
     def create_index(self, collection_name: str) -> bool:
         """Creates an index for the given space key"""
         resp = requests.post(
             self._api_url + "/collections/" + collection_name + "/create_index"
         )
         raise_chroma_error(resp)
         return cast(bool, resp.json())
 
+    @override
     def get_version(self) -> str:
         """Returns the version of the server"""
         resp = requests.get(self._api_url + "/version")
         raise_chroma_error(resp)
         return cast(str, resp.json())
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/api/local.py` & `chromadb-client-0.3.27.dev0/chromadb/api/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from chromadb.api.models.Collection import Collection
 from chromadb.config import System
 import chromadb.utils.embedding_functions as ef
 import re
 
 from chromadb.telemetry import Telemetry
 from chromadb.telemetry.events import CollectionAddEvent, CollectionDeleteEvent
+from overrides import override
+import pandas as pd
 
 
 # mimics s3 bucket requirements for naming
 def check_index_name(index_name: str) -> None:
     msg = (
         "Expected collection name that "
         "(1) contains 3-63 characters, "
@@ -51,29 +53,32 @@
 
 
 class LocalAPI(API):
     _db: DB
     _telemetry_client: Telemetry
 
     def __init__(self, system: System):
-        self._db = system.get_db()
-        self._telemetry_client = system.get_telemetry()
+        super().__init__(system)
+        self._db = self.require(DB)
+        self._telemetry_client = self.require(Telemetry)
 
+    @override
     def heartbeat(self) -> int:
         """Ping the database to ensure it is alive
 
         Returns:
             The current time in milliseconds
 
         """
         return int(1000 * time.time_ns())
 
     #
     # COLLECTION METHODS
     #
+    @override
     def create_collection(
         self,
         name: str,
         metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
         get_or_create: bool = False,
     ) -> Collection:
@@ -107,14 +112,15 @@
             client=self,
             name=name,
             embedding_function=embedding_function,
             id=res[0][0],
             metadata=res[0][2],
         )
 
+    @override
     def get_or_create_collection(
         self,
         name: str,
         metadata: Optional[CollectionMetadata] = None,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
         """Get or create a collection with the given name and metadata.
@@ -132,14 +138,15 @@
             # collection(name="my_collection", metadata={})
             ```
         """
         return self.create_collection(
             name, metadata, embedding_function, get_or_create=True
         )
 
+    @override
     def get_collection(
         self,
         name: str,
         embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Collection:
         """Get a collection with the given name.
         Args:
@@ -165,14 +172,15 @@
             client=self,
             name=name,
             id=res[0][0],
             embedding_function=embedding_function,
             metadata=res[0][2],
         )
 
+    @override
     def list_collections(self) -> Sequence[Collection]:
         """List all collections.
         Returns:
             A list of collections
 
         Examples:
             ```python
@@ -189,25 +197,27 @@
                     id=db_collection[0],
                     name=db_collection[1],
                     metadata=db_collection[2],
                 )
             )
         return collections
 
+    @override
     def _modify(
         self,
         id: UUID,
         new_name: Optional[str] = None,
-        new_metadata: Optional[Metadata] = None,
+        new_metadata: Optional[CollectionMetadata] = None,
     ) -> None:
         if new_name is not None:
             check_index_name(new_name)
 
         self._db.update_collection(id, new_name, new_metadata)
 
+    @override
     def delete_collection(self, name: str) -> None:
         """Delete a collection with the given name.
         Args:
             name: The name of the collection to delete
 
         Raises:
             ValueError: If the collection does not exist
@@ -218,14 +228,15 @@
             ```
         """
         self._db.delete_collection(name)
 
     #
     # ITEM METHODS
     #
+    @override
     def _add(
         self,
         ids: IDs,
         collection_id: UUID,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
@@ -247,25 +258,27 @@
 
         if increment_index:
             self._db.add_incremental(collection_id, added_uuids, embeddings)
 
         self._telemetry_client.capture(CollectionAddEvent(str(collection_id), len(ids)))
         return True  # NIT: should this return the ids of the succesfully added items?
 
+    @override
     def _update(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Optional[Embeddings] = None,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
     ) -> bool:
         self._db.update(collection_id, ids, embeddings, metadatas, documents)
         return True
 
+    @override
     def _upsert(
         self,
         collection_id: UUID,
         ids: IDs,
         embeddings: Embeddings,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
@@ -319,14 +332,15 @@
                 metadatas_to_update,
                 documents_to_update,
             )
         self._db.update(collection_id, ids, embeddings, metadatas, documents)
 
         return True
 
+    @override
     def _get(
         self,
         collection_id: UUID,
         ids: Optional[IDs] = None,
         where: Optional[Where] = {},
         sort: Optional[str] = None,
         limit: Optional[int] = None,
@@ -386,14 +400,15 @@
             if include_metadatas:
                 cast(List, get_result["metadatas"]).append(  # type: ignore
                     entry[column_index["metadata"]]
                 )
             get_result["ids"].append(entry[column_index["id"]])
         return get_result
 
+    @override
     def _delete(
         self,
         collection_id: UUID,
         ids: Optional[IDs] = None,
         where: Optional[Where] = None,
         where_document: Optional[WhereDocument] = None,
     ) -> IDs:
@@ -411,27 +426,29 @@
         )
         self._telemetry_client.capture(
             CollectionDeleteEvent(str(collection_id), len(deleted_uuids))
         )
 
         return deleted_uuids
 
+    @override
     def _count(self, collection_id: UUID) -> int:
         return self._db.count(collection_id)
 
-    def reset(self) -> bool:
+    @override
+    def reset(self) -> None:
         """Reset the database. This will delete all collections and items.
 
         Returns:
             True if the database was reset successfully
 
         """
         self._db.reset()
-        return True
 
+    @override
     def _query(
         self,
         collection_id: UUID,
         query_embeddings: Embeddings,
         n_results: int = 10,
         where: Where = {},
         where_document: WhereDocument = {},
@@ -494,39 +511,44 @@
                 )
             if include_distances:
                 cast(List[float], query_result["distances"]).append(distances[i])
             query_result["ids"].append(ids)
 
         return query_result
 
-    def raw_sql(self, raw_sql: str):  # type: ignore
-        return self._db.raw_sql(raw_sql)  # type: ignore
+    @override
+    def raw_sql(self, sql: str) -> pd.DataFrame:
+        return self._db.raw_sql(sql)  # type: ignore
 
+    @override
     def create_index(self, collection_name: str) -> bool:
         collection_uuid = self._db.get_collection_uuid_from_name(collection_name)
         self._db.create_index(collection_uuid=collection_uuid)
         return True
 
+    @override
     def _peek(self, collection_id: UUID, n: int = 10) -> GetResult:
         return self._get(
             collection_id=collection_id,
             limit=n,
             include=["embeddings", "documents", "metadatas"],
         )
 
+    @override
     def persist(self) -> bool:
         """Persist the database to disk.
 
         Returns:
             True if the database was persisted successfully
 
         """
         self._db.persist()
         return True
 
+    @override
     def get_version(self) -> str:
         """Get the version of Chroma.
 
         Returns:
             The version of Chroma
 
         """
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/api/models/Collection.py` & `chromadb-client-0.3.27.dev0/chromadb/api/models/Collection.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb/api/types.py` & `chromadb-client-0.3.27.dev0/chromadb/api/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 from typing import Any, Optional, Union, Dict, Sequence, TypeVar, List
 from typing_extensions import Literal, TypedDict, Protocol
 import chromadb.errors as errors
+from chromadb.types import (
+    Metadata,
+    Vector,
+    LiteralValue,
+    LogicalOperator,
+    WhereOperator,
+    OperatorExpression,
+    Where,
+    WhereDocumentOperator,
+    WhereDocument,
+)
+
+# Re-export types from chromadb.types
+__all__ = ["Metadata", "Where", "WhereDocument"]
 
 ID = str
 IDs = List[ID]
 
-Number = Union[int, float]
-Embedding = List[Number]
+Embedding = Vector
 Embeddings = List[Embedding]
 
-
-Metadata = Dict[str, Union[str, int, float]]
 Metadatas = List[Metadata]
 
 CollectionMetadata = Dict[Any, Any]
 
 Document = str
 Documents = List[Document]
 
 Parameter = TypeVar("Parameter", Embedding, Document, Metadata, ID)
 T = TypeVar("T")
 OneOrMany = Union[T, List[T]]
 
-Include = List[Literal["documents", "embeddings", "metadatas", "distances"]]
-
-# Grammar for where expressions
-LiteralValue = Union[str, int, float]
-LogicalOperator = Literal["$and", "$or"]
-WhereOperator = Literal["$gt", "$gte", "$lt", "$lte", "$ne", "$eq"]
-OperatorExpression = Dict[Union[WhereOperator, LogicalOperator], LiteralValue]
-
-Where = Dict[
-    Union[str, LogicalOperator], Union[LiteralValue, OperatorExpression, List["Where"]]
+# This should ust be List[Literal["documents", "embeddings", "metadatas", "distances"]]
+# However, this provokes an incompatibility with the Overrides library and Python 3.7
+Include = List[
+    Union[
+        Literal["documents"],
+        Literal["embeddings"],
+        Literal["metadatas"],
+        Literal["distances"],
+    ]
 ]
 
-WhereDocumentOperator = Literal["$contains", LogicalOperator]
-WhereDocument = Dict[WhereDocumentOperator, Union[str, List["WhereDocument"]]]
+# Re-export types from chromadb.types
+LiteralValue = LiteralValue
+LogicalOperator = LogicalOperator
+WhereOperator = WhereOperator
+OperatorExpression = OperatorExpression
+Where = Where
+WhereDocumentOperator = WhereDocumentOperator
 
 
 class GetResult(TypedDict):
     ids: List[ID]
     embeddings: Optional[List[Embedding]]
     documents: Optional[List[Document]]
     metadatas: Optional[List[Metadata]]
@@ -131,14 +146,16 @@
 def validate_where(where: Where) -> Where:
     """
     Validates where to ensure it is a dictionary of strings to strings, ints, floats or operator expressions,
     or in the case of $and and $or, a list of where expressions
     """
     if not isinstance(where, dict):
         raise ValueError(f"Expected where to be a dict, got {where}")
+    if len(where) != 1:
+        raise ValueError(f"Expected where to have exactly one operator, got {where}")
     for key, value in where.items():
         if not isinstance(key, str):
             raise ValueError(f"Expected where key to be a str, got {key}")
         if (
             key != "$and"
             and key != "$or"
             and not isinstance(value, (str, int, float, dict))
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/db/__init__.py` & `chromadb-client-0.3.27.dev0/chromadb/db/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from typing import List, Sequence, Optional, Tuple
 from uuid import UUID
 import numpy.typing as npt
 from chromadb.api.types import (
     Embeddings,
     Documents,
     IDs,
     Metadatas,
     Metadata,
     Where,
     WhereDocument,
 )
+from chromadb.config import Component
+from overrides import override
 
 
-class DB(ABC):
-    @abstractmethod
-    def __init__(self) -> None:
-        pass
-
+class DB(Component):
     @abstractmethod
     def create_collection(
         self,
         name: str,
         metadata: Optional[Metadata] = None,
         get_or_create: bool = False,
-    ) -> Sequence:
+    ) -> Sequence:  # type: ignore
         pass
 
     @abstractmethod
-    def get_collection(self, name: str) -> Sequence:
+    def get_collection(self, name: str) -> Sequence:  # type: ignore
         pass
 
     @abstractmethod
-    def list_collections(self) -> Sequence:
+    def list_collections(self) -> Sequence:  # type: ignore
         pass
 
     @abstractmethod
     def update_collection(
         self,
         id: UUID,
         new_name: Optional[str] = None,
@@ -77,15 +75,15 @@
         collection_uuid: Optional[UUID] = None,
         ids: Optional[IDs] = None,
         sort: Optional[str] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         where_document: WhereDocument = {},
         columns: Optional[List[str]] = None,
-    ) -> Sequence:
+    ) -> Sequence:  # type: ignore
         pass
 
     @abstractmethod
     def update(
         self,
         collection_uuid: UUID,
         ids: IDs,
@@ -106,14 +104,15 @@
         collection_uuid: Optional[UUID] = None,
         ids: Optional[IDs] = None,
         where_document: WhereDocument = {},
     ) -> List[str]:
         pass
 
     @abstractmethod
+    @override
     def reset(self) -> None:
         pass
 
     @abstractmethod
     def get_nearest_neighbors(
         self,
         collection_uuid: UUID,
@@ -123,21 +122,21 @@
         where_document: WhereDocument = {},
     ) -> Tuple[List[List[UUID]], npt.NDArray]:
         pass
 
     @abstractmethod
     def get_by_ids(
         self, uuids: List[UUID], columns: Optional[List[str]] = None
-    ) -> Sequence:
+    ) -> Sequence:  # type: ignore
         pass
 
     @abstractmethod
-    def raw_sql(self, raw_sql):
+    def raw_sql(self, raw_sql):  # type: ignore
         pass
 
     @abstractmethod
-    def create_index(self, collection_uuid: UUID):
+    def create_index(self, collection_uuid: UUID):  # type: ignore
         pass
 
     @abstractmethod
     def persist(self) -> None:
         pass
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/db/base.py` & `chromadb-client-0.3.27.dev0/chromadb/db/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,23 +2,40 @@
 from types import TracebackType
 from typing_extensions import Protocol, Self, Literal
 from abc import ABC, abstractmethod
 from threading import local
 from overrides import override, EnforceOverrides
 import pypika
 import pypika.queries
-import itertools
+from chromadb.config import System, Component
+from uuid import UUID
+from itertools import islice, count
+
+
+class NotFoundError(Exception):
+    """Raised when a delete or update operation affects no rows"""
+
+    pass
+
+
+class UniqueConstraintError(Exception):
+    """Raised when an insert operation would violate a unique constraint"""
+
+    pass
 
 
 class Cursor(Protocol):
     """Reifies methods we use from a DBAPI2 Cursor since DBAPI2 is not typed."""
 
     def execute(self, sql: str, params: Optional[Tuple[Any, ...]] = None) -> Self:
         ...
 
+    def executescript(self, script: str) -> Self:
+        ...
+
     def executemany(
         self, sql: str, params: Optional[Sequence[Tuple[Any, ...]]] = None
     ) -> Self:
         ...
 
     def fetchone(self) -> Tuple[Any, ...]:
         ...
@@ -45,29 +62,25 @@
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> Literal[False]:
         pass
 
 
-class SqlDB(ABC, EnforceOverrides):
+class SqlDB(Component):
     """DBAPI 2.0 interface wrapper to ensure consistent behavior between implementations"""
 
+    def __init__(self, system: System):
+        super().__init__(system)
+
     @abstractmethod
     def tx(self) -> TxWrapper:
         """Return a transaction wrapper"""
         pass
 
-    @abstractmethod
-    def reset(self) -> None:
-        """Reset the database to a clean state. Implementations may throw an exception
-        if they do not support reset. In all cases, implementations should respect the
-        `allow_reset` config setting and throw an exception if it is set to False."""
-        pass
-
     @staticmethod
     @abstractmethod
     def querybuilder() -> Type[pypika.Query]:
         """Return a PyPika Query builder of an appropriate subtype for this database
         implementation (see
         https://pypika.readthedocs.io/en/latest/3_advanced.html#handling-different-database-platforms)
         """
@@ -77,14 +90,37 @@
     @abstractmethod
     def parameter_format() -> str:
         """Return the appropriate parameter format for this database implementation.
         Will be called with str.format(i) where i is the numeric index of the parameter.
         """
         pass
 
+    @staticmethod
+    @abstractmethod
+    def uuid_to_db(uuid: Optional[UUID]) -> Optional[Any]:
+        """Convert a UUID to a value that can be passed to the DB driver"""
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def uuid_from_db(value: Optional[Any]) -> Optional[UUID]:
+        """Convert a value from the DB driver to a UUID"""
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def unique_constraint_error() -> Type[BaseException]:
+        """Return the exception type that the DB raises when a unique constraint is
+        violated"""
+        pass
+
+    def param(self, idx: int) -> pypika.Parameter:
+        """Return a PyPika Parameter object for the given index"""
+        return pypika.Parameter(self.parameter_format().format(idx))
+
 
 _context = local()
 
 
 class ParameterValue(pypika.Parameter):  # type: ignore
     """
     Wrapper class for PyPika paramters that allows the values for Parameters
@@ -93,16 +129,23 @@
     """
 
     def __init__(self, value: Any):
         self.value = value
 
     @override
     def get_sql(self, **kwargs: Any) -> str:
-        _context.values.append(self.value)
-        val = _context.formatstr.format(next(_context.generator))
+        if isinstance(self.value, (list, tuple)):
+            _context.values.extend(self.value)
+            indexes = islice(_context.generator, len(self.value))
+            placeholders = ", ".join(_context.formatstr.format(i) for i in indexes)
+            val = f"({placeholders})"
+        else:
+            _context.values.append(self.value)
+            val = _context.formatstr.format(next(_context.generator))
+
         return str(val)
 
 
 def get_sql(
     query: pypika.queries.QueryBuilder, formatstr: str = "?"
 ) -> Tuple[str, Tuple[Any, ...]]:
     """
@@ -138,12 +181,12 @@
     should be `":{}"`.
 
     See https://pypika.readthedocs.io/en/latest/2_tutorial.html#parametrized-queries for more
     information on parameterized queries in PyPika.
     """
 
     _context.values = []
-    _context.generator = itertools.count(1)
+    _context.generator = count(1)
     _context.formatstr = formatstr
     sql = query.get_sql()
     params = tuple(_context.values)
     return sql, params
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/db/clickhouse.py` & `chromadb-client-0.3.27.dev0/chromadb/db/clickhouse.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,24 @@
     Where,
     WhereDocument,
 )
 from chromadb.db import DB
 from chromadb.db.index.hnswlib import Hnswlib, delete_all_indexes
 import uuid
 import json
-from typing import Dict, Optional, Sequence, List, Tuple, cast
+from typing import Optional, Sequence, List, Tuple, cast
 import clickhouse_connect
 from clickhouse_connect.driver.client import Client
 from clickhouse_connect import common
 import logging
 from uuid import UUID
 from chromadb.config import System
+from overrides import override
+import numpy.typing as npt
+from chromadb.api.types import Metadata
 
 logger = logging.getLogger(__name__)
 
 COLLECTION_TABLE_SCHEMA = [{"uuid": "UUID"}, {"name": "String"}, {"metadata": "String"}]
 
 EMBEDDING_TABLE_SCHEMA = [
     {"collection_uuid": "UUID"},
@@ -49,14 +52,15 @@
 
 
 class Clickhouse(DB):
     #
     #  INIT METHODS
     #
     def __init__(self, system: System):
+        super().__init__(system)
         self._conn = None
         self._settings = system.settings
 
         self._settings.require("clickhouse_host")
         self._settings.require("clickhouse_port")
 
     def _init_conn(self):
@@ -110,23 +114,25 @@
         index = self._index(collection_id)
         index.delete()
         del self.index_cache[collection_id]
 
     #
     #  UTILITY METHODS
     #
+    @override
     def persist(self):
         raise NotImplementedError(
             "Clickhouse is a persistent database, this method is not needed"
         )
 
-    def get_collection_uuid_from_name(self, name: str) -> UUID:
+    @override
+    def get_collection_uuid_from_name(self, collection_name: str) -> UUID:
         res = self._get_conn().query(
             f"""
-            SELECT uuid FROM collections WHERE name = '{name}'
+            SELECT uuid FROM collections WHERE name = '{collection_name}'
         """
         )
         return res.result_rows[0][0]
 
     def _create_where_clause(
         self,
         collection_uuid: str,
@@ -148,16 +154,20 @@
         where_str = " AND ".join(where_clauses)
         where_str = f"WHERE {where_str}"
         return where_str
 
     #
     #  COLLECTION METHODS
     #
+    @override
     def create_collection(
-        self, name: str, metadata: Optional[Dict] = None, get_or_create: bool = False
+        self,
+        name: str,
+        metadata: Optional[Metadata] = None,
+        get_or_create: bool = False,
     ) -> Sequence:
         # poor man's unique constraint
         dupe_check = self.get_collection(name)
 
         if len(dupe_check) > 0:
             if get_or_create:
                 if dupe_check[0][2] != metadata:
@@ -176,15 +186,16 @@
         data_to_insert = [[collection_uuid, name, json.dumps(metadata)]]
 
         self._get_conn().insert(
             "collections", data_to_insert, column_names=["uuid", "name", "metadata"]
         )
         return [[collection_uuid, name, metadata]]
 
-    def get_collection(self, name: str):
+    @override
+    def get_collection(self, name: str) -> Sequence:
         res = (
             self._get_conn()
             .query(
                 f"""
          SELECT * FROM collections WHERE name = '{name}'
          """
             )
@@ -202,23 +213,25 @@
          """
             )
             .result_rows
         )
         # json.loads the metadata
         return [[x[0], x[1], json.loads(x[2])] for x in res][0]
 
+    @override
     def list_collections(self) -> Sequence:
         res = self._get_conn().query("SELECT * FROM collections").result_rows
         return [[x[0], x[1], json.loads(x[2])] for x in res]
 
+    @override
     def update_collection(
         self,
         id: UUID,
         new_name: Optional[str] = None,
-        new_metadata: Optional[Dict] = None,
+        new_metadata: Optional[Metadata] = None,
     ):
         if new_name is not None:
             dupe_check = self.get_collection(new_name)
             if len(dupe_check) > 0 and dupe_check[0][0] != id:
                 raise ValueError(f"Collection with name {new_name} already exists")
 
             self._get_conn().command(
@@ -228,14 +241,15 @@
 
         if new_metadata is not None:
             self._get_conn().command(
                 "ALTER TABLE collections UPDATE metadata = %(new_metadata)s WHERE uuid = %(uuid)s",
                 parameters={"new_metadata": json.dumps(new_metadata), "uuid": id},
             )
 
+    @override
     def delete_collection(self, name: str):
         collection_uuid = self.get_collection_uuid_from_name(name)
         self._get_conn().command(
             f"""
         DELETE FROM embeddings WHERE collection_uuid = '{collection_uuid}'
         """
         )
@@ -247,16 +261,16 @@
          DELETE FROM collections WHERE name = '{name}'
          """
         )
 
     #
     #  ITEM METHODS
     #
-
-    def add(self, collection_uuid, embeddings, metadatas, documents, ids):
+    @override
+    def add(self, collection_uuid, embeddings, metadatas, documents, ids) -> List[UUID]:
         data_to_insert = [
             [
                 collection_uuid,
                 uuid.uuid4(),
                 embedding,
                 json.dumps(metadatas[i]) if metadatas else None,
                 documents[i] if documents else None,
@@ -309,22 +323,23 @@
             updates.append(update_statement)
 
         update_clauses = ("").join(updates)
         self._get_conn().command(
             f"ALTER TABLE embeddings {update_clauses}", parameters=parameters
         )
 
+    @override
     def update(
         self,
         collection_uuid,
         ids: IDs,
         embeddings: Optional[Embeddings] = None,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
-    ):
+    ) -> bool:
         # Verify all IDs exist
         existing_items = self.get(collection_uuid=collection_uuid, ids=ids)
         if len(existing_items) != len(ids):
             raise ValueError(
                 f"Could not find {len(ids) - len(existing_items)} items for update"
             )
 
@@ -448,14 +463,15 @@
             if operator == "$or":
                 results.append(f"({' OR '.join(all_subresults)})")
             if operator == "$and":
                 results.append(f"({' AND '.join(all_subresults)})")
         else:
             raise ValueError(f"Expected one of $contains, $and, $or, got {operator}")
 
+    @override
     def get(
         self,
         where: Where = {},
         collection_name: Optional[str] = None,
         collection_uuid: Optional[UUID] = None,
         ids: Optional[IDs] = None,
         sort: Optional[str] = None,
@@ -491,16 +507,17 @@
         if offset is not None or isinstance(offset, int):
             where_str += f" OFFSET {offset}"
 
         val = self._get(where=where_str, columns=columns)
 
         return val
 
-    def count(self, collection_uuid: UUID) -> int:
-        where_string = f"WHERE collection_uuid = '{collection_uuid}'"
+    @override
+    def count(self, collection_id: UUID) -> int:
+        where_string = f"WHERE collection_uuid = '{collection_id}'"
         return (
             self._get_conn()
             .query(f"SELECT COUNT() FROM embeddings {where_string}")
             .result_rows[0][0]
         )
 
     def _delete(self, where_str: Optional[str] = None) -> List:
@@ -514,21 +531,22 @@
             DELETE FROM
                 embeddings
         {where_str}
         """
         )
         return [res[0] for res in deleted_uuids] if len(deleted_uuids) > 0 else []
 
+    @override
     def delete(
         self,
         where: Where = {},
-        collection_uuid: Optional[str] = None,
+        collection_uuid: Optional[UUID] = None,
         ids: Optional[IDs] = None,
         where_document: WhereDocument = {},
-    ) -> List:
+    ) -> List[str]:
         where_str = self._create_where_clause(
             # collection_uuid must be defined at this point, cast it for typechecker
             cast(str, collection_uuid),
             ids=ids,
             where=where,
             where_document=where_document,
         )
@@ -536,40 +554,44 @@
         deleted_uuids = self._delete(where_str)
 
         index = self._index(collection_uuid)
         index.delete_from_index(deleted_uuids)
 
         return deleted_uuids
 
-    def get_by_ids(self, ids: list, columns: Optional[List] = None):
+    @override
+    def get_by_ids(
+        self, uuids: List[UUID], columns: Optional[List[str]] = None
+    ) -> Sequence:
         columns = columns + ["uuid"] if columns else ["uuid"]
         select_columns = db_schema_to_keys() if columns is None else columns
         response = (
             self._get_conn()
             .query(
                 f"""
-        SELECT {",".join(select_columns)} FROM embeddings WHERE uuid IN ({[id.hex for id in ids]})
+        SELECT {",".join(select_columns)} FROM embeddings WHERE uuid IN ({[id.hex for id in uuids]})
         """
             )
             .result_rows
         )
 
         # sort db results by the order of the uuids
-        response = sorted(response, key=lambda obj: ids.index(obj[len(columns) - 1]))
+        response = sorted(response, key=lambda obj: uuids.index(obj[len(columns) - 1]))
 
         return response
 
+    @override
     def get_nearest_neighbors(
         self,
         collection_uuid: UUID,
-        where: Where,
-        where_document: WhereDocument,
-        embeddings: Embeddings,
-        n_results: int,
-    ) -> Tuple[List[List[uuid.UUID]], List[List[float]]]:
+        where: Where = {},
+        embeddings: Optional[Embeddings] = None,
+        n_results: int = 10,
+        where_document: WhereDocument = {},
+    ) -> Tuple[List[List[UUID]], npt.NDArray]:
         # Either the collection name or the collection uuid must be provided
         if collection_uuid is None:
             raise TypeError("Argument collection_uuid cannot be None")
 
         if len(where) != 0 or len(where_document) != 0:
             results = self.get(
                 collection_uuid=collection_uuid,
@@ -588,15 +610,16 @@
             ids = None
 
         index = self._index(collection_uuid)
         uuids, distances = index.get_nearest_neighbors(embeddings, n_results, ids)
 
         return uuids, distances
 
-    def create_index(self, collection_uuid: str):
+    @override
+    def create_index(self, collection_uuid: UUID):
         """Create an index for a collection_uuid and optionally scoped to a dataset.
         Args:
             collection_uuid (str): The collection_uuid to create an index for
             dataset (str, optional): The dataset to scope the index to. Defaults to None.
         Returns:
             None
         """
@@ -604,26 +627,31 @@
 
         uuids = [x[1] for x in get]
         embeddings = [x[2] for x in get]
 
         index = self._index(collection_uuid)
         index.add(uuids, embeddings)
 
-    def add_incremental(self, collection_uuid, uuids, embeddings):
+    @override
+    def add_incremental(
+        self, collection_uuid: UUID, ids: List[UUID], embeddings: Embeddings
+    ) -> None:
         index = self._index(collection_uuid)
-        index.add(uuids, embeddings)
+        index.add(ids, embeddings)
 
     def reset_indexes(self):
         delete_all_indexes(self._settings)
         self.index_cache = {}
 
+    @override
     def reset(self):
         conn = self._get_conn()
         conn.command("DROP TABLE collections")
         conn.command("DROP TABLE embeddings")
         self._create_table_collections(conn)
         self._create_table_embeddings(conn)
 
         self.reset_indexes()
 
-    def raw_sql(self, sql):
-        return self._get_conn().query(sql).result_rows
+    @override
+    def raw_sql(self, raw_sql):
+        return self._get_conn().query(raw_sql).result_rows
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/db/duckdb.py` & `chromadb-client-0.3.27.dev0/chromadb/db/duckdb.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 from chromadb.db.clickhouse import (
     Clickhouse,
     db_array_schema_to_clickhouse_schema,
     EMBEDDING_TABLE_SCHEMA,
     db_schema_to_keys,
     COLLECTION_TABLE_SCHEMA,
 )
-from typing import List, Optional, Sequence, Dict
+from typing import List, Optional, Sequence
 import pandas as pd
 import json
 import duckdb
 import uuid
 import os
 import logging
 import atexit
+from uuid import UUID
+from overrides import override
+from chromadb.api.types import Metadata
 
 logger = logging.getLogger(__name__)
 
 
 def clickhouse_to_duckdb_schema(table_schema):
     for item in table_schema:
         if "embedding" in item:
@@ -40,49 +43,60 @@
 # TODO: inherits ClickHouse for convenience of copying behavior, not
 # because it's logically a subtype. Factoring out the common behavior
 # to a third superclass they both extend would be preferable.
 class DuckDB(Clickhouse):
     # duckdb has a different way of connecting to the database
     def __init__(self, system: System):
         self._conn = duckdb.connect()
-        self._create_table_collections()
-        self._create_table_embeddings()
+        self._create_table_collections(self._conn)
+        self._create_table_embeddings(self._conn)
         self._settings = system.settings
 
+        # Normally this would be handled by super(), but we actually can't invoke
+        # super().__init__ here because we're (incorrectly) inheriting from Clickhouse
+        self._dependencies = set()
+
         # https://duckdb.org/docs/extensions/overview
         self._conn.execute("LOAD 'json';")
 
-    def _create_table_collections(self):
-        self._conn.execute(
+    @override
+    def _create_table_collections(self, conn):
+        conn.execute(
             f"""CREATE TABLE collections (
             {db_array_schema_to_clickhouse_schema(clickhouse_to_duckdb_schema(COLLECTION_TABLE_SCHEMA))}
         ) """
         )
 
     # duckdb has different types, so we want to convert the clickhouse schema to duckdb schema
-    def _create_table_embeddings(self):
-        self._conn.execute(
+    @override
+    def _create_table_embeddings(self, conn):
+        conn.execute(
             f"""CREATE TABLE embeddings (
             {db_array_schema_to_clickhouse_schema(clickhouse_to_duckdb_schema(EMBEDDING_TABLE_SCHEMA))}
         ) """
         )
 
     #
     #  UTILITY METHODS
     #
-    def get_collection_uuid_from_name(self, name):
+    @override
+    def get_collection_uuid_from_name(self, collection_name: str) -> UUID:
         return self._conn.execute(
-            "SELECT uuid FROM collections WHERE name = ?", [name]
+            "SELECT uuid FROM collections WHERE name = ?", [collection_name]
         ).fetchall()[0][0]
 
     #
     #  COLLECTION METHODS
     #
+    @override
     def create_collection(
-        self, name: str, metadata: Optional[Dict] = None, get_or_create: bool = False
+        self,
+        name: str,
+        metadata: Optional[Metadata] = None,
+        get_or_create: bool = False,
     ) -> Sequence:
         # poor man's unique constraint
         dupe_check = self.get_collection(name)
         if len(dupe_check) > 0:
             if get_or_create is True:
                 if dupe_check[0][2] != metadata:
                     self.update_collection(
@@ -100,42 +114,50 @@
         collection_uuid = uuid.uuid4()
         self._conn.execute(
             """INSERT INTO collections (uuid, name, metadata) VALUES (?, ?, ?)""",
             [str(collection_uuid), name, json.dumps(metadata)],
         )
         return [[str(collection_uuid), name, metadata]]
 
+    @override
     def get_collection(self, name: str) -> Sequence:
         res = self._conn.execute(
             """SELECT * FROM collections WHERE name = ?""", [name]
         ).fetchall()
         # json.loads the metadata
         return [[x[0], x[1], json.loads(x[2])] for x in res]
 
-    def get_collection_by_id(self, uuid: str) -> Sequence:
+    @override
+    def get_collection_by_id(self, collection_uuid: str):
         res = self._conn.execute(
-            """SELECT * FROM collections WHERE uuid = ?""", [uuid]
+            """SELECT * FROM collections WHERE uuid = ?""", [collection_uuid]
         ).fetchone()
         return [res[0], res[1], json.loads(res[2])]
 
+    @override
     def list_collections(self) -> Sequence:
         res = self._conn.execute("""SELECT * FROM collections""").fetchall()
         return [[x[0], x[1], json.loads(x[2])] for x in res]
 
+    @override
     def delete_collection(self, name: str):
         collection_uuid = self.get_collection_uuid_from_name(name)
         self._conn.execute(
             """DELETE FROM embeddings WHERE collection_uuid = ?""", [collection_uuid]
         )
 
         self._delete_index(collection_uuid)
         self._conn.execute("""DELETE FROM collections WHERE name = ?""", [name])
 
+    @override
     def update_collection(
-        self, id: uuid.UUID, new_name: str, new_metadata: Optional[Dict] = None
+        self,
+        id: UUID,
+        new_name: Optional[str] = None,
+        new_metadata: Optional[Metadata] = None,
     ):
         if new_name is not None:
             dupe_check = self.get_collection(new_name)
             if len(dupe_check) > 0 and dupe_check[0][0] != str(id):
                 raise ValueError(f"Collection with name {new_name} already exists")
 
             self._conn.execute(
@@ -149,15 +171,16 @@
                 [json.dumps(new_metadata), id],
             )
 
     #
     #  ITEM METHODS
     #
     # the execute many syntax is different than clickhouse, the (?,?) syntax is different than clickhouse
-    def add(self, collection_uuid, embeddings, metadatas, documents, ids):
+    @override
+    def add(self, collection_uuid, embeddings, metadatas, documents, ids) -> List[UUID]:
         data_to_insert = [
             [
                 collection_uuid,
                 str(uuid.uuid4()),
                 embedding,
                 json.dumps(metadatas[i]) if metadatas else None,
                 documents[i] if documents else None,
@@ -172,20 +195,22 @@
             f"""
          INSERT INTO embeddings ({insert_string}) VALUES (?,?,?,?,?,?)""",
             data_to_insert,
         )
 
         return [uuid.UUID(x[1]) for x in data_to_insert]  # return uuids
 
-    def count(self, collection_uuid) -> int:
-        where_string = f"WHERE collection_uuid = '{collection_uuid}'"
+    @override
+    def count(self, collection_id: UUID) -> int:
+        where_string = f"WHERE collection_uuid = '{collection_id}'"
         return self._conn.query(
             f"SELECT COUNT() FROM embeddings {where_string}"
         ).fetchall()[0][0]
 
+    @override
     def _format_where(self, where, result):
         for key, value in where.items():
             # Shortcut for $eq
             if type(value) == str:
                 result.append(f" json_extract_string(metadata,'$.{key}') = '{value}'")
             if type(value) == int:
                 result.append(
@@ -243,14 +268,15 @@
                 elif key == "$and":
                     result.append(f"({' AND '.join(all_subresults)})")
                 else:
                     raise ValueError(
                         f"Operator {key} not supported with a list of where clauses"
                     )
 
+    @override
     def _format_where_document(self, where_document, results):
         operator = list(where_document.keys())[0]
         if operator == "$contains":
             results.append(f"position('{where_document[operator]}' in document) > 0")
         elif operator == "$and" or operator == "$or":
             all_subresults = []
             for subwhere in where_document[operator]:
@@ -260,14 +286,15 @@
             if operator == "$or":
                 results.append(f"({' OR '.join(all_subresults)})")
             if operator == "$and":
                 results.append(f"({' AND '.join(all_subresults)})")
         else:
             raise ValueError(f"Operator {operator} not supported")
 
+    @override
     def _get(self, where, columns: Optional[List] = None):
         select_columns = db_schema_to_keys() if columns is None else columns
         val = self._conn.execute(
             f"""SELECT {",".join(select_columns)} FROM embeddings {where}"""
         ).fetchall()
         for i in range(len(val)):
             val[i] = list(val[i])
@@ -285,14 +312,15 @@
                     json.loads(val[i][metadata_column_index])
                     if val[i][metadata_column_index]
                     else None
                 )
 
         return val
 
+    @override
     def _update(
         self,
         collection_uuid,
         ids: IDs,
         embeddings: Optional[Embeddings],
         metadatas: Optional[Metadatas],
         documents: Optional[Documents],
@@ -324,73 +352,80 @@
             {", ".join(update_fields)}
         WHERE
             id = ? AND
             collection_uuid = '{collection_uuid}';
         """
         self._conn.executemany(update_statement, update_data)
 
+    @override
     def _delete(self, where_str: Optional[str] = None) -> List:
         uuids_deleted = self._conn.execute(
             f"""SELECT uuid FROM embeddings {where_str}"""
         ).fetchall()
         self._conn.execute(
             f"""
             DELETE FROM
                 embeddings
         {where_str}
         """
         ).fetchall()[0]
         return [uuid.UUID(x[0]) for x in uuids_deleted]
 
-    def get_by_ids(self, ids: List, columns: Optional[List] = None):
+    @override
+    def get_by_ids(
+        self, uuids: List[UUID], columns: Optional[List[str]] = None
+    ) -> Sequence:
         # select from duckdb table where ids are in the list
-        if not isinstance(ids, list):
-            raise TypeError(f"Expected ids to be a list, got {ids}")
+        if not isinstance(uuids, list):
+            raise TypeError(f"Expected ids to be a list, got {uuids}")
 
-        if not ids:
+        if not uuids:
             # create an empty pandas dataframe
             return pd.DataFrame()
 
         columns = columns + ["uuid"] if columns else ["uuid"]
 
         select_columns = db_schema_to_keys() if columns is None else columns
         response = self._conn.execute(
             f"""
             SELECT
                 {",".join(select_columns)}
             FROM
                 embeddings
             WHERE
-                uuid IN ({','.join([("'" + str(x) + "'") for x in ids])})
+                uuid IN ({','.join([("'" + str(x) + "'") for x in uuids])})
         """
         ).fetchall()
 
         # sort db results by the order of the uuids
         response = sorted(
-            response, key=lambda obj: ids.index(uuid.UUID(obj[len(columns) - 1]))
+            response, key=lambda obj: uuids.index(uuid.UUID(obj[len(columns) - 1]))
         )
 
         return response
 
-    def raw_sql(self, sql):
-        return self._conn.execute(sql).df()
+    @override
+    def raw_sql(self, raw_sql):
+        return self._conn.execute(raw_sql).df()
 
     # TODO: This method should share logic with clickhouse impl
+    @override
     def reset(self):
         self._conn.execute("DROP TABLE collections")
         self._conn.execute("DROP TABLE embeddings")
-        self._create_table_collections()
-        self._create_table_embeddings()
+        self._create_table_collections(self._conn)
+        self._create_table_embeddings(self._conn)
 
         self.reset_indexes()
 
     def __del__(self):
         logger.info("Exiting: Cleaning up .chroma directory")
         self.reset_indexes()
 
+    @override
     def persist(self) -> None:
         raise NotImplementedError(
             "Set chroma_db_impl='duckdb+parquet' to get persistence functionality"
         )
 
 
 class PersistentDuckDB(DuckDB):
@@ -413,14 +448,15 @@
 
     def set_save_folder(self, path):
         self._save_folder = path
 
     def get_save_folder(self):
         return self._save_folder
 
+    @override
     def persist(self):
         """
         Persist the database to disk
         """
         logger.info(
             f"Persisting DB to disk, putting it in the save folder: {self._save_folder}"
         )
@@ -483,14 +519,15 @@
                 f"""loaded in {self._conn.query(f"SELECT COUNT() FROM collections").fetchall()[0][0]} collections"""
             )
 
     def __del__(self):
         # No-op for duckdb with persistence since the base class will delete the indexes
         pass
 
+    @override
     def reset(self):
         super().reset()
         # empty the save folder
         import shutil
         import os
 
         shutil.rmtree(self._save_folder)
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/db/impl/sqlite.py` & `chromadb-client-0.3.27.dev0/chromadb/db/impl/sqlite.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,83 @@
 from chromadb.db.migrations import MigratableDB, Migration
 from chromadb.config import System, Settings
 import chromadb.db.base as base
+from chromadb.db.mixins.embeddings_queue import SqlEmbeddingsQueue
+from chromadb.db.mixins.sysdb import SqlSysDB
 import sqlite3
 from overrides import override
 import pypika
-from typing import Sequence, cast, Optional, Type
+from typing import Sequence, cast, Optional, Type, Any
 from typing_extensions import Literal
 from types import TracebackType
 import os
+from uuid import UUID
+from threading import local
 
 
 class TxWrapper(base.TxWrapper):
-    def __init__(self, conn: sqlite3.Connection) -> None:
+    def __init__(self, conn: sqlite3.Connection, stack: local) -> None:
+        self._tx_stack = stack
         self._conn = conn
 
     @override
     def __enter__(self) -> base.Cursor:
-        self._conn.execute("BEGIN;")
+        if len(self._tx_stack.stack) == 0:
+            self._conn.execute("BEGIN;")
+        self._tx_stack.stack.append(self)
         return self._conn.cursor()  # type: ignore
 
     @override
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> Literal[False]:
-        if exc_type is None:
-            self._conn.commit()
-        else:
-            self._conn.rollback()
+        self._tx_stack.stack.pop()
+        if len(self._tx_stack.stack) == 0:
+            if exc_type is None:
+                self._conn.commit()
+            else:
+                self._conn.rollback()
         return False
 
 
-class SqliteDB(MigratableDB):
+class SqliteDB(MigratableDB, SqlEmbeddingsQueue, SqlSysDB):
     _conn: sqlite3.Connection
     _settings: Settings
     _migration_dirs: Sequence[str]
+    _db_file: str
+    _tx_stack: local
 
     def __init__(self, system: System):
         self._settings = system.settings
-        self._migration_dirs = []
-        self._init()
+        self._migration_dirs = [
+            "migrations/embeddings_queue",
+            "migrations/sysdb",
+            "migrations/metadb",
+        ]
+        self._db_file = self._settings.require("sqlite_database")
+        self._tx_stack = local()
         super().__init__(system)
 
-    def _init(self) -> None:
-        sqlite_db = self._settings.require("sqlite_database")
-        self._conn = sqlite3.connect(sqlite_db)
+    @override
+    def start(self) -> None:
+        super().start()
+        self._conn = sqlite3.connect(self._db_file)
+        self._conn.isolation_level = None  # Handle commits explicitly
+        with self.tx() as cur:
+            cur.execute("PRAGMA foreign_keys = ON")
         self.initialize_migrations()
 
+    @override
+    def stop(self) -> None:
+        super().stop()
+        self._conn.close()
+
     @staticmethod
     @override
     def querybuilder() -> Type[pypika.Query]:
         return pypika.Query  # type: ignore
 
     @staticmethod
     @override
@@ -66,27 +91,30 @@
 
     @override
     def migration_dirs(self) -> Sequence[str]:
         return self._migration_dirs
 
     @override
     def tx(self) -> TxWrapper:
-        return TxWrapper(self._conn)
+        if not hasattr(self._tx_stack, "stack"):
+            self._tx_stack.stack = []
+        return TxWrapper(self._conn, stack=self._tx_stack)
 
     @override
     def reset(self) -> None:
         if not self._settings.require("allow_reset"):
             raise ValueError(
                 "Resetting the database is not allowed. Set `allow_reset` to true in the config in tests or other non-production environments where reset should be permitted."
             )
         self._conn.close()
         db_file = self._settings.require("sqlite_database")
         if db_file != ":memory:":
             os.remove(db_file)
-        self._init()
+        self.start()
+        super().reset()
 
     @override
     def setup_migrations(self) -> None:
         with self.tx() as cur:
             cur.execute(
                 """
                  CREATE TABLE IF NOT EXISTS migrations (
@@ -143,21 +171,36 @@
                         scope=self.migration_scope(),
                     )
                 )
             return migrations
 
     @override
     def apply_migration(self, cur: base.Cursor, migration: Migration) -> None:
-        cur.execute(migration["sql"])
+        cur.executescript(migration["sql"])
         cur.execute(
             """
             INSERT INTO migrations (dir, version, filename, sql, hash)
             VALUES (?, ?, ?, ?, ?)
             """,
             (
                 migration["dir"],
                 migration["version"],
                 migration["filename"],
                 migration["sql"],
                 migration["hash"],
             ),
         )
+
+    @staticmethod
+    @override
+    def uuid_from_db(value: Optional[Any]) -> Optional[UUID]:
+        return UUID(value) if value is not None else None
+
+    @staticmethod
+    @override
+    def uuid_to_db(uuid: Optional[UUID]) -> Optional[Any]:
+        return str(uuid) if uuid is not None else None
+
+    @staticmethod
+    @override
+    def unique_constraint_error() -> Type[BaseException]:
+        return sqlite3.IntegrityError
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/db/index/hnswlib.py` & `chromadb-client-0.3.27.dev0/chromadb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb/db/migrations.py` & `chromadb-client-0.3.27.dev0/chromadb/db/migrations.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     identifying the database implementation.
     """
 
     _settings: Settings
 
     def __init__(self, system: System) -> None:
         self._settings = system.settings
-        super().__init__()
+        super().__init__(system)
 
     @staticmethod
     @abstractmethod
     def migration_scope() -> str:
         """The database implementation to use for migrations (e.g, sqlite, pgsql)"""
         pass
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/errors.py` & `chromadb-client-0.3.27.dev0/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb/server/fastapi/__init__.py` & `chromadb-client-0.3.27.dev0/chromadb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb/server/fastapi/types.py` & `chromadb-client-0.3.27.dev0/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb/telemetry/__init__.py` & `chromadb-client-0.3.27.dev0/chromadb/telemetry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dataclasses import asdict, dataclass
 import os
 from typing import Callable, ClassVar, Dict, Any
 import uuid
 import time
 from threading import Event, Thread
 import chromadb
+from chromadb.config import Component
 from pathlib import Path
 from enum import Enum
 
 TELEMETRY_WHITELISTED_SETTINGS = [
     "chroma_db_impl",
     "chroma_api_impl",
     "chroma_server_ssl_enabled",
@@ -49,15 +50,15 @@
         return self.interval - ((time.time() - self.start) % self.interval)
 
     def stop(self) -> None:
         self.event.set()
         self.thread.join()
 
 
-class Telemetry:
+class Telemetry(Component):
     USER_ID_PATH = str(Path.home() / ".cache" / "chroma" / "telemetry_user_id")
     UNKNOWN_USER_ID = "UNKNOWN"
     SERVER_CONTEXT: ServerContext = ServerContext.NONE
     _curr_user_id = None
 
     @abstractmethod
     def capture(self, event: TelemetryEvent) -> None:
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/telemetry/events.py` & `chromadb-client-0.3.27.dev0/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb/telemetry/posthog.py` & `chromadb-client-0.3.27.dev0/chromadb/telemetry/posthog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import posthog
 import logging
 import sys
 from chromadb.config import System
 from chromadb.telemetry import Telemetry, TelemetryEvent
+from overrides import override
 
 logger = logging.getLogger(__name__)
 
 
 class Posthog(Telemetry):
     def __init__(self, system: System):
         if not system.settings.anonymized_telemetry or "pytest" in sys.modules:
@@ -16,15 +17,17 @@
                 "Anonymized telemetry enabled. See https://docs.trychroma.com/telemetry for more information."
             )
 
         posthog.project_api_key = "phc_YeUxaojbKk5KPi8hNlx1bBKHzuZ4FDtl67kH1blv8Bh"
         posthog_logger = logging.getLogger("posthog")
         # Silence posthog's logging
         posthog_logger.disabled = True
+        super().__init__(system)
 
+    @override
     def capture(self, event: TelemetryEvent) -> None:
         try:
             posthog.capture(
                 self.user_id,
                 event.name,
                 {**(event.properties), "chroma_context": self.context},
             )
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/db/test_base.py` & `chromadb-client-0.3.27.dev0/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/db/test_migrations.py` & `chromadb-client-0.3.27.dev0/chromadb/test/db/test_migrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 from chromadb.config import System, Settings
 from pytest import FixtureRequest
 import copy
 
 
 def sqlite() -> Generator[migrations.MigratableDB, None, None]:
     """Fixture generator for sqlite DB"""
-    yield SqliteDB(
+    db = SqliteDB(
         System(
             Settings(sqlite_database=":memory:", migrations="none", allow_reset=True)
         )
     )
+    db.start()
+    yield db
 
 
 def db_fixtures() -> List[Callable[[], Generator[migrations.MigratableDB, None, None]]]:
     return [sqlite]
 
 
 @pytest.fixture(scope="module", params=db_fixtures())
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/hnswlib/test_hnswlib.py` & `chromadb-client-0.3.27.dev0/chromadb/test/hnswlib/test_hnswlib.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/property/invariants.py` & `chromadb-client-0.3.27.dev0/chromadb/test/property/invariants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,183 +1,199 @@
 import math
-from chromadb.test.property.strategies import RecordSet
-from typing import Callable, Optional, Union, List, TypeVar
+from chromadb.test.property.strategies import NormalizedRecordSet, RecordSet
+from typing import Callable, Optional, Tuple, Union, List, TypeVar, cast, Dict
 from typing_extensions import Literal
 import numpy as np
+import numpy.typing as npt
 from chromadb.api import types
 from chromadb.api.models.Collection import Collection
 from hypothesis import note
 from hypothesis.errors import InvalidArgument
 
 T = TypeVar("T")
 
 
-def maybe_wrap(value: Union[T, List[T]]) -> Union[None, List[T]]:
+def wrap(value: Union[T, List[T]]) -> List[T]:
     """Wrap a value in a list if it is not a list"""
     if value is None:
-        return None
+        raise InvalidArgument("value cannot be None")
     elif isinstance(value, List):
         return value
     else:
         return [value]
 
 
-def wrap_all(embeddings: RecordSet) -> RecordSet:
+def wrap_all(record_set: RecordSet) -> NormalizedRecordSet:
     """Ensure that an embedding set has lists for all its values"""
 
-    if embeddings["embeddings"] is None:
+    embedding_list: Optional[types.Embeddings]
+    if record_set["embeddings"] is None:
         embedding_list = None
-    elif isinstance(embeddings["embeddings"], list):
-        if len(embeddings["embeddings"]) > 0:
-            if isinstance(embeddings["embeddings"][0], list):
-                embedding_list = embeddings["embeddings"]
+    elif isinstance(record_set["embeddings"], list):
+        assert record_set["embeddings"] is not None
+        if len(record_set["embeddings"]) > 0 and not all(
+            isinstance(embedding, list) for embedding in record_set["embeddings"]
+        ):
+            if all(isinstance(e, (int, float)) for e in record_set["embeddings"]):
+                embedding_list = cast(types.Embeddings, [record_set["embeddings"]])
             else:
-                embedding_list = [embeddings["embeddings"]]
+                raise InvalidArgument("an embedding must be a list of floats or ints")
         else:
-            embedding_list = []
+            embedding_list = cast(types.Embeddings, record_set["embeddings"])
     else:
-        raise InvalidArgument("embeddings must be a list, list of lists, or None")
+        raise InvalidArgument(
+            "embeddings must be a list of lists, a list of numbers, or None"
+        )
 
     return {
-        "ids": maybe_wrap(embeddings["ids"]),  # type: ignore
-        "documents": maybe_wrap(embeddings["documents"]),  # type: ignore
-        "metadatas": maybe_wrap(embeddings["metadatas"]),  # type: ignore
+        "ids": wrap(record_set["ids"]),
+        "documents": wrap(record_set["documents"])
+        if record_set["documents"] is not None
+        else None,
+        "metadatas": wrap(record_set["metadatas"])
+        if record_set["metadatas"] is not None
+        else None,
         "embeddings": embedding_list,
     }
 
 
-def count(collection: Collection, embeddings: RecordSet):
+def count(collection: Collection, record_set: RecordSet) -> None:
     """The given collection count is equal to the number of embeddings"""
     count = collection.count()
-    embeddings = wrap_all(embeddings)
-    assert count == len(embeddings["ids"])
+    normalized_record_set = wrap_all(record_set)
+    assert count == len(normalized_record_set["ids"])
 
 
 def _field_matches(
     collection: Collection,
-    embeddings: RecordSet,
+    normalized_record_set: NormalizedRecordSet,
     field_name: Union[Literal["documents"], Literal["metadatas"]],
-):
+) -> None:
     """
     The actual embedding field is equal to the expected field
     field_name: one of [documents, metadatas]
     """
-    result = collection.get(ids=embeddings["ids"], include=[field_name])
+    result = collection.get(ids=normalized_record_set["ids"], include=[field_name])
     # The test_out_of_order_ids test fails because of this in test_add.py
     # Here we sort by the ids to match the input order
-    embedding_id_to_index = {id: i for i, id in enumerate(embeddings["ids"])}
+    embedding_id_to_index = {id: i for i, id in enumerate(normalized_record_set["ids"])}
     actual_field = result[field_name]
     # This assert should never happen, if we include metadatas/documents it will be
     # [None, None..] if there is no metadata. It will not be just None.
     assert actual_field is not None
-    actual_field = sorted(
+    sorted_field = sorted(
         enumerate(actual_field),
         key=lambda index_and_field_value: embedding_id_to_index[
             result["ids"][index_and_field_value[0]]
         ],
     )
-    actual_field = [field_value for _, field_value in actual_field]
+    field_values = [field_value for _, field_value in sorted_field]
 
-    expected_field = embeddings[field_name]
+    expected_field = normalized_record_set[field_name]
     if expected_field is None:
         # Since an RecordSet is the user input, we need to convert the documents to
         # a List since thats what the API returns -> none per entry
-        expected_field = [None] * len(embeddings["ids"])
-    assert actual_field == expected_field
+        expected_field = [None] * len(normalized_record_set["ids"])  # type: ignore
+    assert field_values == expected_field
 
 
-def ids_match(collection: Collection, embeddings: RecordSet):
+def ids_match(collection: Collection, record_set: RecordSet) -> None:
     """The actual embedding ids is equal to the expected ids"""
-    embeddings = wrap_all(embeddings)
-    actual_ids = collection.get(ids=embeddings["ids"], include=[])["ids"]
+    normalized_record_set = wrap_all(record_set)
+    actual_ids = collection.get(ids=normalized_record_set["ids"], include=[])["ids"]
     # The test_out_of_order_ids test fails because of this in test_add.py
     # Here we sort the ids to match the input order
-    embedding_id_to_index = {id: i for i, id in enumerate(embeddings["ids"])}
+    embedding_id_to_index = {id: i for i, id in enumerate(normalized_record_set["ids"])}
     actual_ids = sorted(actual_ids, key=lambda id: embedding_id_to_index[id])
-    assert actual_ids == embeddings["ids"]
+    assert actual_ids == normalized_record_set["ids"]
 
 
-def metadatas_match(collection: Collection, embeddings: RecordSet):
+def metadatas_match(collection: Collection, record_set: RecordSet) -> None:
     """The actual embedding metadata is equal to the expected metadata"""
-    embeddings = wrap_all(embeddings)
-    _field_matches(collection, embeddings, "metadatas")
+    normalized_record_set = wrap_all(record_set)
+    _field_matches(collection, normalized_record_set, "metadatas")
 
 
-def documents_match(collection: Collection, embeddings: RecordSet):
+def documents_match(collection: Collection, record_set: RecordSet) -> None:
     """The actual embedding documents is equal to the expected documents"""
-    embeddings = wrap_all(embeddings)
-    _field_matches(collection, embeddings, "documents")
+    normalized_record_set = wrap_all(record_set)
+    _field_matches(collection, normalized_record_set, "documents")
 
 
-def no_duplicates(collection: Collection):
+def no_duplicates(collection: Collection) -> None:
     ids = collection.get()["ids"]
     assert len(ids) == len(set(ids))
 
 
 # These match what the spec of hnswlib is
 # This epsilon is used to prevent division by zero and the value is the same
 # https://github.com/nmslib/hnswlib/blob/359b2ba87358224963986f709e593d799064ace6/python_bindings/bindings.cpp#L238
 NORM_EPS = 1e-30
-distance_functions = {
-    "l2": lambda x, y: np.linalg.norm(x - y) ** 2,
-    "cosine": lambda x, y: 1
-    - np.dot(x, y) / ((np.linalg.norm(x) + NORM_EPS) * (np.linalg.norm(y) + NORM_EPS)),
-    "ip": lambda x, y: 1 - np.dot(x, y),
+distance_functions: Dict[str, Callable[[npt.ArrayLike, npt.ArrayLike], float]] = {
+    "l2": lambda x, y: np.linalg.norm(x - y) ** 2,  # type: ignore
+    "cosine": lambda x, y: 1 - np.dot(x, y) / ((np.linalg.norm(x) + NORM_EPS) * (np.linalg.norm(y) + NORM_EPS)),  # type: ignore
+    "ip": lambda x, y: 1 - np.dot(x, y),  # type: ignore
 }
 
 
 def _exact_distances(
     query: types.Embeddings,
     targets: types.Embeddings,
-    distance_fn: Callable = lambda x, y: np.linalg.norm(x - y) ** 2,
-):
+    distance_fn: Callable[[npt.ArrayLike, npt.ArrayLike], float] = distance_functions[
+        "l2"
+    ],
+) -> Tuple[List[List[int]], List[List[float]]]:
     """Return the ordered indices and distances from each query to each target"""
     np_query = np.array(query)
     np_targets = np.array(targets)
 
     # Compute the distance between each query and each target, using the distance function
     distances = np.apply_along_axis(
         lambda query: np.apply_along_axis(distance_fn, 1, np_targets, query),
         1,
         np_query,
     )
     # Sort the distances and return the indices
-    return np.argsort(distances), distances
+    return np.argsort(distances).tolist(), distances.tolist()
 
 
 def ann_accuracy(
     collection: Collection,
     record_set: RecordSet,
     n_results: int = 1,
     min_recall: float = 0.99,
     embedding_function: Optional[types.EmbeddingFunction] = None,
-):
+) -> None:
     """Validate that the API performs nearest_neighbor searches correctly"""
-    record_set = wrap_all(record_set)
+    normalized_record_set = wrap_all(record_set)
 
-    if len(record_set["ids"]) == 0:
+    if len(normalized_record_set["ids"]) == 0:
         return  # nothing to test here
 
-    embeddings = record_set["embeddings"]
+    embeddings: Optional[types.Embeddings] = normalized_record_set["embeddings"]
     have_embeddings = embeddings is not None and len(embeddings) > 0
     if not have_embeddings:
         assert embedding_function is not None
-        assert record_set["documents"] is not None
+        assert normalized_record_set["documents"] is not None
+        assert isinstance(normalized_record_set["documents"], list)
         # Compute the embeddings for the documents
-        embeddings = embedding_function(record_set["documents"])
+        embeddings = embedding_function(normalized_record_set["documents"])
 
     # l2 is the default distance function
     distance_function = distance_functions["l2"]
     accuracy_threshold = 1e-6
+    assert collection.metadata is not None
+    assert embeddings is not None
     if "hnsw:space" in collection.metadata:
         space = collection.metadata["hnsw:space"]
         # TODO: ip and cosine are numerically unstable in HNSW.
         # The higher the dimensionality, the more noise is introduced, since each float element
         # of the vector has noise added, which is then subsequently included in all normalization calculations.
         # This means that higher dimensions will have more noise, and thus more error.
+        assert all(isinstance(e, list) for e in embeddings)
         dim = len(embeddings[0])
         accuracy_threshold = accuracy_threshold * math.pow(10, int(math.log10(dim)))
 
         if space == "cosine":
             distance_function = distance_functions["cosine"]
 
         if space == "ip":
@@ -185,25 +201,30 @@
 
     # Perform exact distance computation
     indices, distances = _exact_distances(
         embeddings, embeddings, distance_fn=distance_function
     )
 
     query_results = collection.query(
-        query_embeddings=record_set["embeddings"],
-        query_texts=record_set["documents"] if not have_embeddings else None,
+        query_embeddings=normalized_record_set["embeddings"],
+        query_texts=normalized_record_set["documents"] if not have_embeddings else None,
         n_results=n_results,
         include=["embeddings", "documents", "metadatas", "distances"],
     )
 
+    assert query_results["distances"] is not None
+    assert query_results["documents"] is not None
+    assert query_results["metadatas"] is not None
+    assert query_results["embeddings"] is not None
+
     # Dict of ids to indices
-    id_to_index = {id: i for i, id in enumerate(record_set["ids"])}
+    id_to_index = {id: i for i, id in enumerate(normalized_record_set["ids"])}
     missing = 0
     for i, (indices_i, distances_i) in enumerate(zip(indices, distances)):
-        expected_ids = np.array(record_set["ids"])[indices_i[:n_results]]
+        expected_ids = np.array(normalized_record_set["ids"])[indices_i[:n_results]]
         missing += len(set(expected_ids) - set(query_results["ids"][i]))
 
         # For each id in the query results, find the index in the embeddings set
         # and assert that the embeddings are the same
         for j, id in enumerate(query_results["ids"][i]):
             # This may be because the true nth nearest neighbor didn't get returned by the ANN query
             unexpected_id = id not in expected_ids
@@ -221,24 +242,26 @@
                     missing -= 1
                 else:
                     continue
             else:
                 assert correct_distance
 
             assert np.allclose(embeddings[index], query_results["embeddings"][i][j])
-            if record_set["documents"] is not None:
+            if normalized_record_set["documents"] is not None:
                 assert (
-                    record_set["documents"][index] == query_results["documents"][i][j]
+                    normalized_record_set["documents"][index]
+                    == query_results["documents"][i][j]
                 )
-            if record_set["metadatas"] is not None:
+            if normalized_record_set["metadatas"] is not None:
                 assert (
-                    record_set["metadatas"][index] == query_results["metadatas"][i][j]
+                    normalized_record_set["metadatas"][index]
+                    == query_results["metadatas"][i][j]
                 )
 
-    size = len(record_set["ids"])
+    size = len(normalized_record_set["ids"])
     recall = (size - missing) / size
 
     try:
         note(
             f"recall: {recall}, missing {missing} out of {size}, accuracy threshold {accuracy_threshold}"
         )
     except InvalidArgument:
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/property/strategies.py` & `chromadb-client-0.3.27.dev0/chromadb/test/property/strategies.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import hashlib
 import hypothesis
 import hypothesis.strategies as st
-from typing import Optional, List, Dict, Union
+from typing import Any, Optional, List, Dict, Union
 from typing_extensions import TypedDict
 import numpy as np
+import numpy.typing as npt
 import chromadb.api.types as types
 import re
 from hypothesis.strategies._internal.strategies import SearchStrategy
 from hypothesis.errors import InvalidDefinition
+from hypothesis.stateful import RuleBasedStateMachine
 
 from dataclasses import dataclass
 
+from chromadb.api.types import Documents, Embeddings, Metadata
+
 # Set the random seed for reproducibility
 np.random.seed(0)  # unnecessary, hypothesis does this for us
 
 # See Hypothesis documentation for creating strategies at
 # https://hypothesis.readthedocs.io/en/latest/data.html
 
 # NOTE: Because these strategies are used in state machines, we need to
@@ -49,34 +53,77 @@
 
     ids: Union[types.ID, List[types.ID]]
     embeddings: Optional[Union[types.Embeddings, types.Embedding]]
     metadatas: Optional[Union[List[types.Metadata], types.Metadata]]
     documents: Optional[Union[List[types.Document], types.Document]]
 
 
+class NormalizedRecordSet(TypedDict):
+    """
+    A RecordSet, with all fields normalized to lists.
+    """
+
+    ids: List[types.ID]
+    embeddings: Optional[types.Embeddings]
+    metadatas: Optional[List[types.Metadata]]
+    documents: Optional[List[types.Document]]
+
+
+class StateMachineRecordSet(TypedDict):
+    """
+    Represents the internal state of a state machine in hypothesis tests.
+    """
+
+    ids: List[types.ID]
+    embeddings: types.Embeddings
+    metadatas: List[Optional[types.Metadata]]
+    documents: List[Optional[types.Document]]
+
+
+class Record(TypedDict):
+    """
+    A single generated record.
+    """
+
+    id: types.ID
+    embedding: Optional[types.Embedding]
+    metadata: Optional[types.Metadata]
+    document: Optional[types.Document]
+
+
 # TODO: support arbitrary text everywhere so we don't SQL-inject ourselves.
 # TODO: support empty strings everywhere
 sql_alphabet = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789-_"
 safe_text = st.text(alphabet=sql_alphabet, min_size=1)
 
 # Workaround for FastAPI json encoding peculiarities
 # https://github.com/tiangolo/fastapi/blob/8ac8d70d52bb0dd9eb55ba4e22d3e383943da05c/fastapi/encoders.py#L104
 safe_text = safe_text.filter(lambda s: not s.startswith("_sa"))
 
 safe_integers = st.integers(
     min_value=-(2**31), max_value=2**31 - 1
 )  # TODO: handle longs
 safe_floats = st.floats(
-    allow_infinity=False, allow_nan=False, allow_subnormal=False
+    allow_infinity=False,
+    allow_nan=False,
+    allow_subnormal=False,
+    min_value=-1e6,
+    max_value=1e6,
 )  # TODO: handle infinity and NAN
 
-safe_values = [safe_text, safe_integers, safe_floats]
+safe_values: List[SearchStrategy[Union[int, float, str]]] = [
+    safe_text,
+    safe_integers,
+    safe_floats,
+]
 
 
-def one_or_both(strategy_a, strategy_b):
+def one_or_both(
+    strategy_a: st.SearchStrategy[Any], strategy_b: st.SearchStrategy[Any]
+) -> st.SearchStrategy[Any]:
     return st.one_of(
         st.tuples(strategy_a, strategy_b),
         st.tuples(strategy_a, st.none()),
         st.tuples(st.none(), strategy_b),
     )
 
 
@@ -86,47 +133,53 @@
 )
 
 float_types = [np.float16, np.float32, np.float64]
 int_types = [np.int16, np.int32, np.int64]  # TODO: handle int types
 
 
 @st.composite
-def collection_name(draw) -> str:
+def collection_name(draw: st.DrawFn) -> str:
     _collection_name_re = re.compile(r"^[a-zA-Z][a-zA-Z0-9-]{1,60}[a-zA-Z0-9]$")
     _ipv4_address_re = re.compile(r"^([0-9]{1,3}\.){3}[0-9]{1,3}$")
     _two_periods_re = re.compile(r"\.\.")
 
-    name = draw(st.from_regex(_collection_name_re))
+    name: str = draw(st.from_regex(_collection_name_re))
     hypothesis.assume(not _ipv4_address_re.match(name))
     hypothesis.assume(not _two_periods_re.search(name))
 
     return name
 
 
 collection_metadata = st.one_of(
     st.none(), st.dictionaries(safe_text, st.one_of(*safe_values))
 )
 
 
 # TODO: Use a hypothesis strategy while maintaining embedding uniqueness
 #       Or handle duplicate embeddings within a known epsilon
-def create_embeddings(dim: int, count: int, dtype: np.dtype) -> types.Embeddings:
-    return (
+def create_embeddings(
+    dim: int,
+    count: int,
+    dtype: npt.DTypeLike,
+) -> types.Embeddings:
+    embeddings: types.Embeddings = (
         np.random.uniform(
             low=-1.0,
             high=1.0,
             size=(count, dim),
         )
         .astype(dtype)
         .tolist()
     )
 
+    return embeddings
+
 
 class hashing_embedding_function(types.EmbeddingFunction):
-    def __init__(self, dim: int, dtype: np.dtype) -> None:
+    def __init__(self, dim: int, dtype: npt.DTypeLike) -> None:
         self.dim = dim
         self.dtype = dtype
 
     def __call__(self, texts: types.Documents) -> types.Embeddings:
         # Hash the texts and convert to hex strings
         hashed_texts = [
             list(hashlib.sha256(text.encode("utf-8")).hexdigest()) for text in texts
@@ -134,44 +187,51 @@
         # Pad with repetition, or truncate the hex strings to the desired dimension
         padded_texts = [
             text * (self.dim // len(text)) + text[: self.dim % len(text)]
             for text in hashed_texts
         ]
 
         # Convert the hex strings to dtype
-        return np.array(
+        embeddings: types.Embeddings = np.array(
             [[int(char, 16) / 15.0 for char in text] for text in padded_texts],
             dtype=self.dtype,
         ).tolist()
 
+        return embeddings
+
+
+class not_implemented_embedding_function(types.EmbeddingFunction):
+    def __call__(self, texts: Documents) -> Embeddings:
+        assert False, "This embedding function is not implemented"
+
 
 def embedding_function_strategy(
-    dim: int, dtype: np.dtype
+    dim: int, dtype: npt.DTypeLike
 ) -> st.SearchStrategy[types.EmbeddingFunction]:
     return st.just(hashing_embedding_function(dim, dtype))
 
 
 @dataclass
 class Collection:
     name: str
     metadata: Optional[types.Metadata]
     dimension: int
-    dtype: np.dtype
-    known_metadata_keys: Dict[str, st.SearchStrategy]
+    dtype: npt.DTypeLike
+    known_metadata_keys: types.Metadata
     known_document_keywords: List[str]
     has_documents: bool = False
     has_embeddings: bool = False
     embedding_function: Optional[types.EmbeddingFunction] = None
 
 
 @st.composite
 def collections(
-    draw,
-    add_filterable_data=False,
-    with_hnsw_params=False,
+    draw: st.DrawFn,
+    add_filterable_data: bool = False,
+    with_hnsw_params: bool = False,
     has_embeddings: Optional[bool] = None,
     has_documents: Optional[bool] = None,
 ) -> Collection:
     """Strategy to generate a Collection object. If add_filterable_data is True, then known_metadata_keys and known_document_keywords will be populated with consistent data."""
 
     assert not ((has_embeddings is False) and (has_documents is False))
 
@@ -186,32 +246,34 @@
         metadata.update(test_hnsw_config)
         # Sometimes, select a space at random
         if draw(st.booleans()):
             # TODO: pull the distance functions from a source of truth that lives not
             # in tests once https://github.com/chroma-core/issues/issues/61 lands
             metadata["hnsw:space"] = draw(st.sampled_from(["cosine", "l2", "ip"]))
 
-    known_metadata_keys = {}
+    known_metadata_keys: Dict[str, Union[int, str, float]] = {}
     if add_filterable_data:
         while len(known_metadata_keys) < 5:
             key = draw(safe_text)
-            known_metadata_keys[key] = draw(st.sampled_from(safe_values))
+            known_metadata_keys[key] = draw(st.one_of(*safe_values))
 
     if has_documents is None:
         has_documents = draw(st.booleans())
+    assert has_documents is not None
     if has_documents and add_filterable_data:
         known_document_keywords = draw(st.lists(safe_text, min_size=5, max_size=5))
     else:
         known_document_keywords = []
 
     if not has_documents:
         has_embeddings = True
     else:
         if has_embeddings is None:
             has_embeddings = draw(st.booleans())
+    assert has_embeddings is not None
 
     embedding_function = draw(embedding_function_strategy(dimension, dtype))
 
     return Collection(
         name=name,
         metadata=metadata,
         dimension=dimension,
@@ -221,119 +283,113 @@
         known_document_keywords=known_document_keywords,
         has_embeddings=has_embeddings,
         embedding_function=embedding_function,
     )
 
 
 @st.composite
-def metadata(draw, collection: Collection):
+def metadata(draw: st.DrawFn, collection: Collection) -> types.Metadata:
     """Strategy for generating metadata that could be a part of the given collection"""
     # First draw a random dictionary.
-    md = draw(st.dictionaries(safe_text, st.one_of(*safe_values)))
+    metadata: types.Metadata = draw(st.dictionaries(safe_text, st.one_of(*safe_values)))
     # Then, remove keys that overlap with the known keys for the coll
     # to avoid type errors when comparing.
     if collection.known_metadata_keys:
         for key in collection.known_metadata_keys.keys():
-            if key in md:
-                del md[key]
+            if key in metadata:
+                del metadata[key]
         # Finally, add in some of the known keys for the collection
-        md.update(
-            draw(st.fixed_dictionaries({}, optional=collection.known_metadata_keys))
-        )
-    return md
+        sampling_dict: Dict[str, st.SearchStrategy[Union[str, int, float]]] = {
+            k: st.just(v) for k, v in collection.known_metadata_keys.items()
+        }
+        metadata.update(draw(st.fixed_dictionaries({}, optional=sampling_dict)))
+    return metadata
 
 
 @st.composite
-def document(draw, collection: Collection):
+def document(draw: st.DrawFn, collection: Collection) -> types.Document:
     """Strategy for generating documents that could be a part of the given collection"""
 
     if collection.known_document_keywords:
         known_words_st = st.sampled_from(collection.known_document_keywords)
     else:
         known_words_st = st.text(min_size=1)
 
     random_words_st = st.text(min_size=1)
     words = draw(st.lists(st.one_of(known_words_st, random_words_st), min_size=1))
     return " ".join(words)
 
 
 @st.composite
-def record(draw, collection: Collection, id_strategy=safe_text):
-    md = draw(metadata(collection))
-
-    if collection.has_embeddings:
-        embedding = create_embeddings(collection.dimension, 1, collection.dtype)[0]
-    else:
-        embedding = None
-    if collection.has_documents:
-        doc = draw(document(collection))
-    else:
-        doc = None
-
-    return {
-        "id": draw(id_strategy),
-        "embedding": embedding,
-        "metadata": md,
-        "document": doc,
-    }
-
-
-@st.composite
 def recordsets(
-    draw,
-    collection_strategy=collections(),
-    id_strategy=safe_text,
-    min_size=1,
-    max_size=50,
+    draw: st.DrawFn,
+    collection_strategy: SearchStrategy[Collection] = collections(),
+    id_strategy: SearchStrategy[str] = safe_text,
+    min_size: int = 1,
+    max_size: int = 50,
 ) -> RecordSet:
     collection = draw(collection_strategy)
 
-    records = draw(
-        st.lists(record(collection, id_strategy), min_size=min_size, max_size=max_size)
+    ids = list(
+        draw(st.lists(id_strategy, min_size=min_size, max_size=max_size, unique=True))
     )
 
-    records = {r["id"]: r for r in records}.values()  # Remove duplicates
-
-    ids = [r["id"] for r in records]
-    embeddings = (
-        [r["embedding"] for r in records] if collection.has_embeddings else None
+    embeddings: Optional[Embeddings] = None
+    if collection.has_embeddings:
+        embeddings = create_embeddings(collection.dimension, len(ids), collection.dtype)
+    metadatas = draw(
+        st.lists(metadata(collection), min_size=len(ids), max_size=len(ids))
     )
-    metadatas = [r["metadata"] for r in records]
-    documents = [r["document"] for r in records] if collection.has_documents else None
+    documents: Optional[Documents] = None
+    if collection.has_documents:
+        documents = draw(
+            st.lists(document(collection), min_size=len(ids), max_size=len(ids))
+        )
 
     # in the case where we have a single record, sometimes exercise
-    # the code that handles individual values rather than lists
-    if len(records) == 1:
-        if draw(st.booleans()):
-            ids = ids[0]
-        if collection.has_embeddings and draw(st.booleans()):
-            embeddings = embeddings[0]
-        if draw(st.booleans()):
-            metadatas = metadatas[0]
-        if collection.has_documents and draw(st.booleans()):
-            documents = documents[0]
+    # the code that handles individual values rather than lists.
+    # In this case, any field may be a list or a single value.
+    if len(ids) == 1:
+        single_id: Union[str, List[str]] = ids[0] if draw(st.booleans()) else ids
+        single_embedding = (
+            embeddings[0]
+            if embeddings is not None and draw(st.booleans())
+            else embeddings
+        )
+        single_metadata: Union[Metadata, List[Metadata]] = (
+            metadatas[0] if draw(st.booleans()) else metadatas
+        )
+        single_document = (
+            documents[0] if documents is not None and draw(st.booleans()) else documents
+        )
+        return {
+            "ids": single_id,
+            "embeddings": single_embedding,
+            "metadatas": single_metadata,
+            "documents": single_document,
+        }
 
     return {
         "ids": ids,
         "embeddings": embeddings,
         "metadatas": metadatas,
         "documents": documents,
     }
 
 
 # This class is mostly cloned from from hypothesis.stateful.RuleStrategy,
 # but always runs all the rules, instead of using a FeatureStrategy to
 # enable/disable rules. Disabled rules cause the entire test to be marked invalida and,
 # combined with the complexity of our other strategies, leads to an
 # unacceptably increased incidence of hypothesis.errors.Unsatisfiable.
-class DeterministicRuleStrategy(SearchStrategy):
-    def __init__(self, machine):
-        super().__init__()
+class DeterministicRuleStrategy(SearchStrategy):  # type: ignore
+    def __init__(self, machine: RuleBasedStateMachine) -> None:
+        super().__init__()  # type: ignore
         self.machine = machine
-        self.rules = list(machine.rules())
+        self.rules = list(machine.rules())  # type: ignore
 
         # The order is a bit arbitrary. Primarily we're trying to group rules
         # that write to the same location together, and to put rules with no
         # target first as they have less effect on the structure. We order from
         # fewer to more arguments on grounds that it will plausibly need less
         # data. This probably won't work especially well and we could be
         # smarter about it, but it's better than just doing it in definition
@@ -342,114 +398,143 @@
             key=lambda rule: (
                 sorted(rule.targets),
                 len(rule.arguments),
                 rule.function.__name__,
             )
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "{}(machine={}({{...}}))".format(
             self.__class__.__name__,
             self.machine.__class__.__name__,
         )
 
-    def do_draw(self, data):
+    def do_draw(self, data):  # type: ignore
         if not any(self.is_valid(rule) for rule in self.rules):
             msg = f"No progress can be made from state {self.machine!r}"
             raise InvalidDefinition(msg) from None
 
         rule = data.draw(st.sampled_from([r for r in self.rules if self.is_valid(r)]))
         argdata = data.draw(rule.arguments_strategy)
         return (rule, argdata)
 
-    def is_valid(self, rule):
+    def is_valid(self, rule) -> bool:  # type: ignore
         if not all(precond(self.machine) for precond in rule.preconditions):
             return False
 
         for b in rule.bundles:
-            bundle = self.machine.bundle(b.name)
+            bundle = self.machine.bundle(b.name)  # type: ignore
             if not bundle:
                 return False
         return True
 
 
 @st.composite
-def where_clause(draw, collection):
+def where_clause(draw: st.DrawFn, collection: Collection) -> types.Where:
     """Generate a filter that could be used in a query against the given collection"""
 
     known_keys = sorted(collection.known_metadata_keys.keys())
 
     key = draw(st.sampled_from(known_keys))
-    value = draw(collection.known_metadata_keys[key])
+    value = collection.known_metadata_keys[key]
 
-    legal_ops = [None, "$eq", "$ne"]
+    legal_ops: List[Optional[str]] = [None, "$eq", "$ne"]
     if not isinstance(value, str):
-        legal_ops = ["$gt", "$lt", "$lte", "$gte"] + legal_ops
+        legal_ops.extend(["$gt", "$lt", "$lte", "$gte"])
+    if isinstance(value, float):
+        # Add or subtract a small number to avoid floating point rounding errors
+        value = value + draw(st.sampled_from([1e-6, -1e-6]))
 
-    op = draw(st.sampled_from(legal_ops))
+    op: types.WhereOperator = draw(st.sampled_from(legal_ops))
 
     if op is None:
         return {key: value}
     else:
         return {key: {op: value}}
 
 
 @st.composite
-def where_doc_clause(draw, collection):
+def where_doc_clause(draw: st.DrawFn, collection: Collection) -> types.WhereDocument:
     """Generate a where_document filter that could be used against the given collection"""
     if collection.known_document_keywords:
         word = draw(st.sampled_from(collection.known_document_keywords))
     else:
         word = draw(safe_text)
     return {"$contains": word}
 
 
-@st.composite
-def binary_operator_clause(draw, base_st):
-    op = draw(st.sampled_from(["$and", "$or"]))
-    return {op: [draw(base_st), draw(base_st)]}
+def binary_operator_clause(
+    base_st: SearchStrategy[types.Where],
+) -> SearchStrategy[types.Where]:
+    op: SearchStrategy[types.LogicalOperator] = st.sampled_from(["$and", "$or"])
+    return st.dictionaries(
+        keys=op,
+        values=st.lists(base_st, max_size=2, min_size=2),
+        min_size=1,
+        max_size=1,
+    )
+
+
+def binary_document_operator_clause(
+    base_st: SearchStrategy[types.WhereDocument],
+) -> SearchStrategy[types.WhereDocument]:
+    op: SearchStrategy[types.LogicalOperator] = st.sampled_from(["$and", "$or"])
+    return st.dictionaries(
+        keys=op,
+        values=st.lists(base_st, max_size=2, min_size=2),
+        min_size=1,
+        max_size=1,
+    )
 
 
 @st.composite
-def recursive_where_clause(draw, collection):
+def recursive_where_clause(draw: st.DrawFn, collection: Collection) -> types.Where:
     base_st = where_clause(collection)
-    return draw(st.recursive(base_st, binary_operator_clause))
+    where: types.Where = draw(st.recursive(base_st, binary_operator_clause))
+    return where
 
 
 @st.composite
-def recursive_where_doc_clause(draw, collection):
+def recursive_where_doc_clause(
+    draw: st.DrawFn, collection: Collection
+) -> types.WhereDocument:
     base_st = where_doc_clause(collection)
-    return draw(st.recursive(base_st, binary_operator_clause))
+    where: types.WhereDocument = draw(
+        st.recursive(base_st, binary_document_operator_clause)
+    )
+    return where
 
 
 class Filter(TypedDict):
-    where: Optional[Dict[str, Union[str, int, float]]]
+    where: Optional[types.Where]
     ids: Optional[Union[str, List[str]]]
     where_document: Optional[types.WhereDocument]
 
 
 @st.composite
 def filters(
-    draw,
+    draw: st.DrawFn,
     collection_st: st.SearchStrategy[Collection],
     recordset_st: st.SearchStrategy[RecordSet],
-    include_all_ids=False,
+    include_all_ids: bool = False,
 ) -> Filter:
     collection = draw(collection_st)
     recordset = draw(recordset_st)
 
     where_clause = draw(st.one_of(st.none(), recursive_where_clause(collection)))
     where_document_clause = draw(
         st.one_of(st.none(), recursive_where_doc_clause(collection))
     )
 
-    ids = recordset["ids"]
+    ids: Optional[Union[List[types.ID], types.ID]]
     # Record sets can be a value instead of a list of values if there is only one record
-    if isinstance(ids, str):
-        ids = [ids]
+    if isinstance(recordset["ids"], str):
+        ids = [recordset["ids"]]
+    else:
+        ids = recordset["ids"]
 
     if not include_all_ids:
         ids = draw(st.one_of(st.none(), st.lists(st.sampled_from(ids))))
         if ids is not None:
             # Remove duplicates since hypothesis samples with replacement
             ids = list(set(ids))
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/property/test_collections.py` & `chromadb-client-0.3.27.dev0/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/property/test_cross_version_persist.py` & `chromadb-client-0.3.27.dev0/chromadb/test/property/test_cross_version_persist.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+from multiprocessing.connection import Connection
 import sys
 import os
 import shutil
 import subprocess
 import tempfile
-from typing import Generator, Tuple
+from types import ModuleType
+from typing import Callable, Generator, List, Tuple
 from hypothesis import given, settings
 import hypothesis.strategies as st
 import pytest
 import json
 from urllib import request
 from chromadb.api import API
+from chromadb.api.types import Documents, EmbeddingFunction, Embeddings
 import chromadb.test.property.strategies as strategies
 import chromadb.test.property.invariants as invariants
 from packaging import version as packaging_version
 import re
 import multiprocessing
 from chromadb import Client
 from chromadb.config import Settings
@@ -21,58 +24,60 @@
 MINIMUM_VERSION = "0.3.20"
 COLLECTION_NAME_LOWERCASE_VERSION = "0.3.21"
 version_re = re.compile(r"^[0-9]+\.[0-9]+\.[0-9]+$")
 
 
 def _patch_uppercase_coll_name(
     collection: strategies.Collection, embeddings: strategies.RecordSet
-):
+) -> None:
     """Old versions didn't handle uppercase characters in collection names"""
     collection.name = collection.name.lower()
 
 
 def _patch_empty_dict_metadata(
     collection: strategies.Collection, embeddings: strategies.RecordSet
-):
+) -> None:
     """Old versions do the wrong thing when metadata is a single empty dict"""
     if embeddings["metadatas"] == {}:
         embeddings["metadatas"] = None
 
 
-version_patches = [
+version_patches: List[
+    Tuple[str, Callable[[strategies.Collection, strategies.RecordSet], None]]
+] = [
     ("0.3.21", _patch_uppercase_coll_name),
     ("0.3.21", _patch_empty_dict_metadata),
 ]
 
 
 def patch_for_version(
-    version, collection: strategies.Collection, embeddings: strategies.RecordSet
-):
+    version: str, collection: strategies.Collection, embeddings: strategies.RecordSet
+) -> None:
     """Override aspects of the collection and embeddings, before testing, to account for
     breaking changes in old versions."""
 
     for patch_version, patch in version_patches:
         if packaging_version.Version(version) <= packaging_version.Version(
             patch_version
         ):
             patch(collection, embeddings)
 
 
-def versions():
+def versions() -> List[str]:
     """Returns the pinned minimum version and the latest version of chromadb."""
     url = "https://pypi.org/pypi/chromadb/json"
     data = json.load(request.urlopen(request.Request(url)))
     versions = list(data["releases"].keys())
     # Older versions on pypi contain "devXYZ" suffixes
     versions = [v for v in versions if version_re.match(v)]
     versions.sort(key=packaging_version.Version)
     return [MINIMUM_VERSION, versions[-1]]
 
 
-def configurations(versions):
+def configurations(versions: List[str]) -> List[Tuple[str, Settings]]:
     return [
         (
             version,
             Settings(
                 chroma_api_impl="local",
                 chroma_db_impl="duckdb+parquet",
                 persist_directory=tempfile.gettempdir() + "/tests/" + version + "/",
@@ -84,47 +89,47 @@
 
 test_old_versions = versions()
 base_install_dir = tempfile.gettempdir() + "/persistence_test_chromadb_versions"
 
 
 # This fixture is not shared with the rest of the tests because it is unique in how it
 # installs the versions of chromadb
-@pytest.fixture(scope="module", params=configurations(test_old_versions))
+@pytest.fixture(scope="module", params=configurations(test_old_versions))  # type: ignore
 def version_settings(request) -> Generator[Tuple[str, Settings], None, None]:
     configuration = request.param
     version = configuration[0]
     install_version(version)
     yield configuration
     # Cleanup the installed version
     path = get_path_to_version_install(version)
     shutil.rmtree(path)
     # Cleanup the persisted data
     data_path = configuration[1].persist_directory
     if os.path.exists(data_path):
         shutil.rmtree(data_path)
 
 
-def get_path_to_version_install(version):
+def get_path_to_version_install(version: str) -> str:
     return base_install_dir + "/" + version
 
 
-def get_path_to_version_library(version):
+def get_path_to_version_library(version: str) -> str:
     return get_path_to_version_install(version) + "/chromadb/__init__.py"
 
 
-def install_version(version):
+def install_version(version: str) -> None:
     # Check if already installed
     version_library = get_path_to_version_library(version)
     if os.path.exists(version_library):
         return
     path = get_path_to_version_install(version)
     install(f"chromadb=={version}", path)
 
 
-def install(pkg, path):
+def install(pkg: str, path: str) -> int:
     # -q -q to suppress pip output to ERROR level
     # https://pip.pypa.io/en/stable/cli/pip/#quiet
     print(f"Installing chromadb version {pkg} to {path}")
     return subprocess.check_call(
         [
             sys.executable,
             "-m",
@@ -134,15 +139,15 @@
             "install",
             pkg,
             "--target={}".format(path),
         ]
     )
 
 
-def switch_to_version(version):
+def switch_to_version(version: str) -> ModuleType:
     module_name = "chromadb"
     # Remove old version from sys.modules, except test modules
     old_modules = {
         n: m
         for n, m in sys.modules.items()
         if n == module_name or (n.startswith(module_name + "."))
     }
@@ -154,29 +159,35 @@
     sys.path.insert(0, get_path_to_version_install(version))
     import chromadb
 
     assert chromadb.__version__ == version
     return chromadb
 
 
+class not_implemented_ef(EmbeddingFunction):
+    def __call__(self, texts: Documents) -> Embeddings:
+        assert False, "Embedding function should not be called"
+
+
 def persist_generated_data_with_old_version(
-    version,
-    settings,
+    version: str,
+    settings: Settings,
     collection_strategy: strategies.Collection,
     embeddings_strategy: strategies.RecordSet,
-    conn,
-):
+    conn: Connection,
+) -> None:
     try:
         old_module = switch_to_version(version)
         api: API = old_module.Client(settings)
         api.reset()
         coll = api.create_collection(
             name=collection_strategy.name,
             metadata=collection_strategy.metadata,
-            embedding_function=lambda x: None,
+            # In order to test old versions, we can't rely on the not_implemented function
+            embedding_function=not_implemented_ef(),
         )
         coll.add(**embeddings_strategy)
         # We can't use the invariants module here because it uses the current version
         # Just use some basic checks for sanity and manual testing where you break the new
         # version
 
         check_embeddings = invariants.wrap_all(embeddings_strategy)
@@ -191,15 +202,15 @@
         api.persist()
     except Exception as e:
         conn.send(e)
         raise e
 
 
 # Since we can't pickle the embedding function, we always generate record sets with embeddings
-collection_st = st.shared(
+collection_st: st.SearchStrategy[strategies.Collection] = st.shared(
     strategies.collections(with_hnsw_params=True, has_embeddings=True), key="coll"
 )
 
 
 @given(
     collection_strategy=collection_st,
     embeddings_strategy=strategies.recordsets(collection_st),
@@ -210,15 +221,15 @@
     reason="The mininum supported versions of chroma do not work with python <= 3.7",
 )
 @settings(deadline=None)
 def test_cycle_versions(
     version_settings: Tuple[str, Settings],
     collection_strategy: strategies.Collection,
     embeddings_strategy: strategies.RecordSet,
-):
+) -> None:
     # # Test backwards compatibility
     # # For the current version, ensure that we can load a collection from
     # # the previous versions
     version, settings = version_settings
 
     patch_for_version(version, collection_strategy, embeddings_strategy)
 
@@ -242,14 +253,15 @@
         e = conn1.recv()
         raise e
 
     # Switch to the current version (local working directory) and check the invariants
     # are preserved for the collection
     api = Client(settings)
     coll = api.get_collection(
-        name=collection_strategy.name, embedding_function=lambda x: None
+        name=collection_strategy.name,
+        embedding_function=not_implemented_ef(),
     )
     invariants.count(coll, embeddings_strategy)
     invariants.metadatas_match(coll, embeddings_strategy)
     invariants.documents_match(coll, embeddings_strategy)
     invariants.ids_match(coll, embeddings_strategy)
     invariants.ann_accuracy(coll, embeddings_strategy)
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/property/test_embeddings.py` & `chromadb-client-0.3.27.dev0/chromadb/test/property/test_embeddings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 import pytest
 import logging
 import hypothesis.strategies as st
-from typing import Set
+from typing import Set, cast, Union, DefaultDict
 from dataclasses import dataclass
-from chromadb.api.types import Include
+from chromadb.api.types import ID, Include, IDs
 import chromadb.errors as errors
 from chromadb.api import API
 from chromadb.api.models.Collection import Collection
 import chromadb.test.property.strategies as strategies
 from hypothesis.stateful import (
     Bundle,
     RuleBasedStateMachine,
+    MultipleResults,
     rule,
     initialize,
     precondition,
     consumes,
     run_state_machine_as_test,
     multiple,
     invariant,
 )
 from collections import defaultdict
 import chromadb.test.property.invariants as invariants
 import numpy as np
 
 
-traces = defaultdict(lambda: 0)
+traces: DefaultDict[str, int] = defaultdict(lambda: 0)
 
 
-def trace(key):
+def trace(key: str) -> None:
     global traces
     traces[key] += 1
 
 
-def print_traces():
+def print_traces() -> None:
     global traces
     for key, value in traces.items():
         print(f"{key}: {value}")
 
 
-dtype_shared_st = st.shared(st.sampled_from(strategies.float_types), key="dtype")
-dimension_shared_st = st.shared(
+dtype_shared_st: st.SearchStrategy[
+    Union[np.float16, np.float32, np.float64]
+] = st.shared(st.sampled_from(strategies.float_types), key="dtype")
+
+dimension_shared_st: st.SearchStrategy[int] = st.shared(
     st.integers(min_value=2, max_value=2048), key="dimension"
 )
 
 
 @dataclass
 class EmbeddingStateMachineStates:
     initialize = "initialize"
@@ -54,177 +58,201 @@
 
 
 collection_st = st.shared(strategies.collections(with_hnsw_params=True), key="coll")
 
 
 class EmbeddingStateMachine(RuleBasedStateMachine):
     collection: Collection
-    embedding_ids: Bundle = Bundle("embedding_ids")
+    embedding_ids: Bundle[ID] = Bundle("embedding_ids")
 
     def __init__(self, api: API):
         super().__init__()
         self.api = api
-        self._rules_strategy = strategies.DeterministicRuleStrategy(self)
+        self._rules_strategy = strategies.DeterministicRuleStrategy(self)  # type: ignore
 
-    @initialize(collection=collection_st)
+    @initialize(collection=collection_st)  # type: ignore
     def initialize(self, collection: strategies.Collection):
         self.api.reset()
         self.collection = self.api.create_collection(
             name=collection.name,
             metadata=collection.metadata,
             embedding_function=collection.embedding_function,
         )
         self.embedding_function = collection.embedding_function
         trace("init")
         self.on_state_change(EmbeddingStateMachineStates.initialize)
-        self.embeddings = {
-            "ids": [],
-            "embeddings": [],
-            "metadatas": [],
-            "documents": [],
-        }
 
-    @rule(target=embedding_ids, embedding_set=strategies.recordsets(collection_st))
-    def add_embeddings(self, embedding_set):
+        self.record_set_state = strategies.StateMachineRecordSet(
+            ids=[], metadatas=[], documents=[], embeddings=[]
+        )
+
+    @rule(target=embedding_ids, record_set=strategies.recordsets(collection_st))
+    def add_embeddings(self, record_set: strategies.RecordSet) -> MultipleResults[ID]:
         trace("add_embeddings")
         self.on_state_change(EmbeddingStateMachineStates.add_embeddings)
 
-        normalized_embedding_set = invariants.wrap_all(embedding_set)
+        normalized_record_set: strategies.NormalizedRecordSet = invariants.wrap_all(
+            record_set
+        )
 
-        if len(normalized_embedding_set["ids"]) > 0:
+        if len(normalized_record_set["ids"]) > 0:
             trace("add_more_embeddings")
 
-        if set(normalized_embedding_set["ids"]).intersection(
-            set(self.embeddings["ids"])
+        if set(normalized_record_set["ids"]).intersection(
+            set(self.record_set_state["ids"])
         ):
             with pytest.raises(errors.IDAlreadyExistsError):
-                self.collection.add(**embedding_set)
+                self.collection.add(**normalized_record_set)
             return multiple()
         else:
-            self.collection.add(**embedding_set)
-            self._upsert_embeddings(embedding_set)
-            return multiple(*normalized_embedding_set["ids"])
+            self.collection.add(**normalized_record_set)
+            self._upsert_embeddings(cast(strategies.RecordSet, normalized_record_set))
+            return multiple(*normalized_record_set["ids"])
 
-    @precondition(lambda self: len(self.embeddings["ids"]) > 20)
+    @precondition(lambda self: len(self.record_set_state["ids"]) > 20)
     @rule(ids=st.lists(consumes(embedding_ids), min_size=1, max_size=20))
-    def delete_by_ids(self, ids):
+    def delete_by_ids(self, ids: IDs) -> None:
         trace("remove embeddings")
         self.on_state_change(EmbeddingStateMachineStates.delete_by_ids)
-        indices_to_remove = [self.embeddings["ids"].index(id) for id in ids]
+        indices_to_remove = [self.record_set_state["ids"].index(id) for id in ids]
 
         self.collection.delete(ids=ids)
         self._remove_embeddings(set(indices_to_remove))
 
     # Removing the precondition causes the tests to frequently fail as "unsatisfiable"
     # Using a value < 5 causes retries and lowers the number of valid samples
-    @precondition(lambda self: len(self.embeddings["ids"]) >= 5)
+    @precondition(lambda self: len(self.record_set_state["ids"]) >= 5)
     @rule(
-        embedding_set=strategies.recordsets(
+        record_set=strategies.recordsets(
             collection_strategy=collection_st,
             id_strategy=embedding_ids,
             min_size=1,
             max_size=5,
         )
     )
-    def update_embeddings(self, embedding_set):
+    def update_embeddings(self, record_set: strategies.RecordSet) -> None:
         trace("update embeddings")
         self.on_state_change(EmbeddingStateMachineStates.update_embeddings)
-        self.collection.update(**embedding_set)
-        self._upsert_embeddings(embedding_set)
+        self.collection.update(**record_set)
+        self._upsert_embeddings(record_set)
 
     # Using a value < 3 causes more retries and lowers the number of valid samples
-    @precondition(lambda self: len(self.embeddings["ids"]) >= 3)
+    @precondition(lambda self: len(self.record_set_state["ids"]) >= 3)
     @rule(
-        embedding_set=strategies.recordsets(
+        record_set=strategies.recordsets(
             collection_strategy=collection_st,
             id_strategy=st.one_of(embedding_ids, strategies.safe_text),
             min_size=1,
             max_size=5,
         )
     )
-    def upsert_embeddings(self, embedding_set):
+    def upsert_embeddings(self, record_set: strategies.RecordSet) -> None:
         trace("upsert embeddings")
         self.on_state_change(EmbeddingStateMachineStates.upsert_embeddings)
-        self.collection.upsert(**embedding_set)
-        self._upsert_embeddings(embedding_set)
+        self.collection.upsert(**record_set)
+        self._upsert_embeddings(record_set)
 
     @invariant()
-    def count(self):
-        invariants.count(self.collection, self.embeddings)  # type: ignore
+    def count(self) -> None:
+        invariants.count(
+            self.collection, cast(strategies.RecordSet, self.record_set_state)
+        )
 
     @invariant()
-    def no_duplicates(self):
+    def no_duplicates(self) -> None:
         invariants.no_duplicates(self.collection)
 
     @invariant()
-    def ann_accuracy(self):
+    def ann_accuracy(self) -> None:
         invariants.ann_accuracy(
-            collection=self.collection, record_set=self.embeddings, min_recall=0.95, embedding_function=self.embedding_function  # type: ignore
+            collection=self.collection,
+            record_set=cast(strategies.RecordSet, self.record_set_state),
+            min_recall=0.95,
+            embedding_function=self.embedding_function,
         )
 
-    def _upsert_embeddings(self, embeddings: strategies.RecordSet):
-        embeddings = invariants.wrap_all(embeddings)
-        for idx, id in enumerate(embeddings["ids"]):
-            if id in self.embeddings["ids"]:
-                target_idx = self.embeddings["ids"].index(id)
-                if "embeddings" in embeddings and embeddings["embeddings"] is not None:
-                    self.embeddings["embeddings"][target_idx] = embeddings[
-                        "embeddings"
-                    ][idx]
+    def _upsert_embeddings(self, record_set: strategies.RecordSet) -> None:
+        normalized_record_set: strategies.NormalizedRecordSet = invariants.wrap_all(
+            record_set
+        )
+        for idx, id in enumerate(normalized_record_set["ids"]):
+            # Update path
+            if id in self.record_set_state["ids"]:
+                target_idx = self.record_set_state["ids"].index(id)
+                if normalized_record_set["embeddings"] is not None:
+                    self.record_set_state["embeddings"][
+                        target_idx
+                    ] = normalized_record_set["embeddings"][idx]
                 else:
-                    self.embeddings["embeddings"][target_idx] = self.embedding_function(
-                        [embeddings["documents"][idx]]
-                    )[0]
-                if "metadatas" in embeddings and embeddings["metadatas"] is not None:
-                    self.embeddings["metadatas"][target_idx] = embeddings["metadatas"][
-                        idx
-                    ]
-                if "documents" in embeddings and embeddings["documents"] is not None:
-                    self.embeddings["documents"][target_idx] = embeddings["documents"][
-                        idx
+                    assert normalized_record_set["documents"] is not None
+                    assert self.embedding_function is not None
+                    self.record_set_state["embeddings"][
+                        target_idx
+                    ] = self.embedding_function(
+                        [normalized_record_set["documents"][idx]]
+                    )[
+                        0
                     ]
+                if normalized_record_set["metadatas"] is not None:
+                    self.record_set_state["metadatas"][
+                        target_idx
+                    ] = normalized_record_set["metadatas"][idx]
+                if normalized_record_set["documents"] is not None:
+                    self.record_set_state["documents"][
+                        target_idx
+                    ] = normalized_record_set["documents"][idx]
             else:
                 # Add path
-                self.embeddings["ids"].append(id)
-                if "embeddings" in embeddings and embeddings["embeddings"] is not None:
-                    self.embeddings["embeddings"].append(embeddings["embeddings"][idx])
+                self.record_set_state["ids"].append(id)
+                if normalized_record_set["embeddings"] is not None:
+                    self.record_set_state["embeddings"].append(
+                        normalized_record_set["embeddings"][idx]
+                    )
                 else:
-                    self.embeddings["embeddings"].append(
-                        self.embedding_function([embeddings["documents"][idx]])[0]
+                    assert self.embedding_function is not None
+                    assert normalized_record_set["documents"] is not None
+                    self.record_set_state["embeddings"].append(
+                        self.embedding_function(
+                            [normalized_record_set["documents"][idx]]
+                        )[0]
+                    )
+                if normalized_record_set["metadatas"] is not None:
+                    self.record_set_state["metadatas"].append(
+                        normalized_record_set["metadatas"][idx]
                     )
-                if "metadatas" in embeddings and embeddings["metadatas"] is not None:
-                    self.embeddings["metadatas"].append(embeddings["metadatas"][idx])
                 else:
-                    self.embeddings["metadatas"].append(None)
-                if "documents" in embeddings and embeddings["documents"] is not None:
-                    self.embeddings["documents"].append(embeddings["documents"][idx])
+                    self.record_set_state["metadatas"].append(None)
+                if normalized_record_set["documents"] is not None:
+                    self.record_set_state["documents"].append(
+                        normalized_record_set["documents"][idx]
+                    )
                 else:
-                    self.embeddings["documents"].append(None)
+                    self.record_set_state["documents"].append(None)
 
-    def _remove_embeddings(self, indices_to_remove: Set[int]):
+    def _remove_embeddings(self, indices_to_remove: Set[int]) -> None:
         indices_list = list(indices_to_remove)
         indices_list.sort(reverse=True)
 
         for i in indices_list:
-            del self.embeddings["ids"][i]
-            del self.embeddings["embeddings"][i]
-            del self.embeddings["metadatas"][i]
-            del self.embeddings["documents"][i]
+            del self.record_set_state["ids"][i]
+            del self.record_set_state["embeddings"][i]
+            del self.record_set_state["metadatas"][i]
+            del self.record_set_state["documents"][i]
 
-    def on_state_change(self, new_state):
+    def on_state_change(self, new_state: str) -> None:
         pass
 
 
-def test_embeddings_state(caplog, api):
+def test_embeddings_state(caplog: pytest.LogCaptureFixture, api: API) -> None:
     caplog.set_level(logging.ERROR)
-    run_state_machine_as_test(lambda: EmbeddingStateMachine(api))
+    run_state_machine_as_test(lambda: EmbeddingStateMachine(api))  # type: ignore
     print_traces()
 
 
-def test_multi_add(api: API):
+def test_multi_add(api: API) -> None:
     api.reset()
     coll = api.create_collection(name="foo")
     coll.add(ids=["a"], embeddings=[[0.0]])
     assert coll.count() == 1
 
     with pytest.raises(errors.IDAlreadyExistsError):
         coll.add(ids=["a"], embeddings=[[0.0]])
@@ -234,39 +262,41 @@
     results = coll.get()
     assert results["ids"] == ["a"]
 
     coll.delete(ids=["a"])
     assert coll.count() == 0
 
 
-def test_dup_add(api: API):
+def test_dup_add(api: API) -> None:
     api.reset()
     coll = api.create_collection(name="foo")
     with pytest.raises(errors.DuplicateIDError):
         coll.add(ids=["a", "a"], embeddings=[[0.0], [1.1]])
     with pytest.raises(errors.DuplicateIDError):
         coll.upsert(ids=["a", "a"], embeddings=[[0.0], [1.1]])
 
 
-def test_query_without_add(api: API):
+def test_query_without_add(api: API) -> None:
     api.reset()
     coll = api.create_collection(name="foo")
     fields: Include = ["documents", "metadatas", "embeddings", "distances"]
     N = np.random.randint(1, 2000)
     K = np.random.randint(1, 100)
     results = coll.query(
         query_embeddings=np.random.random((N, K)).tolist(), include=fields
     )
     for field in fields:
-        all([len(result) == 0 for result in results[field]])
+        field_results = results[field]
+        assert field_results is not None
+        assert all([len(result) == 0 for result in field_results])
 
 
 # TODO: Use SQL escaping correctly internally
 @pytest.mark.xfail(reason="We don't properly escape SQL internally, causing problems")
-def test_escape_chars_in_ids(api: API):
+def test_escape_chars_in_ids(api: API) -> None:
     api.reset()
     id = "\x1f"
     coll = api.create_collection(name="foo")
     coll.add(ids=[id], embeddings=[[0.0]])
     assert coll.count() == 1
     coll.delete(ids=[id])
     assert coll.count() == 0
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/property/test_persist.py` & `chromadb-client-0.3.27.dev0/chromadb/test/property/test_persist.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import multiprocessing
+from multiprocessing.connection import Connection
 from typing import Generator, Callable
 from hypothesis import given
 import hypothesis.strategies as st
 import pytest
 import chromadb
 from chromadb.api import API
 from chromadb.config import Settings
@@ -26,15 +27,15 @@
         chroma_db_impl="duckdb+parquet",
         persist_directory=tempfile.gettempdir() + "/tests",
     )
 ]
 
 
 @pytest.fixture(scope="module", params=configurations)
-def settings(request) -> Generator[Settings, None, None]:
+def settings(request: pytest.FixtureRequest) -> Generator[Settings, None, None]:
     configuration = request.param
     yield configuration
     save_path = configuration.persist_directory
     # Remove if it exists
     if os.path.exists(save_path):
         shutil.rmtree(save_path)
 
@@ -46,15 +47,15 @@
     collection_strategy=collection_st,
     embeddings_strategy=strategies.recordsets(collection_st),
 )
 def test_persist(
     settings: Settings,
     collection_strategy: strategies.Collection,
     embeddings_strategy: strategies.RecordSet,
-):
+) -> None:
     api_1 = chromadb.Client(settings)
     api_1.reset()
     coll = api_1.create_collection(
         name=collection_strategy.name,
         metadata=collection_strategy.metadata,
         embedding_function=collection_strategy.embedding_function,
     )
@@ -86,25 +87,31 @@
     invariants.ann_accuracy(
         coll,
         embeddings_strategy,
         embedding_function=collection_strategy.embedding_function,
     )
 
 
-def load_and_check(settings: Settings, collection_name: str, embeddings_set, conn):
+def load_and_check(
+    settings: Settings,
+    collection_name: str,
+    record_set: strategies.RecordSet,
+    conn: Connection,
+) -> None:
     try:
         api = chromadb.Client(settings)
         coll = api.get_collection(
-            name=collection_name, embedding_function=lambda x: None
+            name=collection_name,
+            embedding_function=strategies.not_implemented_embedding_function(),
         )
-        invariants.count(coll, embeddings_set)
-        invariants.metadatas_match(coll, embeddings_set)
-        invariants.documents_match(coll, embeddings_set)
-        invariants.ids_match(coll, embeddings_set)
-        invariants.ann_accuracy(coll, embeddings_set)
+        invariants.count(coll, record_set)
+        invariants.metadatas_match(coll, record_set)
+        invariants.documents_match(coll, record_set)
+        invariants.ids_match(coll, record_set)
+        invariants.ann_accuracy(coll, record_set)
     except Exception as e:
         conn.send(e)
         raise e
 
 
 class PersistEmbeddingsStateMachineStates(EmbeddingStateMachineStates):
     persist = "persist"
@@ -114,42 +121,46 @@
     def __init__(self, api: API, settings: Settings):
         self.api = api
         self.settings = settings
         self.last_persist_delay = 10
         self.api.reset()
         super().__init__(self.api)
 
-    @precondition(lambda self: len(self.embeddings["ids"]) >= 1)
-    @precondition(lambda self: self.last_persist_delay <= 0)
+    @precondition(
+        lambda self: len(self.record_set_state["ids"]) >= 1
+        and self.last_persist_delay <= 0
+    )
     @rule()
-    def persist(self):
+    def persist(self) -> None:
         self.on_state_change(PersistEmbeddingsStateMachineStates.persist)
         self.api.persist()
         collection_name = self.collection.name
         # Create a new process and then inside the process run the invariants
         # TODO: Once we switch off of duckdb and onto sqlite we can remove this
         ctx = multiprocessing.get_context("spawn")
         conn1, conn2 = multiprocessing.Pipe()
         p = ctx.Process(
             target=load_and_check,
-            args=(self.settings, collection_name, self.embeddings, conn2),
+            args=(self.settings, collection_name, self.record_set_state, conn2),
         )
         p.start()
         p.join()
 
         if conn1.poll():
             e = conn1.recv()
             raise e
 
-    def on_state_change(self, new_state):
+    def on_state_change(self, new_state: str) -> None:
         if new_state == PersistEmbeddingsStateMachineStates.persist:
             self.last_persist_delay = 10
         else:
             self.last_persist_delay -= 1
 
 
-def test_persist_embeddings_state(caplog, settings: Settings):
+def test_persist_embeddings_state(
+    caplog: pytest.LogCaptureFixture, settings: Settings
+) -> None:
     caplog.set_level(logging.ERROR)
     api = chromadb.Client(settings)
     run_state_machine_as_test(
         lambda: PersistEmbeddingsStateMachine(settings=settings, api=api)
-    )
+    )  # type: ignore
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/test_api.py` & `chromadb-client-0.3.27.dev0/chromadb/test/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 def test_reset_db(api):
     api.reset()
 
     collection = api.create_collection("testspace")
     collection.add(**batch_records)
     assert collection.count() == 2
 
-    assert api.reset()
+    api.reset()
     assert len(api.list_collections()) == 0
 
 
 def test_get_nearest_neighbors(api):
     api.reset()
     collection = api.create_collection("testspace")
     collection.add(**batch_records)
@@ -856,32 +856,31 @@
             ]
         }
     )
     assert len(items["metadatas"]) == 2
 
     items = collection.get(
         where={
-            "$or": [
+            "$and": [
                 {
-                    "$and": [
-                        {"int_value": {"$eq": 3}},
-                        {"string_value": {"$eq": "three"}},
+                    "$or": [
+                        {"int_value": {"$eq": 1}},
+                        {"string_value": {"$eq": "two"}},
                     ]
                 },
                 {
-                    "$and": [
-                        {"int_value": {"$eq": 4}},
-                        {"string_value": {"$eq": "four"}},
+                    "$or": [
+                        {"int_value": {"$eq": 2}},
+                        {"string_value": {"$eq": "one"}},
                     ]
                 },
-            ],
-            "$and": [{"is": "doc"}, {"string_value": "four"}],
+            ]
         }
     )
-    assert len(items["metadatas"]) == 1
+    assert len(items["metadatas"]) == 2
 
 
 def test_where_document_logical_operators(api):
     api.reset()
     collection = api.create_collection("test_document_logical_operators")
     collection.add(**logical_operator_records)
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/test/test_chroma.py` & `chromadb-client-0.3.27.dev0/chromadb/test/test_chroma.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import unittest
 import os
 from unittest.mock import patch, Mock
 
 import chromadb
 import chromadb.config
+from chromadb.db import DB
 
 
 class GetDBTest(unittest.TestCase):
     @patch("chromadb.db.duckdb.DuckDB", autospec=True)
     def test_default_db(self, mock: Mock) -> None:
         system = chromadb.config.System(
             chromadb.config.Settings(persist_directory="./foo")
         )
-        system.get_db()
+        system.instance(DB)
         assert mock.called
 
     @patch("chromadb.db.duckdb.PersistentDuckDB", autospec=True)
     def test_persistent_duckdb(self, mock: Mock) -> None:
         system = chromadb.config.System(
             chromadb.config.Settings(
                 chroma_db_impl="duckdb+parquet", persist_directory="./foo"
             )
         )
-        system.get_db()
+        system.instance(DB)
         assert mock.called
 
     @patch("chromadb.db.clickhouse.Clickhouse", autospec=True)
     def test_clickhouse(self, mock: Mock) -> None:
         system = chromadb.config.System(
             chromadb.config.Settings(
                 chroma_db_impl="clickhouse",
                 persist_directory="./foo",
                 clickhouse_host="foo",
                 clickhouse_port="666",
             )
         )
-        system.get_db()
+        system.instance(DB)
         assert mock.called
 
 
 class GetAPITest(unittest.TestCase):
     @patch("chromadb.api.local.LocalAPI", autospec=True)
     @patch.dict(os.environ, {}, clear=True)
     def test_local(self, mock_api: Mock) -> None:
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb/utils/embedding_functions.py` & `chromadb-client-0.3.27.dev0/chromadb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/chromadb_client.egg-info/PKG-INFO` & `chromadb-client-0.3.27.dev0/chromadb_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb-client
-Version: 0.3.26.dev9
+Version: 0.3.27.dev0
 Summary: Chroma Client.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,17 @@
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest", chroma_server_host="localhost", chroma_server_port=8000))
+client = chromadb.Client(Settings(chroma_api_impl="rest",
+                                  chroma_server_host="localhost",
+                                  chroma_server_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.26.dev9 Summary:
+Metadata-Version: 2.1 Name: chromadb-client Version: 0.3.27.dev0 Summary:
 Chroma Client. Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-client-0.3.26.dev9/chromadb_client.egg-info/SOURCES.txt` & `chromadb-client-0.3.27.dev0/chromadb_client.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 pull_request_template.md
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/feature_request.yaml
 .github/ISSUE_TEMPLATE/installation_trouble.yaml
+.github/workflows/chroma-client-integration-test.yml
 .github/workflows/chroma-integration-test.yml
 .github/workflows/chroma-release-python-client.yml
 .github/workflows/chroma-release.yml
 .github/workflows/chroma-test.yml
 .github/workflows/pr-review-checklist.yml
 .vscode/settings.json
 bin/backup.sh
@@ -37,56 +38,72 @@
 bin/version
 bin/templates/docker-compose.yml
 chromadb/__init__.py
 chromadb/app.py
 chromadb/config.py
 chromadb/errors.py
 chromadb/is_thin_client.py
+chromadb/types.py
 chromadb/api/__init__.py
 chromadb/api/fastapi.py
 chromadb/api/local.py
 chromadb/api/types.py
 chromadb/api/models/Collection.py
 chromadb/db/__init__.py
 chromadb/db/base.py
 chromadb/db/clickhouse.py
 chromadb/db/duckdb.py
 chromadb/db/migrations.py
+chromadb/db/system.py
 chromadb/db/impl/__init__.py
 chromadb/db/impl/sqlite.py
 chromadb/db/index/__init__.py
 chromadb/db/index/hnswlib.py
+chromadb/db/mixins/embeddings_queue.py
+chromadb/db/mixins/sysdb.py
+chromadb/ingest/__init__.py
+chromadb/segment/__init__.py
+chromadb/segment/impl/manager/local.py
+chromadb/segment/impl/metadata/sqlite.py
+chromadb/segment/impl/vector/local_hnsw.py
 chromadb/server/__init__.py
 chromadb/server/fastapi/__init__.py
 chromadb/server/fastapi/types.py
 chromadb/telemetry/__init__.py
 chromadb/telemetry/events.py
 chromadb/telemetry/posthog.py
 chromadb/test/conftest.py
 chromadb/test/test_api.py
 chromadb/test/test_chroma.py
+chromadb/test/test_config.py
 chromadb/test/db/test_base.py
 chromadb/test/db/test_migrations.py
+chromadb/test/db/test_system.py
 chromadb/test/db/migrations/00001-migration-1.psql.sql
 chromadb/test/db/migrations/00001-migration-1.sqlite.sql
 chromadb/test/db/migrations/00002-migration-2.psql.sql
 chromadb/test/db/migrations/00002-migration-2.sqlite.sql
 chromadb/test/db/migrations/00003-migration-3.psql.sql
 chromadb/test/db/migrations/00003-migration-3.sqlite.sql
 chromadb/test/hnswlib/test_hnswlib.py
+chromadb/test/ingest/test_producer_consumer.py
 chromadb/test/property/invariants.py
 chromadb/test/property/strategies.py
 chromadb/test/property/test_add.py
 chromadb/test/property/test_collections.py
 chromadb/test/property/test_cross_version_persist.py
 chromadb/test/property/test_embeddings.py
 chromadb/test/property/test_filtering.py
 chromadb/test/property/test_persist.py
+chromadb/test/segment/test_metadata.py
+chromadb/test/segment/test_vector.py
+chromadb/test/utils/test_messagid.py
 chromadb/utils/__init__.py
 chromadb/utils/embedding_functions.py
+chromadb/utils/messageid.py
 chromadb_client.egg-info/PKG-INFO
 chromadb_client.egg-info/SOURCES.txt
 chromadb_client.egg-info/dependency_links.txt
 chromadb_client.egg-info/requires.txt
 chromadb_client.egg-info/top_level.txt
 clients/js/.gitignore
 clients/js/.prettierignore
@@ -117,14 +134,15 @@
 clients/js/src/Collection.ts
 clients/js/src/index.ts
 clients/js/src/types.ts
 clients/js/src/utils.ts
 clients/js/src/embeddings/CohereEmbeddingFunction.ts
 clients/js/src/embeddings/IEmbeddingFunction.ts
 clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+clients/js/src/embeddings/WebAIEmbeddingFunction.ts
 clients/js/src/generated/README.md
 clients/js/src/generated/api.ts
 clients/js/src/generated/configuration.ts
 clients/js/src/generated/index.ts
 clients/js/src/generated/models.ts
 clients/js/src/generated/runtime.ts
 clients/js/test/add.collections.test.ts
@@ -137,19 +155,24 @@
 clients/js/test/initClient.ts
 clients/js/test/peek.collection.test.ts
 clients/js/test/query.collection.test.ts
 clients/js/test/update.collection.test.ts
 clients/js/test/upsert.collections.test.ts
 clients/python/README.md
 clients/python/build_python_thin_client.sh
+clients/python/integration-test.sh
 clients/python/is_thin_client.py
 clients/python/pyproject.toml
 config/backup_disk.xml
 config/chroma_users.xml
 examples/alternative_embeddings.ipynb
 examples/local_persistence.ipynb
 examples/where_filtering.ipynb
 examples/deployments/google-cloud-compute/README.md
 examples/deployments/google-cloud-compute/chroma.tf
 examples/deployments/google-cloud-compute/main.tf
 examples/deployments/google-cloud-compute/startup.sh
-examples/deployments/google-cloud-compute/variables.tf
+examples/deployments/google-cloud-compute/variables.tf
+migrations/embeddings_queue/00001-embeddings.sqlite.sql
+migrations/metadb/00001-embedding-metadata.sqlite.sql
+migrations/sysdb/00001-collections.sqlite.sql
+migrations/sysdb/00002-segments.sqlite.sql
```

### Comparing `chromadb-client-0.3.26.dev9/clients/js/DEVELOP.md` & `chromadb-client-0.3.27.dev0/clients/js/DEVELOP.md`

 * *Files 23% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 `yarn test` will launch a test docker backend.
 `yarn test:run` will run against the docker backend you have running. But CAUTION, it will delete data.
 
 ### Pushing to npm
 
 The goal of the design is that this will be added to our github action releases so that the JS API is always up to date and pinned against the python backend API.
 
-`npm publish` pushes the `package.json` defined packaged to the package manager for authenticated users.
+`yarn release` pushes the `package.json` defined packaged to the package manager for authenticated users. It will build, test, and then publish the new version.
 
 ### Useful links
 
 https://gaganpreet.in/posts/hyperproductive-apis-fastapi/
```

### Comparing `chromadb-client-0.3.26.dev9/clients/js/LICENSE` & `chromadb-client-0.3.27.dev0/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/README.md` & `chromadb-client-0.3.27.dev0/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/examples/browser/app.ts` & `chromadb-client-0.3.27.dev0/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/examples/browser/index.html` & `chromadb-client-0.3.27.dev0/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/examples/browser/yarn.lock` & `chromadb-client-0.3.27.dev0/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/examples/node/app.js` & `chromadb-client-0.3.27.dev0/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/examples/node/package-lock.json` & `chromadb-client-0.3.27.dev0/clients/js/examples/node/package-lock.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/examples/node/yarn.lock` & `chromadb-client-0.3.27.dev0/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/genapi.sh` & `chromadb-client-0.3.27.dev0/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/package-lock.json` & `chromadb-client-0.3.27.dev0/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/package.json` & `chromadb-client-0.3.27.dev0/clients/js/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9512987012987012%*

 * *Differences: {"'scripts'": "{'release': 'run-s build test:run && npm publish'}", "'version'": "'1.5.2'"}*

```diff
@@ -28,15 +28,16 @@
         "build:main": "tsc -p tsconfig.json",
         "build:module": "tsc -p tsconfig.module.json",
         "clean": "rimraf dist",
         "db:clean": "cd ../.. && CHROMA_PORT=8001 docker-compose -f docker-compose.test.yml down --volumes",
         "db:run": "cd ../.. && CHROMA_PORT=8001 docker-compose -f docker-compose.test.yml up --detach && sleep 5",
         "genapi": "./genapi.sh",
         "prettier": "prettier --write .",
+        "release": "run-s build test:run && npm publish",
         "test": "run-s db:clean db:run test:runfull db:clean",
         "test:run": "jest --runInBand",
         "test:runfull": "PORT=8001 jest --runInBand",
         "test:set-port": "cross-env URL=localhost:8001",
         "test:update": "run-s db:clean db:run && jest --runInBand --updateSnapshot && run-s db:clean"
     },
-    "version": "1.5.0"
+    "version": "1.5.2"
 }
```

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/ChromaClient.ts` & `chromadb-client-0.3.27.dev0/clients/js/src/ChromaClient.ts`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,18 @@
         embeddingFunction?: IEmbeddingFunction
     }): Promise<Collection> {
         const response = await this.api
             .getCollection(name)
             .then(handleSuccess)
             .catch(handleError);
 
+        if (response.error) {
+            throw new Error(response.error);
+        }
+
         return new Collection(
             response.name,
             response.id,
             this.api,
             response.metadata,
             embeddingFunction
         );
@@ -253,8 +257,8 @@
     }): Promise<void> {
         return await this.api
             .deleteCollection(name)
             .then(handleSuccess)
             .catch(handleError);
     }
 
-}
+}
```

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/Collection.ts` & `chromadb-client-0.3.27.dev0/clients/js/src/Collection.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `chromadb-client-0.3.27.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `chromadb-client-0.3.27.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/generated/README.md` & `chromadb-client-0.3.27.dev0/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/generated/api.ts` & `chromadb-client-0.3.27.dev0/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/generated/configuration.ts` & `chromadb-client-0.3.27.dev0/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/generated/models.ts` & `chromadb-client-0.3.27.dev0/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/generated/runtime.ts` & `chromadb-client-0.3.27.dev0/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/types.ts` & `chromadb-client-0.3.27.dev0/clients/js/src/types.ts`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,18 @@
   documents: (null | Document)[];
   metadatas: (null | Metadata)[];
   error: null | string;
 };
 
 export type QueryResponse = {
   ids: IDs[];
-  embeddings: null | Embeddings[][];
+  embeddings: null | Embeddings[];
   documents: (null | Document)[][];
   metadatas: (null | Metadata)[][];
-  distances: null | number[][][];
+  distances: null | number[][];
 }
 
 export type AddResponse = {
   error: string;
 }
 
 export type CollectionMetadata = Record<string, unknown>;
```

### Comparing `chromadb-client-0.3.26.dev9/clients/js/src/utils.ts` & `chromadb-client-0.3.27.dev0/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/test/add.collections.test.ts` & `chromadb-client-0.3.27.dev0/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/test/client.test.ts` & `chromadb-client-0.3.27.dev0/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/test/collection.client.test.ts` & `chromadb-client-0.3.27.dev0/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/test/collection.test.ts` & `chromadb-client-0.3.27.dev0/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/test/delete.collection.test.ts` & `chromadb-client-0.3.27.dev0/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/test/get.collection.test.ts` & `chromadb-client-0.3.27.dev0/clients/js/test/get.collection.test.ts`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,16 @@
   const results2 = await collection.get({ where: { test: "test1" } });
   expect(results2).toBeDefined();
   expect(results2).toBeInstanceOf(Object);
   expect(results2.ids.length).toBe(1);
   expect(["test1"]).toEqual(expect.arrayContaining(results2.ids));
 });
 
+
+
 test("wrong code returns an error", async () => {
   await chroma.reset();
   const collection = await chroma.createCollection({ name: "test" });
   await collection.add({ ids: IDS, embeddings: EMBEDDINGS, metadatas: METADATAS });
   const results = await collection.get({
     where: {
       //@ts-ignore supposed to fail
@@ -49,7 +51,16 @@
   await chroma.reset();
   const collection = await chroma.createCollection({ name: "test" });
   await collection.add({ ids: IDS, embeddings: EMBEDDINGS, metadatas: METADATAS });
   const items = await collection.get({ where: { float_value: { $gt: -1.4 } } });
   expect(items.ids.length).toBe(2);
   expect(["test2", "test3"]).toEqual(expect.arrayContaining(items.ids));
 });
+
+
+test("it should throw an error if the collection does not exist", async () => {
+  await chroma.reset();
+
+  await expect(
+    async () => await chroma.getCollection({ name: "test" })
+  ).rejects.toThrow(Error);
+});
```

### Comparing `chromadb-client-0.3.26.dev9/clients/js/test/peek.collection.test.ts` & `chromadb-client-0.3.27.dev0/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/test/query.collection.test.ts` & `chromadb-client-0.3.27.dev0/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/test/update.collection.test.ts` & `chromadb-client-0.3.27.dev0/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/test/upsert.collections.test.ts` & `chromadb-client-0.3.27.dev0/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/js/yarn.lock` & `chromadb-client-0.3.27.dev0/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/clients/python/README.md` & `chromadb-client-0.3.27.dev0/clients/python/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 To connect to your server and perform operations using the client only library, you can do the following:
 
 ```python
 import chromadb
 from chromadb.config import Settings
 # Example setup of the client to connect to your chroma server
-client = chromadb.Client(Settings(chroma_api_impl="rest", chroma_server_host="localhost", chroma_server_port=8000))
+client = chromadb.Client(Settings(chroma_api_impl="rest",
+                                  chroma_server_host="localhost",
+                                  chroma_server_port=8000))
 
 collection = client.create_collection("all-my-documents")
 
 collection.add(
     documents=["This is document1", "This is document2"],
     metadatas=[{"source": "notion"}, {"source": "google-docs"}], # filter on these!
     ids=["doc1", "doc2"], # unique for each doc
```

### Comparing `chromadb-client-0.3.26.dev9/clients/python/build_python_thin_client.sh` & `chromadb-client-0.3.27.dev0/clients/python/build_python_thin_client.sh`

 * *Files 8% similar despite different names*

```diff
@@ -16,27 +16,31 @@
 staged_toml="staged_pyproject.toml"
 mv "$existing_toml" "$staged_toml"
 
 # Stage the existing readme file
 staged_readme="staged_README.md"
 mv "$existing_readme" "$staged_readme"
 
+function cleanup {
+  # Teardown: Remove the new toml file and put the old one back
+  rm "$existing_toml"
+  mv "$staged_toml" "$existing_toml"
+
+  rm "$is_thin_client_target"
+
+  # Teardown: Remove the new readme file and put the old one back
+  rm "$existing_readme"
+  mv "$staged_readme" "$existing_readme"
+}
+
+trap cleanup EXIT
+
 # Copy the new toml file in place
 cp "$thin_client_toml" "$existing_toml"
 
 # Copy the thin client flag script in place
 cp "$is_thin_client_py" "$is_thin_client_target"
 
 # Copy the new readme file in place
 cp "$thin_client_readme" "$existing_readme"
 
 python -m build
-
-# Teardown: Remove the new toml file and put the old one back
-rm "$existing_toml"
-mv "$staged_toml" "$existing_toml"
-
-rm "$is_thin_client_target"
-
-# Teardown: Remove the new readme file and put the old one back
-rm "$existing_readme"
-mv "$staged_readme" "$existing_readme"
```

### Comparing `chromadb-client-0.3.26.dev9/clients/python/pyproject.toml` & `chromadb-client-0.3.27.dev0/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/docker-compose.server.example.yml` & `chromadb-client-0.3.27.dev0/docker-compose.server.example.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/docker-compose.test.yml` & `chromadb-client-0.3.27.dev0/docker-compose.test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   test_server:
     build:
       context: .
       dockerfile: Dockerfile
     volumes:
       - ./:/chroma
       - test_index_data:/index_data
-    command: uvicorn chromadb.app:app --reload --workers 1 --host 0.0.0.0 --port 8000 --log-config log_config.yml
+    command: uvicorn chromadb.app:app --workers 1 --host 0.0.0.0 --port 8000 --log-config log_config.yml
     environment:
       - CHROMA_DB_IMPL=clickhouse
       - CLICKHOUSE_HOST=test_clickhouse
       - CLICKHOUSE_PORT=8123
       - ANONYMIZED_TELEMETRY=False
     ports:
       - ${CHROMA_PORT}:8000
```

### Comparing `chromadb-client-0.3.26.dev9/docker-compose.yml` & `chromadb-client-0.3.27.dev0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/examples/alternative_embeddings.ipynb` & `chromadb-client-0.3.27.dev0/examples/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/README.md` & `chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/examples/deployments/google-cloud-compute/startup.sh` & `chromadb-client-0.3.27.dev0/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/examples/local_persistence.ipynb` & `chromadb-client-0.3.27.dev0/examples/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/examples/where_filtering.ipynb` & `chromadb-client-0.3.27.dev0/examples/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.3.26.dev9/pyproject.toml` & `chromadb-client-0.3.27.dev0/pyproject.toml`

 * *Files identical despite different names*

