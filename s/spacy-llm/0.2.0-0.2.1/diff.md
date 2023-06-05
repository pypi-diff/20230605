# Comparing `tmp/spacy-llm-0.2.0.tar.gz` & `tmp/spacy-llm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.2.0.tar", last modified: Tue May 30 16:13:29 2023, max compression
+gzip compressed data, was "spacy-llm-0.2.1.tar", last modified: Mon Jun  5 14:11:25 2023, max compression
```

## Comparing `spacy-llm-0.2.0.tar` & `spacy-llm-0.2.1.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    51685 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    50441 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      644 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1819 2023-05-30 16:13:29.249338 spacy-llm-0.2.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (122)      187 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)      348 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/backends/integration/
--rw-r--r--   0 vsts      (1001) docker     (122)      328 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/integration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1233 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/integration/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3788 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/integration/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2791 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/integration/langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2574 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/integration/minichain.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/backends/rest/
--rw-r--r--   0 vsts      (1001) docker     (122)       63 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/backends/rest/backend/
--rw-r--r--   0 vsts      (1001) docker     (122)      239 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6223 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/backend/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/backend/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6601 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/backend/openai.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1721 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/backends/rest/registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7682 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6431 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1702 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)      534 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4299 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4264 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4156 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/spancat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/ner.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/ner.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/rel.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/spancat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/spancat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1203 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/textcat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/templates/textcat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     6917 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/textcat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tasks/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/util/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/util/parsing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4104 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tasks/util/span.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tests/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/backends/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/backends/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/backends/test_minichain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3307 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/backends/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (122)      110 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)      836 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4703 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.241338 spacy-llm-0.2.0/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/ner_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/ner_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/ner_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/rel_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/spacy_llm/tests/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/templates/ner_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/templates/textcat_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)    18403 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2685 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/test_rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13930 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/test_spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16984 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5507 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2001 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7852 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/ty.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1458 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/spacy_llm/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.237338 spacy-llm-0.2.0/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    51685 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3872 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      158 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-05-30 16:13:29.000000 spacy-llm-0.2.0/spacy_llm.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/multitask_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/multitask_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/multitask_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/ner_dolly/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_dolly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_dolly/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/ner_langchain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_langchain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_langchain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/ner_minichain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_minichain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/ner_minichain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/rel_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/rel_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/rel_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3483 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/tests/test_readme_examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/tests/test_usage_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-30 16:13:29.245338 spacy-llm-0.2.0/usage_examples/textcat_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/textcat_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-05-30 16:13:18.000000 spacy-llm-0.2.0/usage_examples/textcat_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    52005 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    50761 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      698 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1819 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.439660 spacy-llm-0.2.1/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      187 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.443660 spacy-llm-0.2.1/spacy_llm/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)      348 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.443660 spacy-llm-0.2.1/spacy_llm/backends/integration/
+-rw-r--r--   0 vsts      (1001) docker     (122)      328 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/integration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1233 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/integration/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3788 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/integration/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2791 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/integration/langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2574 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/integration/minichain.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.447660 spacy-llm-0.2.1/spacy_llm/backends/rest/
+-rw-r--r--   0 vsts      (1001) docker     (122)       63 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.447660 spacy-llm-0.2.1/spacy_llm/backends/rest/backend/
+-rw-r--r--   0 vsts      (1001) docker     (122)      239 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6223 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/backend/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/backend/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6601 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/backend/openai.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1721 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7765 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.447660 spacy-llm-0.2.1/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6937 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.447660 spacy-llm-0.2.1/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1702 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.451660 spacy-llm-0.2.1/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)      534 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4525 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4282 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4490 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/spancat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.455660 spacy-llm-0.2.1/spacy_llm/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/ner.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/ner.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/rel.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/spancat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/spancat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     8673 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/textcat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.455660 spacy-llm-0.2.1/spacy_llm/tasks/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/util/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/util/parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4104 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/util/span.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.455660 spacy-llm-0.2.1/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.459660 spacy-llm-0.2.1/spacy_llm/tests/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/backends/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/backends/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/backends/test_minichain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3307 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/backends/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      110 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      836 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.459660 spacy-llm-0.2.1/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4703 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.459660 spacy-llm-0.2.1/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/ner_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/ner_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/ner_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/rel_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/spacy_llm/tests/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/templates/ner_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/templates/textcat_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)    19490 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2690 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/test_rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15057 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20909 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5926 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2001 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7848 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1727 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.443660 spacy-llm-0.2.1/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    52005 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3915 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      158 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/usage_examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/usage_examples/multitask_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/multitask_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/multitask_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/usage_examples/ner_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/usage_examples/ner_langchain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_langchain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_langchain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/usage_examples/ner_minichain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_minichain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_minichain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/usage_examples/rel_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/rel_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/rel_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/usage_examples/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3508 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/tests/test_readme_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/tests/test_usage_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/usage_examples/textcat_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/textcat_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/textcat_openai/run_pipeline.py
```

### Comparing `spacy-llm-0.2.0/LICENSE` & `spacy-llm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/PKG-INFO` & `spacy-llm-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.2.0
+Version: 0.2.1
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -93,15 +93,15 @@
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
-labels = COMPLIMENT,INSULT
+labels = ["COMPLIMENT", "INSULT"]
 
 [components.llm.backend]
 @llm_backends = "spacy.REST.v1"
 api = "OpenAI"
 config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
 ```
 
@@ -131,15 +131,15 @@
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
-labels = PERSON,ORGANISATION,LOCATION
+labels = ["PERSON", "ORGANISATION", "LOCATION"]
 
 [components.llm.backend]
 @llm_backends = "spacy.DollyHF.v1"
 # For better performance, use databricks/dolly-v2-12b instead
 model = "databricks/dolly-v2-3b"
 ```
 
@@ -168,15 +168,15 @@
 
 nlp = spacy.blank("en")
 nlp.add_pipe(
     "llm",
     config={
         "task": {
             "@llm_tasks": "spacy.NER.v2",
-            "labels": "PERSON,ORGANISATION,LOCATION"
+            "labels": ["PERSON", "ORGANISATION", "LOCATION"]
         },
         "backend": {
             "@llm_backends": "spacy.REST.v1",
             "api": "OpenAI",
             "config": {"model": "gpt-3.5-turbo"},
         },
     },
@@ -197,14 +197,16 @@
 them into a list of prompts, and `parse_responses` that transforms the LLM outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity spans, text categories and more.
 
 To register your custom task with spaCy, decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator with a custom name that you can refer to in your config.
 
 > 📖 For more details, see the [**usage example on writing your own task**](usage_examples/README.md#writing-your-own-task)
 
 ```python
+from typing import Iterable, List
+from spacy.tokens import Doc
 from spacy_llm.registry import registry
 from spacy_llm.util import split_labels
 
 
 @registry.llm_tasks("my_namespace.MyTask.v1")
 def make_my_task(labels: str, my_other_config_val: float) -> "MyTask":
     labels_list = split_labels(labels)
@@ -248,14 +250,18 @@
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
 
+Moreover, the task may define an optional [`scorer` method](https://spacy.io/api/scorer#score).
+It should accept an iterable of `Example`s as input and return a score dictionary.
+If the `scorer` method is defined, `spacy-llm` will call it to evaluate the component.
+
 #### <kbd>function</kbd> `task.generate_prompts`
 
 Takes a collection of documents, and returns a collection of "prompts", which can be of type `Any`.
 Often, prompts are of type `str` - but this is not enforced to allow for maximum flexibility in the framework.
 
 | Argument    | Type            | Description            |
 | ----------- | --------------- | ---------------------- |
@@ -280,21 +286,21 @@
 #### spacy.NER.v2
 
 The built-in NER task supports both zero-shot and few-shot prompting. This version also supports explicitly defining the provided labels with custom descriptions.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
-labels = PERSON,ORGANISATION,LOCATION
+labels = ["PERSON", "ORGANISATION", "LOCATION"]
 examples = null
 ```
 
 | Argument                  | Type                                    | Default                                                  | Description                                                                                                                                           |
 | ------------------------- | --------------------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `labels`                  | `str`                                   |                                                          | Comma-separated list of labels.                                                                                                                       |
+| `labels`                  | `Union[List[str], str]`                 |                                                          | List of labels or str of comma-separated list of labels.                                                                                              |
 | `template`                | `str`                                   | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
 | `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                   | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                   | Optional function that generates examples for few-shot learning.                                                                                      |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                   | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
 | `alignment_mode`          | `str`                                   | `"contract"`                                             | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
 | `case_sensitive_matching` | `bool`                                  | `False`                                                  | Whether to search without case sensitivity.                                                                                                           |
 | `single_match`            | `bool`                                  | `False`                                                  | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                         |
@@ -365,15 +371,14 @@
 | `labels`                  | `str`                                   |              | Comma-separated list of labels.                                                                                                              |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`       | Optional function that generates examples for few-shot learning.                                                                             |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`       | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                           |
 | `alignment_mode`          | `str`                                   | `"contract"` | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`. |
 | `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
 | `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
 
-[ner]: https://github.com/explosion/spacy-llm/blob/main/spacy_llm/tasks/ner.py#L14
 
 The NER task implementation doesn't currently ask the LLM for specific offsets, but simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured by the following parameters:
 
 - The `single_match` parameter is typically set to `False` to allow for multiple matches. For instance, the response from the LLM might only mention the entity "Paris" once, but you'd still
   want to mark it every time it occurs in the document.
 - The case-sensitive matching is typically set to `False` to be robust against case variances in the LLM's output.
@@ -412,21 +417,21 @@
 
 The built-in SpanCat task is a simple adaptation of the NER task to
 support overlapping entities and store its annotations in `doc.spans`.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.SpanCat.v2"
-labels = PERSON,ORGANISATION,LOCATION
+labels = ["PERSON", "ORGANISATION", "LOCATION"]
 examples = null
 ```
 
 | Argument                  | Type                                    | Default                                                            | Description                                                                                                                                           |
 | ------------------------- | --------------------------------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `labels`                  | `str`                                   |                                                                    | Comma-separated list of labels.                                                                                                                       |
+| `labels`                  | `Union[List[str], str]`                 |                                                                    | List of labels or str of comma-separated list of labels.                                                                                              |
 | `template`                | `str`                                   | [`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
 | `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                             | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
 | `spans_key`               | `str`                                   | `"sc"`                                                             | Key of the `Doc.spans` dict to save the spans under.                                                                                                  |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                             | Optional function that generates examples for few-shot learning.                                                                                      |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                             | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
 | `alignment_mode`          | `str`                                   | `"contract"`                                                       | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
 | `case_sensitive_matching` | `bool`                                  | `False`                                                            | Whether to search without case sensitivity.                                                                                                           |
@@ -465,21 +470,21 @@
 #### spacy.TextCat.v2
 
 The built-in TextCat task supports both zero-shot and few-shot prompting.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
-labels = COMPLIMENT,INSULT
+labels = ["COMPLIMENT", "INSULT"]
 examples = null
 ```
 
 | Argument            | Type                                    | Default                                                      | Description                                                                                                                                      |
 | ------------------- | --------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
-| `labels`            | `str`                                   |                                                              | Comma-separated list of labels.                                                                                                                  |
+| `labels`            | `Union[List[str], str]`                 |                                                              | List of labels or str of comma-separated list of labels.                                                                                         |
 | `template`          | `str`                                   | [`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.         |
 | `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                       | Optional function that generates examples for few-shot learning.                                                                                 |
 | `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                                       | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                             |
 | `exclusive_classes` | `bool`                                  | `False`                                                      | If set to `True`, only one label per document should be valid. If set to `False`, one document can have multiple labels.                         |
 | `allow_none`        | `bool`                                  | `True`                                                       | When set to `True`, allows the LLM to not return any of the given label. The resulting dict in `doc.cats` will have `0.0` scores for all labels. |
 | `verbose`           | `bool`                                  | `False`                                                      | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                             |
 
@@ -498,15 +503,15 @@
   }
 ]
 ```
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
-labels = COMPLIMENT,INSULT
+labels = ["COMPLIMENT", "INSULT"]
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "textcat_examples.json"
 ```
 
 #### spacy.TextCat.v1
 
@@ -557,20 +562,20 @@
 
 The built-in REL task supports both zero-shot and few-shot prompting.
 It relies on an upstream NER component for entities extraction.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.REL.v1"
-labels = LivesIn,Visits
+labels = ["LivesIn", "Visits"]
 ```
 
 | Argument            | Type                                    | Default                                              | Description                                                                                                                              |
 | ------------------- | --------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
-| `labels`            | `str`                                   |                                                      | Comma-separated list of relation labels.                                                                                                 |
+| `labels`            | `Union[List[str], str]`                 |                                                      | List of labels or str of comma-separated list of labels.                                                                                 |
 | `template`          | `str`                                   | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
 | `label_description` | `Optional[Dict[str, str]]`              | `None`                                               | Dictionary providing a description for each relation label.                                                                              |
 | `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                               | Optional function that generates examples for few-shot learning.                                                                         |
 | `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                               | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                     |
 | `verbose`           | `bool`                                  | `False`                                              | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                     |
 
 To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
@@ -584,15 +589,15 @@
 Note: the REL task relies on pre-extracted entities to make its prediction.
 Hence, you'll need to add a component that populates `doc.ents` with recognized
 spans to your spaCy pipeline and put it _before_ the REL component.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.REL.v1"
-labels = LivesIn,Visits
+labels = ["LivesIn", "Visits"]
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "rel_examples.jsonl"
 ```
 
 #### spacy.NoOp.v1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.2.0 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.2.1 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
@@ -77,63 +77,64 @@
 api) documentation. ### Example 1: Add a text classifier using a GPT-3 model
 from OpenAI Create a new API key from openai.com or fetch an existing one, and
 ensure the keys are set as environmental variables. For more background
 information, see the [OpenAI](#openai) section. Create a config file
 `config.cfg` containing at least the following (or see the full example [here]
 (usage_examples/textcat_openai)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
-= "spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.backend]
+= "spacy.TextCat.v2" labels = ["COMPLIMENT", "INSULT"] [components.llm.backend]
 @llm_backends = "spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-
 turbo", "temperature": 0.3} ``` Now run: ```python from spacy_llm.util import
 assemble nlp = assemble("config.cfg") doc = nlp("You look gorgeous!") print
 (doc.cats) ``` ### Example 2: Add NER using an open-source model through
 Hugging Face To run this example, ensure that you have a GPU enabled, and
 `transformers`, `torch` and CUDA installed. For more background information,
 see the [DollyHF](#spacydollyhfv1) section. Create a config file `config.cfg`
 containing at least the following (or see the full example [here]
 (usage_examples/ner_dolly)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
-= "spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION [components.llm.backend]
-@llm_backends = "spacy.DollyHF.v1" # For better performance, use databricks/
-dolly-v2-12b instead model = "databricks/dolly-v2-3b" ``` Now run: ```python
-from spacy_llm.util import assemble nlp = assemble("config.cfg") doc = nlp
-("Jack and Jill rode up the hill in Les Deux Alpes") print([(ent.text,
-ent.label_) for ent in doc.ents]) ``` Note that Hugging Face will download the
-`"databricks/dolly-v2-3b"` model the first time you use it. You can [define the
-cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/
-manage-cache) by setting the environmental variable `HF_HOME`. Also, you can
-upgrade the model to be `"databricks/dolly-v2-12b"` for better performance. ###
-Example 3: Create the component directly in Python The `llm` component behaves
-as any other spaCy component does, so adding it to an existing pipeline follows
-the same pattern: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
-( "llm", config={ "task": { "@llm_tasks": "spacy.NER.v2", "labels":
-"PERSON,ORGANISATION,LOCATION" }, "backend": { "@llm_backends":
-"spacy.REST.v1", "api": "OpenAI", "config": {"model": "gpt-3.5-turbo"}, }, }, )
-nlp.initialize() doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
-print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient
-usage of resources, typically you would use [`nlp.pipe(docs)`](https://
-spacy.io/api/language#pipe) with a batch, instead of calling `nlp(doc)` with a
-single document. ### Example 4: Implement your own custom task To write a
-[`task`](#tasks), you need to implement two functions: `generate_prompts` that
-takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
-them into a list of prompts, and `parse_responses` that transforms the LLM
-outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity
-spans, text categories and more. To register your custom task with spaCy,
-decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator
-with a custom name that you can refer to in your config. > ð For more
-details, see the [**usage example on writing your own task**](usage_examples/
-README.md#writing-your-own-task) ```python from spacy_llm.registry import
-registry from spacy_llm.util import split_labels @registry.llm_tasks
-("my_namespace.MyTask.v1") def make_my_task(labels: str, my_other_config_val:
-float) -> "MyTask": labels_list = split_labels(labels) return MyTask
-(labels=labels_list, my_other_config_val=my_other_config_val) class MyTask: def
-__init__(self, labels: List[str], my_other_config_val: float): ... def
-generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]: ... def
-parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] ) -
-> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
+= "spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"]
+[components.llm.backend] @llm_backends = "spacy.DollyHF.v1" # For better
+performance, use databricks/dolly-v2-12b instead model = "databricks/dolly-v2-
+3b" ``` Now run: ```python from spacy_llm.util import assemble nlp = assemble
+("config.cfg") doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
+print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that Hugging Face
+will download the `"databricks/dolly-v2-3b"` model the first time you use it.
+You can [define the cached directory](https://huggingface.co/docs/
+huggingface_hub/main/en/guides/manage-cache) by setting the environmental
+variable `HF_HOME`. Also, you can upgrade the model to be `"databricks/dolly-
+v2-12b"` for better performance. ### Example 3: Create the component directly
+in Python The `llm` component behaves as any other spaCy component does, so
+adding it to an existing pipeline follows the same pattern: ```python import
+spacy nlp = spacy.blank("en") nlp.add_pipe( "llm", config={ "task":
+{ "@llm_tasks": "spacy.NER.v2", "labels": ["PERSON", "ORGANISATION",
+"LOCATION"] }, "backend": { "@llm_backends": "spacy.REST.v1", "api": "OpenAI",
+"config": {"model": "gpt-3.5-turbo"}, }, }, ) nlp.initialize() doc = nlp("Jack
+and Jill rode up the hill in Les Deux Alpes") print([(ent.text, ent.label_) for
+ent in doc.ents]) ``` Note that for efficient usage of resources, typically you
+would use [`nlp.pipe(docs)`](https://spacy.io/api/language#pipe) with a batch,
+instead of calling `nlp(doc)` with a single document. ### Example 4: Implement
+your own custom task To write a [`task`](#tasks), you need to implement two
+functions: `generate_prompts` that takes a list of spaCy [`Doc`](https://
+spacy.io/api/doc) objects and transforms them into a list of prompts, and
+`parse_responses` that transforms the LLM outputs into annotations on the
+[`Doc`](https://spacy.io/api/doc), e.g. entity spans, text categories and more.
+To register your custom task with spaCy, decorate a factory function using the
+`spacy_llm.registry.llm_tasks` decorator with a custom name that you can refer
+to in your config. > ð For more details, see the [**usage example on writing
+your own task**](usage_examples/README.md#writing-your-own-task) ```python from
+typing import Iterable, List from spacy.tokens import Doc from
+spacy_llm.registry import registry from spacy_llm.util import split_labels
+@registry.llm_tasks("my_namespace.MyTask.v1") def make_my_task(labels: str,
+my_other_config_val: float) -> "MyTask": labels_list = split_labels(labels)
+return MyTask(labels=labels_list, my_other_config_val=my_other_config_val)
+class MyTask: def __init__(self, labels: List[str], my_other_config_val:
+float): ... def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
+... def parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] )
+-> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
 @llm_tasks = "my_namespace.MyTask.v1" labels = LABEL1,LABEL2,LABEL3
 my_other_config_val = 0.3 ``` ## ð API Each `llm` component is defined by
 two main settings: - A [**task**](#tasks), defining the prompt to send to the
 LLM as well as the functionality to parse the resulting response back into
 structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects. - A
 [**backend**](#backends) defining the model to use and how to connect to it.
 Note that `spacy-llm` supports both access to external APIs (such as OpenAI) as
@@ -142,50 +143,55 @@
 functionality to avoid running the same document through an LLM service (be it
 local or through a REST API) more than once. ### Tasks A _task_ defines an NLP
 problem or question, that will be sent to the LLM via a prompt. Further, the
 task defines how to parse the LLM's responses back into structured information.
 All tasks are registered in spaCy's `llm_tasks` registry. Practically speaking,
 a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`]
 (spacy_llm/ty.py). It needs to define a `generate_prompts` function and a
-`parse_responses` function. #### function `task.generate_prompts` Takes a
-collection of documents, and returns a collection of "prompts", which can be of
-type `Any`. Often, prompts are of type `str` - but this is not enforced to
-allow for maximum flexibility in the framework. | Argument | Type | Description
-| | ----------- | --------------- | ---------------------- | | `docs` |
-`Iterable[Doc]` | The input documents. | | **RETURNS** | `Iterable[Any]` | The
-generated prompts. | #### function `task.parse_responses` Takes a collection of
-LLM responses and the original documents, parses the responses into structured
-information, and sets the annotations on the documents. The `parse_responses`
-function is free to set the annotations in any way, including `Doc` fields like
-`ents`, `spans` or `cats`, or using custom defined fields. The `responses` are
-of type `Iterable[Any]`, though they will often be `str` objects. This depends
-on the return type of the [backend](#backends). | Argument | Type | Description
-| | ----------- | --------------- | ------------------------ | | `docs` |
-`Iterable[Doc]` | The input documents. | | `responses` | `Iterable[Any]` | The
-generated prompts. | | **RETURNS** | `Iterable[Doc]` | The annotated documents.
-| #### spacy.NER.v2 The built-in NER task supports both zero-shot and few-shot
-prompting. This version also supports explicitly defining the provided labels
-with custom descriptions. ```ini [components.llm.task] @llm_tasks =
-"spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION examples = null ``` |
-Argument | Type | Default | Description | | ------------------------- | -------
--------------------------------- | --------------------------------------------
------------- | ----------------------------------------------------------------
+`parse_responses` function. Moreover, the task may define an optional [`scorer`
+method](https://spacy.io/api/scorer#score). It should accept an iterable of
+`Example`s as input and return a score dictionary. If the `scorer` method is
+defined, `spacy-llm` will call it to evaluate the component. #### function
+`task.generate_prompts` Takes a collection of documents, and returns a
+collection of "prompts", which can be of type `Any`. Often, prompts are of type
+`str` - but this is not enforced to allow for maximum flexibility in the
+framework. | Argument | Type | Description | | ----------- | --------------- |
+---------------------- | | `docs` | `Iterable[Doc]` | The input documents. | |
+**RETURNS** | `Iterable[Any]` | The generated prompts. | #### function
+`task.parse_responses` Takes a collection of LLM responses and the original
+documents, parses the responses into structured information, and sets the
+annotations on the documents. The `parse_responses` function is free to set the
+annotations in any way, including `Doc` fields like `ents`, `spans` or `cats`,
+or using custom defined fields. The `responses` are of type `Iterable[Any]`,
+though they will often be `str` objects. This depends on the return type of the
+[backend](#backends). | Argument | Type | Description | | ----------- | -------
+-------- | ------------------------ | | `docs` | `Iterable[Doc]` | The input
+documents. | | `responses` | `Iterable[Any]` | The generated prompts. | |
+**RETURNS** | `Iterable[Doc]` | The annotated documents. | #### spacy.NER.v2
+The built-in NER task supports both zero-shot and few-shot prompting. This
+version also supports explicitly defining the provided labels with custom
+descriptions. ```ini [components.llm.task] @llm_tasks = "spacy.NER.v2" labels =
+["PERSON", "ORGANISATION", "LOCATION"] examples = null ``` | Argument | Type |
+Default | Description | | ------------------------- | -------------------------
+-------------- | -------------------------------------------------------- | ---
 -------------------------------------------------------------------------------
------- | | `labels` | `str` | | Comma-separated list of labels. | | `template`
-| `str` | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom
-prompt template to send to LLM backend. Default templates for each task are
-located in the `spacy_llm/tasks/templates` directory. | | `label_definitions` |
-`Optional[Dict[str, str]]` | `None` | Optional dict mapping a label to a
-description of that label. These descriptions are added to the prompt to help
-instruct the LLM on what to extract. | | `examples` | `Optional[Callable[[],
-Iterable[Any]]]` | `None` | Optional function that generates examples for few-
-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None` |
-Function that normalizes the labels as returned by the LLM. If `None`, defaults
-to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"`
-| Alignment mode in case the LLM returns entities that do not align with token
+------------------------------------------------------------------- | |
+`labels` | `Union[List[str], str]` | | List of labels or str of comma-separated
+list of labels. | | `template` | `str` | [ner.v2.jinja](./spacy_llm/tasks/
+templates/ner.v2.jinja) | Custom prompt template to send to LLM backend.
+Default templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `label_definitions` | `Optional[Dict[str, str]]` | `None` |
+Optional dict mapping a label to a description of that label. These
+descriptions are added to the prompt to help instruct the LLM on what to
+extract. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
+Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, defaults to
+`spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
+Alignment mode in case the LLM returns entities that do not align with token
 boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
 `case_sensitive_matching` | `bool` | `False` | Whether to search without case
 sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
 in the LLM's response only once (the first hit) or multiple times. | The NER
 task implementation doesn't currently ask the LLM for specific offsets, but
 simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured
@@ -234,16 +240,15 @@
 [[str], str]]` | `None` | Function that normalizes the labels as returned by
 the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`. | |
 `alignment_mode` | `str` | `"contract"` | Alignment mode in case the LLM
 returns entities that do not align with token boundaries. Options are
 `"strict"`, `"contract"` or `"expand"`. | | `case_sensitive_matching` | `bool`
 | `False` | Whether to search without case sensitivity. | | `single_match` |
 `bool` | `False` | Whether to match an entity in the LLM's response only once
-(the first hit) or multiple times. | [ner]: https://github.com/explosion/spacy-
-llm/blob/main/spacy_llm/tasks/ner.py#L14 The NER task implementation doesn't
+(the first hit) or multiple times. | The NER task implementation doesn't
 currently ask the LLM for specific offsets, but simply expects a list of
 strings that represent the enties in the document. This means that a form of
 string matching is required. This can be configured by the following
 parameters: - The `single_match` parameter is typically set to `False` to allow
 for multiple matches. For instance, the response from the LLM might only
 mention the entity "Paris" once, but you'd still want to mark it every time it
 occurs in the document. - The case-sensitive matching is typically set to
@@ -261,148 +266,150 @@
 ```yaml - text: Jack and Jill went up the hill. entities: PERSON: - Jack - Jill
 LOCATION: - hill - text: Jack fell down and broke his crown. entities: PERSON:
 - Jack ``` ```ini [components.llm.task] @llm_tasks = "spacy.NER.v1" labels =
 PERSON,ORGANISATION,LOCATION [components.llm.task.examples] @misc =
 "spacy.FewShotReader.v1" path = "ner_examples.yml" ``` #### spacy.SpanCat.v2
 The built-in SpanCat task is a simple adaptation of the NER task to support
 overlapping entities and store its annotations in `doc.spans`. ```ini
-[components.llm.task] @llm_tasks = "spacy.SpanCat.v2" labels =
-PERSON,ORGANISATION,LOCATION examples = null ``` | Argument | Type | Default |
+[components.llm.task] @llm_tasks = "spacy.SpanCat.v2" labels = ["PERSON",
+"ORGANISATION", "LOCATION"] examples = null ``` | Argument | Type | Default |
 Description | | ------------------------- | -----------------------------------
 ---- | ------------------------------------------------------------------ | ---
 -------------------------------------------------------------------------------
 ------------------------------------------------------------------- | |
-`labels` | `str` | | Comma-separated list of labels. | | `template` | `str` |
-[`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom
-prompt template to send to LLM backend. Default templates for each task are
-located in the `spacy_llm/tasks/templates` directory. | | `label_definitions` |
-`Optional[Dict[str, str]]` | `None` | Optional dict mapping a label to a
-description of that label. These descriptions are added to the prompt to help
-instruct the LLM on what to extract. | | `spans_key` | `str` | `"sc"` | Key of
-the `Doc.spans` dict to save the spans under. | | `examples` | `Optional
-[Callable[[], Iterable[Any]]]` | `None` | Optional function that generates
-examples for few-shot learning. | | `normalizer` | `Optional[Callable[[str],
-str]]` | `None` | Function that normalizes the labels as returned by the LLM.
-If `None`, defaults to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` |
-`str` | `"contract"` | Alignment mode in case the LLM returns entities that do
-not align with token boundaries. Options are `"strict"`, `"contract"` or
-`"expand"`. | | `case_sensitive_matching` | `bool` | `False` | Whether to
-search without case sensitivity. | | `single_match` | `bool` | `False` |
-Whether to match an entity in the LLM's response only once (the first hit) or
-multiple times. | Except for the `spans_key` parameter, the SpanCat task reuses
-the configuration from the NER task. Refer to [its documentation](#spacynerv2)
-for more insight. #### spacy.SpanCat.v1 The original version of the built-in
-SpanCat task is a simple adaptation of the v1 NER task to support overlapping
-entities and store its annotations in `doc.spans`. ```ini [components.llm.task]
-@llm_tasks = "spacy.SpanCat.v1" labels = PERSON,ORGANISATION,LOCATION examples
-= null ``` | Argument | Type | Default | Description | | ----------------------
---- | --------------------------------------- | ------------ | ----------------
+`labels` | `Union[List[str], str]` | | List of labels or str of comma-separated
+list of labels. | | `template` | `str` | [`spancat.v2.jinja`](./spacy_llm/
+tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM
+backend. Default templates for each task are located in the `spacy_llm/tasks/
+templates` directory. | | `label_definitions` | `Optional[Dict[str, str]]` |
+`None` | Optional dict mapping a label to a description of that label. These
+descriptions are added to the prompt to help instruct the LLM on what to
+extract. | | `spans_key` | `str` | `"sc"` | Key of the `Doc.spans` dict to save
+the spans under. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` |
+`None` | Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, defaults to
+`spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
+Alignment mode in case the LLM returns entities that do not align with token
+boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
+`case_sensitive_matching` | `bool` | `False` | Whether to search without case
+sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
+in the LLM's response only once (the first hit) or multiple times. | Except for
+the `spans_key` parameter, the SpanCat task reuses the configuration from the
+NER task. Refer to [its documentation](#spacynerv2) for more insight. ####
+spacy.SpanCat.v1 The original version of the built-in SpanCat task is a simple
+adaptation of the v1 NER task to support overlapping entities and store its
+annotations in `doc.spans`. ```ini [components.llm.task] @llm_tasks =
+"spacy.SpanCat.v1" labels = PERSON,ORGANISATION,LOCATION examples = null ``` |
+Argument | Type | Default | Description | | ------------------------- | -------
+-------------------------------- | ------------ | -----------------------------
 -------------------------------------------------------------------------------
---------------------------------------------- | | `labels` | `str` | | Comma-
-separated list of labels. | | `spans_key` | `str` | `"sc"` | Key of the
-`Doc.spans` dict to save the spans under. | | `examples` | `Optional[Callable[
-[], Iterable[Any]]]` | `None` | Optional function that generates examples for
-few-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None`
-| Function that normalizes the labels as returned by the LLM. If `None`,
-defaults to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` |
-`"contract"` | Alignment mode in case the LLM returns entities that do not
-align with token boundaries. Options are `"strict"`, `"contract"` or
-`"expand"`. | | `case_sensitive_matching` | `bool` | `False` | Whether to
-search without case sensitivity. | | `single_match` | `bool` | `False` |
-Whether to match an entity in the LLM's response only once (the first hit) or
-multiple times. | Except for the `spans_key` parameter, the SpanCat task reuses
-the configuration from the NER task. Refer to [its documentation](#spacynerv1)
-for more insight. #### spacy.TextCat.v2 The built-in TextCat task supports both
-zero-shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks =
-"spacy.TextCat.v2" labels = COMPLIMENT,INSULT examples = null ``` | Argument |
-Type | Default | Description | | ------------------- | ------------------------
---------------- | -----------------------------------------------------------
-- | ---------------------------------------------------------------------------
---------------------------------------------------------------------- | |
-`labels` | `str` | | Comma-separated list of labels. | | `template` | `str` |
-[`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt
-template to send to LLM backend. Default templates for each task are located in
-the `spacy_llm/tasks/templates` directory. | | `examples` | `Optional[Callable[
-[], Iterable[Any]]]` | `None` | Optional function that generates examples for
-few-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None`
-| Function that normalizes the labels as returned by the LLM. If `None`, falls
-back to `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` |
-`False` | If set to `True`, only one label per document should be valid. If set
-to `False`, one document can have multiple labels. | | `allow_none` | `bool` |
-`True` | When set to `True`, allows the LLM to not return any of the given
-label. The resulting dict in `doc.cats` will have `0.0` scores for all labels.
-| | `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
-when the LLM returns invalid responses. | To perform few-shot learning, you can
-write down a few examples in a separate file, and provide these to be injected
-into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
-supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
-great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
-"answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
-"spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.task.examples]
-@misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
-spacy.TextCat.v1 The original version of the built-in TextCat task supports
-both zero-shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks
-= "spacy.TextCat.v1" labels = COMPLIMENT,INSULT examples = null ``` | Argument
-| Type | Default | Description | | ------------------- | ----------------------
------------------ | ------- | -------------------------------------------------
+-------------------------------- | | `labels` | `str` | | Comma-separated list
+of labels. | | `spans_key` | `str` | `"sc"` | Key of the `Doc.spans` dict to
+save the spans under. | | `examples` | `Optional[Callable[[], Iterable[Any]]]`
+| `None` | Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, defaults to
+`spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
+Alignment mode in case the LLM returns entities that do not align with token
+boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
+`case_sensitive_matching` | `bool` | `False` | Whether to search without case
+sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
+in the LLM's response only once (the first hit) or multiple times. | Except for
+the `spans_key` parameter, the SpanCat task reuses the configuration from the
+NER task. Refer to [its documentation](#spacynerv1) for more insight. ####
+spacy.TextCat.v2 The built-in TextCat task supports both zero-shot and few-shot
+prompting. ```ini [components.llm.task] @llm_tasks = "spacy.TextCat.v2" labels
+= ["COMPLIMENT", "INSULT"] examples = null ``` | Argument | Type | Default |
+Description | | ------------------- | --------------------------------------- |
+------------------------------------------------------------ | ----------------
 -------------------------------------------------------------------------------
----------------- | | `labels` | str | | Comma-separated list of labels. | |
-`examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` | Optional
-function that generates examples for few-shot learning. | | `normalizer` |
-`Optional[Callable[[str], str]]` | `None` | Function that normalizes the labels
-as returned by the LLM. If `None`, falls back to
+------------------------------------------------- | | `labels` | `Union[List
+[str], str]` | | List of labels or str of comma-separated list of labels. | |
+`template` | `str` | [`textcat.jinja`](./spacy_llm/tasks/templates/
+textcat.jinja) | Custom prompt template to send to LLM backend. Default
+templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
+Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, falls back to
 `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` | `False` | If
 set to `True`, only one label per document should be valid. If set to `False`,
 one document can have multiple labels. | | `allow_none` | `bool` | `True` |
 When set to `True`, allows the LLM to not return any of the given label. The
 resulting dict in `doc.cats` will have `0.0` scores for all labels. | |
 `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
 when the LLM returns invalid responses. | To perform few-shot learning, you can
 write down a few examples in a separate file, and provide these to be injected
 into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
 supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
 great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
 "answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
+"spacy.TextCat.v2" labels = ["COMPLIMENT", "INSULT"]
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"textcat_examples.json" ``` #### spacy.TextCat.v1 The original version of the
+built-in TextCat task supports both zero-shot and few-shot prompting. ```ini
+[components.llm.task] @llm_tasks = "spacy.TextCat.v1" labels =
+COMPLIMENT,INSULT examples = null ``` | Argument | Type | Default | Description
+| | ------------------- | --------------------------------------- | ------- | -
+-------------------------------------------------------------------------------
+---------------------------------------------------------------- | | `labels` |
+str | | Comma-separated list of labels. | | `examples` | `Optional[Callable[[],
+Iterable[Any]]]` | `None` | Optional function that generates examples for few-
+shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None` |
+Function that normalizes the labels as returned by the LLM. If `None`, falls
+back to `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` |
+`False` | If set to `True`, only one label per document should be valid. If set
+to `False`, one document can have multiple labels. | | `allow_none` | `bool` |
+`True` | When set to `True`, allows the LLM to not return any of the given
+label. The resulting dict in `doc.cats` will have `0.0` scores for all labels.
+| | `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
+when the LLM returns invalid responses. | To perform few-shot learning, you can
+write down a few examples in a separate file, and provide these to be injected
+into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
+supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
+great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
+"answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
 "spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
 spacy.REL.v1 The built-in REL task supports both zero-shot and few-shot
 prompting. It relies on an upstream NER component for entities extraction.
-```ini [components.llm.task] @llm_tasks = "spacy.REL.v1" labels =
-LivesIn,Visits ``` | Argument | Type | Default | Description | | --------------
------ | --------------------------------------- | -----------------------------
------------------------ | -----------------------------------------------------
--------------------------------------------------------------------------------
----- | | `labels` | `str` | | Comma-separated list of relation labels. | |
-`template` | `str` | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) |
-Custom prompt template to send to LLM backend. Default templates for each task
-are located in the `spacy_llm/tasks/templates` directory. | |
-`label_description` | `Optional[Dict[str, str]]` | `None` | Dictionary
-providing a description for each relation label. | | `examples` | `Optional
-[Callable[[], Iterable[Any]]]` | `None` | Optional function that generates
-examples for few-shot learning. | | `normalizer` | `Optional[Callable[[str],
-str]]` | `None` | Function that normalizes the labels as returned by the LLM.
-If `None`, falls back to `spacy.LowercaseNormalizer.v1`. | | `verbose` | `bool`
-| `False` | If set to `True`, warnings will be generated when the LLM returns
-invalid responses. | To perform few-shot learning, you can write down a few
-examples in a separate file, and provide these to be injected into the prompt
-to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
+```ini [components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
+"Visits"] ``` | Argument | Type | Default | Description | | ------------------
+- | --------------------------------------- | ---------------------------------
+------------------- | ---------------------------------------------------------
+------------------------------------------------------------------------------
+- | | `labels` | `Union[List[str], str]` | | List of labels or str of comma-
+separated list of labels. | | `template` | `str` | [`rel.jinja`](./spacy_llm/
+tasks/templates/rel.jinja) | Custom prompt template to send to LLM backend.
+Default templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `label_description` | `Optional[Dict[str, str]]` | `None` |
+Dictionary providing a description for each relation label. | | `examples` |
+`Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
+generates examples for few-shot learning. | | `normalizer` | `Optional[Callable
+[[str], str]]` | `None` | Function that normalizes the labels as returned by
+the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`. | | `verbose`
+| `bool` | `False` | If set to `True`, warnings will be generated when the LLM
+returns invalid responses. | To perform few-shot learning, you can write down a
+few examples in a separate file, and provide these to be injected into the
+prompt to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
 `.yaml`, `.json` and `.jsonl`. ```json {"text": "Laura bought a house in Boston
 with her husband Mark.", "ents": [{"start_char": 0, "end_char": 5, "label":
 "PERSON"}, {"start_char": 24, "end_char": 30, "label": "GPE"}, {"start_char":
 48, "end_char": 52, "label": "PERSON"}], "relations": [{"dep": 0, "dest": 1,
 "relation": "LivesIn"}, {"dep": 2, "dest": 1, "relation": "LivesIn"}]} {"text":
 "Michael travelled through South America by bike.", "ents": [{"start_char": 0,
 "end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label":
 "LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]} ``` Note:
 the REL task relies on pre-extracted entities to make its prediction. Hence,
 you'll need to add a component that populates `doc.ents` with recognized spans
 to your spaCy pipeline and put it _before_ the REL component. ```ini
-[components.llm.task] @llm_tasks = "spacy.REL.v1" labels = LivesIn,Visits
-[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
-"rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
+[components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
+"Visits"] [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path
+= "rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
 testing - it tells the LLM to do nothing, and does not set any fields on the
 `docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
 Backends A _backend_ defines which LLM model to query, and how to query it. It
 can be a simple function taking a collection of prompts (consistent with the
 output type of `task.generate_prompts()`) and returning a collection of
 responses (consistent with the expected input of `parse_responses`). Generally
 speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
```

### Comparing `spacy-llm-0.2.0/README.md` & `spacy-llm-0.2.1/spacy_llm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: spacy-llm
+Version: 0.2.1
+Summary: Integrating LLMs into structured NLP pipelines
+Author: Explosion
+Author-email: contact@explosion.ai
+License: MIT
+Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
+Project-URL: Source, https://github.com/explosion/spacy-llm
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: minichain
+Provides-Extra: langchain
+Provides-Extra: transformers
+License-File: LICENSE
+
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-llm: Integrating LLMs into structured NLP pipelines
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/spacy-llm/actions/workflows/test.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
@@ -61,15 +93,15 @@
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
-labels = COMPLIMENT,INSULT
+labels = ["COMPLIMENT", "INSULT"]
 
 [components.llm.backend]
 @llm_backends = "spacy.REST.v1"
 api = "OpenAI"
 config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
 ```
 
@@ -99,15 +131,15 @@
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
-labels = PERSON,ORGANISATION,LOCATION
+labels = ["PERSON", "ORGANISATION", "LOCATION"]
 
 [components.llm.backend]
 @llm_backends = "spacy.DollyHF.v1"
 # For better performance, use databricks/dolly-v2-12b instead
 model = "databricks/dolly-v2-3b"
 ```
 
@@ -136,15 +168,15 @@
 
 nlp = spacy.blank("en")
 nlp.add_pipe(
     "llm",
     config={
         "task": {
             "@llm_tasks": "spacy.NER.v2",
-            "labels": "PERSON,ORGANISATION,LOCATION"
+            "labels": ["PERSON", "ORGANISATION", "LOCATION"]
         },
         "backend": {
             "@llm_backends": "spacy.REST.v1",
             "api": "OpenAI",
             "config": {"model": "gpt-3.5-turbo"},
         },
     },
@@ -165,14 +197,16 @@
 them into a list of prompts, and `parse_responses` that transforms the LLM outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity spans, text categories and more.
 
 To register your custom task with spaCy, decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator with a custom name that you can refer to in your config.
 
 > 📖 For more details, see the [**usage example on writing your own task**](usage_examples/README.md#writing-your-own-task)
 
 ```python
+from typing import Iterable, List
+from spacy.tokens import Doc
 from spacy_llm.registry import registry
 from spacy_llm.util import split_labels
 
 
 @registry.llm_tasks("my_namespace.MyTask.v1")
 def make_my_task(labels: str, my_other_config_val: float) -> "MyTask":
     labels_list = split_labels(labels)
@@ -216,14 +250,18 @@
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
 
+Moreover, the task may define an optional [`scorer` method](https://spacy.io/api/scorer#score).
+It should accept an iterable of `Example`s as input and return a score dictionary.
+If the `scorer` method is defined, `spacy-llm` will call it to evaluate the component.
+
 #### <kbd>function</kbd> `task.generate_prompts`
 
 Takes a collection of documents, and returns a collection of "prompts", which can be of type `Any`.
 Often, prompts are of type `str` - but this is not enforced to allow for maximum flexibility in the framework.
 
 | Argument    | Type            | Description            |
 | ----------- | --------------- | ---------------------- |
@@ -248,21 +286,21 @@
 #### spacy.NER.v2
 
 The built-in NER task supports both zero-shot and few-shot prompting. This version also supports explicitly defining the provided labels with custom descriptions.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
-labels = PERSON,ORGANISATION,LOCATION
+labels = ["PERSON", "ORGANISATION", "LOCATION"]
 examples = null
 ```
 
 | Argument                  | Type                                    | Default                                                  | Description                                                                                                                                           |
 | ------------------------- | --------------------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `labels`                  | `str`                                   |                                                          | Comma-separated list of labels.                                                                                                                       |
+| `labels`                  | `Union[List[str], str]`                 |                                                          | List of labels or str of comma-separated list of labels.                                                                                              |
 | `template`                | `str`                                   | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
 | `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                   | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                   | Optional function that generates examples for few-shot learning.                                                                                      |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                   | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
 | `alignment_mode`          | `str`                                   | `"contract"`                                             | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
 | `case_sensitive_matching` | `bool`                                  | `False`                                                  | Whether to search without case sensitivity.                                                                                                           |
 | `single_match`            | `bool`                                  | `False`                                                  | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                         |
@@ -333,15 +371,14 @@
 | `labels`                  | `str`                                   |              | Comma-separated list of labels.                                                                                                              |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`       | Optional function that generates examples for few-shot learning.                                                                             |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`       | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                           |
 | `alignment_mode`          | `str`                                   | `"contract"` | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`. |
 | `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
 | `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
 
-[ner]: https://github.com/explosion/spacy-llm/blob/main/spacy_llm/tasks/ner.py#L14
 
 The NER task implementation doesn't currently ask the LLM for specific offsets, but simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured by the following parameters:
 
 - The `single_match` parameter is typically set to `False` to allow for multiple matches. For instance, the response from the LLM might only mention the entity "Paris" once, but you'd still
   want to mark it every time it occurs in the document.
 - The case-sensitive matching is typically set to `False` to be robust against case variances in the LLM's output.
@@ -380,21 +417,21 @@
 
 The built-in SpanCat task is a simple adaptation of the NER task to
 support overlapping entities and store its annotations in `doc.spans`.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.SpanCat.v2"
-labels = PERSON,ORGANISATION,LOCATION
+labels = ["PERSON", "ORGANISATION", "LOCATION"]
 examples = null
 ```
 
 | Argument                  | Type                                    | Default                                                            | Description                                                                                                                                           |
 | ------------------------- | --------------------------------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `labels`                  | `str`                                   |                                                                    | Comma-separated list of labels.                                                                                                                       |
+| `labels`                  | `Union[List[str], str]`                 |                                                                    | List of labels or str of comma-separated list of labels.                                                                                              |
 | `template`                | `str`                                   | [`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
 | `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                             | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
 | `spans_key`               | `str`                                   | `"sc"`                                                             | Key of the `Doc.spans` dict to save the spans under.                                                                                                  |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                             | Optional function that generates examples for few-shot learning.                                                                                      |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                             | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
 | `alignment_mode`          | `str`                                   | `"contract"`                                                       | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
 | `case_sensitive_matching` | `bool`                                  | `False`                                                            | Whether to search without case sensitivity.                                                                                                           |
@@ -433,21 +470,21 @@
 #### spacy.TextCat.v2
 
 The built-in TextCat task supports both zero-shot and few-shot prompting.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
-labels = COMPLIMENT,INSULT
+labels = ["COMPLIMENT", "INSULT"]
 examples = null
 ```
 
 | Argument            | Type                                    | Default                                                      | Description                                                                                                                                      |
 | ------------------- | --------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
-| `labels`            | `str`                                   |                                                              | Comma-separated list of labels.                                                                                                                  |
+| `labels`            | `Union[List[str], str]`                 |                                                              | List of labels or str of comma-separated list of labels.                                                                                         |
 | `template`          | `str`                                   | [`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.         |
 | `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                       | Optional function that generates examples for few-shot learning.                                                                                 |
 | `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                                       | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                             |
 | `exclusive_classes` | `bool`                                  | `False`                                                      | If set to `True`, only one label per document should be valid. If set to `False`, one document can have multiple labels.                         |
 | `allow_none`        | `bool`                                  | `True`                                                       | When set to `True`, allows the LLM to not return any of the given label. The resulting dict in `doc.cats` will have `0.0` scores for all labels. |
 | `verbose`           | `bool`                                  | `False`                                                      | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                             |
 
@@ -466,15 +503,15 @@
   }
 ]
 ```
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
-labels = COMPLIMENT,INSULT
+labels = ["COMPLIMENT", "INSULT"]
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "textcat_examples.json"
 ```
 
 #### spacy.TextCat.v1
 
@@ -525,20 +562,20 @@
 
 The built-in REL task supports both zero-shot and few-shot prompting.
 It relies on an upstream NER component for entities extraction.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.REL.v1"
-labels = LivesIn,Visits
+labels = ["LivesIn", "Visits"]
 ```
 
 | Argument            | Type                                    | Default                                              | Description                                                                                                                              |
 | ------------------- | --------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
-| `labels`            | `str`                                   |                                                      | Comma-separated list of relation labels.                                                                                                 |
+| `labels`            | `Union[List[str], str]`                 |                                                      | List of labels or str of comma-separated list of labels.                                                                                 |
 | `template`          | `str`                                   | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
 | `label_description` | `Optional[Dict[str, str]]`              | `None`                                               | Dictionary providing a description for each relation label.                                                                              |
 | `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                               | Optional function that generates examples for few-shot learning.                                                                         |
 | `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                               | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                     |
 | `verbose`           | `bool`                                  | `False`                                              | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                     |
 
 To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
@@ -552,15 +589,15 @@
 Note: the REL task relies on pre-extracted entities to make its prediction.
 Hence, you'll need to add a component that populates `doc.ents` with recognized
 spans to your spaCy pipeline and put it _before_ the REL component.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.REL.v1"
-labels = LivesIn,Visits
+labels = ["LivesIn", "Visits"]
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "rel_examples.jsonl"
 ```
 
 #### spacy.NoOp.v1
```

#### html2text {}

```diff
@@ -1,12 +1,29 @@
-[https://explosion.ai/assets/img/logo.svg] # spacy-llm: Integrating LLMs into
-structured NLP pipelines [![GitHub Workflow Status](https://img.shields.io/
-github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)]
-(https://github.com/explosion/spacy-llm/actions/workflows/test.yml) [![pypi
-Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.2.1 Summary: Integrating LLMs
+into structured NLP pipelines Author: Explosion Author-email:
+contact@explosion.ai License: MIT Project-URL: Release notes, https://
+github.com/explosion/spacy-llm/releases Project-URL: Source, https://
+github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
+Content-Type: text/markdown Provides-Extra: minichain Provides-Extra: langchain
+Provides-Extra: transformers License-File: LICENSE [https://explosion.ai/
+assets/img/logo.svg] # spacy-llm: Integrating LLMs into structured NLP
+pipelines [![GitHub Workflow Status](https://img.shields.io/github/actions/
+workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/
+explosion/spacy-llm/actions/workflows/test.yml) [![pypi Version](https://
+img.shields.io/pypi/v/spacy-llm.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg?style=flat-square)](https://github.com/ambv/black) This package
 integrates Large Language Models (LLMs) into [spaCy](https://spacy.io),
 featuring a modular system for **fast prototyping** and **prompting**, and
 turning unstructured responses into **robust outputs** for various NLP tasks,
 **no training data** required. - Serializable `llm` **component** to integrate
@@ -60,63 +77,64 @@
 api) documentation. ### Example 1: Add a text classifier using a GPT-3 model
 from OpenAI Create a new API key from openai.com or fetch an existing one, and
 ensure the keys are set as environmental variables. For more background
 information, see the [OpenAI](#openai) section. Create a config file
 `config.cfg` containing at least the following (or see the full example [here]
 (usage_examples/textcat_openai)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
-= "spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.backend]
+= "spacy.TextCat.v2" labels = ["COMPLIMENT", "INSULT"] [components.llm.backend]
 @llm_backends = "spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-
 turbo", "temperature": 0.3} ``` Now run: ```python from spacy_llm.util import
 assemble nlp = assemble("config.cfg") doc = nlp("You look gorgeous!") print
 (doc.cats) ``` ### Example 2: Add NER using an open-source model through
 Hugging Face To run this example, ensure that you have a GPU enabled, and
 `transformers`, `torch` and CUDA installed. For more background information,
 see the [DollyHF](#spacydollyhfv1) section. Create a config file `config.cfg`
 containing at least the following (or see the full example [here]
 (usage_examples/ner_dolly)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
-= "spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION [components.llm.backend]
-@llm_backends = "spacy.DollyHF.v1" # For better performance, use databricks/
-dolly-v2-12b instead model = "databricks/dolly-v2-3b" ``` Now run: ```python
-from spacy_llm.util import assemble nlp = assemble("config.cfg") doc = nlp
-("Jack and Jill rode up the hill in Les Deux Alpes") print([(ent.text,
-ent.label_) for ent in doc.ents]) ``` Note that Hugging Face will download the
-`"databricks/dolly-v2-3b"` model the first time you use it. You can [define the
-cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/
-manage-cache) by setting the environmental variable `HF_HOME`. Also, you can
-upgrade the model to be `"databricks/dolly-v2-12b"` for better performance. ###
-Example 3: Create the component directly in Python The `llm` component behaves
-as any other spaCy component does, so adding it to an existing pipeline follows
-the same pattern: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
-( "llm", config={ "task": { "@llm_tasks": "spacy.NER.v2", "labels":
-"PERSON,ORGANISATION,LOCATION" }, "backend": { "@llm_backends":
-"spacy.REST.v1", "api": "OpenAI", "config": {"model": "gpt-3.5-turbo"}, }, }, )
-nlp.initialize() doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
-print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient
-usage of resources, typically you would use [`nlp.pipe(docs)`](https://
-spacy.io/api/language#pipe) with a batch, instead of calling `nlp(doc)` with a
-single document. ### Example 4: Implement your own custom task To write a
-[`task`](#tasks), you need to implement two functions: `generate_prompts` that
-takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
-them into a list of prompts, and `parse_responses` that transforms the LLM
-outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity
-spans, text categories and more. To register your custom task with spaCy,
-decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator
-with a custom name that you can refer to in your config. > ð For more
-details, see the [**usage example on writing your own task**](usage_examples/
-README.md#writing-your-own-task) ```python from spacy_llm.registry import
-registry from spacy_llm.util import split_labels @registry.llm_tasks
-("my_namespace.MyTask.v1") def make_my_task(labels: str, my_other_config_val:
-float) -> "MyTask": labels_list = split_labels(labels) return MyTask
-(labels=labels_list, my_other_config_val=my_other_config_val) class MyTask: def
-__init__(self, labels: List[str], my_other_config_val: float): ... def
-generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]: ... def
-parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] ) -
-> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
+= "spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"]
+[components.llm.backend] @llm_backends = "spacy.DollyHF.v1" # For better
+performance, use databricks/dolly-v2-12b instead model = "databricks/dolly-v2-
+3b" ``` Now run: ```python from spacy_llm.util import assemble nlp = assemble
+("config.cfg") doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
+print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that Hugging Face
+will download the `"databricks/dolly-v2-3b"` model the first time you use it.
+You can [define the cached directory](https://huggingface.co/docs/
+huggingface_hub/main/en/guides/manage-cache) by setting the environmental
+variable `HF_HOME`. Also, you can upgrade the model to be `"databricks/dolly-
+v2-12b"` for better performance. ### Example 3: Create the component directly
+in Python The `llm` component behaves as any other spaCy component does, so
+adding it to an existing pipeline follows the same pattern: ```python import
+spacy nlp = spacy.blank("en") nlp.add_pipe( "llm", config={ "task":
+{ "@llm_tasks": "spacy.NER.v2", "labels": ["PERSON", "ORGANISATION",
+"LOCATION"] }, "backend": { "@llm_backends": "spacy.REST.v1", "api": "OpenAI",
+"config": {"model": "gpt-3.5-turbo"}, }, }, ) nlp.initialize() doc = nlp("Jack
+and Jill rode up the hill in Les Deux Alpes") print([(ent.text, ent.label_) for
+ent in doc.ents]) ``` Note that for efficient usage of resources, typically you
+would use [`nlp.pipe(docs)`](https://spacy.io/api/language#pipe) with a batch,
+instead of calling `nlp(doc)` with a single document. ### Example 4: Implement
+your own custom task To write a [`task`](#tasks), you need to implement two
+functions: `generate_prompts` that takes a list of spaCy [`Doc`](https://
+spacy.io/api/doc) objects and transforms them into a list of prompts, and
+`parse_responses` that transforms the LLM outputs into annotations on the
+[`Doc`](https://spacy.io/api/doc), e.g. entity spans, text categories and more.
+To register your custom task with spaCy, decorate a factory function using the
+`spacy_llm.registry.llm_tasks` decorator with a custom name that you can refer
+to in your config. > ð For more details, see the [**usage example on writing
+your own task**](usage_examples/README.md#writing-your-own-task) ```python from
+typing import Iterable, List from spacy.tokens import Doc from
+spacy_llm.registry import registry from spacy_llm.util import split_labels
+@registry.llm_tasks("my_namespace.MyTask.v1") def make_my_task(labels: str,
+my_other_config_val: float) -> "MyTask": labels_list = split_labels(labels)
+return MyTask(labels=labels_list, my_other_config_val=my_other_config_val)
+class MyTask: def __init__(self, labels: List[str], my_other_config_val:
+float): ... def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
+... def parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] )
+-> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
 @llm_tasks = "my_namespace.MyTask.v1" labels = LABEL1,LABEL2,LABEL3
 my_other_config_val = 0.3 ``` ## ð API Each `llm` component is defined by
 two main settings: - A [**task**](#tasks), defining the prompt to send to the
 LLM as well as the functionality to parse the resulting response back into
 structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects. - A
 [**backend**](#backends) defining the model to use and how to connect to it.
 Note that `spacy-llm` supports both access to external APIs (such as OpenAI) as
@@ -125,50 +143,55 @@
 functionality to avoid running the same document through an LLM service (be it
 local or through a REST API) more than once. ### Tasks A _task_ defines an NLP
 problem or question, that will be sent to the LLM via a prompt. Further, the
 task defines how to parse the LLM's responses back into structured information.
 All tasks are registered in spaCy's `llm_tasks` registry. Practically speaking,
 a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`]
 (spacy_llm/ty.py). It needs to define a `generate_prompts` function and a
-`parse_responses` function. #### function `task.generate_prompts` Takes a
-collection of documents, and returns a collection of "prompts", which can be of
-type `Any`. Often, prompts are of type `str` - but this is not enforced to
-allow for maximum flexibility in the framework. | Argument | Type | Description
-| | ----------- | --------------- | ---------------------- | | `docs` |
-`Iterable[Doc]` | The input documents. | | **RETURNS** | `Iterable[Any]` | The
-generated prompts. | #### function `task.parse_responses` Takes a collection of
-LLM responses and the original documents, parses the responses into structured
-information, and sets the annotations on the documents. The `parse_responses`
-function is free to set the annotations in any way, including `Doc` fields like
-`ents`, `spans` or `cats`, or using custom defined fields. The `responses` are
-of type `Iterable[Any]`, though they will often be `str` objects. This depends
-on the return type of the [backend](#backends). | Argument | Type | Description
-| | ----------- | --------------- | ------------------------ | | `docs` |
-`Iterable[Doc]` | The input documents. | | `responses` | `Iterable[Any]` | The
-generated prompts. | | **RETURNS** | `Iterable[Doc]` | The annotated documents.
-| #### spacy.NER.v2 The built-in NER task supports both zero-shot and few-shot
-prompting. This version also supports explicitly defining the provided labels
-with custom descriptions. ```ini [components.llm.task] @llm_tasks =
-"spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION examples = null ``` |
-Argument | Type | Default | Description | | ------------------------- | -------
--------------------------------- | --------------------------------------------
------------- | ----------------------------------------------------------------
+`parse_responses` function. Moreover, the task may define an optional [`scorer`
+method](https://spacy.io/api/scorer#score). It should accept an iterable of
+`Example`s as input and return a score dictionary. If the `scorer` method is
+defined, `spacy-llm` will call it to evaluate the component. #### function
+`task.generate_prompts` Takes a collection of documents, and returns a
+collection of "prompts", which can be of type `Any`. Often, prompts are of type
+`str` - but this is not enforced to allow for maximum flexibility in the
+framework. | Argument | Type | Description | | ----------- | --------------- |
+---------------------- | | `docs` | `Iterable[Doc]` | The input documents. | |
+**RETURNS** | `Iterable[Any]` | The generated prompts. | #### function
+`task.parse_responses` Takes a collection of LLM responses and the original
+documents, parses the responses into structured information, and sets the
+annotations on the documents. The `parse_responses` function is free to set the
+annotations in any way, including `Doc` fields like `ents`, `spans` or `cats`,
+or using custom defined fields. The `responses` are of type `Iterable[Any]`,
+though they will often be `str` objects. This depends on the return type of the
+[backend](#backends). | Argument | Type | Description | | ----------- | -------
+-------- | ------------------------ | | `docs` | `Iterable[Doc]` | The input
+documents. | | `responses` | `Iterable[Any]` | The generated prompts. | |
+**RETURNS** | `Iterable[Doc]` | The annotated documents. | #### spacy.NER.v2
+The built-in NER task supports both zero-shot and few-shot prompting. This
+version also supports explicitly defining the provided labels with custom
+descriptions. ```ini [components.llm.task] @llm_tasks = "spacy.NER.v2" labels =
+["PERSON", "ORGANISATION", "LOCATION"] examples = null ``` | Argument | Type |
+Default | Description | | ------------------------- | -------------------------
+-------------- | -------------------------------------------------------- | ---
 -------------------------------------------------------------------------------
------- | | `labels` | `str` | | Comma-separated list of labels. | | `template`
-| `str` | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom
-prompt template to send to LLM backend. Default templates for each task are
-located in the `spacy_llm/tasks/templates` directory. | | `label_definitions` |
-`Optional[Dict[str, str]]` | `None` | Optional dict mapping a label to a
-description of that label. These descriptions are added to the prompt to help
-instruct the LLM on what to extract. | | `examples` | `Optional[Callable[[],
-Iterable[Any]]]` | `None` | Optional function that generates examples for few-
-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None` |
-Function that normalizes the labels as returned by the LLM. If `None`, defaults
-to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"`
-| Alignment mode in case the LLM returns entities that do not align with token
+------------------------------------------------------------------- | |
+`labels` | `Union[List[str], str]` | | List of labels or str of comma-separated
+list of labels. | | `template` | `str` | [ner.v2.jinja](./spacy_llm/tasks/
+templates/ner.v2.jinja) | Custom prompt template to send to LLM backend.
+Default templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `label_definitions` | `Optional[Dict[str, str]]` | `None` |
+Optional dict mapping a label to a description of that label. These
+descriptions are added to the prompt to help instruct the LLM on what to
+extract. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
+Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, defaults to
+`spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
+Alignment mode in case the LLM returns entities that do not align with token
 boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
 `case_sensitive_matching` | `bool` | `False` | Whether to search without case
 sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
 in the LLM's response only once (the first hit) or multiple times. | The NER
 task implementation doesn't currently ask the LLM for specific offsets, but
 simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured
@@ -217,16 +240,15 @@
 [[str], str]]` | `None` | Function that normalizes the labels as returned by
 the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`. | |
 `alignment_mode` | `str` | `"contract"` | Alignment mode in case the LLM
 returns entities that do not align with token boundaries. Options are
 `"strict"`, `"contract"` or `"expand"`. | | `case_sensitive_matching` | `bool`
 | `False` | Whether to search without case sensitivity. | | `single_match` |
 `bool` | `False` | Whether to match an entity in the LLM's response only once
-(the first hit) or multiple times. | [ner]: https://github.com/explosion/spacy-
-llm/blob/main/spacy_llm/tasks/ner.py#L14 The NER task implementation doesn't
+(the first hit) or multiple times. | The NER task implementation doesn't
 currently ask the LLM for specific offsets, but simply expects a list of
 strings that represent the enties in the document. This means that a form of
 string matching is required. This can be configured by the following
 parameters: - The `single_match` parameter is typically set to `False` to allow
 for multiple matches. For instance, the response from the LLM might only
 mention the entity "Paris" once, but you'd still want to mark it every time it
 occurs in the document. - The case-sensitive matching is typically set to
@@ -244,148 +266,150 @@
 ```yaml - text: Jack and Jill went up the hill. entities: PERSON: - Jack - Jill
 LOCATION: - hill - text: Jack fell down and broke his crown. entities: PERSON:
 - Jack ``` ```ini [components.llm.task] @llm_tasks = "spacy.NER.v1" labels =
 PERSON,ORGANISATION,LOCATION [components.llm.task.examples] @misc =
 "spacy.FewShotReader.v1" path = "ner_examples.yml" ``` #### spacy.SpanCat.v2
 The built-in SpanCat task is a simple adaptation of the NER task to support
 overlapping entities and store its annotations in `doc.spans`. ```ini
-[components.llm.task] @llm_tasks = "spacy.SpanCat.v2" labels =
-PERSON,ORGANISATION,LOCATION examples = null ``` | Argument | Type | Default |
+[components.llm.task] @llm_tasks = "spacy.SpanCat.v2" labels = ["PERSON",
+"ORGANISATION", "LOCATION"] examples = null ``` | Argument | Type | Default |
 Description | | ------------------------- | -----------------------------------
 ---- | ------------------------------------------------------------------ | ---
 -------------------------------------------------------------------------------
 ------------------------------------------------------------------- | |
-`labels` | `str` | | Comma-separated list of labels. | | `template` | `str` |
-[`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom
-prompt template to send to LLM backend. Default templates for each task are
-located in the `spacy_llm/tasks/templates` directory. | | `label_definitions` |
-`Optional[Dict[str, str]]` | `None` | Optional dict mapping a label to a
-description of that label. These descriptions are added to the prompt to help
-instruct the LLM on what to extract. | | `spans_key` | `str` | `"sc"` | Key of
-the `Doc.spans` dict to save the spans under. | | `examples` | `Optional
-[Callable[[], Iterable[Any]]]` | `None` | Optional function that generates
-examples for few-shot learning. | | `normalizer` | `Optional[Callable[[str],
-str]]` | `None` | Function that normalizes the labels as returned by the LLM.
-If `None`, defaults to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` |
-`str` | `"contract"` | Alignment mode in case the LLM returns entities that do
-not align with token boundaries. Options are `"strict"`, `"contract"` or
-`"expand"`. | | `case_sensitive_matching` | `bool` | `False` | Whether to
-search without case sensitivity. | | `single_match` | `bool` | `False` |
-Whether to match an entity in the LLM's response only once (the first hit) or
-multiple times. | Except for the `spans_key` parameter, the SpanCat task reuses
-the configuration from the NER task. Refer to [its documentation](#spacynerv2)
-for more insight. #### spacy.SpanCat.v1 The original version of the built-in
-SpanCat task is a simple adaptation of the v1 NER task to support overlapping
-entities and store its annotations in `doc.spans`. ```ini [components.llm.task]
-@llm_tasks = "spacy.SpanCat.v1" labels = PERSON,ORGANISATION,LOCATION examples
-= null ``` | Argument | Type | Default | Description | | ----------------------
---- | --------------------------------------- | ------------ | ----------------
+`labels` | `Union[List[str], str]` | | List of labels or str of comma-separated
+list of labels. | | `template` | `str` | [`spancat.v2.jinja`](./spacy_llm/
+tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM
+backend. Default templates for each task are located in the `spacy_llm/tasks/
+templates` directory. | | `label_definitions` | `Optional[Dict[str, str]]` |
+`None` | Optional dict mapping a label to a description of that label. These
+descriptions are added to the prompt to help instruct the LLM on what to
+extract. | | `spans_key` | `str` | `"sc"` | Key of the `Doc.spans` dict to save
+the spans under. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` |
+`None` | Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, defaults to
+`spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
+Alignment mode in case the LLM returns entities that do not align with token
+boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
+`case_sensitive_matching` | `bool` | `False` | Whether to search without case
+sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
+in the LLM's response only once (the first hit) or multiple times. | Except for
+the `spans_key` parameter, the SpanCat task reuses the configuration from the
+NER task. Refer to [its documentation](#spacynerv2) for more insight. ####
+spacy.SpanCat.v1 The original version of the built-in SpanCat task is a simple
+adaptation of the v1 NER task to support overlapping entities and store its
+annotations in `doc.spans`. ```ini [components.llm.task] @llm_tasks =
+"spacy.SpanCat.v1" labels = PERSON,ORGANISATION,LOCATION examples = null ``` |
+Argument | Type | Default | Description | | ------------------------- | -------
+-------------------------------- | ------------ | -----------------------------
 -------------------------------------------------------------------------------
---------------------------------------------- | | `labels` | `str` | | Comma-
-separated list of labels. | | `spans_key` | `str` | `"sc"` | Key of the
-`Doc.spans` dict to save the spans under. | | `examples` | `Optional[Callable[
-[], Iterable[Any]]]` | `None` | Optional function that generates examples for
-few-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None`
-| Function that normalizes the labels as returned by the LLM. If `None`,
-defaults to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` |
-`"contract"` | Alignment mode in case the LLM returns entities that do not
-align with token boundaries. Options are `"strict"`, `"contract"` or
-`"expand"`. | | `case_sensitive_matching` | `bool` | `False` | Whether to
-search without case sensitivity. | | `single_match` | `bool` | `False` |
-Whether to match an entity in the LLM's response only once (the first hit) or
-multiple times. | Except for the `spans_key` parameter, the SpanCat task reuses
-the configuration from the NER task. Refer to [its documentation](#spacynerv1)
-for more insight. #### spacy.TextCat.v2 The built-in TextCat task supports both
-zero-shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks =
-"spacy.TextCat.v2" labels = COMPLIMENT,INSULT examples = null ``` | Argument |
-Type | Default | Description | | ------------------- | ------------------------
---------------- | -----------------------------------------------------------
-- | ---------------------------------------------------------------------------
---------------------------------------------------------------------- | |
-`labels` | `str` | | Comma-separated list of labels. | | `template` | `str` |
-[`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt
-template to send to LLM backend. Default templates for each task are located in
-the `spacy_llm/tasks/templates` directory. | | `examples` | `Optional[Callable[
-[], Iterable[Any]]]` | `None` | Optional function that generates examples for
-few-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None`
-| Function that normalizes the labels as returned by the LLM. If `None`, falls
-back to `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` |
-`False` | If set to `True`, only one label per document should be valid. If set
-to `False`, one document can have multiple labels. | | `allow_none` | `bool` |
-`True` | When set to `True`, allows the LLM to not return any of the given
-label. The resulting dict in `doc.cats` will have `0.0` scores for all labels.
-| | `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
-when the LLM returns invalid responses. | To perform few-shot learning, you can
-write down a few examples in a separate file, and provide these to be injected
-into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
-supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
-great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
-"answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
-"spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.task.examples]
-@misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
-spacy.TextCat.v1 The original version of the built-in TextCat task supports
-both zero-shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks
-= "spacy.TextCat.v1" labels = COMPLIMENT,INSULT examples = null ``` | Argument
-| Type | Default | Description | | ------------------- | ----------------------
------------------ | ------- | -------------------------------------------------
+-------------------------------- | | `labels` | `str` | | Comma-separated list
+of labels. | | `spans_key` | `str` | `"sc"` | Key of the `Doc.spans` dict to
+save the spans under. | | `examples` | `Optional[Callable[[], Iterable[Any]]]`
+| `None` | Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, defaults to
+`spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
+Alignment mode in case the LLM returns entities that do not align with token
+boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
+`case_sensitive_matching` | `bool` | `False` | Whether to search without case
+sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
+in the LLM's response only once (the first hit) or multiple times. | Except for
+the `spans_key` parameter, the SpanCat task reuses the configuration from the
+NER task. Refer to [its documentation](#spacynerv1) for more insight. ####
+spacy.TextCat.v2 The built-in TextCat task supports both zero-shot and few-shot
+prompting. ```ini [components.llm.task] @llm_tasks = "spacy.TextCat.v2" labels
+= ["COMPLIMENT", "INSULT"] examples = null ``` | Argument | Type | Default |
+Description | | ------------------- | --------------------------------------- |
+------------------------------------------------------------ | ----------------
 -------------------------------------------------------------------------------
----------------- | | `labels` | str | | Comma-separated list of labels. | |
-`examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` | Optional
-function that generates examples for few-shot learning. | | `normalizer` |
-`Optional[Callable[[str], str]]` | `None` | Function that normalizes the labels
-as returned by the LLM. If `None`, falls back to
+------------------------------------------------- | | `labels` | `Union[List
+[str], str]` | | List of labels or str of comma-separated list of labels. | |
+`template` | `str` | [`textcat.jinja`](./spacy_llm/tasks/templates/
+textcat.jinja) | Custom prompt template to send to LLM backend. Default
+templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
+Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, falls back to
 `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` | `False` | If
 set to `True`, only one label per document should be valid. If set to `False`,
 one document can have multiple labels. | | `allow_none` | `bool` | `True` |
 When set to `True`, allows the LLM to not return any of the given label. The
 resulting dict in `doc.cats` will have `0.0` scores for all labels. | |
 `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
 when the LLM returns invalid responses. | To perform few-shot learning, you can
 write down a few examples in a separate file, and provide these to be injected
 into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
 supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
 great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
 "answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
+"spacy.TextCat.v2" labels = ["COMPLIMENT", "INSULT"]
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"textcat_examples.json" ``` #### spacy.TextCat.v1 The original version of the
+built-in TextCat task supports both zero-shot and few-shot prompting. ```ini
+[components.llm.task] @llm_tasks = "spacy.TextCat.v1" labels =
+COMPLIMENT,INSULT examples = null ``` | Argument | Type | Default | Description
+| | ------------------- | --------------------------------------- | ------- | -
+-------------------------------------------------------------------------------
+---------------------------------------------------------------- | | `labels` |
+str | | Comma-separated list of labels. | | `examples` | `Optional[Callable[[],
+Iterable[Any]]]` | `None` | Optional function that generates examples for few-
+shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None` |
+Function that normalizes the labels as returned by the LLM. If `None`, falls
+back to `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` |
+`False` | If set to `True`, only one label per document should be valid. If set
+to `False`, one document can have multiple labels. | | `allow_none` | `bool` |
+`True` | When set to `True`, allows the LLM to not return any of the given
+label. The resulting dict in `doc.cats` will have `0.0` scores for all labels.
+| | `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
+when the LLM returns invalid responses. | To perform few-shot learning, you can
+write down a few examples in a separate file, and provide these to be injected
+into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
+supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
+great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
+"answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
 "spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
 spacy.REL.v1 The built-in REL task supports both zero-shot and few-shot
 prompting. It relies on an upstream NER component for entities extraction.
-```ini [components.llm.task] @llm_tasks = "spacy.REL.v1" labels =
-LivesIn,Visits ``` | Argument | Type | Default | Description | | --------------
------ | --------------------------------------- | -----------------------------
------------------------ | -----------------------------------------------------
--------------------------------------------------------------------------------
----- | | `labels` | `str` | | Comma-separated list of relation labels. | |
-`template` | `str` | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) |
-Custom prompt template to send to LLM backend. Default templates for each task
-are located in the `spacy_llm/tasks/templates` directory. | |
-`label_description` | `Optional[Dict[str, str]]` | `None` | Dictionary
-providing a description for each relation label. | | `examples` | `Optional
-[Callable[[], Iterable[Any]]]` | `None` | Optional function that generates
-examples for few-shot learning. | | `normalizer` | `Optional[Callable[[str],
-str]]` | `None` | Function that normalizes the labels as returned by the LLM.
-If `None`, falls back to `spacy.LowercaseNormalizer.v1`. | | `verbose` | `bool`
-| `False` | If set to `True`, warnings will be generated when the LLM returns
-invalid responses. | To perform few-shot learning, you can write down a few
-examples in a separate file, and provide these to be injected into the prompt
-to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
+```ini [components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
+"Visits"] ``` | Argument | Type | Default | Description | | ------------------
+- | --------------------------------------- | ---------------------------------
+------------------- | ---------------------------------------------------------
+------------------------------------------------------------------------------
+- | | `labels` | `Union[List[str], str]` | | List of labels or str of comma-
+separated list of labels. | | `template` | `str` | [`rel.jinja`](./spacy_llm/
+tasks/templates/rel.jinja) | Custom prompt template to send to LLM backend.
+Default templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `label_description` | `Optional[Dict[str, str]]` | `None` |
+Dictionary providing a description for each relation label. | | `examples` |
+`Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
+generates examples for few-shot learning. | | `normalizer` | `Optional[Callable
+[[str], str]]` | `None` | Function that normalizes the labels as returned by
+the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`. | | `verbose`
+| `bool` | `False` | If set to `True`, warnings will be generated when the LLM
+returns invalid responses. | To perform few-shot learning, you can write down a
+few examples in a separate file, and provide these to be injected into the
+prompt to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
 `.yaml`, `.json` and `.jsonl`. ```json {"text": "Laura bought a house in Boston
 with her husband Mark.", "ents": [{"start_char": 0, "end_char": 5, "label":
 "PERSON"}, {"start_char": 24, "end_char": 30, "label": "GPE"}, {"start_char":
 48, "end_char": 52, "label": "PERSON"}], "relations": [{"dep": 0, "dest": 1,
 "relation": "LivesIn"}, {"dep": 2, "dest": 1, "relation": "LivesIn"}]} {"text":
 "Michael travelled through South America by bike.", "ents": [{"start_char": 0,
 "end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label":
 "LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]} ``` Note:
 the REL task relies on pre-extracted entities to make its prediction. Hence,
 you'll need to add a component that populates `doc.ents` with recognized spans
 to your spaCy pipeline and put it _before_ the REL component. ```ini
-[components.llm.task] @llm_tasks = "spacy.REL.v1" labels = LivesIn,Visits
-[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
-"rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
+[components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
+"Visits"] [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path
+= "rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
 testing - it tells the LLM to do nothing, and does not set any fields on the
 `docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
 Backends A _backend_ defines which LLM model to query, and how to query it. It
 can be a simple function taking a collection of prompts (consistent with the
 output type of `task.generate_prompts()`) and returning a collection of
 responses (consistent with the expected input of `parse_responses`). Generally
 speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
```

### Comparing `spacy-llm-0.2.0/pyproject.toml` & `spacy-llm-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -17,7 +17,11 @@
     "ignore:^.*pkg_resources.*:DeprecationWarning",
     "ignore:.*function is now available as sqlalchemy.orm.declarative_base().*:",
     "ignore:^.*You are trying to use a chat model. This way of initializing it is no longer supported. Instead, please use.*:UserWarning",
 ]
 markers = [
     "external: interacts with a (potentially cost-incurring) third-party API"
 ]
+
+[tool.isort]
+multi_line_output = 9
+profile = "black"
```

### Comparing `spacy-llm-0.2.0/setup.cfg` & `spacy-llm-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.2.0
+version = 0.2.1
 description = Integrating LLMs into structured NLP pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `spacy-llm-0.2.0/spacy_llm/backends/integration/base.py` & `spacy-llm-0.2.1/spacy_llm/backends/integration/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/backends/integration/dolly.py` & `spacy-llm-0.2.1/spacy_llm/backends/integration/dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/backends/integration/langchain.py` & `spacy-llm-0.2.1/spacy_llm/backends/integration/langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/backends/integration/minichain.py` & `spacy-llm-0.2.1/spacy_llm/backends/integration/minichain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/backends/rest/backend/base.py` & `spacy-llm-0.2.1/spacy_llm/backends/rest/backend/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/backends/rest/backend/noop.py` & `spacy-llm-0.2.1/spacy_llm/backends/rest/backend/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/backends/rest/backend/openai.py` & `spacy-llm-0.2.1/spacy_llm/backends/rest/backend/openai.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/backends/rest/registry.py` & `spacy-llm-0.2.1/spacy_llm/backends/rest/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/cache.py` & `spacy-llm-0.2.1/spacy_llm/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,17 @@
         # Container for currently loaded batch of Docs (batch hash -> doc hash -> Doc).
         self._loaded_docs: Dict[int, Dict[int, Doc]] = {}
         # Queue for processed, not yet persisted docs.
         self._cache_queue: List[Doc] = []
         # Statistics.
         self._stats: Dict[str, int] = {
             "hit": 0,
+            "hit_contains": 0,
             "missed": 0,
+            "missed_contains": 0,
             "added": 0,
             "persisted": 0,
         }
 
         self._init_cache_index()
 
     @property
@@ -163,17 +165,17 @@
 
     def __contains__(self, doc: Doc) -> bool:
         """Checks whether doc has been processed and cached.
         doc (Doc): Doc to check for.
         RETURNS (bool): Whether doc has been processed and cached.
         """
         if self._doc_id(doc) not in self._doc2batch:
-            self._stats["missed"] += 1
+            self._stats["missed_contains"] += 1
             return False
-        self._stats["hit"] += 1
+        self._stats["hit_contains"] += 1
         return True
 
     def __getitem__(self, doc: Doc) -> Optional[Doc]:
         """Returns processed doc, if available in cache. Note that if doc is not in the set of currently loaded
         documents, its batch will be loaded (and an older batch potentially discarded from memory).
         If doc is not in cache, None is returned.
         doc (Doc): Unprocessed doc whose processed equivalent should be returned.
```

### Comparing `spacy-llm-0.2.0/spacy_llm/compat.py` & `spacy-llm-0.2.1/spacy_llm/compat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/pipeline/llm.py` & `spacy-llm-0.2.1/spacy_llm/pipeline/llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
-from typing import Iterable, Iterator, Optional, Tuple, cast
+from typing import Dict, Iterable, Iterator, List, Optional, Tuple, Union, cast
 
 import spacy
 from spacy.language import Language
 from spacy.pipeline import Pipe
 from spacy.tokens import Doc
+from spacy.training import Example
 from spacy.vocab import Vocab
 
 from .. import registry  # noqa: F401
-from ..ty import Cache
 from ..compat import TypedDict
-from ..ty import LLMTask, PromptExecutor, validate_types
+from ..ty import Cache, LLMTask, PromptExecutor, validate_types
 
 
 class CacheConfigType(TypedDict):
     path: Optional[Path]
     batch_size: int
     max_batches_in_mem: int
 
@@ -103,57 +103,71 @@
 
     def __call__(self, doc: Doc) -> Doc:
         """Apply the LLM wrapper to a Doc instance.
 
         doc (Doc): The Doc instance to process.
         RETURNS (Doc): The processed Doc.
         """
-        docs = [self._cache[doc]]
-        if docs[0] is None:
-            prompts = self._task.generate_prompts([doc])
-            responses = self._backend(prompts)
-            docs = list(self._task.parse_responses([doc], responses))
-            assert len(docs) == 1
-            assert isinstance(docs[0], Doc)
-            self._cache.add(docs[0])
-
+        docs = self._process_docs([doc])
         assert isinstance(docs[0], Doc)
         return docs[0]
 
+    def score(
+        self, examples: Iterable[Example], **kwargs
+    ) -> Dict[str, Union[float, Dict[str, float]]]:
+        """Score a batch of examples.
+
+        examples (Iterable[Example]): The examples to score.
+        RETURNS (Dict[str, Any]): The scores.
+
+        DOCS: https://spacy.io/api/pipe#score
+        """
+        if hasattr(self._task, "scorer") and self._task.scorer is not None:
+            return self._task.scorer(examples)
+        return {}
+
     def pipe(self, stream: Iterable[Doc], *, batch_size: int = 128) -> Iterator[Doc]:
         """Apply the LLM prompt to a stream of documents.
 
         stream (Iterable[Doc]): A stream of documents.
         batch_size (int): The number of documents to buffer.
         YIELDS (Doc): Processed documents in order.
         """
         error_handler = self.get_error_handler()
         for doc_batch in spacy.util.minibatch(stream, batch_size):
-            is_cached = [doc in self._cache for doc in doc_batch]
-            noncached_doc_batch = [
-                doc for doc, cached_doc in zip(doc_batch, is_cached) if not cached_doc
-            ]
             try:
-                prompts = self._task.generate_prompts(noncached_doc_batch)
-                responses = self._backend(prompts)
-                modified_docs = iter(
-                    self._task.parse_responses(noncached_doc_batch, responses)
-                )
-                for doc, cached_doc in zip(doc_batch, is_cached):
-                    if cached_doc:
-                        doc = self._cache[doc]
-                        assert isinstance(doc, Doc)
-                        yield doc
-                    else:
-                        doc = next(modified_docs)
-                        self._cache.add(doc)
-                        yield doc
+                yield from iter(self._process_docs(doc_batch))
             except Exception as e:
                 error_handler(self._name, self, doc_batch, e)
 
+    def _process_docs(self, docs: List[Doc]) -> List[Doc]:
+        """Process a batch of docs with the configured LLM backend and task.
+        If a cache is configured, only sends prompts to backend for docs not found in cache.
+
+        docs (List[Doc]): Input batch of docs
+        RETURNS (List[Doc]): Processed batch of docs with task annotations set
+        """
+        is_cached = [doc in self._cache for doc in docs]
+        noncached_doc_batch = [doc for i, doc in enumerate(docs) if not is_cached[i]]
+        prompts = self._task.generate_prompts(noncached_doc_batch)
+        responses = self._backend(prompts)
+        modified_docs = iter(self._task.parse_responses(noncached_doc_batch, responses))
+        final_docs = []
+        for i, doc in enumerate(docs):
+            if is_cached[i]:
+                cached_doc = self._cache[doc]
+                assert cached_doc is not None
+                final_docs.append(cached_doc)
+            else:
+                doc = next(modified_docs)
+                self._cache.add(doc)
+                final_docs.append(doc)
+
+        return final_docs
+
     def to_bytes(self, *, exclude: Tuple[str] = cast(Tuple[str], tuple())) -> bytes:
         """Serialize the LLMWrapper to a bytestring.
 
         exclude (Tuple): Names of properties to exclude from serialization.
         RETURNS (bytes): The serialized object.
         """
         return b""
```

### Comparing `spacy-llm-0.2.0/spacy_llm/registry/normalizer.py` & `spacy-llm-0.2.1/spacy_llm/registry/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/registry/reader.py` & `spacy-llm-0.2.1/spacy_llm/registry/reader.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/__init__.py` & `spacy-llm-0.2.1/spacy_llm/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/ner.py` & `spacy-llm-0.2.1/spacy_llm/tasks/ner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Callable, Dict, Iterable, List, Optional
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
+from spacy.scorer import get_ner_prf
 from spacy.tokens import Doc, Span
+from spacy.training import Example
 from spacy.util import filter_spans
 
-from .templates import read_template
-from .util import SpanTask, SpanExample
 from ..compat import Literal
 from ..registry import registry
 from ..ty import ExamplesConfigType
 from ..util import split_labels
-
+from .templates import read_template
+from .util import SpanExample, SpanTask
 
 _DEFAULT_NER_TEMPLATE_V1 = read_template("ner")
 _DEFAULT_NER_TEMPLATE_V2 = read_template("ner.v2")
 
 
 @registry.llm_tasks("spacy.NER.v1")
 def make_ner_task(
@@ -37,15 +38,15 @@
         case_sensitive_matching=case_sensitive_matching,
         single_match=single_match,
     )
 
 
 @registry.llm_tasks("spacy.NER.v2")
 def make_ner_task_v2(
-    labels: str,
+    labels: Union[List[str], str],
     template: str = _DEFAULT_NER_TEMPLATE_V2,
     label_definitions: Optional[Dict[str, str]] = None,
     examples: ExamplesConfigType = None,
     normalizer: Optional[Callable[[str], str]] = None,
     alignment_mode: Literal["strict", "contract", "expand"] = "contract",  # noqa: F821
     case_sensitive_matching: bool = False,
     single_match: bool = False,
@@ -110,7 +111,13 @@
     def assign_spans(
         self,
         doc: Doc,
         spans: List[Span],
     ) -> None:
         """Assign spans to the document."""
         doc.set_ents(filter_spans(spans))
+
+    def scorer(
+        self,
+        examples: Iterable[Example],
+    ) -> Dict[str, Any]:
+        return get_ner_prf(examples)
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/rel.py` & `spacy-llm-0.2.1/spacy_llm/tasks/rel.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 
 _DEFAULT_REL_TEMPLATE = read_template("rel")
 
 
 @registry.llm_tasks("spacy.REL.v1")
 def make_rel_task(
-    labels: str,
+    labels: Union[List[str], str],
     template: str = _DEFAULT_REL_TEMPLATE,
     label_definitions: Optional[Dict[str, str]] = None,
     examples: ExamplesConfigType = None,
     normalizer: Optional[Callable[[str], str]] = None,
     verbose: bool = False,
 ) -> "RELTask":
     labels_list = split_labels(labels)
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/spancat.py` & `spacy-llm-0.2.1/spacy_llm/tasks/spancat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Any, Callable, Dict, Iterable, List, Optional
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
+from spacy.pipeline.spancat import spancat_score
 from spacy.tokens import Doc, Span
+from spacy.training import Example
 
 from ..compat import Literal
 from ..registry import registry
 from ..ty import ExamplesConfigType
 from ..util import split_labels
 from .templates import read_template
-from .util import SpanTask, SpanExample
-
+from .util import SpanExample, SpanTask
 
 _DEFAULT_SPANCAT_TEMPLATE_V1 = read_template("spancat")
 _DEFAULT_SPANCAT_TEMPLATE_V2 = read_template("spancat.v2")
 
 
 @registry.llm_tasks("spacy.SpanCat.v1")
 def make_spancat_task(
@@ -36,15 +37,15 @@
         case_sensitive_matching=case_sensitive_matching,
         single_match=single_match,
     )
 
 
 @registry.llm_tasks("spacy.SpanCat.v2")
 def make_spancat_task_v2(
-    labels: str,
+    labels: Union[List[str], str],
     template: str = _DEFAULT_SPANCAT_TEMPLATE_V2,
     label_definitions: Optional[Dict[str, str]] = None,
     examples: ExamplesConfigType = None,
     normalizer: Optional[Callable[[str], str]] = None,
     alignment_mode: Literal["strict", "contract", "expand"] = "contract",  # noqa: F821
     case_sensitive_matching: bool = False,
     single_match: bool = False,
@@ -107,7 +108,17 @@
     def assign_spans(
         self,
         doc: Doc,
         spans: List[Span],
     ) -> None:
         """Assign spans to the document."""
         doc.spans[self._spans_key] = sorted(spans)  # type: ignore [type-var]
+
+    def scorer(
+        self,
+        examples: Iterable[Example],
+    ) -> Dict[str, Any]:
+        return spancat_score(
+            examples,
+            spans_key=self._spans_key,
+            allow_overlap=True,
+        )
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/templates/ner.jinja` & `spacy-llm-0.2.1/spacy_llm/tasks/templates/ner.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/templates/ner.v2.jinja` & `spacy-llm-0.2.1/spacy_llm/tasks/templates/ner.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/templates/rel.jinja` & `spacy-llm-0.2.1/spacy_llm/tasks/templates/rel.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/templates/spancat.jinja` & `spacy-llm-0.2.1/spacy_llm/tasks/templates/spancat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/templates/spancat.v2.jinja` & `spacy-llm-0.2.1/spacy_llm/tasks/templates/spancat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/templates/textcat.jinja` & `spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.v2.jinja`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+You are an expert Text Classification system. Your task is to accept Text as input
+and provide a category for the text based on the predefined labels.
+{# whitespace #}
+{# whitespace #}
 {%- if labels|length == 1 -%}
 {%- set label = labels[0] -%}
 Classify whether the text below belongs to the {{ label }} category or not.
 If it is a {{ label }}, answer `POS`. If it is not a {{ label }}, answer `NEG`.
+Do not put any other text in your answer, only one of 'POS' or 'NEG' with nothing before or after.
 {%- else -%}
 Classify the text below to any of the following labels: {{ labels|join(", ") }}
 {# whitespace #}
 {%- if exclusive_classes -%}
 The task is exclusive, so only choose one label from what I provided.
+Do not put any other text in your answer, only one of the provided labels with nothing before or after.
 {%- else -%}
 The task is non-exclusive, so you can provide more than one label as long as
 they're comma-delimited. For example: Label1, Label2, Label3.
+Do not put any other text in your answer, only one or more of the provided labels with nothing before or after.
 {%- if allow_none -%}
 {# whitespace #}
 If the text cannot be classified into any of the provided labels, answer `==NONE==`.
 {%- endif -%}
 {%- endif -%}
 {# whitespace #}
 {%- endif -%}
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/templates/textcat.v2.jinja` & `spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.v3.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 {%- set label = labels[0] -%}
 Classify whether the text below belongs to the {{ label }} category or not.
 If it is a {{ label }}, answer `POS`. If it is not a {{ label }}, answer `NEG`.
 Do not put any other text in your answer, only one of 'POS' or 'NEG' with nothing before or after.
 {%- else -%}
 Classify the text below to any of the following labels: {{ labels|join(", ") }}
 {# whitespace #}
+{# whitespace #}
 {%- if exclusive_classes -%}
 The task is exclusive, so only choose one label from what I provided.
 Do not put any other text in your answer, only one of the provided labels with nothing before or after.
 {%- else -%}
 The task is non-exclusive, so you can provide more than one label as long as
 they're comma-delimited. For example: Label1, Label2, Label3.
 Do not put any other text in your answer, only one or more of the provided labels with nothing before or after.
@@ -21,14 +22,28 @@
 {# whitespace #}
 If the text cannot be classified into any of the provided labels, answer `==NONE==`.
 {%- endif -%}
 {%- endif -%}
 {# whitespace #}
 {%- endif -%}
 {# whitespace #}
+{%- if label_definitions -%}
+{# whitespace #}
+{# whitespace #}
+Below are definitions of each label to help aid you in correctly classifying the text.
+Assume these definitions are written by an expert and follow them closely.
+{# whitespace #}
+{# whitespace #}
+{%- for label, definition in label_definitions.items() -%}
+{{ label }}: {{ definition }}
+{# whitespace #}
+{%- endfor -%}
+{# whitespace #}
+{%- endif -%}
+{# whitespace #}
 {%- if examples -%}
 {# whitespace #}
 Below are some examples (only use these as a guide):
 {# whitespace #}
 {# whitespace #}
 {%- for example in examples -%}
 {# whitespace #}
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/textcat.py` & `spacy-llm-0.2.1/spacy_llm/tasks/textcat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from typing import Callable, Dict, List, Iterable, Optional
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 import jinja2
 from pydantic import BaseModel
+from spacy.scorer import Scorer
 from spacy.tokens import Doc
+from spacy.training import Example
 from wasabi import msg
 
 from ..registry import lowercase_normalizer, registry
 from ..ty import ExamplesConfigType
 from ..util import split_labels
 from .templates import read_template
 
-
-_DEFAULT_TEXTCAT_TEMPLATE_v1 = read_template("textcat")
-_DEFAULT_TEXTCAT_TEMPLATE_v2 = read_template("textcat.v2")
+_DEFAULT_TEXTCAT_TEMPLATE_V1 = read_template("textcat")
+_DEFAULT_TEXTCAT_TEMPLATE_V2 = read_template("textcat.v2")
+_DEFAULT_TEXTCAT_TEMPLATE_V3 = read_template("textcat.v3")
 
 
 class TextCatExample(BaseModel):
     text: str
     answer: str
 
 
@@ -32,54 +34,83 @@
     labels_list = split_labels(labels)
     raw_examples = examples() if callable(examples) else examples
     textcat_examples = (
         [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
     )
     return TextCatTask(
         labels=labels_list,
-        template=_DEFAULT_TEXTCAT_TEMPLATE_v1,
+        template=_DEFAULT_TEXTCAT_TEMPLATE_V1,
         examples=textcat_examples,
         normalizer=normalizer,
         exclusive_classes=exclusive_classes,
         allow_none=allow_none,
         verbose=verbose,
     )
 
 
 @registry.llm_tasks("spacy.TextCat.v2")
 def make_textcat_task_v2(
-    labels: str,
-    template: str = _DEFAULT_TEXTCAT_TEMPLATE_v2,
+    labels: Union[List[str], str],
+    template: str = _DEFAULT_TEXTCAT_TEMPLATE_V2,
+    examples: ExamplesConfigType = None,
+    normalizer: Optional[Callable[[str], str]] = None,
+    exclusive_classes: bool = False,
+    allow_none: bool = True,
+    verbose: bool = False,
+) -> "TextCatTask":
+    labels_list = split_labels(labels)
+    raw_examples = examples() if callable(examples) else examples
+    textcat_examples = (
+        [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
+    )
+    return TextCatTask(
+        labels=labels_list,
+        template=template,
+        examples=textcat_examples,
+        normalizer=normalizer,
+        exclusive_classes=exclusive_classes,
+        allow_none=allow_none,
+        verbose=verbose,
+    )
+
+
+@registry.llm_tasks("spacy.TextCat.v3")
+def make_textcat_task_v3(
+    labels: Union[List[str], str],
+    template: str = _DEFAULT_TEXTCAT_TEMPLATE_V3,
+    label_definitions: Optional[Dict[str, str]] = None,
     examples: ExamplesConfigType = None,
     normalizer: Optional[Callable[[str], str]] = None,
     exclusive_classes: bool = False,
     allow_none: bool = True,
     verbose: bool = False,
 ) -> "TextCatTask":
     labels_list = split_labels(labels)
     raw_examples = examples() if callable(examples) else examples
     textcat_examples = (
         [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
     )
     return TextCatTask(
         labels=labels_list,
         template=template,
+        label_definitions=label_definitions,
         examples=textcat_examples,
         normalizer=normalizer,
         exclusive_classes=exclusive_classes,
         allow_none=allow_none,
         verbose=verbose,
     )
 
 
 class TextCatTask:
     def __init__(
         self,
         labels: List[str],
-        template: str = _DEFAULT_TEXTCAT_TEMPLATE_v2,
+        template: str = _DEFAULT_TEXTCAT_TEMPLATE_V3,
+        label_definitions: Optional[Dict[str, str]] = None,
         examples: Optional[List[TextCatExample]] = None,
         normalizer: Optional[Callable[[str], str]] = None,
         exclusive_classes: bool = False,
         allow_none: bool = True,
         verbose: bool = False,
     ):
         """Default TextCat task.
@@ -96,26 +127,29 @@
 
         Lastly, you can toggle between exclusive or no-exclusive text
         categorization by passing a flag to the `exclusive_classes` parameter.
 
         labels (str): Comma-separated list of labels to pass to the template. This task
             assumes binary classification if a single label is provided.
         template (str): Prompt template passed to the model.
+        label_definitions (Optional[Dict[str, str]]): Optional dict mapping a label to a description of that label.
+            These descriptions are added to the prompt to help instruct the LLM on what to extract.
         examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
             reads a file containing task examples for few-shot learning. If None is
             passed, then zero-shot learning will be used.
         normalizer (Optional[Callable[[str], str]]): Optional normalizer function.
         exclusive_classes (bool): If True, require the language model to suggest only one
             label per class. This is automatically set when using binary classification.
         allow_none (bool): if True, there might be cases where no label is applicable.
         verbose (bool): If True, show extra information.
         """
         self._template = template
         self._normalizer = normalizer if normalizer else lowercase_normalizer()
         self._label_dict = {self._normalizer(label): label for label in labels}
+        self._label_definitions = label_definitions
         self._examples = examples
         # Textcat configuration
         self._use_binary = True if len(self._label_dict) == 1 else False
         self._exclusive_classes = exclusive_classes
         self._allow_none = allow_none
         self._verbose = verbose
 
@@ -129,14 +163,15 @@
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
         _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
                 text=doc.text,
                 labels=list(self._label_dict.values()),
+                label_definitions=self._label_definitions,
                 examples=self._examples,
                 exclusive_classes=self._exclusive_classes,
                 allow_none=self._allow_none,
             )
             yield prompt
 
     def _format_response(self, response: str) -> Dict[str, float]:
@@ -175,7 +210,18 @@
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[str]
     ) -> Iterable[Doc]:
         for doc, prompt_response in zip(docs, responses):
             cats = self._format_response(prompt_response)
             doc.cats = cats
             yield doc
+
+    def scorer(
+        self,
+        examples: Iterable[Example],
+    ) -> Dict[str, Any]:
+        return Scorer.score_cats(
+            examples,
+            attr="cats",
+            labels=self._label_dict.values(),
+            multi_label=not self._exclusive_classes,
+        )
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/util/parsing.py` & `spacy-llm-0.2.1/spacy_llm/tasks/util/parsing.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tasks/util/span.py` & `spacy-llm-0.2.1/spacy_llm/tasks/util/span.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/backends/test_dolly.py` & `spacy-llm-0.2.1/spacy_llm/tests/backends/test_dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/backends/test_langchain.py` & `spacy-llm-0.2.1/spacy_llm/tests/backends/test_langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/backends/test_minichain.py` & `spacy-llm-0.2.1/spacy_llm/tests/backends/test_minichain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/backends/test_rest.py` & `spacy-llm-0.2.1/spacy_llm/tests/backends/test_rest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/conftest.py` & `spacy-llm-0.2.1/spacy_llm/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/pipeline/test_llm.py` & `spacy-llm-0.2.1/spacy_llm/tests/pipeline/test_llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/tasks/examples/rel_examples.jsonl` & `spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/rel_examples.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/tasks/test_ner.py` & `spacy-llm-0.2.1/spacy_llm/tests/tasks/test_ner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 from pathlib import Path
+from typing import Iterable
 
 import pytest
 import spacy
 import srsly
 from confection import Config
 from pydantic import ValidationError
+from spacy.tokens import Span
+from spacy.training import Example
 from spacy.util import make_tempdir
 
-from spacy_llm.registry import strip_normalizer, lowercase_normalizer
-from spacy_llm.registry import fewshot_reader, file_reader
+from spacy_llm.registry import (
+    fewshot_reader,
+    file_reader,
+    lowercase_normalizer,
+    registry,
+    strip_normalizer,
+)
 from spacy_llm.tasks.ner import make_ner_task_v2
 from spacy_llm.tasks.util import find_substrings
+from spacy_llm.util import assemble_from_config
+
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 TEMPLATES_DIR = Path(__file__).parent / "templates"
 
 
 @pytest.fixture
@@ -118,15 +128,15 @@
     [components]
 
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
     @llm_tasks = "spacy.NER.v2"
-    labels = PER,ORG,LOC
+    labels = ["PER", "ORG", "LOC"]
 
     [components.llm.task.examples]
     @misc = "spacy.FewShotReader.v1"
     path = {str((Path(__file__).parent / "examples" / "ner_examples.yml"))}
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
@@ -660,7 +670,39 @@
 PER
 ORG
 LOC
 
 Here is the text: Alice and Bob went to the supermarket
 """.strip()
     )
+
+
+@pytest.mark.parametrize("n_detections", [0, 1, 2])
+def test_ner_scoring(zeroshot_cfg_string, n_detections):
+    @registry.llm_backends("Dummy")
+    def factory():
+        def b(prompts: Iterable[str]) -> Iterable[str]:
+            for _ in prompts:
+                yield ("PER: Alice,Bob")
+
+        return b
+
+    config = Config().from_str(zeroshot_cfg_string)
+    config["components"]["llm"]["backend"] = {"@llm_backends": "Dummy"}
+    nlp = assemble_from_config(config)
+
+    examples = []
+
+    for text in ["Alice works with Bob.", "Bob lives with Alice."]:
+        predicted = nlp.make_doc(text)
+        reference = predicted.copy()
+
+        reference.ents = [
+            Span(reference, 0, 1, label="PER"),
+            Span(reference, 3, 4, label="PER"),
+        ][:n_detections]
+
+        examples.append(Example(predicted, reference))
+
+    scores = nlp.evaluate(examples)
+
+    assert scores["ents_p"] == n_detections / 2
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/tasks/test_rel.py` & `spacy-llm-0.2.1/spacy_llm/tests/tasks/test_rel.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     source = "en_core_web_md"
 
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
     @llm_tasks = "spacy.REL.v1"
-    labels = "LivesIn,Visits"
+    labels = ["LivesIn", "Visits"]
 
     [components.llm.task.examples]
     @misc = "spacy.FewShotReader.v1"
     path = {str(EXAMPLES_DIR / "rel_examples.jsonl")}
 
     [components.llm.backend]
     @llm_backends = "spacy.REST.v1"
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/tasks/test_spancat.py` & `spacy-llm-0.2.1/spacy_llm/tests/tasks/test_spancat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from pathlib import Path
+from typing import Iterable
 
 import pytest
 import spacy
 import srsly
 from confection import Config
 from pydantic import ValidationError
+from spacy.tokens import Span
+from spacy.training import Example
 from spacy.util import make_tempdir
 
-from spacy_llm.registry import fewshot_reader, lowercase_normalizer, strip_normalizer
+from spacy_llm.registry import (
+    fewshot_reader,
+    lowercase_normalizer,
+    registry,
+    strip_normalizer,
+)
 from spacy_llm.tasks import make_spancat_task_v2
 from spacy_llm.tasks.util import find_substrings
+from spacy_llm.util import assemble_from_config
 
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 
 
 @pytest.fixture
@@ -54,15 +63,15 @@
     [components]
 
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
     @llm_tasks = "spacy.SpanCat.v2"
-    labels = PER,ORG,LOC
+    labels = ["PER", "ORG", "LOC"]
 
     [components.llm.task.examples]
     @misc = "spacy.FewShotReader.v1"
     path = {str((Path(__file__).parent / "examples" / "ner_examples.yml"))}
 
     [components.llm.task.normalizer]
     @misc = "spacy.LowercaseNormalizer.v1"
@@ -468,7 +477,39 @@
         tmp_path = tmpdir / "wrong_example.yml"
         srsly.write_yaml(tmp_path, wrong_example)
 
         with pytest.raises(ValidationError):
             make_spancat_task_v2(
                 labels="PER,ORG,LOC", examples=fewshot_reader(tmp_path)
             )
+
+
+@pytest.mark.parametrize("n_detections", [0, 1, 2])
+def test_spancat_scoring(zeroshot_cfg_string, n_detections):
+    @registry.llm_backends("Dummy")
+    def factory():
+        def b(prompts: Iterable[str]) -> Iterable[str]:
+            for _ in prompts:
+                yield ("PER: Alice,Bob")
+
+        return b
+
+    config = Config().from_str(zeroshot_cfg_string)
+    config["components"]["llm"]["backend"] = {"@llm_backends": "Dummy"}
+    nlp = assemble_from_config(config)
+
+    examples = []
+
+    for text in ["Alice works with Bob.", "Bob lives with Alice."]:
+        predicted = nlp.make_doc(text)
+        reference = predicted.copy()
+
+        reference.spans["sc"] = [
+            Span(reference, 0, 1, label="PER"),
+            Span(reference, 3, 4, label="PER"),
+        ][:n_detections]
+
+        examples.append(Example(predicted, reference))
+
+    scores = nlp.evaluate(examples)
+
+    assert scores["spans_sc_p"] == n_detections / 2
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/tasks/test_textcat.py` & `spacy-llm-0.2.1/spacy_llm/tests/tasks/test_textcat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from pathlib import Path
+from typing import Iterable
 
 import pytest
 import spacy
 import srsly
 from confection import Config
 from pydantic import ValidationError
+from spacy.training import Example
 from spacy.util import make_tempdir
 
-from spacy_llm.registry import lowercase_normalizer
-from spacy_llm.registry import fewshot_reader, file_reader
-from spacy_llm.tasks.textcat import make_textcat_task_v2
+from spacy_llm.registry import (
+    fewshot_reader,
+    file_reader,
+    lowercase_normalizer,
+    registry,
+)
+from spacy_llm.tasks.textcat import make_textcat_task_v3
+from spacy_llm.util import assemble_from_config
 
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 TEMPLATES_DIR = Path(__file__).parent / "templates"
 
 
@@ -90,15 +97,15 @@
     [components]
 
     [components.llm]
     factory = "llm"
 
     [components.llm.task]
     @llm_tasks = "spacy.TextCat.v2"
-    labels = "Recipe"
+    labels = ["Recipe"]
     exclusive_classes = true
 
     [components.llm.task.template]
     @misc = "spacy.FileReader.v1"
     path = {str((Path(__file__).parent / "templates" / "textcat_template.jinja2"))}
 
     [components.llm.task.normalizer]
@@ -108,14 +115,45 @@
     @llm_backends = "spacy.REST.v1"
     api = "OpenAI"
     config = {{}}
     """
 
 
 @pytest.fixture
+def zeroshot_cfg_string_v3_lds():
+    return """
+    [nlp]
+    lang = "en"
+    pipeline = ["llm"]
+    batch_size = 128
+
+    [components]
+
+    [components.llm]
+    factory = "llm"
+
+    [components.llm.task]
+    @llm_tasks = "spacy.TextCat.v3"
+    labels = "Recipe"
+    exclusive_classes = true
+
+    [components.llm.task.label_definitions]
+    Recipe = "A recipe is a set of instructions for preparing a meal, including a list of the ingredients required."
+
+    [components.llm.task.normalizer]
+    @misc = "spacy.LowercaseNormalizer.v1"
+
+    [components.llm.backend]
+    @llm_backends = "spacy.REST.v1"
+    api = "OpenAI"
+    config = {}
+    """
+
+
+@pytest.fixture
 def binary():
     text = "Get 1 cup of sugar, half a cup of butter, and mix them together to make a cream"
     labels = "Recipe"
     gold_cats = ["Recipe"]
     exclusive_classes = True
     examples_path = str(EXAMPLES_DIR / "textcat_binary_examples.yml")
     return text, labels, gold_cats, exclusive_classes, examples_path
@@ -145,15 +183,20 @@
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize(
     "task",
     ["binary", "multilabel_nonexcl", "multilabel_excl"],
 )
 @pytest.mark.parametrize(
     "cfg_string",
-    ["zeroshot_cfg_string", "fewshot_cfg_string", "ext_template_cfg_string"],
+    [
+        "zeroshot_cfg_string",
+        "fewshot_cfg_string",
+        "ext_template_cfg_string",
+        "zeroshot_cfg_string_v3_lds",
+    ],
 )
 def test_textcat_config(task, cfg_string, request):
     """Simple test to check if the config loads properly given different settings"""
 
     task = request.getfixturevalue(task)
     _, labels, _, exclusive_classes, examples = task
     overrides = {
@@ -171,15 +214,20 @@
 
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize("task", ["binary", "multilabel_nonexcl", "multilabel_excl"])
 @pytest.mark.parametrize(
     "cfg_string",
-    ["zeroshot_cfg_string", "fewshot_cfg_string", "ext_template_cfg_string"],
+    [
+        "zeroshot_cfg_string",
+        "fewshot_cfg_string",
+        "ext_template_cfg_string",
+        "zeroshot_cfg_string_v3_lds",
+    ],
 )
 def test_textcat_predict(task, cfg_string, request):
     """Use OpenAI to get Textcat results.
     Note that this test may fail randomly, as the LLM's output is unguaranteed
     to be consistent/predictable.
     """
     task = request.getfixturevalue(task)
@@ -202,15 +250,20 @@
 
 
 @pytest.mark.external
 @pytest.mark.skipif(has_openai_key is False, reason="OpenAI API key not available")
 @pytest.mark.parametrize("task", ["binary", "multilabel_nonexcl", "multilabel_excl"])
 @pytest.mark.parametrize(
     "cfg_string",
-    ["zeroshot_cfg_string", "fewshot_cfg_string", "ext_template_cfg_string"],
+    [
+        "zeroshot_cfg_string",
+        "fewshot_cfg_string",
+        "ext_template_cfg_string",
+        "zeroshot_cfg_string_v3_lds",
+    ],
 )
 def test_textcat_io(task, cfg_string, request):
     task = request.getfixturevalue(task)
     text, labels, gold_cats, exclusive_classes, examples = task
     overrides = {
         "components.llm.task.labels": labels,
         "components.llm.task.exclusive_classes": exclusive_classes,
@@ -233,15 +286,15 @@
     assert len(doc.cats) >= 0  # can be 0 if binary and negative
     for cat in list(doc.cats.keys()):
         assert cat in gold_cats
 
 
 def test_textcat_sets_exclusive_classes_if_binary():
     """Test if the textcat task automatically sets exclusive classes to True if binary"""
-    llm_textcat = make_textcat_task_v2(labels="Recipe", exclusive_classes=False)
+    llm_textcat = make_textcat_task_v3(labels="Recipe", exclusive_classes=False)
     assert llm_textcat._exclusive_classes
 
 
 @pytest.mark.parametrize(
     "text,response,expected_score",
     [
         ("Some test text with positive response", "POS", 1.0),
@@ -254,15 +307,15 @@
     ],
 )
 def test_textcat_binary_labels_are_correct(text, response, expected_score):
     """Test if positive label for textcat binary is always the label name and the negative
     label is an empty dictionary
     """
     label = "Recipe"
-    llm_textcat = make_textcat_task_v2(
+    llm_textcat = make_textcat_task_v3(
         labels=label, exclusive_classes=True, normalizer=lowercase_normalizer()
     )
 
     nlp = spacy.blank("xx")
     doc = nlp(text)
     pred = list(llm_textcat.parse_responses([doc], [response]))[0]
     assert list(pred.cats.keys())[0] == label
@@ -285,15 +338,15 @@
         # fmt: on
     ],
 )
 def test_textcat_multilabel_labels_are_correct(
     text, exclusive_classes, response, expected
 ):
     labels = "Recipe,Comment,Feedback"
-    llm_textcat = make_textcat_task_v2(
+    llm_textcat = make_textcat_task_v3(
         labels=labels,
         exclusive_classes=exclusive_classes,
         normalizer=lowercase_normalizer(),
     )
     nlp = spacy.blank("xx")
     doc = nlp.make_doc(text)
     pred = list(llm_textcat.parse_responses([doc], [response]))[0]
@@ -317,15 +370,15 @@
     with annoying newlines and spaces at the edge of the text.
     """
     text, labels, _, exclusive_classes, _ = binary
     nlp = spacy.blank("xx")
     doc = nlp(text)
 
     examples = fewshot_reader(examples_path)
-    llm_textcat = make_textcat_task_v2(
+    llm_textcat = make_textcat_task_v3(
         labels=labels,
         examples=examples,
         exclusive_classes=exclusive_classes,
     )
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
@@ -383,27 +436,28 @@
     examples_path, multilabel_excl
 ):
     text, labels, _, exclusive_classes, _ = multilabel_excl
     nlp = spacy.blank("xx")
     doc = nlp(text)
 
     examples = fewshot_reader(examples_path)
-    llm_textcat = make_textcat_task_v2(
+    llm_textcat = make_textcat_task_v3(
         labels=labels,
         examples=examples,
         exclusive_classes=exclusive_classes,
     )
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == """
 You are an expert Text Classification system. Your task is to accept Text as input
 and provide a category for the text based on the predefined labels.
 
 Classify the text below to any of the following labels: Recipe, Feedback, Comment
+
 The task is exclusive, so only choose one label from what I provided.
 Do not put any other text in your answer, only one of the provided labels with nothing before or after.
 Below are some examples (only use these as a guide):
 
 
 Text:
 '''
@@ -449,27 +503,28 @@
     examples_path, multilabel_nonexcl
 ):
     text, labels, _, exclusive_classes, _ = multilabel_nonexcl
     nlp = spacy.blank("xx")
     doc = nlp(text)
 
     examples = fewshot_reader(examples_path)
-    llm_textcat = make_textcat_task_v2(
+    llm_textcat = make_textcat_task_v3(
         labels=labels,
         examples=examples,
         exclusive_classes=exclusive_classes,
     )
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == """
 You are an expert Text Classification system. Your task is to accept Text as input
 and provide a category for the text based on the predefined labels.
 
 Classify the text below to any of the following labels: Recipe, Feedback, Comment
+
 The task is non-exclusive, so you can provide more than one label as long as
 they're comma-delimited. For example: Label1, Label2, Label3.
 Do not put any other text in your answer, only one or more of the provided labels with nothing before or after.
 If the text cannot be classified into any of the provided labels, answer `==NONE==`.
 Below are some examples (only use these as a guide):
 
 
@@ -517,32 +572,138 @@
 )
 def test_example_not_following_basemodel(wrong_example, labels, exclusive_classes):
     with make_tempdir() as tmpdir:
         tmp_path = tmpdir / "wrong_example.yml"
         srsly.write_yaml(tmp_path, wrong_example)
 
         with pytest.raises(ValidationError):
-            make_textcat_task_v2(
+            make_textcat_task_v3(
                 labels=labels,
                 examples=fewshot_reader(tmp_path),
                 exclusive_classes=exclusive_classes,
             )
 
 
 def test_external_template_actually_loads():
     template_path = str(TEMPLATES_DIR / "textcat_template.jinja2")
     template = file_reader(template_path)
     labels = "Recipe"
     nlp = spacy.blank("xx")
     doc = nlp.make_doc("Combine 2 cloves of garlic with soy sauce")
 
-    llm_textcat = make_textcat_task_v2(labels=labels, template=template)
+    llm_textcat = make_textcat_task_v3(labels=labels, template=template)
     prompt = list(llm_textcat.generate_prompts([doc]))[0]
     assert (
         prompt.strip()
         == """
 This is a test textcat template. Here is/are the label/s
 Recipe
 
 Here is the text: Combine 2 cloves of garlic with soy sauce
 """.strip()
     )
+
+
+INSULTS = [
+    "Gobbledygooks!",
+    "Filibusters!",
+    "Slubberdegullions!",
+    "Vampires!",
+    "Sycophant!",
+    "Kleptomaniacs!",
+    "Egoists!",
+    "Tramps!",
+    "Monopolizers!",
+    "Pockmarks!",
+    "Belemnite!",
+    "Crooks!",
+    "Miserable earthworms!",
+    "Harlequin!",
+    "Parasites!",
+    "Macrocephalic baboon!",
+    "Brutes!",
+    "Pachyrhizus!",
+    "Toads!",
+    "Gyroscope!",
+    "Bougainvillea!",
+    "Bloodsuckers!",
+    "Nincompoop!",
+    "Shipwreckers!",
+]
+
+
+@pytest.mark.parametrize("n_insults", range(len(INSULTS) + 1))
+def test_textcat_scoring(zeroshot_cfg_string, n_insults):
+    @registry.llm_backends("Dummy")
+    def factory():
+        def b(prompts: Iterable[str]) -> Iterable[str]:
+            for _ in prompts:
+                yield "POS"
+
+        return b
+
+    config = Config().from_str(zeroshot_cfg_string)
+    config["components"]["llm"]["backend"] = {"@llm_backends": "Dummy"}
+    config["components"]["llm"]["task"]["labels"] = "Insult"
+    nlp = assemble_from_config(config)
+
+    examples = []
+
+    for i, text in enumerate(INSULTS):
+        predicted = nlp.make_doc(text)
+        reference = predicted.copy()
+
+        if i < n_insults:
+            reference.cats = {"Insult": 1.0}
+
+        examples.append(Example(predicted, reference))
+
+    scores = nlp.evaluate(examples)
+
+    pos = n_insults / len(INSULTS)
+
+    assert scores["cats_micro_p"] == pos
+    assert not n_insults or scores["cats_micro_r"] == 1
+
+
+def test_jinja_template_rendering_with_label_definitions(multilabel_excl):
+    text, labels, _, exclusive_classes, _ = multilabel_excl
+    nlp = spacy.blank("xx")
+    doc = nlp(text)
+
+    llm_textcat = make_textcat_task_v3(
+        labels=labels,
+        label_definitions={
+            "Recipe": "A Recipe is a set of instructions to make a food of some kind",
+            "Feedback": "Feedback description",
+            "Comment": "Comment description",
+        },
+        exclusive_classes=exclusive_classes,
+    )
+    prompt = list(llm_textcat.generate_prompts([doc]))[0]
+    assert (
+        prompt.strip()
+        == """
+You are an expert Text Classification system. Your task is to accept Text as input
+and provide a category for the text based on the predefined labels.
+
+Classify the text below to any of the following labels: Recipe, Feedback, Comment
+
+The task is exclusive, so only choose one label from what I provided.
+Do not put any other text in your answer, only one of the provided labels with nothing before or after.
+
+Below are definitions of each label to help aid you in correctly classifying the text.
+Assume these definitions are written by an expert and follow them closely.
+
+Recipe: A Recipe is a set of instructions to make a food of some kind
+Feedback: Feedback description
+Comment: Comment description
+
+
+Here is the text that needs classification
+
+
+Text:
+'''
+You need to increase the temperature when baking, it looks undercooked.
+'''""".strip()
+    )
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/test_cache.py` & `spacy-llm-0.2.1/spacy_llm/tests/test_cache.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,15 +50,17 @@
         index = list(srsly.read_jsonl(tmpdir / "index.jsonl"))
         index_dict: Dict[int, int] = {}
         for rec in index:
             index_dict = {**index_dict, **{int(k): int(v) for k, v in rec.items()}}
         assert len(index) == len(index_dict) == n
         cache = nlp.get_pipe("llm")._cache  # type: ignore
         assert cache._stats["hit"] == 0
-        assert cache._stats["missed"] == n
+        assert cache._stats["hit_contains"] == 0
+        assert cache._stats["missed"] == 0
+        assert cache._stats["missed_contains"] == n
         assert cache._stats["added"] == n
         assert cache._stats["persisted"] == n
         # Check whether docs are in the batch files they are supposed to be in.
         for doc in docs:
             doc_id = BatchCache._doc_id(doc)
             batch_id = index_dict[doc_id]
             batch_path = cache._batch_path(batch_id)
@@ -71,15 +73,17 @@
         # Test cache reading
         #######################################################
 
         nlp_2 = _init_nlp(tmpdir)
         [nlp_2(text) for text in texts]
         cache = nlp_2.get_pipe("llm")._cache  # type: ignore
         assert cache._stats["hit"] == n
+        assert cache._stats["hit_contains"] == n
         assert cache._stats["missed"] == 0
+        assert cache._stats["missed_contains"] == 0
         assert cache._stats["added"] == 0
         assert cache._stats["persisted"] == 0
 
 
 @pytest.mark.skip(reason="Flaky test - needs to be updated")
 def test_caching_interrupted() -> None:
     """Test pipeline with caching with simulated interruption (i. e. pipeline stops writing before entire batch is
@@ -103,29 +107,33 @@
             nlp2(texts[i])
         pass1_duration = time.time() - start
         pass1_cache = nlp2.get_pipe("llm")._cache  # type: ignore
         # Arbitrary time check to ensure that first pass through half of the doc batch takes up roughly half of the time
         # of a full pass.
         assert abs(ref_duration / 2 - pass1_duration) < ref_duration / 2 * 0.3
         assert pass1_cache._stats["hit"] == 0
+        assert pass1_cache._stats["hit"] == 0
         assert pass1_cache._stats["missed"] == n / 2
+        assert pass1_cache._stats["missed_contains"] == n / 2
         assert pass1_cache._stats["added"] == n / 2
         assert pass1_cache._stats["persisted"] == n / 2
 
         nlp3 = _init_nlp(tmpdir)
         start = time.time()
         for i in range(n):
             nlp3(texts[i])
         pass2_duration = time.time() - start
         cache = nlp3.get_pipe("llm")._cache  # type: ignore
         # Arbitrary time check to ensure second pass (leveraging caching) is at least 30% faster (re-utilizing 50% of
         # the entire doc batch, so max. theoretical speed-up is 50%).
         assert ref_duration - pass2_duration >= ref_duration * 0.3
         assert cache._stats["hit"] == n / 2
+        assert cache._stats["hit_contains"] == n / 2
         assert cache._stats["missed"] == n / 2
+        assert cache._stats["missed_contains"] == n / 2
         assert cache._stats["added"] == n / 2
         assert cache._stats["persisted"] == n / 2
 
 
 def test_path_file_invalid():
     with spacy.util.make_tempdir() as tmpdir:
         # File path instead of directory path.
```

### Comparing `spacy-llm-0.2.0/spacy_llm/tests/test_combinations.py` & `spacy-llm-0.2.1/spacy_llm/tests/test_combinations.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/spacy_llm/ty.py` & `spacy-llm-0.2.1/spacy_llm/ty.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     if not (len(type_hints["parse"]) == 3 and "return" in type_hints["parse"]):
         raise ValueError(
             "The 'task.parse_responses()' function should have two input arguments and one return value."
         )
     for k in type_hints["parse"]:
         # find the 'prompt_responses' var without assuming its name
         type_k = type_hints["parse"][k]
-        if type_k is not typing.Iterable[Doc]:
+        if type_k != typing.Iterable[Doc]:
             parse_input = type_hints["parse"][k]
 
     template_output = type_hints["template"]["return"]
 
     # Check that all variables are Iterables.
     for var, msg in (
         (template_output, "`task.generate_prompts()` needs to return an `Iterable`."),
```

### Comparing `spacy-llm-0.2.0/spacy_llm/util.py` & `spacy-llm-0.2.1/spacy_llm/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Dict, Iterable, List, Union
 from pathlib import Path
 
 from confection import Config
+from spacy.language import Language
 from spacy.util import SimpleFrozenDict, get_sourced_components, load_config
 from spacy.util import load_model_from_config
 
 
 def split_labels(labels: Union[str, Iterable[str]]) -> List[str]:
     """Split a comma-separated list of labels.
     If input is a list already, just strip each entry of the list
@@ -13,33 +14,34 @@
     labels (Union[str, Iterable[str]]): comma-separated string or list of labels
     RETURNS (List[str]): a split and stripped list of labels
     """
     labels = labels.split(",") if isinstance(labels, str) else labels
     return [label.strip() for label in labels]
 
 
-def assemble_from_config(
-    config: Config,
-):
+def assemble_from_config(config: Config) -> Language:
+    """Assemble a spaCy pipeline from a confection Config object.
+
+    config (Config): Config to load spaCy pipeline from.
+    RETURNS (Language): An initialized spaCy pipeline.
+    """
     nlp = load_model_from_config(config, auto_fill=True)
     config = config.interpolate()
     sourced = get_sourced_components(config)
     nlp._link_components()
     with nlp.select_pipes(disable=[*sourced]):
         nlp.initialize()
     return nlp
 
 
 def assemble(
-    config_path: Union[str, Path],
-    *,
-    overrides: Dict[str, Any] = SimpleFrozenDict(),
-):
+    config_path: Union[str, Path], *, overrides: Dict[str, Any] = SimpleFrozenDict()
+) -> Language:
+    """Assemble a spaCy pipeline from a config file.
+
+    config_path (Union[str, Path]): Path to config file.
+    overrides (Dict[str, Any], optional): Dictionary of config overrides.
+    RETURNS (Language): An initialized spaCy pipeline.
+    """
     config_path = Path(config_path)
     config = load_config(config_path, overrides=overrides, interpolate=False)
-    nlp = load_model_from_config(config, auto_fill=True)
-    config = config.interpolate()
-    sourced = get_sourced_components(config)
-    nlp._link_components()
-    with nlp.select_pipes(disable=[*sourced]):
-        nlp.initialize()
-    return nlp
+    return assemble_from_config(config)
```

### Comparing `spacy-llm-0.2.0/spacy_llm.egg-info/PKG-INFO` & `spacy-llm-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: spacy-llm
-Version: 0.2.0
-Summary: Integrating LLMs into structured NLP pipelines
-Author: Explosion
-Author-email: contact@explosion.ai
-License: MIT
-Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
-Project-URL: Source, https://github.com/explosion/spacy-llm
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: minichain
-Provides-Extra: langchain
-Provides-Extra: transformers
-License-File: LICENSE
-
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-llm: Integrating LLMs into structured NLP pipelines
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/spacy-llm/actions/workflows/test.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
@@ -93,15 +61,15 @@
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
-labels = COMPLIMENT,INSULT
+labels = ["COMPLIMENT", "INSULT"]
 
 [components.llm.backend]
 @llm_backends = "spacy.REST.v1"
 api = "OpenAI"
 config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
 ```
 
@@ -131,15 +99,15 @@
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
-labels = PERSON,ORGANISATION,LOCATION
+labels = ["PERSON", "ORGANISATION", "LOCATION"]
 
 [components.llm.backend]
 @llm_backends = "spacy.DollyHF.v1"
 # For better performance, use databricks/dolly-v2-12b instead
 model = "databricks/dolly-v2-3b"
 ```
 
@@ -168,15 +136,15 @@
 
 nlp = spacy.blank("en")
 nlp.add_pipe(
     "llm",
     config={
         "task": {
             "@llm_tasks": "spacy.NER.v2",
-            "labels": "PERSON,ORGANISATION,LOCATION"
+            "labels": ["PERSON", "ORGANISATION", "LOCATION"]
         },
         "backend": {
             "@llm_backends": "spacy.REST.v1",
             "api": "OpenAI",
             "config": {"model": "gpt-3.5-turbo"},
         },
     },
@@ -197,14 +165,16 @@
 them into a list of prompts, and `parse_responses` that transforms the LLM outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity spans, text categories and more.
 
 To register your custom task with spaCy, decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator with a custom name that you can refer to in your config.
 
 > 📖 For more details, see the [**usage example on writing your own task**](usage_examples/README.md#writing-your-own-task)
 
 ```python
+from typing import Iterable, List
+from spacy.tokens import Doc
 from spacy_llm.registry import registry
 from spacy_llm.util import split_labels
 
 
 @registry.llm_tasks("my_namespace.MyTask.v1")
 def make_my_task(labels: str, my_other_config_val: float) -> "MyTask":
     labels_list = split_labels(labels)
@@ -248,14 +218,18 @@
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
 
+Moreover, the task may define an optional [`scorer` method](https://spacy.io/api/scorer#score).
+It should accept an iterable of `Example`s as input and return a score dictionary.
+If the `scorer` method is defined, `spacy-llm` will call it to evaluate the component.
+
 #### <kbd>function</kbd> `task.generate_prompts`
 
 Takes a collection of documents, and returns a collection of "prompts", which can be of type `Any`.
 Often, prompts are of type `str` - but this is not enforced to allow for maximum flexibility in the framework.
 
 | Argument    | Type            | Description            |
 | ----------- | --------------- | ---------------------- |
@@ -280,21 +254,21 @@
 #### spacy.NER.v2
 
 The built-in NER task supports both zero-shot and few-shot prompting. This version also supports explicitly defining the provided labels with custom descriptions.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
-labels = PERSON,ORGANISATION,LOCATION
+labels = ["PERSON", "ORGANISATION", "LOCATION"]
 examples = null
 ```
 
 | Argument                  | Type                                    | Default                                                  | Description                                                                                                                                           |
 | ------------------------- | --------------------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `labels`                  | `str`                                   |                                                          | Comma-separated list of labels.                                                                                                                       |
+| `labels`                  | `Union[List[str], str]`                 |                                                          | List of labels or str of comma-separated list of labels.                                                                                              |
 | `template`                | `str`                                   | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
 | `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                   | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                   | Optional function that generates examples for few-shot learning.                                                                                      |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                   | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
 | `alignment_mode`          | `str`                                   | `"contract"`                                             | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
 | `case_sensitive_matching` | `bool`                                  | `False`                                                  | Whether to search without case sensitivity.                                                                                                           |
 | `single_match`            | `bool`                                  | `False`                                                  | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                         |
@@ -365,15 +339,14 @@
 | `labels`                  | `str`                                   |              | Comma-separated list of labels.                                                                                                              |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`       | Optional function that generates examples for few-shot learning.                                                                             |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`       | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                           |
 | `alignment_mode`          | `str`                                   | `"contract"` | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`. |
 | `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
 | `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
 
-[ner]: https://github.com/explosion/spacy-llm/blob/main/spacy_llm/tasks/ner.py#L14
 
 The NER task implementation doesn't currently ask the LLM for specific offsets, but simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured by the following parameters:
 
 - The `single_match` parameter is typically set to `False` to allow for multiple matches. For instance, the response from the LLM might only mention the entity "Paris" once, but you'd still
   want to mark it every time it occurs in the document.
 - The case-sensitive matching is typically set to `False` to be robust against case variances in the LLM's output.
@@ -412,21 +385,21 @@
 
 The built-in SpanCat task is a simple adaptation of the NER task to
 support overlapping entities and store its annotations in `doc.spans`.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.SpanCat.v2"
-labels = PERSON,ORGANISATION,LOCATION
+labels = ["PERSON", "ORGANISATION", "LOCATION"]
 examples = null
 ```
 
 | Argument                  | Type                                    | Default                                                            | Description                                                                                                                                           |
 | ------------------------- | --------------------------------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `labels`                  | `str`                                   |                                                                    | Comma-separated list of labels.                                                                                                                       |
+| `labels`                  | `Union[List[str], str]`                 |                                                                    | List of labels or str of comma-separated list of labels.                                                                                              |
 | `template`                | `str`                                   | [`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
 | `label_definitions`       | `Optional[Dict[str, str]]`              | `None`                                                             | Optional dict mapping a label to a description of that label. These descriptions are added to the prompt to help instruct the LLM on what to extract. |
 | `spans_key`               | `str`                                   | `"sc"`                                                             | Key of the `Doc.spans` dict to save the spans under.                                                                                                  |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                             | Optional function that generates examples for few-shot learning.                                                                                      |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`                                                             | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                                    |
 | `alignment_mode`          | `str`                                   | `"contract"`                                                       | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`.          |
 | `case_sensitive_matching` | `bool`                                  | `False`                                                            | Whether to search without case sensitivity.                                                                                                           |
@@ -465,21 +438,21 @@
 #### spacy.TextCat.v2
 
 The built-in TextCat task supports both zero-shot and few-shot prompting.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
-labels = COMPLIMENT,INSULT
+labels = ["COMPLIMENT", "INSULT"]
 examples = null
 ```
 
 | Argument            | Type                                    | Default                                                      | Description                                                                                                                                      |
 | ------------------- | --------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
-| `labels`            | `str`                                   |                                                              | Comma-separated list of labels.                                                                                                                  |
+| `labels`            | `Union[List[str], str]`                 |                                                              | List of labels or str of comma-separated list of labels.                                                                                         |
 | `template`          | `str`                                   | [`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.         |
 | `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                       | Optional function that generates examples for few-shot learning.                                                                                 |
 | `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                                       | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                             |
 | `exclusive_classes` | `bool`                                  | `False`                                                      | If set to `True`, only one label per document should be valid. If set to `False`, one document can have multiple labels.                         |
 | `allow_none`        | `bool`                                  | `True`                                                       | When set to `True`, allows the LLM to not return any of the given label. The resulting dict in `doc.cats` will have `0.0` scores for all labels. |
 | `verbose`           | `bool`                                  | `False`                                                      | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                             |
 
@@ -498,15 +471,15 @@
   }
 ]
 ```
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.TextCat.v2"
-labels = COMPLIMENT,INSULT
+labels = ["COMPLIMENT", "INSULT"]
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "textcat_examples.json"
 ```
 
 #### spacy.TextCat.v1
 
@@ -557,20 +530,20 @@
 
 The built-in REL task supports both zero-shot and few-shot prompting.
 It relies on an upstream NER component for entities extraction.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.REL.v1"
-labels = LivesIn,Visits
+labels = ["LivesIn", "Visits"]
 ```
 
 | Argument            | Type                                    | Default                                              | Description                                                                                                                              |
 | ------------------- | --------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
-| `labels`            | `str`                                   |                                                      | Comma-separated list of relation labels.                                                                                                 |
+| `labels`            | `Union[List[str], str]`                 |                                                      | List of labels or str of comma-separated list of labels.                                                                                 |
 | `template`          | `str`                                   | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory. |
 | `label_description` | `Optional[Dict[str, str]]`              | `None`                                               | Dictionary providing a description for each relation label.                                                                              |
 | `examples`          | `Optional[Callable[[], Iterable[Any]]]` | `None`                                               | Optional function that generates examples for few-shot learning.                                                                         |
 | `normalizer`        | `Optional[Callable[[str], str]]`        | `None`                                               | Function that normalizes the labels as returned by the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`.                     |
 | `verbose`           | `bool`                                  | `False`                                              | If set to `True`, warnings will be generated when the LLM returns invalid responses.                                                     |
 
 To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
@@ -584,15 +557,15 @@
 Note: the REL task relies on pre-extracted entities to make its prediction.
 Hence, you'll need to add a component that populates `doc.ents` with recognized
 spans to your spaCy pipeline and put it _before_ the REL component.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.REL.v1"
-labels = LivesIn,Visits
+labels = ["LivesIn", "Visits"]
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "rel_examples.jsonl"
 ```
 
 #### spacy.NoOp.v1
```

#### html2text {}

```diff
@@ -1,29 +1,12 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.2.0 Summary: Integrating LLMs
-into structured NLP pipelines Author: Explosion Author-email:
-contact@explosion.ai License: MIT Project-URL: Release notes, https://
-github.com/explosion/spacy-llm/releases Project-URL: Source, https://
-github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: minichain Provides-Extra: langchain
-Provides-Extra: transformers License-File: LICENSE [https://explosion.ai/
-assets/img/logo.svg] # spacy-llm: Integrating LLMs into structured NLP
-pipelines [![GitHub Workflow Status](https://img.shields.io/github/actions/
-workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/
-explosion/spacy-llm/actions/workflows/test.yml) [![pypi Version](https://
-img.shields.io/pypi/v/spacy-llm.svg?style=flat-
+[https://explosion.ai/assets/img/logo.svg] # spacy-llm: Integrating LLMs into
+structured NLP pipelines [![GitHub Workflow Status](https://img.shields.io/
+github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)]
+(https://github.com/explosion/spacy-llm/actions/workflows/test.yml) [![pypi
+Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg?style=flat-square)](https://github.com/ambv/black) This package
 integrates Large Language Models (LLMs) into [spaCy](https://spacy.io),
 featuring a modular system for **fast prototyping** and **prompting**, and
 turning unstructured responses into **robust outputs** for various NLP tasks,
 **no training data** required. - Serializable `llm` **component** to integrate
@@ -77,63 +60,64 @@
 api) documentation. ### Example 1: Add a text classifier using a GPT-3 model
 from OpenAI Create a new API key from openai.com or fetch an existing one, and
 ensure the keys are set as environmental variables. For more background
 information, see the [OpenAI](#openai) section. Create a config file
 `config.cfg` containing at least the following (or see the full example [here]
 (usage_examples/textcat_openai)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
-= "spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.backend]
+= "spacy.TextCat.v2" labels = ["COMPLIMENT", "INSULT"] [components.llm.backend]
 @llm_backends = "spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-
 turbo", "temperature": 0.3} ``` Now run: ```python from spacy_llm.util import
 assemble nlp = assemble("config.cfg") doc = nlp("You look gorgeous!") print
 (doc.cats) ``` ### Example 2: Add NER using an open-source model through
 Hugging Face To run this example, ensure that you have a GPU enabled, and
 `transformers`, `torch` and CUDA installed. For more background information,
 see the [DollyHF](#spacydollyhfv1) section. Create a config file `config.cfg`
 containing at least the following (or see the full example [here]
 (usage_examples/ner_dolly)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
-= "spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION [components.llm.backend]
-@llm_backends = "spacy.DollyHF.v1" # For better performance, use databricks/
-dolly-v2-12b instead model = "databricks/dolly-v2-3b" ``` Now run: ```python
-from spacy_llm.util import assemble nlp = assemble("config.cfg") doc = nlp
-("Jack and Jill rode up the hill in Les Deux Alpes") print([(ent.text,
-ent.label_) for ent in doc.ents]) ``` Note that Hugging Face will download the
-`"databricks/dolly-v2-3b"` model the first time you use it. You can [define the
-cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/
-manage-cache) by setting the environmental variable `HF_HOME`. Also, you can
-upgrade the model to be `"databricks/dolly-v2-12b"` for better performance. ###
-Example 3: Create the component directly in Python The `llm` component behaves
-as any other spaCy component does, so adding it to an existing pipeline follows
-the same pattern: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
-( "llm", config={ "task": { "@llm_tasks": "spacy.NER.v2", "labels":
-"PERSON,ORGANISATION,LOCATION" }, "backend": { "@llm_backends":
-"spacy.REST.v1", "api": "OpenAI", "config": {"model": "gpt-3.5-turbo"}, }, }, )
-nlp.initialize() doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
-print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that for efficient
-usage of resources, typically you would use [`nlp.pipe(docs)`](https://
-spacy.io/api/language#pipe) with a batch, instead of calling `nlp(doc)` with a
-single document. ### Example 4: Implement your own custom task To write a
-[`task`](#tasks), you need to implement two functions: `generate_prompts` that
-takes a list of spaCy [`Doc`](https://spacy.io/api/doc) objects and transforms
-them into a list of prompts, and `parse_responses` that transforms the LLM
-outputs into annotations on the [`Doc`](https://spacy.io/api/doc), e.g. entity
-spans, text categories and more. To register your custom task with spaCy,
-decorate a factory function using the `spacy_llm.registry.llm_tasks` decorator
-with a custom name that you can refer to in your config. > ð For more
-details, see the [**usage example on writing your own task**](usage_examples/
-README.md#writing-your-own-task) ```python from spacy_llm.registry import
-registry from spacy_llm.util import split_labels @registry.llm_tasks
-("my_namespace.MyTask.v1") def make_my_task(labels: str, my_other_config_val:
-float) -> "MyTask": labels_list = split_labels(labels) return MyTask
-(labels=labels_list, my_other_config_val=my_other_config_val) class MyTask: def
-__init__(self, labels: List[str], my_other_config_val: float): ... def
-generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]: ... def
-parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] ) -
-> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
+= "spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"]
+[components.llm.backend] @llm_backends = "spacy.DollyHF.v1" # For better
+performance, use databricks/dolly-v2-12b instead model = "databricks/dolly-v2-
+3b" ``` Now run: ```python from spacy_llm.util import assemble nlp = assemble
+("config.cfg") doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
+print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that Hugging Face
+will download the `"databricks/dolly-v2-3b"` model the first time you use it.
+You can [define the cached directory](https://huggingface.co/docs/
+huggingface_hub/main/en/guides/manage-cache) by setting the environmental
+variable `HF_HOME`. Also, you can upgrade the model to be `"databricks/dolly-
+v2-12b"` for better performance. ### Example 3: Create the component directly
+in Python The `llm` component behaves as any other spaCy component does, so
+adding it to an existing pipeline follows the same pattern: ```python import
+spacy nlp = spacy.blank("en") nlp.add_pipe( "llm", config={ "task":
+{ "@llm_tasks": "spacy.NER.v2", "labels": ["PERSON", "ORGANISATION",
+"LOCATION"] }, "backend": { "@llm_backends": "spacy.REST.v1", "api": "OpenAI",
+"config": {"model": "gpt-3.5-turbo"}, }, }, ) nlp.initialize() doc = nlp("Jack
+and Jill rode up the hill in Les Deux Alpes") print([(ent.text, ent.label_) for
+ent in doc.ents]) ``` Note that for efficient usage of resources, typically you
+would use [`nlp.pipe(docs)`](https://spacy.io/api/language#pipe) with a batch,
+instead of calling `nlp(doc)` with a single document. ### Example 4: Implement
+your own custom task To write a [`task`](#tasks), you need to implement two
+functions: `generate_prompts` that takes a list of spaCy [`Doc`](https://
+spacy.io/api/doc) objects and transforms them into a list of prompts, and
+`parse_responses` that transforms the LLM outputs into annotations on the
+[`Doc`](https://spacy.io/api/doc), e.g. entity spans, text categories and more.
+To register your custom task with spaCy, decorate a factory function using the
+`spacy_llm.registry.llm_tasks` decorator with a custom name that you can refer
+to in your config. > ð For more details, see the [**usage example on writing
+your own task**](usage_examples/README.md#writing-your-own-task) ```python from
+typing import Iterable, List from spacy.tokens import Doc from
+spacy_llm.registry import registry from spacy_llm.util import split_labels
+@registry.llm_tasks("my_namespace.MyTask.v1") def make_my_task(labels: str,
+my_other_config_val: float) -> "MyTask": labels_list = split_labels(labels)
+return MyTask(labels=labels_list, my_other_config_val=my_other_config_val)
+class MyTask: def __init__(self, labels: List[str], my_other_config_val:
+float): ... def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
+... def parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] )
+-> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
 @llm_tasks = "my_namespace.MyTask.v1" labels = LABEL1,LABEL2,LABEL3
 my_other_config_val = 0.3 ``` ## ð API Each `llm` component is defined by
 two main settings: - A [**task**](#tasks), defining the prompt to send to the
 LLM as well as the functionality to parse the resulting response back into
 structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects. - A
 [**backend**](#backends) defining the model to use and how to connect to it.
 Note that `spacy-llm` supports both access to external APIs (such as OpenAI) as
@@ -142,50 +126,55 @@
 functionality to avoid running the same document through an LLM service (be it
 local or through a REST API) more than once. ### Tasks A _task_ defines an NLP
 problem or question, that will be sent to the LLM via a prompt. Further, the
 task defines how to parse the LLM's responses back into structured information.
 All tasks are registered in spaCy's `llm_tasks` registry. Practically speaking,
 a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`]
 (spacy_llm/ty.py). It needs to define a `generate_prompts` function and a
-`parse_responses` function. #### function `task.generate_prompts` Takes a
-collection of documents, and returns a collection of "prompts", which can be of
-type `Any`. Often, prompts are of type `str` - but this is not enforced to
-allow for maximum flexibility in the framework. | Argument | Type | Description
-| | ----------- | --------------- | ---------------------- | | `docs` |
-`Iterable[Doc]` | The input documents. | | **RETURNS** | `Iterable[Any]` | The
-generated prompts. | #### function `task.parse_responses` Takes a collection of
-LLM responses and the original documents, parses the responses into structured
-information, and sets the annotations on the documents. The `parse_responses`
-function is free to set the annotations in any way, including `Doc` fields like
-`ents`, `spans` or `cats`, or using custom defined fields. The `responses` are
-of type `Iterable[Any]`, though they will often be `str` objects. This depends
-on the return type of the [backend](#backends). | Argument | Type | Description
-| | ----------- | --------------- | ------------------------ | | `docs` |
-`Iterable[Doc]` | The input documents. | | `responses` | `Iterable[Any]` | The
-generated prompts. | | **RETURNS** | `Iterable[Doc]` | The annotated documents.
-| #### spacy.NER.v2 The built-in NER task supports both zero-shot and few-shot
-prompting. This version also supports explicitly defining the provided labels
-with custom descriptions. ```ini [components.llm.task] @llm_tasks =
-"spacy.NER.v2" labels = PERSON,ORGANISATION,LOCATION examples = null ``` |
-Argument | Type | Default | Description | | ------------------------- | -------
--------------------------------- | --------------------------------------------
------------- | ----------------------------------------------------------------
+`parse_responses` function. Moreover, the task may define an optional [`scorer`
+method](https://spacy.io/api/scorer#score). It should accept an iterable of
+`Example`s as input and return a score dictionary. If the `scorer` method is
+defined, `spacy-llm` will call it to evaluate the component. #### function
+`task.generate_prompts` Takes a collection of documents, and returns a
+collection of "prompts", which can be of type `Any`. Often, prompts are of type
+`str` - but this is not enforced to allow for maximum flexibility in the
+framework. | Argument | Type | Description | | ----------- | --------------- |
+---------------------- | | `docs` | `Iterable[Doc]` | The input documents. | |
+**RETURNS** | `Iterable[Any]` | The generated prompts. | #### function
+`task.parse_responses` Takes a collection of LLM responses and the original
+documents, parses the responses into structured information, and sets the
+annotations on the documents. The `parse_responses` function is free to set the
+annotations in any way, including `Doc` fields like `ents`, `spans` or `cats`,
+or using custom defined fields. The `responses` are of type `Iterable[Any]`,
+though they will often be `str` objects. This depends on the return type of the
+[backend](#backends). | Argument | Type | Description | | ----------- | -------
+-------- | ------------------------ | | `docs` | `Iterable[Doc]` | The input
+documents. | | `responses` | `Iterable[Any]` | The generated prompts. | |
+**RETURNS** | `Iterable[Doc]` | The annotated documents. | #### spacy.NER.v2
+The built-in NER task supports both zero-shot and few-shot prompting. This
+version also supports explicitly defining the provided labels with custom
+descriptions. ```ini [components.llm.task] @llm_tasks = "spacy.NER.v2" labels =
+["PERSON", "ORGANISATION", "LOCATION"] examples = null ``` | Argument | Type |
+Default | Description | | ------------------------- | -------------------------
+-------------- | -------------------------------------------------------- | ---
 -------------------------------------------------------------------------------
------- | | `labels` | `str` | | Comma-separated list of labels. | | `template`
-| `str` | [ner.v2.jinja](./spacy_llm/tasks/templates/ner.v2.jinja) | Custom
-prompt template to send to LLM backend. Default templates for each task are
-located in the `spacy_llm/tasks/templates` directory. | | `label_definitions` |
-`Optional[Dict[str, str]]` | `None` | Optional dict mapping a label to a
-description of that label. These descriptions are added to the prompt to help
-instruct the LLM on what to extract. | | `examples` | `Optional[Callable[[],
-Iterable[Any]]]` | `None` | Optional function that generates examples for few-
-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None` |
-Function that normalizes the labels as returned by the LLM. If `None`, defaults
-to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"`
-| Alignment mode in case the LLM returns entities that do not align with token
+------------------------------------------------------------------- | |
+`labels` | `Union[List[str], str]` | | List of labels or str of comma-separated
+list of labels. | | `template` | `str` | [ner.v2.jinja](./spacy_llm/tasks/
+templates/ner.v2.jinja) | Custom prompt template to send to LLM backend.
+Default templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `label_definitions` | `Optional[Dict[str, str]]` | `None` |
+Optional dict mapping a label to a description of that label. These
+descriptions are added to the prompt to help instruct the LLM on what to
+extract. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
+Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, defaults to
+`spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
+Alignment mode in case the LLM returns entities that do not align with token
 boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
 `case_sensitive_matching` | `bool` | `False` | Whether to search without case
 sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
 in the LLM's response only once (the first hit) or multiple times. | The NER
 task implementation doesn't currently ask the LLM for specific offsets, but
 simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured
@@ -234,16 +223,15 @@
 [[str], str]]` | `None` | Function that normalizes the labels as returned by
 the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`. | |
 `alignment_mode` | `str` | `"contract"` | Alignment mode in case the LLM
 returns entities that do not align with token boundaries. Options are
 `"strict"`, `"contract"` or `"expand"`. | | `case_sensitive_matching` | `bool`
 | `False` | Whether to search without case sensitivity. | | `single_match` |
 `bool` | `False` | Whether to match an entity in the LLM's response only once
-(the first hit) or multiple times. | [ner]: https://github.com/explosion/spacy-
-llm/blob/main/spacy_llm/tasks/ner.py#L14 The NER task implementation doesn't
+(the first hit) or multiple times. | The NER task implementation doesn't
 currently ask the LLM for specific offsets, but simply expects a list of
 strings that represent the enties in the document. This means that a form of
 string matching is required. This can be configured by the following
 parameters: - The `single_match` parameter is typically set to `False` to allow
 for multiple matches. For instance, the response from the LLM might only
 mention the entity "Paris" once, but you'd still want to mark it every time it
 occurs in the document. - The case-sensitive matching is typically set to
@@ -261,148 +249,150 @@
 ```yaml - text: Jack and Jill went up the hill. entities: PERSON: - Jack - Jill
 LOCATION: - hill - text: Jack fell down and broke his crown. entities: PERSON:
 - Jack ``` ```ini [components.llm.task] @llm_tasks = "spacy.NER.v1" labels =
 PERSON,ORGANISATION,LOCATION [components.llm.task.examples] @misc =
 "spacy.FewShotReader.v1" path = "ner_examples.yml" ``` #### spacy.SpanCat.v2
 The built-in SpanCat task is a simple adaptation of the NER task to support
 overlapping entities and store its annotations in `doc.spans`. ```ini
-[components.llm.task] @llm_tasks = "spacy.SpanCat.v2" labels =
-PERSON,ORGANISATION,LOCATION examples = null ``` | Argument | Type | Default |
+[components.llm.task] @llm_tasks = "spacy.SpanCat.v2" labels = ["PERSON",
+"ORGANISATION", "LOCATION"] examples = null ``` | Argument | Type | Default |
 Description | | ------------------------- | -----------------------------------
 ---- | ------------------------------------------------------------------ | ---
 -------------------------------------------------------------------------------
 ------------------------------------------------------------------- | |
-`labels` | `str` | | Comma-separated list of labels. | | `template` | `str` |
-[`spancat.v2.jinja`](./spacy_llm/tasks/templates/spancat.v2.jinja) | Custom
-prompt template to send to LLM backend. Default templates for each task are
-located in the `spacy_llm/tasks/templates` directory. | | `label_definitions` |
-`Optional[Dict[str, str]]` | `None` | Optional dict mapping a label to a
-description of that label. These descriptions are added to the prompt to help
-instruct the LLM on what to extract. | | `spans_key` | `str` | `"sc"` | Key of
-the `Doc.spans` dict to save the spans under. | | `examples` | `Optional
-[Callable[[], Iterable[Any]]]` | `None` | Optional function that generates
-examples for few-shot learning. | | `normalizer` | `Optional[Callable[[str],
-str]]` | `None` | Function that normalizes the labels as returned by the LLM.
-If `None`, defaults to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` |
-`str` | `"contract"` | Alignment mode in case the LLM returns entities that do
-not align with token boundaries. Options are `"strict"`, `"contract"` or
-`"expand"`. | | `case_sensitive_matching` | `bool` | `False` | Whether to
-search without case sensitivity. | | `single_match` | `bool` | `False` |
-Whether to match an entity in the LLM's response only once (the first hit) or
-multiple times. | Except for the `spans_key` parameter, the SpanCat task reuses
-the configuration from the NER task. Refer to [its documentation](#spacynerv2)
-for more insight. #### spacy.SpanCat.v1 The original version of the built-in
-SpanCat task is a simple adaptation of the v1 NER task to support overlapping
-entities and store its annotations in `doc.spans`. ```ini [components.llm.task]
-@llm_tasks = "spacy.SpanCat.v1" labels = PERSON,ORGANISATION,LOCATION examples
-= null ``` | Argument | Type | Default | Description | | ----------------------
---- | --------------------------------------- | ------------ | ----------------
+`labels` | `Union[List[str], str]` | | List of labels or str of comma-separated
+list of labels. | | `template` | `str` | [`spancat.v2.jinja`](./spacy_llm/
+tasks/templates/spancat.v2.jinja) | Custom prompt template to send to LLM
+backend. Default templates for each task are located in the `spacy_llm/tasks/
+templates` directory. | | `label_definitions` | `Optional[Dict[str, str]]` |
+`None` | Optional dict mapping a label to a description of that label. These
+descriptions are added to the prompt to help instruct the LLM on what to
+extract. | | `spans_key` | `str` | `"sc"` | Key of the `Doc.spans` dict to save
+the spans under. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` |
+`None` | Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, defaults to
+`spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
+Alignment mode in case the LLM returns entities that do not align with token
+boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
+`case_sensitive_matching` | `bool` | `False` | Whether to search without case
+sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
+in the LLM's response only once (the first hit) or multiple times. | Except for
+the `spans_key` parameter, the SpanCat task reuses the configuration from the
+NER task. Refer to [its documentation](#spacynerv2) for more insight. ####
+spacy.SpanCat.v1 The original version of the built-in SpanCat task is a simple
+adaptation of the v1 NER task to support overlapping entities and store its
+annotations in `doc.spans`. ```ini [components.llm.task] @llm_tasks =
+"spacy.SpanCat.v1" labels = PERSON,ORGANISATION,LOCATION examples = null ``` |
+Argument | Type | Default | Description | | ------------------------- | -------
+-------------------------------- | ------------ | -----------------------------
 -------------------------------------------------------------------------------
---------------------------------------------- | | `labels` | `str` | | Comma-
-separated list of labels. | | `spans_key` | `str` | `"sc"` | Key of the
-`Doc.spans` dict to save the spans under. | | `examples` | `Optional[Callable[
-[], Iterable[Any]]]` | `None` | Optional function that generates examples for
-few-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None`
-| Function that normalizes the labels as returned by the LLM. If `None`,
-defaults to `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` |
-`"contract"` | Alignment mode in case the LLM returns entities that do not
-align with token boundaries. Options are `"strict"`, `"contract"` or
-`"expand"`. | | `case_sensitive_matching` | `bool` | `False` | Whether to
-search without case sensitivity. | | `single_match` | `bool` | `False` |
-Whether to match an entity in the LLM's response only once (the first hit) or
-multiple times. | Except for the `spans_key` parameter, the SpanCat task reuses
-the configuration from the NER task. Refer to [its documentation](#spacynerv1)
-for more insight. #### spacy.TextCat.v2 The built-in TextCat task supports both
-zero-shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks =
-"spacy.TextCat.v2" labels = COMPLIMENT,INSULT examples = null ``` | Argument |
-Type | Default | Description | | ------------------- | ------------------------
---------------- | -----------------------------------------------------------
-- | ---------------------------------------------------------------------------
---------------------------------------------------------------------- | |
-`labels` | `str` | | Comma-separated list of labels. | | `template` | `str` |
-[`textcat.jinja`](./spacy_llm/tasks/templates/textcat.jinja) | Custom prompt
-template to send to LLM backend. Default templates for each task are located in
-the `spacy_llm/tasks/templates` directory. | | `examples` | `Optional[Callable[
-[], Iterable[Any]]]` | `None` | Optional function that generates examples for
-few-shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None`
-| Function that normalizes the labels as returned by the LLM. If `None`, falls
-back to `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` |
-`False` | If set to `True`, only one label per document should be valid. If set
-to `False`, one document can have multiple labels. | | `allow_none` | `bool` |
-`True` | When set to `True`, allows the LLM to not return any of the given
-label. The resulting dict in `doc.cats` will have `0.0` scores for all labels.
-| | `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
-when the LLM returns invalid responses. | To perform few-shot learning, you can
-write down a few examples in a separate file, and provide these to be injected
-into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
-supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
-great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
-"answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
-"spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.task.examples]
-@misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
-spacy.TextCat.v1 The original version of the built-in TextCat task supports
-both zero-shot and few-shot prompting. ```ini [components.llm.task] @llm_tasks
-= "spacy.TextCat.v1" labels = COMPLIMENT,INSULT examples = null ``` | Argument
-| Type | Default | Description | | ------------------- | ----------------------
------------------ | ------- | -------------------------------------------------
+-------------------------------- | | `labels` | `str` | | Comma-separated list
+of labels. | | `spans_key` | `str` | `"sc"` | Key of the `Doc.spans` dict to
+save the spans under. | | `examples` | `Optional[Callable[[], Iterable[Any]]]`
+| `None` | Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, defaults to
+`spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
+Alignment mode in case the LLM returns entities that do not align with token
+boundaries. Options are `"strict"`, `"contract"` or `"expand"`. | |
+`case_sensitive_matching` | `bool` | `False` | Whether to search without case
+sensitivity. | | `single_match` | `bool` | `False` | Whether to match an entity
+in the LLM's response only once (the first hit) or multiple times. | Except for
+the `spans_key` parameter, the SpanCat task reuses the configuration from the
+NER task. Refer to [its documentation](#spacynerv1) for more insight. ####
+spacy.TextCat.v2 The built-in TextCat task supports both zero-shot and few-shot
+prompting. ```ini [components.llm.task] @llm_tasks = "spacy.TextCat.v2" labels
+= ["COMPLIMENT", "INSULT"] examples = null ``` | Argument | Type | Default |
+Description | | ------------------- | --------------------------------------- |
+------------------------------------------------------------ | ----------------
 -------------------------------------------------------------------------------
----------------- | | `labels` | str | | Comma-separated list of labels. | |
-`examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` | Optional
-function that generates examples for few-shot learning. | | `normalizer` |
-`Optional[Callable[[str], str]]` | `None` | Function that normalizes the labels
-as returned by the LLM. If `None`, falls back to
+------------------------------------------------- | | `labels` | `Union[List
+[str], str]` | | List of labels or str of comma-separated list of labels. | |
+`template` | `str` | [`textcat.jinja`](./spacy_llm/tasks/templates/
+textcat.jinja) | Custom prompt template to send to LLM backend. Default
+templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
+Optional function that generates examples for few-shot learning. | |
+`normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
+normalizes the labels as returned by the LLM. If `None`, falls back to
 `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` | `False` | If
 set to `True`, only one label per document should be valid. If set to `False`,
 one document can have multiple labels. | | `allow_none` | `bool` | `True` |
 When set to `True`, allows the LLM to not return any of the given label. The
 resulting dict in `doc.cats` will have `0.0` scores for all labels. | |
 `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
 when the LLM returns invalid responses. | To perform few-shot learning, you can
 write down a few examples in a separate file, and provide these to be injected
 into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
 supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
 great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
 "answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
+"spacy.TextCat.v2" labels = ["COMPLIMENT", "INSULT"]
+[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
+"textcat_examples.json" ``` #### spacy.TextCat.v1 The original version of the
+built-in TextCat task supports both zero-shot and few-shot prompting. ```ini
+[components.llm.task] @llm_tasks = "spacy.TextCat.v1" labels =
+COMPLIMENT,INSULT examples = null ``` | Argument | Type | Default | Description
+| | ------------------- | --------------------------------------- | ------- | -
+-------------------------------------------------------------------------------
+---------------------------------------------------------------- | | `labels` |
+str | | Comma-separated list of labels. | | `examples` | `Optional[Callable[[],
+Iterable[Any]]]` | `None` | Optional function that generates examples for few-
+shot learning. | | `normalizer` | `Optional[Callable[[str], str]]` | `None` |
+Function that normalizes the labels as returned by the LLM. If `None`, falls
+back to `spacy.LowercaseNormalizer.v1`. | | `exclusive_classes` | `bool` |
+`False` | If set to `True`, only one label per document should be valid. If set
+to `False`, one document can have multiple labels. | | `allow_none` | `bool` |
+`True` | When set to `True`, allows the LLM to not return any of the given
+label. The resulting dict in `doc.cats` will have `0.0` scores for all labels.
+| | `verbose` | `bool` | `False` | If set to `True`, warnings will be generated
+when the LLM returns invalid responses. | To perform few-shot learning, you can
+write down a few examples in a separate file, and provide these to be injected
+into the prompt to the LLM. The default reader `spacy.FewShotReader.v1`
+supports `.yml`, `.yaml`, `.json` and `.jsonl`. ```json [ { "text": "You look
+great!", "answer": "Compliment" }, { "text": "You are not very clever at all.",
+"answer": "Insult" } ] ``` ```ini [components.llm.task] @llm_tasks =
 "spacy.TextCat.v2" labels = COMPLIMENT,INSULT [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1" path = "textcat_examples.json" ``` ####
 spacy.REL.v1 The built-in REL task supports both zero-shot and few-shot
 prompting. It relies on an upstream NER component for entities extraction.
-```ini [components.llm.task] @llm_tasks = "spacy.REL.v1" labels =
-LivesIn,Visits ``` | Argument | Type | Default | Description | | --------------
------ | --------------------------------------- | -----------------------------
------------------------ | -----------------------------------------------------
--------------------------------------------------------------------------------
----- | | `labels` | `str` | | Comma-separated list of relation labels. | |
-`template` | `str` | [`rel.jinja`](./spacy_llm/tasks/templates/rel.jinja) |
-Custom prompt template to send to LLM backend. Default templates for each task
-are located in the `spacy_llm/tasks/templates` directory. | |
-`label_description` | `Optional[Dict[str, str]]` | `None` | Dictionary
-providing a description for each relation label. | | `examples` | `Optional
-[Callable[[], Iterable[Any]]]` | `None` | Optional function that generates
-examples for few-shot learning. | | `normalizer` | `Optional[Callable[[str],
-str]]` | `None` | Function that normalizes the labels as returned by the LLM.
-If `None`, falls back to `spacy.LowercaseNormalizer.v1`. | | `verbose` | `bool`
-| `False` | If set to `True`, warnings will be generated when the LLM returns
-invalid responses. | To perform few-shot learning, you can write down a few
-examples in a separate file, and provide these to be injected into the prompt
-to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
+```ini [components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
+"Visits"] ``` | Argument | Type | Default | Description | | ------------------
+- | --------------------------------------- | ---------------------------------
+------------------- | ---------------------------------------------------------
+------------------------------------------------------------------------------
+- | | `labels` | `Union[List[str], str]` | | List of labels or str of comma-
+separated list of labels. | | `template` | `str` | [`rel.jinja`](./spacy_llm/
+tasks/templates/rel.jinja) | Custom prompt template to send to LLM backend.
+Default templates for each task are located in the `spacy_llm/tasks/templates`
+directory. | | `label_description` | `Optional[Dict[str, str]]` | `None` |
+Dictionary providing a description for each relation label. | | `examples` |
+`Optional[Callable[[], Iterable[Any]]]` | `None` | Optional function that
+generates examples for few-shot learning. | | `normalizer` | `Optional[Callable
+[[str], str]]` | `None` | Function that normalizes the labels as returned by
+the LLM. If `None`, falls back to `spacy.LowercaseNormalizer.v1`. | | `verbose`
+| `bool` | `False` | If set to `True`, warnings will be generated when the LLM
+returns invalid responses. | To perform few-shot learning, you can write down a
+few examples in a separate file, and provide these to be injected into the
+prompt to the LLM. The default reader `spacy.FewShotReader.v1` supports `.yml`,
 `.yaml`, `.json` and `.jsonl`. ```json {"text": "Laura bought a house in Boston
 with her husband Mark.", "ents": [{"start_char": 0, "end_char": 5, "label":
 "PERSON"}, {"start_char": 24, "end_char": 30, "label": "GPE"}, {"start_char":
 48, "end_char": 52, "label": "PERSON"}], "relations": [{"dep": 0, "dest": 1,
 "relation": "LivesIn"}, {"dep": 2, "dest": 1, "relation": "LivesIn"}]} {"text":
 "Michael travelled through South America by bike.", "ents": [{"start_char": 0,
 "end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label":
 "LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]} ``` Note:
 the REL task relies on pre-extracted entities to make its prediction. Hence,
 you'll need to add a component that populates `doc.ents` with recognized spans
 to your spaCy pipeline and put it _before_ the REL component. ```ini
-[components.llm.task] @llm_tasks = "spacy.REL.v1" labels = LivesIn,Visits
-[components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path =
-"rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
+[components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
+"Visits"] [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path
+= "rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
 testing - it tells the LLM to do nothing, and does not set any fields on the
 `docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
 Backends A _backend_ defines which LLM model to query, and how to query it. It
 can be a simple function taking a collection of prompts (consistent with the
 output type of `task.generate_prompts()`) and returning a collection of
 responses (consistent with the expected input of `parse_responses`). Generally
 speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
```

### Comparing `spacy-llm-0.2.0/spacy_llm.egg-info/SOURCES.txt` & `spacy-llm-0.2.1/spacy_llm.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 spacy_llm/tasks/templates/ner.jinja
 spacy_llm/tasks/templates/ner.v2.jinja
 spacy_llm/tasks/templates/rel.jinja
 spacy_llm/tasks/templates/spancat.jinja
 spacy_llm/tasks/templates/spancat.v2.jinja
 spacy_llm/tasks/templates/textcat.jinja
 spacy_llm/tasks/templates/textcat.v2.jinja
+spacy_llm/tasks/templates/textcat.v3.jinja
 spacy_llm/tasks/util/__init__.py
 spacy_llm/tasks/util/examples.py
 spacy_llm/tasks/util/parsing.py
 spacy_llm/tasks/util/span.py
 spacy_llm/tests/__init__.py
 spacy_llm/tests/compat.py
 spacy_llm/tests/conftest.py
```

### Comparing `spacy-llm-0.2.0/usage_examples/multitask_openai/run_pipeline.py` & `spacy-llm-0.2.1/usage_examples/multitask_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/usage_examples/ner_dolly/run_pipeline.py` & `spacy-llm-0.2.1/usage_examples/ner_dolly/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/usage_examples/ner_langchain_openai/run_pipeline.py` & `spacy-llm-0.2.1/usage_examples/ner_langchain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/usage_examples/ner_minichain_openai/run_pipeline.py` & `spacy-llm-0.2.1/usage_examples/ner_minichain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/usage_examples/rel_openai/run_pipeline.py` & `spacy-llm-0.2.1/usage_examples/rel_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/usage_examples/tests/test_readme_examples.py` & `spacy-llm-0.2.1/usage_examples/tests/test_readme_examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         [components]
 
         [components.llm]
         factory = "llm"
 
         [components.llm.task]
         @llm_tasks = "spacy.TextCat.v2"
-        labels = COMPLIMENT,INSULT
+        labels = ["COMPLIMENT", "INSULT"]
 
         [components.llm.backend]
         @llm_backends = "spacy.REST.v1"
         api = "OpenAI"
         config = {"model": "gpt-3.5-turbo", "temperature": 0.3}
         """
 
@@ -51,15 +51,15 @@
         [components]
 
         [components.llm]
         factory = "llm"
 
         [components.llm.task]
         @llm_tasks = "spacy.NER.v2"
-        labels = PERSON,ORGANISATION,LOCATION
+        labels = ["PERSON", "ORGANISATION", "LOCATION"]
 
         [components.llm.backend]
         @llm_backends = "spacy.DollyHF.v1"
         # For better performance, use databricks/dolly-v2-12b instead
         model = "databricks/dolly-v2-3b"
         """
 
@@ -75,15 +75,15 @@
 def test_example_3_python():
     nlp = spacy.blank("en")
     nlp.add_pipe(
         "llm",
         config={
             "task": {
                 "@llm_tasks": "spacy.NER.v2",
-                "labels": "PERSON,ORGANISATION,LOCATION",
+                "labels": ["PERSON", "ORGANISATION", "LOCATION"],
             },
             "backend": {
                 "@llm_backends": "spacy.REST.v1",
                 "api": "OpenAI",
                 "config": {"model": "gpt-3.5-turbo"},
             },
         },
```

### Comparing `spacy-llm-0.2.0/usage_examples/tests/test_usage_examples.py` & `spacy-llm-0.2.1/usage_examples/tests/test_usage_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.0/usage_examples/textcat_openai/run_pipeline.py` & `spacy-llm-0.2.1/usage_examples/textcat_openai/run_pipeline.py`

 * *Files identical despite different names*

