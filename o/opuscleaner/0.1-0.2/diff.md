# Comparing `tmp/opuscleaner-0.1.tar.gz` & `tmp/opuscleaner-0.2.tar.gz`

## Comparing `opuscleaner-0.1.tar` & `opuscleaner-0.2.tar`

### file list

```diff
@@ -1,92 +1,107 @@
--rwxr-xr-x   0        0        0     2689 2020-02-02 00:00:00.000000 opuscleaner-0.1/dump-parameter-schema.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 opuscleaner-0.1/requirements-all.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 opuscleaner-0.1/requirements.txt
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 opuscleaner-0.1/.vscode/extensions.json
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/__init__.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/categories.py
--rwxr-xr-x   0        0        0    20648 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/clean.py
--rwxr-xr-x   0        0        0     2013 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/col.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/config.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/datasets.py
--rw-r--r--   0        0        0     8901 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/download.py
--rwxr-xr-x   0        0        0     4531 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/sample.py
--rw-r--r--   0        0        0    18503 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/server.py
--rwxr-xr-x   0        0        0     8153 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/threshold.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/alpha_ratio.json
--rwxr-xr-x   0        0        0     3974 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/alpha_ratio.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/bicleaner_hardrules.json
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/bifixer.json
--rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/bifixer_dedupe.py
--rwxr-xr-x   0        0        0     2410 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/clean_common.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/deescape-special-chars.json
--rwxr-xr-x   0        0        0      631 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/deescape-special-chars.perl
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/deescape_tsv.json
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/deescape_tsv.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/detokenizer.json
--rwxr-xr-x   0        0        0    12473 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/detokenizer.perl
--rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/fasttext_filter.json
--rwxr-xr-x   0        0        0     3171 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/fasttext_filter.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/fix_elitr_eca.json
--rwxr-xr-x   0        0        0     1473 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/fix_elitr_eca.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/fix_quotes.json
--rwxr-xr-x   0        0        0      320 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/fix_quotes.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/fix_un_chinese.json
--rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/fix_un_chinese.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/fix_wiki.json
--rwxr-xr-x   0        0        0     3567 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/fix_wiki.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/head.json
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/jieba.json
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/langid.json
--rwxr-xr-x   0        0        0     3017 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/langid.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/laser_similarity.json
--rwxr-xr-x   0        0        0     4510 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/laser_similarity.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/max_length.json
--rwxr-xr-x   0        0        0     1539 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/max_length.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/max_word_length.json
--rwxr-xr-x   0        0        0      862 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/max_word_length.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/num_mismatch.json
--rwxr-xr-x   0        0        0     1246 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/num_mismatch.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/regexp.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/remove_empty_lines.json
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/remove_frequent_patterns.json
--rwxr-xr-x   0        0        0     2696 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/remove_frequent_patterns.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/remove_frequent_patterns.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/sed.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/segment_chinese.json
--rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/segment_chinese.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/segment_japanese.json
--rwxr-xr-x   0        0        0      588 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/segment_japanese.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/simplify_chinese.json
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/split_sentences.json
--rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/split_sentences.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/src_trg_ratio.json
--rwxr-xr-x   0        0        0     2291 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/src_trg_ratio.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/strip_suffix.json
--rwxr-xr-x   0        0        0     2269 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/strip_suffix.py
--rw-r--r--   0        0        0   376832 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/test.bin
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/test.tsv
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/filters/traditionalise_chinese.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 opuscleaner-0.1/.gitignore
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 opuscleaner-0.1/README.md
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 opuscleaner-0.1/pyproject.toml
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/index.html
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/AddDatasetView.4182f0f7.css
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/AddDatasetView.5dcf722c.js
--rw-r--r--   0        0        0   118077 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/EditFiltersView.272e0d14.js
--rw-r--r--   0        0        0     8929 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/EditFiltersView.4490d98b.css
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/EditFiltersYamlView.45bdcb50.js
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/ListDatasetsView.02d1a0b3.css
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/ListDatasetsView.1513f813.js
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/TagsEditor.8b755087.js
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css
--rw-r--r--   0        0        0    38943 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/data-cuate.84693c76.svg
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg
--rw-r--r--   0        0        0    22166 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/eu.24cff2c1.png
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/filtersteps.2a7228ad.js
--rw-r--r--   0        0        0   101750 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/horizon-europe.80625b0c.png
--rw-r--r--   0        0        0   123668 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/index.490d1368.js
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/index.a7233265.css
--rw-r--r--   0        0        0    17440 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/vue-select.6aaeaff8.js
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 opuscleaner-0.1/opuscleaner/frontend/assets/vue-select.b0fac2a1.css
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 opuscleaner-0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     2689 2020-02-02 00:00:00.000000 opuscleaner-0.2/dump-parameter-schema.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 opuscleaner-0.2/requirements-all.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 opuscleaner-0.2/requirements.txt
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/index.html
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/AddDatasetView.4182f0f7.css
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/AddDatasetView.ff526466.js
+-rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/EditFiltersView.a7795492.css
+-rw-r--r--   0        0        0   121398 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/EditFiltersView.bc0dd7c3.js
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/EditFiltersYamlView.28a1a7c9.js
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/ListDatasetsView.0c61d7cc.js
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/ListDatasetsView.79aac80d.css
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/TagsEditor.23cf196f.js
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css
+-rw-r--r--   0        0        0    38943 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/data-cuate.84693c76.svg
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg
+-rw-r--r--   0        0        0    22166 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/eu.24cff2c1.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/hacks.1ae1ba64.js
+-rw-r--r--   0        0        0   101750 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/horizon-europe.80625b0c.png
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/index.47848488.css
+-rw-r--r--   0        0        0   124624 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/index.6cc31f0d.js
+-rw-r--r--   0        0        0    17440 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/vue-select.9ddbca8a.js
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/vue-select.b0fac2a1.css
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/_util.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/categories.py
+-rwxr-xr-x   0        0        0    21105 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/clean.py
+-rwxr-xr-x   0        0        0     2015 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/col.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/config.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/datasets.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/download.py
+-rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters.py
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/opusfilter_compat.py
+-rwxr-xr-x   0        0        0     4581 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/sample.py
+-rw-r--r--   0        0        0    16891 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/server.py
+-rwxr-xr-x   0        0        0     8153 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/threshold.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/alpha_ratio.json
+-rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/alpha_ratio.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/bicleaner_hardrules.json
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/bifixer.json
+-rwxr-xr-x   0        0        0      454 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/bifixer_dedupe.py
+-rwxr-xr-x   0        0        0     2440 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/clean_common.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/deescape-special-chars.json
+-rwxr-xr-x   0        0        0      631 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/deescape-special-chars.perl
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/deescape_tsv.json
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/deescape_tsv.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/detokenizer.json
+-rwxr-xr-x   0        0        0    12473 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/detokenizer.perl
+-rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fasttext_filter.json
+-rwxr-xr-x   0        0        0     3173 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fasttext_filter.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_elitr_eca.json
+-rwxr-xr-x   0        0        0     1473 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_elitr_eca.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_quotes.json
+-rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_quotes.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_un_chinese.json
+-rwxr-xr-x   0        0        0      354 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_un_chinese.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_wiki.json
+-rwxr-xr-x   0        0        0     3569 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_wiki.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/langid.json
+-rwxr-xr-x   0        0        0     3019 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/langid.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/laser_similarity.json
+-rwxr-xr-x   0        0        0     4525 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/laser_similarity.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/max_length.json
+-rwxr-xr-x   0        0        0     1545 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/max_length.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/max_word_length.json
+-rwxr-xr-x   0        0        0      869 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/max_word_length.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/num_mismatch.json
+-rwxr-xr-x   0        0        0     1248 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/num_mismatch.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/regexp.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/remove_empty_lines.json
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/remove_frequent_patterns.json
+-rwxr-xr-x   0        0        0     2700 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/remove_frequent_patterns.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/remove_frequent_patterns.txt
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/sed.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/segment_chinese.json
+-rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/segment_chinese.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/segment_japanese.json
+-rwxr-xr-x   0        0        0      588 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/segment_japanese.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/simplify_chinese.json
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/split_sentences.json
+-rwxr-xr-x   0        0        0     1059 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/split_sentences.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/src_trg_ratio.json
+-rwxr-xr-x   0        0        0     2298 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/src_trg_ratio.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/strip_suffix.json
+-rwxr-xr-x   0        0        0     2271 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/strip_suffix.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/traditionalise_chinese.json
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/AlphabetRatioFilter.json
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/AverageWordLengthFilter.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/CharacterScoreFilter.json
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/Detokenizer.json
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/HtmlTagFilter.json
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/LengthFilter.json
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/LengthRatioFilter.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/LongWordFilter.json
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/RegExpFilter.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/RegExpSub.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/Tokenizer.json
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/WhitespaceNormalizer.json
+-rwxr-xr-x   0        0        0     1808 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/opusfilter-ersatz.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 opuscleaner-0.2/utils/dedup/README.md
+-rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 opuscleaner-0.2/utils/dedup/dedup.sh
+-rwxr-xr-x   0        0        0     1046 2020-02-02 00:00:00.000000 opuscleaner-0.2/utils/dedup/hash-seg.py
+-rwxr-xr-x   0        0        0      906 2020-02-02 00:00:00.000000 opuscleaner-0.2/utils/dedup/superdedup.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 opuscleaner-0.2/.gitignore
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 opuscleaner-0.2/README.md
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 opuscleaner-0.2/pyproject.toml
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 opuscleaner-0.2/PKG-INFO
```

### Comparing `opuscleaner-0.1/dump-parameter-schema.py` & `opuscleaner-0.2/dump-parameter-schema.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/categories.py` & `opuscleaner-0.2/opuscleaner/categories.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 import os
 import json
 from fastapi import FastAPI
 from pydantic import BaseModel, parse_obj_as, validator
-from typing import List, Dict, TextIO, cast
+from typing import Any, List, Dict, TextIO, cast
 
-from .config import CATEGORIES_PATH, DATA_PATH, DEFAULT_CATEGORIES
+from opuscleaner.config import CATEGORIES_PATH, DATA_PATH, DEFAULT_CATEGORIES
 
 
 class Category(BaseModel):
 	name: str
 
 	@validator('name')
-	def name_must_not_be_empty(cls, value):
+	def name_must_not_be_empty(cls, value:str) -> str:
 		assert len(value.strip()) > 0, 'must not be empty'
 		return value.strip()
 
 
 class CategoryMapping(BaseModel):
 	categories: List[Category]
 	mapping: Dict[str,List[str]]
 
 	@validator('categories')
-	def categories_must_be_unique(cls, value):
+	def categories_must_be_unique(cls, value:List[Category]) -> List[Category]:
 		assert len(set(category.name.strip() for category in value)) == len(value), 'categories must have unique names'
 		return value
 
 	@validator('mapping')
-	def mapping_must_only_contain_categories(cls, value, values, **kwargs):
+	def mapping_must_only_contain_categories(cls, value:Dict[str,List[str]], values: Dict[str,Any], **kwargs) -> Dict[str,List[str]]:
 		assert len(set(value.keys()) - set(category.name.strip() for category in values.get('categories', ''))) == 0, 'mapping must only contain keys that are defined in `categories`'
 		return value
 
 
-def read_categories(fh: TextIO):
+def read_categories(fh:TextIO) -> CategoryMapping:
 	return parse_obj_as(CategoryMapping, json.load(fh))
 
-def write_categories(mapping: CategoryMapping, fh: TextIO):
+def write_categories(mapping:CategoryMapping, fh:TextIO) -> None:
 	json.dump(mapping.dict(), fh, indent=2)
 
 
 app = FastAPI()
 
 @app.get('/')
 def get_mapping() -> CategoryMapping:
 	if os.path.exists(CATEGORIES_PATH):
 		with open(CATEGORIES_PATH, 'r') as fh:
 			return read_categories(fh)
 	else:
 		return CategoryMapping(categories=DEFAULT_CATEGORIES, mapping=dict())
 
 @app.put('/')
-def update_categories(body: CategoryMapping):
+def update_categories(body:CategoryMapping) -> None:
 	with open(CATEGORIES_PATH, 'w') as fh:
 		write_categories(body, fh)
```

### Comparing `opuscleaner-0.1/opuscleaner/clean.py` & `opuscleaner-0.2/opuscleaner/clean.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,59 +7,47 @@
 import argparse
 import json
 import os
 import shlex
 import signal
 import sys
 import traceback
+from contextlib import ExitStack
 from glob import glob
 from pprint import pprint
 from queue import Queue, SimpleQueue
 from shlex import quote
 from shutil import copyfileobj
 from subprocess import Popen, PIPE
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from threading import Thread
 from typing import Dict, List, Any, BinaryIO, Optional, TypeVar, Iterable, Tuple, NamedTuple, Union
 
-from .config import COL_PY
+from pydantic import parse_obj_as
 
+from opuscleaner.config import COL_PY, FILTER_PATH
+from opuscleaner.filters import list_filters, set_global_filters, filter_format_command, Filter, FilterStep, FilterPipeline
+from opuscleaner._util import none_throws
 
-T = TypeVar("T")
 
-def none_throws(optional: Optional[T], message: str = "Unexpected `None`") -> T:
-    if optional is None:
-        raise AssertionError(message)
-    return optional
+# Queue for printing lines to stdout or stderr. None means end of input.
+PrintQueue = SimpleQueue[Union[None,bytes]]
 
+# Control queue for communicating the return code of a child back to the parent.
+ControlQueue = SimpleQueue[Tuple[int,int]]
 
-def encode_env(type_name: str, value: Any) -> str:
-    if type_name == 'bool':
-        return '1' if value else ''
-    else:
-        return str(value)
+# Batches to be processed. tuple[batch index,batch path]. None means end of input.
+# Using a Queue here to limit the maximum capacity.
+BatchQueue = Queue[Union[None,Tuple[int,str]]]
 
-
-def list_filters(path: str) -> Iterable[dict]:
-    """Scans all files matching the path pattern and attempts to parse them as
-    filter json definitions.
-    """
-    for filename in glob(path, recursive=True):
-        try:
-            with open(filename) as fh:
-                defaults = {
-                    "name": os.path.splitext(os.path.basename(filename))[0],
-                    "basedir": os.path.dirname(filename)
-                }
-                yield {**defaults, **json.load(fh)}
-        except Exception as e:
-            print(f"Could not parse {filename}: {e}", file=sys.stderr)
+# Batches to be merged. Same format as BatchQueue
+MergeQueue = SimpleQueue[Union[None,Tuple[int,str]]]
 
 
-def babysit_child(n: int, child: Popen, name: str, print_queue: SimpleQueue, ctrl_queue: SimpleQueue):
+def babysit_child(n: int, child: Popen, name: str, print_queue: PrintQueue, ctrl_queue: ControlQueue) -> None:
     """Thread that looks after a child process and passes (and prefixes) all of
     its stderr to a queue. It will tell the parent thread about the end of the
     child through the ctrl_queue.
     """
     prefix = f'[{name}] '.encode()
 
     for line in none_throws(child.stderr):
@@ -68,15 +56,15 @@
     child.wait()
 
     print_queue.put(f'[run.py] {name} exited with status code {child.returncode}\n'.encode())
 
     ctrl_queue.put((n, child.returncode))
 
 
-def print_lines(queue: SimpleQueue, fout: BinaryIO):
+def print_lines(queue: PrintQueue, fout: BinaryIO) -> None:
     """Thread that prints stderr lines from all the children to stderr in an
     orderly fashion.
     """
     while True:
         line = queue.get()
         if line is None:
             break
@@ -109,47 +97,47 @@
     babysitter: Thread
 
 
 class ProcessPipeline:
     """Context manager for spawning and babysitting child processes that are
     siblings connected by their pipes.
     """
-    ctrl_queue: SimpleQueue
+    ctrl_queue: ControlQueue
 
-    print_queue: SimpleQueue
+    print_queue: PrintQueue
 
     environ: Dict[str,str]
 
     children: List[Child]
 
-    def __init__(self, print_queue: SimpleQueue, *, env:Dict[str,str]={}):
+    def __init__(self, print_queue: PrintQueue, *, env:Dict[str,str]={}):
         self.ctrl_queue = SimpleQueue()
         self.print_queue = print_queue
         self.environ = dict(env)
         self.children = []
 
     def start(self, name:str, cmd: Union[str,List[str]], **kwargs) -> Popen:
         child = Popen(cmd, **{
             **kwargs,
             'env': {
                 **os.environ,
                 **self.environ,
-                **kwargs.get('env', dict())
+                **(kwargs.get('env') or dict())
             }
         })
         n = len(self.children)
         thread = Thread(target=babysit_child, args=[n, child, name, self.print_queue, self.ctrl_queue])
         thread.start()
         self.children.append(Child(name, child, thread))
         return child
 
-    def __enter__(self):
+    def __enter__(self) -> 'ProcessPipeline':
         return self
 
-    def __exit__(self, err_type, err_inst, err_trace):
+    def __exit__(self, err_type, err_inst, err_trace) -> None:
         # Wait for the children to exit, and depending on their retval exit early
         running_children = len(self.children)
 
         print(f"Waiting for {running_children} subprocesses to finish...", file=sys.stderr)
 
         if err_type:
             for child in self.children:
@@ -168,15 +156,15 @@
         except KeyboardInterrupt:
             # TODO: Wait, how does the interrupt stop the children?
             print('[run.py] KeyboardInterrupt', file=sys.stderr)
             pass
 
         # If supported, print usage for each child?
         if False and os.path.isdir('/proc'):
-            for child in children:
+            for child in self.children:
                 with open(f'/proc/{child.process.pid}/stat', 'r') as fh:
                     sys.stderr.write(child.name + "\t")
                     sys.stderr.write(fh.readline())
 
         # Wait for all the processes to prevent zombies
         for child in self.children:
             if child.process.returncode is None:
@@ -195,51 +183,55 @@
 
 class PipelineStep(NamedTuple):
     command: str
     basedir: str
 
 
 class Pipeline:
-    def __init__(self, filters: Dict[str,Dict], languages: List[str], pipeline: List[Dict]):
+    def __init__(self, filters:Dict[str,Filter], languages: List[str], pipeline: FilterPipeline):
         self.steps: List[PipelineStep] = []
 
-        # Assert we have all filters we need
-        assert set(step['filter'] for step in pipeline['filters']) - set(filters.keys()) == set()
-
-        for step in pipeline['filters']:
-            filter_definition = filters[step['filter']]
-            
-            if filter_definition['type'] == 'bilingual':
-                command = filter_definition['command']
-            elif filter_definition['type'] == 'monolingual':
-                column = languages.index(step['language'])
-                command = f'{" ".join(map(shlex.quote, COL_PY))} {column} {filter_definition["command"]}'
-            else:
-                raise NotImplementedError()
-
-            # List of k=v shell variable definitions
-            filter_params = [
-                '{}={}'.format(name, quote(encode_env(props['type'], step['parameters'].get(name, props.get('default', None)))))
-                for name, props in filter_definition['parameters'].items()
-            ]
+        # Make sure the path to the python binary (and the installed utils)
+        # is in the PATH variable. If you load a virtualenv this happens by
+        # default, but if you call it with the virtualenv's python binary 
+        # directly it wont.
+        pyenv_bin_path = os.path.dirname(sys.executable)
+        os_env_bin_paths = os.environ.get('PATH', '').split(os.pathsep)
+        self.env: Optional[Dict[str,str]] = {
+            **os.environ,
+            'PATH': os.pathsep.join([pyenv_bin_path] + os_env_bin_paths)
+        } if pyenv_bin_path not in os_env_bin_paths else None
 
-            # Command, prefixed by variable definitions so they get expanded
-            # correctly in the command bit.
-            command_str = '; '.join(filter_params + [command])
+        # Assert we have all filters we need
+        assert set(step.filter for step in pipeline.filters) - set(filters.keys()) == set()
 
-            self.steps.append(PipelineStep(command_str, filter_definition['basedir']))
+        # Make sure the path to the python binary (and the installed utils)
+        # is in the PATH variable. If you load a virtualenv this happens by
+        # default, but if you call it with the virtualenv's python binary 
+        # directly it wont.
+        pyenv_bin_path = os.path.dirname(sys.executable)
+        os_env_bin_paths = os.environ.get('PATH', '').split(os.pathsep)
+        self.env: Optional[Dict[str,str]] = {
+            **os.environ,
+            'PATH': os.pathsep.join([pyenv_bin_path] + os_env_bin_paths)
+        } if pyenv_bin_path not in os_env_bin_paths else None
+
+        for step in pipeline.filters:
+            filter_def = filters[step.filter]
+            command_str = filter_format_command(filter_def, step, languages)
+            self.steps.append(PipelineStep(command_str, filter_def.basedir))
 
-    def run(self, pool:ProcessPipeline, stdin:BinaryIO, stdout:BinaryIO, *, tee:bool=False, basename:str=""):
+    def run(self, pool:ProcessPipeline, stdin:BinaryIO, stdout:BinaryIO, *, tee:bool=False, basename:str="") -> None:
         for i, (is_last_step, step) in enumerate(mark_last(self.steps)):
-        
             child = pool.start(f'step {i}', step.command,
                 stdin=stdin,
                 stdout=stdout if is_last_step and not tee else PIPE,
                 stderr=PIPE,
                 cwd=step.basedir,
+                env=self.env,
                 shell=True)
 
             # Close our reference to the previous child, now taken over by the next child
             stdin.close()
             
             # Set stdin for next step (unless there is none, then child.stdout is None)
             if not is_last_step and not tee:
@@ -256,15 +248,15 @@
                     stdout=stdout if is_last_step else PIPE,
                     stderr=PIPE)
 
                 stdin.close()
                 stdin = none_throws(tee_child.stdout)
 
 
-def split_input(print_queue:SimpleQueue, parallel: int, batch_queue: Queue, batch_size:int, stdin:BinaryIO):
+def split_input(print_queue:PrintQueue, parallel: int, batch_queue: BatchQueue, batch_size:int, stdin:BinaryIO) -> None:
     """Reads data from `stdin` and splits it into chunks of `batch_size` lines.
     These chunks are stored in temporary files, whose filenames are put onto
     `batch_queue`.
     """
     more = True
 
     batch_index = 0
@@ -297,15 +289,15 @@
             batch_index += 1
     finally:
         # In any scenario, tell all the runners there will be no more batches coming.
         for _ in range(parallel):
             batch_queue.put(None)
 
 
-def run_pipeline(print_queue:SimpleQueue, batch_queue: Queue, merge_queue: SimpleQueue, pipeline: Pipeline):
+def run_pipeline(print_queue:PrintQueue, batch_queue:BatchQueue, merge_queue:MergeQueue, pipeline:Pipeline) -> None:
     """Receives an input filename from `batch_queue`, and once that has been processed
     with `pipeline`, it will post the output filename to `merge_queue`.
 
     TODO: This could also instead run ./run.py on the input and output files
     directly as opposed to using `ProcessPipeline` + `pipeline.run()`.
 
     TODO: We can rewrite this to call `srun` on SLUM clusters so that the
@@ -343,15 +335,15 @@
                     os.unlink(filename)
     finally:
         # In any case, tell the merger that they should not be expecting more
         # input from you.
         merge_queue.put(None)
 
 
-def merge_output(print_queue:SimpleQueue, parallel: int, merge_queue: SimpleQueue, stdout:BinaryIO):
+def merge_output(print_queue:PrintQueue, parallel:int, merge_queue:MergeQueue, stdout:BinaryIO) -> None:
     """Takes batch filenames and numbers from `merge_queue` and will concatenate
     files in the order of the batches. If batches arrive out of order, it will
     wait for the next in order batch to arrive before continuing to concatenate.
     """
     next_batch_index = 0
 
     pending_batches: Dict[int, str] = {}
@@ -383,18 +375,18 @@
 
             batch_index, filename = entry
 
             assert batch_index not in pending_batches
             pending_batches[batch_index] = filename
 
 
-def run_parallel(pipeline:Pipeline, stdin:BinaryIO, stdout:BinaryIO, *, parallel:int, batch_size:int, print_queue: SimpleQueue):
-    batch_queue = Queue(parallel * 2)
+def run_parallel(pipeline:Pipeline, stdin:BinaryIO, stdout:BinaryIO, *, parallel:int, batch_size:int, print_queue: PrintQueue) -> None:
+    batch_queue: BatchQueue = Queue(parallel * 2)
 
-    merge_queue = SimpleQueue()
+    merge_queue: MergeQueue = SimpleQueue()
 
     # Splits stdin into files of `batch_size` lines, and puts those on `batch_queue`
     splitter = Thread(target=split_input, args=[print_queue, parallel, batch_queue, batch_size, stdin])
     splitter.start();
 
     # Read `batch_queue` for batch filenames, and process them. Put output files
     # on `merge_queue`.
@@ -423,17 +415,17 @@
     for runner in runners:
         runner.join()
 
     print_queue.put(f'[run.py] Waiting for merger to finish\n'.encode())
     merger.join()
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser()
-    parser.add_argument('--filters', '-f', type=str, default='./filters', help='Path to directory with filter specifications')
+    parser.add_argument('--filters', '-f', type=str, default=FILTER_PATH, help='Path to directory with filter specifications')
     parser.add_argument('--input', '-i', type=argparse.FileType('rb'), help='Input tsv. If unspecified input files are read from filter json; use - to read from stdin')
     parser.add_argument('--output', '-o', type=argparse.FileType('wb'), default=sys.stdout.buffer, help='Output tsv (defaults to stdout)')
     parser.add_argument('--basedir', '-b', type=str, help='Directory to look for data files when --input is not used (defaults to same as input pipeline file)')
     parser.add_argument('--tee', action='store_true', help='Write output after each step to a separate file')
     parser.add_argument('--parallel', type=int, default=1, help='Run N parallel copies of the pipeline processing batches')
     parser.add_argument('--batch-size', type=int, default=1_000_000, help='Batch size in lines that each parallel copy processes (only if --parallel > 1)')
     parser.add_argument('--first', type=int, default=0, help='Limit reading input to the N first lines')
@@ -441,43 +433,45 @@
     parser.add_argument('languages', metavar='LANG', type=str, nargs='*', help='Language codes of the columns in the input TSV. Only used when --input is set')
 
     args = parser.parse_args()
 
     # default search path for the data files is next to the configuration file
     # which is the default save location for empty-train.
     if not args.basedir:
-        args.basedir = os.path.dirname(args.pipeline.name)
+        args.basedir = os.path.dirname(args.pipeline.name) or os.getcwd()
 
     if args.input is not None and not args.languages:
         parser.error('When --input is specified, each colum\'s LANG has to be specified as well.')
 
-    pipeline_config = json.load(args.pipeline)
-
     # load all filter definitions (we need to, to get their name)
-    FILTERS = {
-        definition['name']: definition
-        for definition in list_filters(os.path.join(args.filters, '*.json'))
+    filters = {
+        definition.name: definition
+        for definition in list_filters(args.filters)
     }
 
+    # set_global_filters() provides the filters to the validators in FilterPipeline
+    set_global_filters(filters)
+    pipeline_config = parse_obj_as(FilterPipeline, json.load(args.pipeline))
+
     # Queue filled by the babysitters with the stderr of the children, consumed
     # by `print_lines()` to prevent racing on stderr.
     print_queue = SimpleQueue() # type: SimpleQueue[Optional[bytes]]
 
     # First start the print thread so that we get immediate feedback from the
     # children even if all of them haven't started yet.
     print_thread = Thread(target=print_lines, args=[print_queue, sys.stderr.buffer])
     print_thread.start()
 
     # Order of columns. Matches datasets.py:list_datasets(path)
-    languages: List[str] = args.languages if args.input else [filename.rsplit('.', 2)[1] for filename in pipeline_config['files']]
+    languages: List[str] = args.languages if args.input else [filename.rsplit('.', 2)[1] for filename in pipeline_config.files]
 
     # Directory plus basename to write debug (`--tee`) files to
-    basename: str = 'stdin' if args.input else os.path.commonprefix(pipeline_config['files']).rstrip('.')
+    basename: str = 'stdin' if args.input else os.path.commonprefix(pipeline_config.files).rstrip('.')
 
-    pipeline = Pipeline(FILTERS, languages, pipeline_config)
+    pipeline = Pipeline(filters, languages, pipeline_config)
 
     # Input for next child
     stdin: BinaryIO
 
     # Output of this program
     stdout:BinaryIO = args.output
 
@@ -491,15 +485,15 @@
                 # Open `gzunip` for each language file
                 gunzips = [
                     pool.start(f'gunzip {filename}',
                         ['gzip', '-cd', filename],
                         stdout=PIPE,
                         stderr=PIPE,
                         cwd=args.basedir)
-                    for filename in pipeline_config['files']
+                    for filename in pipeline_config.files
                 ]
 
                 fds = [none_throws(gunzip.stdout).fileno() for gunzip in gunzips]
 
                 # .. and a `paste` to combine them into columns
                 paste = pool.start('paste',
                     ['paste'] + [f'/dev/fd/{fd}' for fd in fds],
```

### Comparing `opuscleaner-0.1/opuscleaner/col.py` & `opuscleaner-0.2/opuscleaner/col.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         raise AssertionError(message)
     return optional
 
 
 def split(column, queue, fin, fout):
 	try:
 		for line in fin:
-			fields = line.rstrip(b'\n').split(b'\t')
+			fields = line.rstrip(b'\r\n').split(b'\t')
 			field = fields[column] # Doing column selection first so that if this fails, we haven't already written it to the queue
 			queue.put(fields[:column] + fields[(column+1):])
 			fout.write(field + b'\n')
 		fout.close()
 	except BrokenPipeError:
 		pass
 	finally:
```

### Comparing `opuscleaner-0.1/opuscleaner/config.py` & `opuscleaner-0.2/opuscleaner/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,23 +15,25 @@
 ]
 
 # TODO: Derive this from DATA_PATH. The `train-parts` is a mtdata compatibility
 # thing. I'm now used to also have a data/clean directory there, so keeping it.
 DOWNLOAD_PATH = 'data/train-parts'
 
 # glob expression that looks for the filter files. Unfortunately you can't use
-# commas and {} in this expression. TODO: fix that, you should be able to name
-# multiple paths.
-FILTER_PATH = os.path.join(os.path.dirname(__file__), 'filters/*.json')
+# commas and {} in this expression.
+FILTER_PATH = os.pathsep.join([
+	'filters/**/*.json',
+	os.path.join(os.path.dirname(__file__), 'filters/**/*.json')
+])
 
 # col.py is used to apply a monolingual filter to a bilingual dataset. Needs
 # to be absolute since filters can run from different cwds.
-COL_PY = [sys.executable, '-m', 'opuscleaner.col']
+COL_PY = [sys.executable, os.path.join(os.path.dirname(__file__), 'col.py')]
 
 # Program used to derive a sample from the dataset. Will be called like
 # `./sample.py -n $SAMPLE_SIZE ...file-per-lang.gz`. Absolute because filters
 # can specify their own `cwd`.
-SAMPLE_PY = [sys.executable, '-m', 'opuscleaner.sample']
+SAMPLE_PY = [sys.executable, os.path.join(os.path.dirname(__file__), 'sample.py')]
 
 # Size of each of the three sections (head, random sample of middle, tail) of
 # the dataset sample that we operate on.
 SAMPLE_SIZE = int(os.getenv('SAMPLE_SIZE', '1000'))
```

### Comparing `opuscleaner-0.1/opuscleaner/datasets.py` & `opuscleaner-0.2/opuscleaner/datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 #!/usr/bin/env python3
 """Lists datasets given a directory. It works by scanning the directory and looking for gz files."""
 import os
-import glob
+from functools import wraps
+from glob import glob
 from itertools import groupby
-from pathlib import Path
+from pathlib import Path as Path
 from typing import Iterable, Dict
 
 
-def _glob(*args, **kwargs) -> Iterable[Path]:
-    for entry in glob.glob(*args, **kwargs):
-        yield Path(entry)
-
-
-def list_datasets(path) -> Dict[str,Dict[str,Path]]:
+def list_datasets(path:str) -> Dict[str,Dict[str,Path]]:
     """Lists datasets given a directory. Scans the directories and returns a dictionary of the
     datasets encoutered. Dictionary looks like {dataset_name : { lang: path}}"""
     root = Path(path.split('*')[0])
 
+    entries = (Path(entry) for entry in glob(path, recursive=True))
+
     files = [
         entry
-        for entry in _glob(path, recursive=True)
+        for entry in entries
         if entry.is_file()
         and entry.name.endswith('.gz')
         and not entry.name.startswith('.')
     ]
 
     datasets = [
         (name, list(files))
@@ -38,15 +36,15 @@
             for entry in files
         }
         for name, files in datasets
         if len(files) > 1
     }
 
 
-def main():
+def main() -> None:
     import sys
     import pprint
     pprint.pprint(list_datasets(sys.argv[1]))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `opuscleaner-0.1/opuscleaner/download.py` & `opuscleaner-0.2/opuscleaner/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 import asyncio
 import json
 import gzip
 from glob import iglob
 from itertools import chain
-from typing import Iterable, Dict, List, Optional, Set, Union, Tuple, cast
+from typing import Iterable, Dict, List, Optional, Set, Union, Tuple, cast, Any
 from enum import Enum
 from queue import SimpleQueue
 from subprocess import Popen, PIPE
 from threading import Thread
 from collections import defaultdict
 from urllib.request import Request, urlopen
 from urllib.parse import urlencode
@@ -22,15 +22,15 @@
 from shutil import copyfileobj
 from multiprocessing import Process
 from zipfile import ZipFile
 
 from pydantic import BaseModel
 from fastapi import FastAPI, HTTPException
 
-from .config import DATA_PATH, DOWNLOAD_PATH
+from opuscleaner.config import DATA_PATH, DOWNLOAD_PATH
 
 
 class EntryRef(BaseModel):
     id: int
 
 
 class Entry(EntryRef):
@@ -57,15 +57,15 @@
     PENDING = 'pending'
     CANCELLED = 'cancelled'
     DOWNLOADING = 'downloading'
     DOWNLOADED = 'downloaded'
     FAILED = 'failed'
 
 
-def get_dataset(entry: RemoteEntry, path: str):
+def get_dataset(entry:RemoteEntry, path:str) -> None:
     # List of extensions of the expected files, e.g. `.en-mt.mt` and `.en-mt.en`.
     suffixes = [f'.{"-".join(entry.langs)}.{lang}' for lang in entry.langs]
 
     with TemporaryFile() as temp_archive:
         # Download zip file to temporary file
         with urlopen(entry.url) as fh:
             copyfileobj(fh, temp_archive)
@@ -103,58 +103,61 @@
     entry: RemoteEntry
     _child: Optional[Process]
 
     def __init__(self, entry:RemoteEntry):
         self.entry = entry
         self._child = None
     
-    def start(self):
+    def start(self) -> None:
         self._child = Process(target=get_dataset, args=(self.entry, DOWNLOAD_PATH))
         self._child.start()
 
-    def run(self):
+    def run(self) -> None:
         self.start()
         assert self._child is not None
         self._child.join()
 
-    def cancel(self):
+    def cancel(self) -> None:
         if self._child and self._child.exitcode is None:
             self._child.kill()
 
     @property
-    def state(self):
+    def state(self) -> DownloadState:
         if not self._child:
             return DownloadState.PENDING
         elif self._child.exitcode is None:
             return DownloadState.DOWNLOADING
         elif self._child.exitcode == 0:
             return DownloadState.DOWNLOADED
         elif self._child.exitcode > 0:
             return DownloadState.FAILED
         else:
             return DownloadState.CANCELLED
 
 
+DownloadQueue = SimpleQueue[Optional[EntryDownload]]
+
+
 class Downloader:
     def __init__(self, workers:int):
-        self.queue = SimpleQueue()
-        self.threads = []
+        self.queue: DownloadQueue = SimpleQueue()
+        self.threads: List[Thread] = []
 
         for _ in range(workers):
             thread = Thread(target=self.__class__.worker_thread, args=[self.queue], daemon=True)
             thread.start()
             self.threads.append(thread)
 
     def download(self, entry:RemoteEntry) -> EntryDownload:
         download = EntryDownload(entry=entry)
         self.queue.put(download)
         return download
 
     @staticmethod
-    def worker_thread(queue):
+    def worker_thread(queue:DownloadQueue) -> None:
         while True:
             entry = queue.get()
             if not entry:
                 break
             entry.run()
 
 
@@ -164,26 +167,26 @@
 
 
 class OpusAPI:
     endpoint: str
 
     _datasets: Dict[int,Entry] = {}
 
-    def __init__(self, endpoint):
+    def __init__(self, endpoint:str):
         self.endpoint = endpoint
         self._datasets = {}
 
     def languages(self, lang1: Optional[str] = None) -> List[str]:
         query = {'languages': 'True'}
 
         if lang1 is not None:
             query['source'] = lang1
 
         with urlopen(f'{self.endpoint}?{urlencode(query)}') as fh:
-            return json.load(fh).get('languages', [])
+            return [str(lang) for lang in json.load(fh).get('languages', [])]
 
     def get_dataset(self, id:int) -> Entry:
         return self._datasets[id]
 
     def find_datasets(self, lang1:str, lang2:str) -> List[Entry]:
         query = {
             'source': lang1,
@@ -208,28 +211,28 @@
 
 downloads: Dict[int,EntryDownload] = {}
 
 downloader = Downloader(2)
 
 datasets_by_id: Dict[int, Entry] = {}
 
-def cast_entry(data) -> Entry:
+def cast_entry(data:Dict[str,Any]) -> Entry:
     entry = Entry(
         id=int(data['id']),
         corpus=str(data['corpus']),
         version=str(data['version']),
         pairs=int(data['alignment_pairs']) if data.get('alignment_pairs') != '' else None,
         size=int(data['size']) * 1024, # FIXME file size but do we care?
         langs=(data['source'], data['target']), # FIXME these are messy OPUS-API lang codes :(
     )
 
     paths = set(
         filename
         for data_root in [os.path.dirname(DATA_PATH), DOWNLOAD_PATH]
-        for lang in cast(Tuple[str,str], entry.langs)
+        for lang in entry.langs
         for filename in iglob(os.path.join(data_root, f'{entry.basename}.{lang}.gz'), recursive=True)
     )
 
     # Print search paths
     # print('\n'.join(
     #     filename
     #     for data_root in [os.path.dirname(DATA_PATH), DOWNLOAD_PATH]
@@ -284,15 +287,15 @@
         assert isinstance(entry, RemoteEntry)
         downloads[entry.id] = downloader.download(entry)
 
     return list_downloads()
 
 
 @app.delete('/downloads/{dataset_id}')
-def cancel_download(dataset_id:str) -> EntryDownloadView:
+def cancel_download(dataset_id:int) -> EntryDownloadView:
     """Cancel a download. Removes it from the queue, does not kill the process
     if download is already happening.
     """
     if dataset_id not in downloads:
         raise HTTPException(status_code=404, detail='Download not found')
 
     download = downloads[dataset_id]
```

### Comparing `opuscleaner-0.1/opuscleaner/sample.py` & `opuscleaner-0.2/opuscleaner/sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import subprocess
 import sys
 
 from contextlib import ExitStack, contextmanager
 from itertools import count
 from math import exp, log, floor
 from typing import IO, Iterator
-from typing import TypeVar, Iterable, Iterator, Generic, List, Tuple
+from typing import TypeVar, Iterable, Iterator, Generic, List, Tuple, IO
 
 
 T = TypeVar('T')
 
 
-def reservoir_sample(k:int, it:Iterable[T], *, rand: random.Random = random._inst, sort=False) -> List[T]:
+def reservoir_sample(k:int, it:Iterable[T], *, rand:random.Random = random._inst, sort:bool=False) -> List[T]:
 	"""Take k samples from iterable by reading from start to end. If sort is
 	True, it will return the selected samples in the order they appeared in.
 	"""
 	sample: List[Tuple[int,T]] = []
 
 	numbered_it = enumerate(it)
 
@@ -78,15 +78,15 @@
 		# the entire buffer in one go.
 		if len(self.sample) < self.k:
 			return self.sample
 
 		return self.sample[(self.i % len(self.sample)):] + self.sample[0:(self.i % len(self.sample))]
 
 
-def sample(k:int, iterable:Iterable[T], sort=False) -> Iterable[Iterable[T]]:
+def sample(k:int, iterable:Iterable[T], sort:bool=False) -> Iterable[Iterable[T]]:
 	"""Take `k` items from the start, the end and the middle from `iterable`. If
 	`sort` is True, the items in the middle will be in the order they appeared
 	in."""
 	it = iter(iterable)
 
 	yield (val for _, val in zip(range(k), it))
 
@@ -94,15 +94,15 @@
 
 	yield reservoir_sample(k, tailer, sort=sort)
 
 	yield tailer.tail
 
 
 @contextmanager
-def gunzip(path):
+def gunzip(path:str) -> Iterator[IO[bytes]]:
 	"""Like gzip.open(), but using external gzip process which for some reason
 	is a lot faster on macOS."""
 	with subprocess.Popen(['gzip', '-cd', path], stdout=subprocess.PIPE) as proc:
 		assert proc.stdout is not None
 		yield proc.stdout
 		if proc.wait() != 0:
 			raise RuntimeError(f'gzip returned error code {proc.returncode}')
@@ -116,15 +116,15 @@
 		return ctx.enter_context(gunzip(path))
 	elif path == '-':
 		return sys.stdin.buffer
 	else:
 		return ctx.enter_context(open(path, 'rb'))
 
 
-def main():
+def main() -> None:
 	parser = argparse.ArgumentParser(description="Take a file's head, tail and a random sample from the rest.")
 	parser.add_argument('-n', dest='lines', type=int, default=10, help="number of lines for each section of the sample")
 	parser.add_argument('-d', dest='delimiter', type=str, default="\\t", help="column delimiter. Defaults to \\t.")
 	parser.add_argument('-N', '--line-numbers', action='store_true', help="print line numbers")
 	parser.add_argument('files', metavar='file', type=str, nargs='*', default=['-'], help="files to sample. Multiple files for multiple columns. Use '-' for stdin. If none, reads from stdin.")
 	args = parser.parse_args()
 
@@ -139,14 +139,14 @@
 		delimiter = args.delimiter.replace("\\t", "\t").replace("\\n", "\n").encode()
 
 		for section in sample(args.lines, pairs, sort=True):
 			for pair in section:
 				for col, entry in enumerate(pair):
 					if col > 0:
 						sys.stdout.buffer.write(delimiter)
-					sys.stdout.buffer.write(entry.rstrip(b"\n"))
+					sys.stdout.buffer.write(entry.rstrip(b"\r\n"))
 				sys.stdout.buffer.write(b"\n")
 			sys.stdout.buffer.flush()
 
 
 if __name__ == '__main__':
 	main()
```

### Comparing `opuscleaner-0.1/opuscleaner/server.py` & `opuscleaner-0.2/opuscleaner/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 #!/usr/bin/env python3
 import asyncio
 import gzip
 import hashlib
 import json
 import os
 import re
-import shlex
 import subprocess
 import sys
 import traceback
 from contextlib import ExitStack
 from enum import Enum
 from glob import glob
 from itertools import chain, zip_longest
 from pprint import pprint
-from shlex import quote
 from shutil import copyfileobj
 from tempfile import TemporaryFile
-from typing import NamedTuple, Optional, Iterable, TypeVar, Union, Literal, Any, AsyncIterator, Awaitable, cast, IO, List, Dict, Tuple
+from typing import NamedTuple, Optional, Iterable, TypeVar, Union, Literal, Any, AsyncIterator, Awaitable, cast, IO, List, Dict, Tuple, AsyncIterator
 from warnings import warn
 
+import yaml
 from fastapi import FastAPI, HTTPException
 from fastapi.encoders import jsonable_encoder
 from fastapi.responses import RedirectResponse, StreamingResponse
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel, parse_obj_as, validator, ValidationError
 from starlette.datastructures import URL
-from starlette.exceptions import HTTPException
 from starlette.responses import FileResponse, RedirectResponse, Response
 from starlette.types import Scope
 
-from .categories import app as categories_app
-from .config import DATA_PATH, FILTER_PATH, COL_PY, SAMPLE_PY, SAMPLE_SIZE
-from .datasets import list_datasets, Path
-from .download import app as download_app
-from .sample import sample
+from opuscleaner._util import none_throws
+from opuscleaner.categories import app as categories_app
+from opuscleaner.config import DATA_PATH, FILTER_PATH, COL_PY, SAMPLE_PY, SAMPLE_SIZE
+from opuscleaner.datasets import list_datasets, Path
+from opuscleaner.download import app as download_app
+from opuscleaner.filters import filter_format_command, get_global_filter, get_global_filters, set_global_filters, list_filters, FilterType, FilterStep, FilterPipeline
+from opuscleaner.sample import sample
+
 
 import mimetypes
 mimetypes.add_type('application/javascript', '.js')
 
 
 FRONTEND_PATH = next(iter(path
     for path in [
@@ -55,170 +56,20 @@
 
 
 class Dataset(BaseModel):
     name: str
     columns: Dict[str,File]
 
 
-class FilterType(Enum):
-    BILINGUAL = "bilingual"
-    MONOLINGUAL = "monolingual"
-
-
-class FilterParameterBase(BaseModel):
-    type: str
-    help: Optional[str]
-
-    def export(self, value: Any) -> str:
-        return str(value)
-
-
-class FilterParameterFloat(FilterParameterBase):
-    type: Literal["float"]
-    min: Optional[float]
-    max: Optional[float]
-    default: Optional[float]
-
-
-class FilterParameterInt(FilterParameterBase):
-    type: Literal["int"]
-    min: Optional[int]
-    max: Optional[int]
-    default: Optional[int]
-
-
-class FilterParameterBool(FilterParameterBase):
-    type: Literal["bool"]
-    default: Optional[bool]
-
-    def export(self, value: Any) -> str:
-        return "1" if value else ""
-
-
-class FilterParameterStr(FilterParameterBase):
-    type: Literal["str"]
-    default: Optional[str]
-    allowed_values: Optional[List[str]]
-
-
-FilterParameter = Union[
-    FilterParameterFloat,
-    FilterParameterInt,
-    FilterParameterBool,
-    FilterParameterStr
-]
-
-
-class Filter(BaseModel):
-    type: FilterType
-    name: str # comes from filename by default
-    description: Optional[str]
-    command: str
-    basedir: Optional[str] # same as .json file by default
-    parameters: Dict[str,FilterParameter]
-
-    @validator('parameters')
-    def check_keys(cls, parameters):
-        for var_name in parameters.keys():
-            if not re.match(r"^[a-zA-Z_][a-zA-Z_0-9]*$", var_name):
-                raise ValueError(f"Parameter name is not a valid bash variable: {var_name}")
-        return parameters
-
-
-class FilterStep(BaseModel):
-    filter: str
-    parameters: Dict[str,Any]
-    language: Optional[str]
-
-    @validator('filter')
-    def check_filter(cls, filter):
-        if filter not in FILTERS:
-            raise ValueError(f'Unknown filter `{filter}`')
-        return filter
-
-    @validator('parameters')
-    def check_parameters(cls, parameters, values, **kwargs):
-        if 'filter' in values:
-            required = set(FILTERS[values['filter']].parameters.keys())
-            provided = set(parameters.keys())
-
-            missing_keys = required - provided
-            if missing_keys:
-                warn(f"Missing filter parameters: {' '.join(missing_keys)}")
-                # Just add their default values in that case.
-                parameters |= {
-                    key: parameter.default
-                    for key, parameter in FILTERS[values['filter']].parameters.items()
-                    if key in missing_keys
-                }
-            
-            superfluous_keys = provided - required
-            if superfluous_keys:
-                warn(f"Provided parameters not supported by the filter: {' '.join(superfluous_keys)}")
-                # Not doing anything though, might be that we have just loaded an
-                # old version of the filter definition and we don't want to lose
-                # any of these keys.
-
-        return parameters
-
-    @validator('language', always=True)
-    def check_language_is_provided(cls, language, values, **kwargs):
-        if 'filter' in values:
-            if FILTERS[values['filter']].type == FilterType.BILINGUAL and language is not None:
-                raise ValueError('Cannot `language` attribute for a bilingual filter')
-            elif FILTERS[values['filter']].type == FilterType.MONOLINGUAL and language is None:
-                raise ValueError('`language` attribute required for a monolingual filter')
-        return language
-
-
-class FilterPipeline(BaseModel):
-    version: Literal[1]
-    files: List[str]
-    filters: List[FilterStep]
-
-
 class FilterPipelinePatch(BaseModel):
     """A list of changes to a filter pipeline (used when updating filters)"""
     filters: List[FilterStep]
 
 
-def list_filters(path) -> Iterable[Filter]:
-    for filename in glob(path, recursive=True):
-        try:
-            with open(filename) as fh:
-                defaults = {
-                    "name": os.path.splitext(os.path.basename(filename))[0],
-                    "basedir": os.path.dirname(filename)
-                }
-                yield parse_obj_as(Filter, {**defaults, **json.load(fh)})
-        except Exception as e:
-            print(f"Could not parse {filename}: {e}", file=sys.stderr)
-
-
-
-FILTERS: Dict[str,Filter] = {}
-
-def reload_filters():
-    global FILTERS
-    FILTERS = {definition.name: definition for definition in list_filters(FILTER_PATH)}
-
-reload_filters()
-
-
-T = TypeVar("T")
-
-def none_throws(optional: Optional[T], message: str = "Unexpected `None`") -> T:
-    """Convert an optional to its value. Raises an `AssertionError` if the
-    value is `None`"""
-    if optional is None:
-        raise AssertionError(message)
-    return optional
-
-
-def dataset_path(name:str, template:str):
+def dataset_path(name:str, template:str) -> str:
     # TODO: fix this hack to get the file path from the name this is silly we
     # should just use get_dataset(name).path or something
     root = DATA_PATH.split('*')[0]
 
     # If the dataset name is a subdirectory, do some hacky shit to get to a
     # .sample.gz file in said subdirectory.
     parts = name.rsplit('/', maxsplit=2)
@@ -227,26 +78,26 @@
         filename = parts[1]
     else:
         filename = parts[0]
 
     return os.path.join(root, template.format(filename))
 
 
-def sample_path(name:str, langs: Iterable[str]):
+def sample_path(name:str, langs:Iterable[str]) -> str:
     languages = '.'.join(sorted(langs))
     return dataset_path(name, f'.sample.{{}}.{languages}')
 
 
 def filter_configuration_path(name:str) -> str:
     return dataset_path(name, '{}.filters.json')
 
 
-async def compute_sample(name:str, columns:List[Tuple[str,Path]]):
+async def compute_sample(name:str, columns:List[Tuple[str,Path]]) -> None:
     langs = [lang for lang, _ in columns]
-    with TemporaryFile() as tempfile:  # type: ignore[name-defined]
+    with TemporaryFile() as tempfile:
         proc = await asyncio.subprocess.create_subprocess_exec(
             *SAMPLE_PY,
             '-n', str(SAMPLE_SIZE),
             *[str(file.resolve()) for _, file in columns],
             stdout=tempfile,
             stderr=asyncio.subprocess.PIPE)
 
@@ -257,104 +108,115 @@
 
         tempfile.seek(0)
 
         with open(sample_path(name, langs), 'wb') as fdest:
             copyfileobj(tempfile, fdest)
 
 
-async def get_dataset_sample(name, columns) -> Tuple[bytes,bytes]:
-    print("Called get_dataset_sample")
-    langs = [lang for lang, _ in columns]
+class FilterOutput(NamedTuple):
+    langs: List[str] # order of columns
+    returncode: int
+    stdout: bytes
+    stderr: bytes
 
-    if not os.path.exists(sample_path(name, langs)):
-        print("Computing sample")
-        await compute_sample(name, columns)
-
-    print("Reading sample from disk")
-    with open(sample_path(name, langs), 'rb') as fh:
-        return fh.read(), bytes()
 
-
-class FilterOutput(BaseModel):
+class ParsedFilterOutput(BaseModel):
+    """JSON serializable version of FilterOutput that has stdout parsed into
+       an array of dicts, with a field per language.
+    """
+    returncode: int
     stdout: List[Dict[str,str]]
-    stderr: Optional[str]
-    retval: Optional[int]
-
-    def __init__(self, langs:List[str], stdout:bytes, stderr:Optional[bytes] = None, retval:Optional[int] = None):
+    stderr: str
+    
+    def __init__(self, output:FilterOutput):
         lines = []
 
-        for lineno, line in enumerate(stdout.rstrip(b'\n').split(b'\n'), start=1):
+        for lineno, line in enumerate(output.stdout.rstrip(b'\r\n').split(b'\n'), start=1):
             values = []
-            for colno, field in enumerate(line.split(b'\t'), start=1):
+            for colno, field in enumerate(line.rstrip(b'\r').split(b'\t'), start=1):
                 try:
                     values.append(field.decode())
                 except UnicodeDecodeError as e:
                     values.append(f'[Error: Cannot decode line {lineno} column {colno}: {e!s}]')
-            lines.append(dict(zip_longest(langs, values, fillvalue='')))
+            lines.append(dict(zip_longest(output.langs, values, fillvalue='')))
 
         super().__init__(
+            returncode=output.returncode,
             stdout=lines,
-            stderr=stderr.decode() if stderr is not None else None,
-            retval=retval)
+            stderr=output.stderr.decode())
 
 
 class SampleCacheEntry(NamedTuple):
-    description: str
     checksum: bytes
-    future: asyncio.Task[Tuple[bytes, bytes]]
+    future: asyncio.Task[FilterOutput]
 
 
 sample_cache: Dict[str,List[SampleCacheEntry]] = {}
 
 
 def cache_hash(obj: Any, seed: bytes = bytes()) -> bytes:
     impl = hashlib.sha256(seed)
     impl.update(json.dumps(obj, sort_keys=True).encode())
     return impl.digest()
 
 
-async def exec_filter_step(filter_step: FilterStep, langs: List[str], input: bytes) -> Tuple[bytes,bytes]:
-    try:
-        print(f"Executing {filter_step.filter}")
-        filter_definition = FILTERS[filter_step.filter]
-
-        if filter_definition.type == FilterType.BILINGUAL:
-                command = filter_definition.command
-        elif filter_definition.type == FilterType.MONOLINGUAL:
-            column = langs.index(none_throws(filter_step.language))
-            command = f'{" ".join(map(shlex.quote, COL_PY))} {column} {filter_definition.command}'
-        else:
-            raise NotImplementedError()
+async def get_dataset_sample(name:str, columns:List[Tuple[str,Path]]) -> FilterOutput:
+    langs = [lang for lang, _ in columns]
+
+    if not os.path.exists(sample_path(name, langs)):
+        await compute_sample(name, columns)
+
+    with open(sample_path(name, langs), 'rb') as fh:
+        stdout = fh.read()
+
+    return FilterOutput([lang for lang, _ in columns], 0, stdout, bytes())
 
-        params = {name: props.export(filter_step.parameters[name])
-                  for name, props in filter_definition.parameters.items()}
 
-        if params:
-            vars_setter = '; '.join(f"{k}={quote(v)}" for k, v in params.items())
-            command = f'{vars_setter}; {command}'
+def format_shell(val: Any) -> str:
+    if isinstance(val, bool):
+        return '1' if val else ''
+    elif isinstance(val, tuple):
+        raise NotImplementedError()
+    elif isinstance(val, list):
+        raise NotImplementedError()
+    else:
+        return str(val)
+
+
+async def exec_filter_step(filter_step: FilterStep, langs: List[str], input: bytes) -> Tuple[bytes,bytes]:
+    filter_definition = get_global_filter(filter_step.filter)
 
-        p_filter = await asyncio.create_subprocess_shell(command,
-            stdin=asyncio.subprocess.PIPE,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-            cwd=filter_definition.basedir)
+    command = filter_format_command(filter_definition, filter_step, langs)
 
-        # Check exit codes, testing most obvious problems first.
-        stdout, stderr = await p_filter.communicate(input=input)
+    # Make sure the path to the python binary (and the installed utils)
+    # is in the PATH variable. If you load a virtualenv this happens by
+    # default, but if you call it with the virtualenv's python binary 
+    # directly it wont.
+    pyenv_bin_path = os.path.dirname(sys.executable)
+    os_env_bin_paths = os.environ.get('PATH', '').split(os.pathsep)
+    filter_env = {
+        **os.environ,
+        'PATH': os.pathsep.join([pyenv_bin_path] + os_env_bin_paths)
+    } if pyenv_bin_path not in os_env_bin_paths else None
+    
+    p_filter = await asyncio.create_subprocess_shell(command,
+        stdin=asyncio.subprocess.PIPE,
+        stdout=asyncio.subprocess.PIPE,
+        stderr=asyncio.subprocess.PIPE,
+        cwd=filter_definition.basedir,
+        env=filter_env)
 
-        print(f"{filter_step.filter} finished with {p_filter.returncode}")
+    # Check exit codes, testing most obvious problems first.
+    stdout, stderr = await p_filter.communicate(input=input)
 
-        return p_filter.returncode, stdout, stderr
-    except asyncio.CancelledError:
-        print(f"{filter_step.filter} cancelled")
+    return FilterOutput(langs, p_filter.returncode, stdout, stderr)
 
 
-def cancel_cached_tasks(name:str, offset:int):
+def cancel_cached_tasks(name:str, offset:int) -> None:
     for entry in sample_cache[name][offset:]:
-        print(f"Cancelling {entry.description}")
         entry.future.cancel()
     del sample_cache[name][offset:]
 
 
 async def get_sample(name:str, filters:List[FilterStep]) -> AsyncIterator[FilterOutput]:
     columns: List[Tuple[str,Path]] = sorted(list_datasets(DATA_PATH)[name].items(), key=lambda pair: pair[0])
     langs = [lang for lang, _ in columns]
@@ -365,76 +227,61 @@
     ])
 
     # If we don't have a sample stored, generate one. Doing it in bytes because
     # it might save us parsing utf-8 (also assumptions! It it utf-8?)
     if not name in sample_cache or sample_cache[name][0].checksum != checksum:
         sample_cache[name] = [
             SampleCacheEntry(
-                description='get_dataset_sample',
                 checksum=checksum,
                 future=asyncio.create_task(get_dataset_sample(name, columns))
             )
         ]
 
-    sample, _ = await sample_cache[name][0].future
+    sample = await sample_cache[name][0].future
 
-    yield FilterOutput(langs, sample)
+    # Return a clean unfiltered sample first
+    yield sample
 
     for i, filter_step in enumerate(filters, start=1):
-        filter_definition = FILTERS[filter_step.filter]
+        filter_definition = get_global_filter(filter_step.filter)
 
         checksum = cache_hash(jsonable_encoder(filter_step),
             cache_hash(jsonable_encoder(filter_definition),
                 sample_cache[name][i-1].checksum))
 
         # If we do not have a cache entry for this point
         if len(sample_cache[name]) <= i or sample_cache[name][i].checksum != checksum:
             # Invalidate all the cache after this step
             cancel_cached_tasks(name, i)
 
             sample_cache[name].append(SampleCacheEntry(
-                description=filter_step.filter,
                 checksum=checksum,
-                future=asyncio.create_task(exec_filter_step(filter_step, langs, sample))
+                future=asyncio.create_task(exec_filter_step(filter_step, langs, sample.stdout))
             ))
 
             assert len(sample_cache[name]) == i + 1
         
-        filter_retval, filter_output, filter_stderr = await sample_cache[name][i].future
-
-        yield FilterOutput(langs, filter_output, filter_stderr, filter_retval)
-
-        # Don't continue the filter chain if a filter fails
-        if filter_retval != 0:
-            break
+        sample = await sample_cache[name][i].future    
+        
+        # Return the (partially) filtered sample
+        yield sample
 
-        sample = filter_output
 
     # if there are additional steps left in the cache, remove them
     if len(sample_cache[name]) > len(filters) + 1:
         cancel_cached_tasks(name, len(filters) + 1)
 
 
-async def stream_jsonl(iterable):
-    async def generator():
-        try:
-            print("START")
-            async for line in iterable:
-                print("LINE")
-                yield line
-            print("END")
-        except Exception as err:
-            print("ERROR")
-            traceback.print_exc()
-            yield {'_error': str(err)}
-
-    return StreamingResponse((
-        json.dumps(jsonable_encoder(line), separators=(',', ':')).encode() + b"\n"
-        async for line in generator()
-    ), media_type='application/json')
+def stream_jsonl(iterable:AsyncIterator[Any]) -> StreamingResponse:
+    return StreamingResponse(
+        (
+            json.dumps(jsonable_encoder(line), separators=(',', ':')).encode() + b"\n"
+            async for line in iterable
+        ),
+        media_type='application/json')
 
 
 app = FastAPI()
 
 @app.get('/api/datasets/')
 def api_list_datasets() -> List[Dataset]:
     return [
@@ -456,37 +303,37 @@
     return Dataset(name=name, columns={
         lang: File(path=file.name, size=file.stat().st_size)
         for lang, file in columns.items()
     })
 
 
 @app.get('/api/datasets/{name:path}/sample')
-async def api_get_sample(name:str) -> AsyncIterator[FilterOutput]:
-    return await stream_jsonl(get_sample(name, []))
+async def api_get_sample(name:str) -> Response:
+    return stream_jsonl(ParsedFilterOutput(output) async for output in get_sample(name, []))
 
 
 @app.post('/api/datasets/{name:path}/sample')
-async def api_get_filtered_sample(name:str, filters:List[FilterStep]) -> AsyncIterator[FilterOutput]:
-    return await stream_jsonl(get_sample(name, filters))
+async def api_get_filtered_sample(name:str, filters:List[FilterStep]) -> Response:
+    return stream_jsonl(ParsedFilterOutput(output) async for output in get_sample(name, filters))
 
 
-def make_pipeline(name, filters=[]):
+def make_pipeline(name:str, filters:List[FilterStep] = []) -> FilterPipeline:
     columns = list_datasets(DATA_PATH)[name]
     return FilterPipeline(
         version=1,
         files=[file.name
             for _, file in
             sorted(columns.items(), key=lambda pair: pair[0])
         ],
         filters=filters
     )
 
 
 @app.get('/api/datasets/{name:path}/configuration.json')
-def api_get_dataset_filters(name:str) -> List[FilterStep]:
+def api_get_dataset_filters(name:str) -> FilterPipeline:
 
     if not os.path.exists(filter_configuration_path(name)):
         return make_pipeline(name)
 
     with open(filter_configuration_path(name), 'r') as fh:
         data = json.load(fh)
         try:
@@ -504,18 +351,103 @@
 @app.patch('/api/datasets/{name:path}/configuration.json')
 def api_update_dataset_filters(name:str, patch:FilterPipelinePatch):
     pipeline = make_pipeline(name, patch.filters)
     with open(filter_configuration_path(name), 'w') as fh:
         return json.dump(pipeline.dict(), fh, indent=2)
 
 
+@app.get('/api/datasets/{name:path}/configuration-for-opusfilter.yaml')
+def api_get_dataset_filters_as_openfilter(name:str) -> Response:
+    if not os.path.exists(filter_configuration_path(name)):
+        raise HTTPException(status_code=404, detail='Dataset not found')
+
+    with open(filter_configuration_path(name), 'r') as fh:
+        data = json.load(fh)
+
+    pipeline = parse_obj_as(FilterPipeline, data)
+
+    opusfilter_config: Dict[str,Any] = {
+        'steps': []
+    }
+
+    input_files = pipeline.files
+    
+    preprocess_steps = []
+
+    filter_steps: List[Dict[str,Any]] = []
+
+    for step in pipeline.filters:
+        if (match := re.search(r'\bopusfilter\.preprocessors\.(\w+)\b', get_global_filter(step.filter).command)):
+            preprocess_steps.append({
+                str(match.group(1)): step.parameters
+            })
+        elif (match := re.search(r'\bopusfilter\.filters\.(\w+)\b', get_global_filter(step.filter).command)):
+            filter_steps.append({
+                str(match.group(1)): step.parameters
+            })
+        elif get_global_filter(step.filter).type == FilterType.BILINGUAL:
+            filter_steps.append({
+                'OpusCleanerFilter': {
+                    'filter': step.filter,
+                    'parameters': step.parameters
+                },
+                'module': 'opuscleaner.opusfilter_compat'
+            })
+        elif get_global_filter(step.filter).type == FilterType.MONOLINGUAL:
+            filter_steps.append({
+                'OpusCleanerFilter': {
+                    'filter': step.filter,
+                    'parameters': step.parameters
+                },
+                'module': 'opuscleaner.opusfilter_compat'
+            })
+        else:
+            raise ValueError(f'Cannot convert "{step.filter}" to opusfilter configuration')
+
+    if preprocess_steps:
+        output_files = [
+            os.path.join(os.path.dirname(file), 'preprocessed.' + os.path.basename(file))
+            for file in pipeline.files
+        ]
+
+        opusfilter_config['steps'].append({
+            'type': 'preprocess',
+            'parameters': {
+                'inputs': input_files,
+                'outputs': output_files,
+                'preprocessors': preprocess_steps
+            }
+        })
+
+        input_files = output_files
+
+    if filter_steps:
+        output_files = [
+            os.path.join(os.path.dirname(file), 'filtered.' + os.path.basename(file))
+            for file in pipeline.files
+        ]
+
+        opusfilter_config['steps'].append({
+            'type': 'filter',
+            'parameters': {
+                'inputs': input_files,
+                'outputs': output_files,
+                'filters': filter_steps
+            }
+        })
+
+        input_files = output_files
+
+    return Response(yaml.safe_dump(opusfilter_config, sort_keys=False), media_type='application/yaml')
+
+
 @app.get('/api/filters/')
 def api_get_filters():
-    reload_filters()
-    return FILTERS
+    set_global_filters(list_filters(FILTER_PATH))
+    return get_global_filters()
 
 
 @app.get('/')
 def redirect_to_interface():
     return RedirectResponse('/frontend/index.html')
 
 
@@ -570,8 +502,13 @@
     parser_serve.add_argument('--reload', action='store_true', help='Enable auto-reload.')
     parser_serve.set_defaults(func=main_serve)
 
     parser_sample = subparsers.add_parser('sample')
     parser_sample.set_defaults(func=main_sample)
 
     args = parser.parse_args()
+
+    set_global_filters(list_filters(FILTER_PATH))
     args.func(args)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `opuscleaner-0.1/opuscleaner/threshold.py` & `opuscleaner-0.2/opuscleaner/threshold.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/alpha_ratio.json` & `opuscleaner-0.2/opuscleaner/filters/alpha_ratio.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998840249662618%*

 * *Differences: {"'parameters'": "{'LANG1': {'allowed_values': {insert: [(19, 'hy')]}}, 'LANG2': "*

 * *                 "{'allowed_values': {insert: [(19, 'hy')]}}}"}*

```diff
@@ -24,14 +24,15 @@
                 "fi",
                 "fr",
                 "ga",
                 "gl",
                 "hi",
                 "hr",
                 "hu",
+                "hy",
                 "is",
                 "it",
                 "ko",
                 "lt",
                 "lv",
                 "mt",
                 "nb",
@@ -66,14 +67,15 @@
                 "fi",
                 "fr",
                 "ga",
                 "gl",
                 "hi",
                 "hr",
                 "hu",
+                "hy",
                 "is",
                 "it",
                 "ko",
                 "lt",
                 "lv",
                 "mt",
                 "nb",
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/alpha_ratio.py` & `opuscleaner-0.2/opuscleaner/filters/alpha_ratio.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     return parser.parse_args()
 
 def clean_parallel(src_lang: str, ratio_words_src: float, ratio_alpha_src: float,\
 trg_lang: Optional[str], ratio_words_trg: float, ratio_alpha_trg: float,\
  debug: bool = True) -> None:
     """Cleans the parallel (or monolingual) dataset based on the number of characters"""
     for line in stdin:
-        fields = line.strip().split('\t')
+        fields = line.rstrip('\r\n').split('\t')
         if len(fields) == 1:
             src = fields[-1].strip()
             trg = None
         else: # Assumes that the multiline filter already run
             src = fields[-2].strip()
             trg = fields[-1].strip()
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/bicleaner_hardrules.json` & `opuscleaner-0.2/opuscleaner/filters/bicleaner_hardrules.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/bifixer.json` & `opuscleaner-0.2/opuscleaner/filters/bifixer.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/clean_common.py` & `opuscleaner-0.2/opuscleaner/filters/clean_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'fi': r'[a-zÅåÄäÖö]',
     'fr': r'[a-zÂâÁáÀàâÇçÉéÈèÊêÓóÒòÔôŒœÜüÛûŸÿ]',
     'ga': r'[abcdefghilmnoprstuáéíóúÁÉÍÓÚ]',
     'gl': r'[a-zÁáÉéÍíÓóÚúÑñ]',
     'hi': r'[\u0900-\u097F]', # devanagari
     'hr': r'[abcčČćĆdđĐefghijklmnoprsšŠtuvzžŽ]',
     'hu': r'[a-zÁáÉéÍíÓóÖöŐőŰű]',
+    'hy': r'[\u0530-\u058F]',
     'is': r'[abdefghijklmnoprstuvxyÁáðÐÉéÍíÓóÚúÝýÞþÆæÖö]',
     'it': r'[a-zàÀèÈéÉìÌíÍîÎòÒóÓùÙúÚ]',
     'ko': r'[\uac00-\ud7af]|[\u1100-\u11ff]|[\u3130-\u318f]|[\ua960-\ua97f]|[\ud7b0-\ud7ff]',
     'lt': r'[aąbcČčdeĘęĖėfghiĮįyjklmnoprsŠštuŲųŪūvzŽž]',
     'lv': r'[aĀābcČčdeĒēfgĢģhiĪījkĶķlĻļmnŅņoprsŠštuŪūvzŽž]',
     'mt': r'[abĊċdefĠġghĦħiiejklmnopqrstuvwxŻżz]',
     'nb': r'[a-zÂâÁáÀàâÉéÈèÊêÓóÒòÔôÜüÆæØøÅå]',
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/deescape-special-chars.perl` & `opuscleaner-0.2/opuscleaner/filters/deescape-special-chars.perl`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/detokenizer.json` & `opuscleaner-0.2/opuscleaner/filters/detokenizer.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'command'": "'sacremoses -l $LANG1 detokenize'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "command": "sacremoses detokenize -l $LANG1",
+    "command": "sacremoses -l $LANG1 detokenize",
     "description": "Detokenizes tokenized text. If the language is unsupported, enter 'other'. Uses sacremoses",
     "parameters": {
         "LANG1": {
             "allowed_values": [
                 "ar",
                 "bg",
                 "bn",
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/detokenizer.perl` & `opuscleaner-0.2/opuscleaner/filters/detokenizer.perl`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/fasttext_filter.json` & `opuscleaner-0.2/opuscleaner/filters/fasttext_filter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/fasttext_filter.py` & `opuscleaner-0.2/opuscleaner/filters/fasttext_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     target_lang = "__label__" + args.target_lang
     download_model(args.model_type)
     # Disable fasttext to notify us about loading the model
     fasttext.FastText.eprint = lambda x: None
     model = fasttext.load_model(f"{args.model_type}.bin")
     for batch in chunked(sys.stdin, args.batch_size):
         # Remove newlines
-        batch = [row.rstrip("\n") for row in batch]
+        batch = [row.rstrip("\r\n") for row in batch]
         sources, targets = zip(*[row.split("\t", 1) for row in batch])
         sources_ok = verify_lang(model, list(sources), source_lang, args.debug)
         targets_ok = verify_lang(model, list(targets), target_lang, args.debug)
         for row, source_ok, target_ok in zip(batch, sources_ok, targets_ok):
             if source_ok and target_ok:
                 sys.stdout.write(row + "\n")
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/fix_elitr_eca.py` & `opuscleaner-0.2/opuscleaner/filters/fix_elitr_eca.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/fix_wiki.json` & `opuscleaner-0.2/opuscleaner/filters/fix_wiki.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/fix_wiki.py` & `opuscleaner-0.2/opuscleaner/filters/fix_wiki.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 	if args.wikilinks:
 		patterns.append(WIKILINKS_PATTERN)
 
 	if args.headings:
 		patterns.append(HEADINGS_PATTERN)
 
 	for n, line in enumerate(sys.stdin, start=1):
-		fields = line.rstrip("\n").split("\t")
+		fields = line.rstrip("\r\n").split("\t")
 
 		if args.code and any(is_code(field) for field in fields):
 			continue
 
 		for pattern in patterns:
 			if args.always or is_mismatch(pattern, fields[:2]):
 				fields[:2] = [filter_matches(pattern, field) for field in fields[:2]]
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/langid.json` & `opuscleaner-0.2/opuscleaner/filters/langid.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/langid.py` & `opuscleaner-0.2/opuscleaner/filters/langid.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     parser.add_argument("--allow-unknown", action="store_true")
     parser.add_argument("--debug", action="store_true")
     return parser.parse_args()
 
 
 def detect_language_parallel(args: argparse.Namespace, fin: BinaryIO, fout: BinaryIO):
     for n, line in enumerate(fin):
-        fields = line.rstrip(b"\n").split(b"\t")
+        fields = line.rstrip(b"\r\n").split(b"\t")
 
         for field, lang in zip(fields, args.languages):
             try:
                 isReliable, _, [(_, detected_lang, _, _), *_] = pycld2.detect(field)
 
                 # Accept field if reliable and detected language
                 if isReliable and detected_lang == lang:
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/laser_similarity.json` & `opuscleaner-0.2/opuscleaner/filters/laser_similarity.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/laser_similarity.py` & `opuscleaner-0.2/opuscleaner/filters/laser_similarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     if not args.scores and args.threshold is None:
         print("Either use --threshold or --scores")
 
     laser = Laser()
 
     for batch in chunked(sys.stdin, chunk_size=args.batch_size, chunk_time=args.batch_latency, verbose=sys.stderr if args.verbose else NullIO()):
         # TODO error checking of column count?
-        scores = _compute_similarity(laser, [tuple(line.split("\t")[:2]) for line in batch], args.src_lang, args.tgt_lang)
+        scores = _compute_similarity(laser, [tuple(line.rstrip("\r\n").split("\t")[:2]) for line in batch], args.src_lang, args.tgt_lang)
 
         if args.scores:
             for score in scores:
                 print(score, file=sys.stdout)
         else:
             for line, score in zip(batch, scores):
                 if score >= args.threshold:
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/max_length.py` & `opuscleaner-0.2/opuscleaner/filters/max_length.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     parser.add_argument("--debug", action='store_true')
     return parser.parse_args()
 
 
 def clean_parallel(max_length: float, min_length: float, debug: bool=True) -> None:
     """Cleans the parallel or mono dataset based on line lengths"""
     for line in stdin:
-        fields = line.strip().split('\t')
+        fields = line.strip('\r\n').split('\t')
         if len(fields) == 1:
             src = fields[-1].strip()
             trg = None
         else: # Assumes that the multiline filter already run
             src = fields[-2].strip()
             trg = fields[-1].strip()
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/max_word_length.py` & `opuscleaner-0.2/opuscleaner/filters/max_word_length.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     parser.add_argument("--max-word-length", default=150, type=int)
     return parser.parse_args()
 
 
 def clean_parallel(max_word_length: float, fin: TextIO, fout: TextIO) -> None:
     """Cleans the parallel or mono dataset based on line lengths"""
     for line in fin:
-        fields = line.strip().split('\t')
+        fields = line.rstrip('\r\n').split('\t')
 
         if any(len(token) > max_word_length
             for field in fields
             for token in field.split(' ')):
             continue
 
         fout.write(line)
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/num_mismatch.py` & `opuscleaner-0.2/opuscleaner/filters/num_mismatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def normalize(numstr:Match) -> str:
 	return re.sub(r'[^\d]+', '*', numstr[0])
 
 
 def filter_numerical_mismatch(fin: TextIO, fout: TextIO, ratio: float, *, debug: bool = False):
 	for line in fin:
-		cols = line.rstrip('\n').split('\t')
+		cols = line.rstrip('\r\n').split('\t')
 
 		assert len(cols) >= 2
 
 		nums_left, nums_right = (set(map(normalize, re.finditer(r'\d+(?:[\.,]\d+)*', col))) for col in cols[:2])
 
 		# Only bother calculating the ratio if there were any numbers to begin with
 		if nums_left and nums_right:
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/remove_frequent_patterns.py` & `opuscleaner-0.2/opuscleaner/filters/remove_frequent_patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     replacement: str
     pattern_on_both_cols: Optional[re.Pattern] = None
 
 
 def load_patterns(file_path: str) -> List[Pattern]:
     with open(file_path) as f:
         # Skip comment lines
-        lines = [line.rstrip("\n") for line in f.readlines() if line[0] != "#"]
+        lines = [line.rstrip("\r\n") for line in f.readlines() if line[0] != "#"]
         patterns = []
         for line in lines:
             parts = line.split("\t")
             if len(parts) == 2:
                 patterns.append(Pattern(group_match=re.compile(parts[0]), replacement=parts[1]))
             elif len(parts) == 3:
                 patterns.append(Pattern(pattern_on_both_cols=re.compile(parts[0]), group_match=re.compile(parts[1]), replacement=parts[2]))
@@ -49,15 +49,15 @@
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--pattern-file", type=str, help="Path to the file with patterns.")
     parser.add_argument("--debug", action="store_true")
     args = parser.parse_args()
     patterns = load_patterns(args.pattern_file)
 
     for line in sys.stdin:
-        line = line.rstrip("\n")
+        line = line.rstrip("\r\n")
         source, target = line.split("\t", 1)
         for pattern in patterns:
             # Either pattern_on_both_cols is not set or it matches the whole line
             if pattern.pattern_on_both_cols is None or pattern.pattern_on_both_cols.match(line):
                 source = pattern.group_match.sub(pattern.replacement, source)
                 target = pattern.group_match.sub(pattern.replacement, target)
         sys.stdout.write(f"{source}\t{target}\n")
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/segment_japanese.py` & `opuscleaner-0.2/opuscleaner/filters/segment_japanese.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/split_sentences.json` & `opuscleaner-0.2/opuscleaner/filters/split_sentences.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/split_sentences.py` & `opuscleaner-0.2/opuscleaner/filters/split_sentences.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sentence_splitter import SentenceSplitter
 
 
 def split_sentences_in_bitext(fin: TextIO, fout: TextIO, languages: List[str], keep_unbalanced: bool = False):
 	splitters = [SentenceSplitter(language=lang) for lang in languages]
 	
 	for line in fin:
-		cols = line.rstrip('\n').split('\t')
+		cols = line.rstrip('\r\n').split('\t')
 
 		assert len(cols) == len(splitters)
 
 		splitted = [splitter.split(col) for splitter, col in zip(splitters, cols)]
 
 		if any(len(col) != len(splitted[0]) for col in splitted[1:]):
 			if keep_unbalanced:
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/src_trg_ratio.py` & `opuscleaner-0.2/opuscleaner/filters/src_trg_ratio.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 Comparator = Callable[[List[str], List[str], float], bool]
 
 
 def clean_parallel(ratio: float, filter_identical: bool, *, debug: bool=False, compare: Comparator=compare_lin) -> None:
     """Cleans the parallel dataset based on the ratio of source to target tokens and vice versa"""
     for line in stdin:
-        fields = line.strip().split('\t')
+        fields = line.rstrip('\r\n').split('\t')
         if len(fields) != 2:
             stderr.write(f'SINGLE/MULTIPLE_LINES\t{line}')
             continue
 
         src = fields[0].strip()
         trg = fields[1].strip()
```

### Comparing `opuscleaner-0.1/opuscleaner/filters/strip_suffix.json` & `opuscleaner-0.2/opuscleaner/filters/strip_suffix.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/filters/strip_suffix.py` & `opuscleaner-0.2/opuscleaner/filters/strip_suffix.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 if __name__  == "__main__":
 	parser = argparse.ArgumentParser()
 	parser.add_argument("--minlen", type=int, default=4)
 	parser.add_argument("--minocc", type=int, default=5)
 	parser.add_argument("--count", action="store_true")
 	args = parser.parse_args()
 
-	lines = (line.rstrip("\n") for line in sys.stdin)
+	lines = (line.rstrip("\r\n") for line in sys.stdin)
 
 	if args.count:
 		counter = Counter()
 	else:
 		counter = None
 
 	for line in strip_suffix(lines, minlen=args.minlen, minocc=args.minocc, counter=counter):
```

### Comparing `opuscleaner-0.1/README.md` & `opuscleaner-0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 # OpusCleaner
-OpusCleaner is a machine translation/language model data cleaner and training scheduler. The Training scheduler has moved to [empty-trainer](https://github.com/hplt-project/empty-trainer).
+OpusCleaner is a machine translation/language model data cleaner and training scheduler. The Training scheduler has moved to [OpusTrainer](https://github.com/hplt-project/OpusTrainer).
 
 ## Cleaner
 The cleaner bit takes care of downloading and cleaning multiple different datasets and preparing them for translation.
 
+### Installation for cleaning
+If you just want to use OpusCleaner for cleaning, you can install it from PyPI, and then run it
+
+```sh
+pip3 install opuscleaner
+opuscleaner-server serve
+```
+
+Then you can go to http://127.0.0.1:8000/ to show the interface.
+
+You can also install and run OpusCleaner on a remote machine, and use [SSH local forwarding](https://www.ssh.com/academy/ssh/tunneling-example) (e.g. `ssh -L 8000:localhost:8000 you@remote.machine`) to access the interface on your local machine.
+
 ### Dependencies
 (Mainly listed as shortcuts to documentation)
 
 - [FastAPI](https://fastapi.tiangolo.com) as the base for the backend part.
 - [Pydantic](https://pydantic-docs.helpmanual.io/) for conversion of untyped JSON to typed objects. And because FastAPI automatically supports it and gives you useful error messages if you mess up things.
 - [Vue](https://vuejs.org/guide/introduction.html) for frontend
 
@@ -23,39 +35,33 @@
 [<img src=".github/screenshots/filter-datasets.png" width="100%">](.github/screenshots/filter-datasets.png)
 
 Compare the dataset at different stages of filtering to see what the impact is of each filter.
 [<img src=".github/screenshots/diff-filter-output.png" width="100%">](.github/screenshots/diff-filter-output.png)
 
 
 ### Paths
-- `data/train-parts` is scanned for datasets
-- `filters` should contain filter json (but that's not implemented yet, right now it just has a hard-coded `FILTERS` dict in code)
+- `data/train-parts` is scanned for datasets. You can change this by setting the `DATA_PATH` environment variable, the default is `data/train-parts/*.*.gz`.
+- `filters` should contain filter json files. You can change the `FILTER_PATH` environment variable, the default is `<PYTHON_PACKAGE>/filters/*.json`.
 
 ### Installation for development
 ```sh
-python3 -m venv .env
-bash --init-file .env/bin/activate
-pip install -e .
-
 cd frontend
 npm clean-install
 npm run build
 cd ..
-```
-
-Link the frontend build folder into opuscleaner. Normally this is done during packaging but when opuscleaner is installed as an editable package, this doesn't happen.
 
-```sh
-ln -s ../frontend/dist opuscleaner/frontend
+python3 -m venv .env
+bash --init-file .env/bin/activate
+pip install -e .
 ```
 
 Finally you can run `opuscleaner-server` as normal. The `--reload` option will cause it to restart when any of the python files change.
 
 ```sh
-opuscleaner-server --reload
+opuscleaner-server serve --reload
 ```
 
 Then go to http://127.0.0.1:8000/ for the "interface" or http://127.0.0.1:8000/docs for the API.
 
 ### Frontend development
 
 If you're doing frontend development, try also running:
@@ -75,13 +81,13 @@
 
 ```sh
 python -m laserembeddings download-models
 ```
 
 ## Packaging
 
-Run `pip wheel .` to build & package OpusCleaner. Packaging is done through hatch, see the `pyproject.toml` and `build_frontend.py` files for details. You'll need to have a recent version of `node` and `npm` in your `PATH` for this to work.
+Run `npm build` in the `frontend/` directory first, and then run `hatch build .` in the project directory to build the wheel and source distribution.
 
 # Acknowledgements
 
 This project has received funding from the European Union’s Horizon Europe research and innovation programme under grant agreement No 101070350 and from UK Research and Innovation (UKRI) under the UK government’s Horizon Europe funding guarantee [grant number 10052546]
```

### Comparing `opuscleaner-0.1/pyproject.toml` & `opuscleaner-0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -60,21 +60,20 @@
 exclude = [
   "/.github",
   "/.gitignore",
   "/frontend",
   "/placeholders",
   "/build_frontend.py"
 ]
+artifacts = [
+  "/frontend/dist/*"
+]
 
 [tool.hatch.build.sources]
-"frontend/dist" = "opuscleaner/frontend"
-
-[tool.hatch.build.hooks.custom]
-path = "build_frontend.py"
-code = "frontend"
+"/frontend/dist" = "/opuscleaner/frontend"
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
 
 [tool.hatch.metadata.hooks.requirements_txt.optional-dependencies]
 all = ["requirements-all.txt"]
```

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/AddDatasetView.4182f0f7.css` & `opuscleaner-0.2/opuscleaner/frontend/assets/AddDatasetView.4182f0f7.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/AddDatasetView.5dcf722c.js` & `opuscleaner-0.2/opuscleaner/frontend/assets/AddDatasetView.ff526466.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -7,40 +7,40 @@
         o instanceof WeakSet ? o.add(n) : o.set(n, l)
     },
     U = (n, o, l, _) => (x(n, o, "write to private field"), _ ? _.call(n, l) : o.set(n, l), l);
 var A = (n, o, l) => (x(n, o, "access private method"), l);
 import {
     _ as ae,
     i as r,
-    k as S,
+    m as S,
     j as se,
-    aK as ne,
-    l as oe,
+    aL as ne,
+    k as oe,
     o as g,
     c as y,
     d as s,
-    m as T,
+    n as L,
     bw as le,
-    a3 as j,
+    a4 as j,
     v as N,
     f as h,
-    b as L,
+    b as T,
     u as c,
     F as P,
     r as J,
     a as re,
     T as ie,
     t as p,
-    bE as ue,
+    bF as ue,
     p as ce,
     h as de
-} from "./index.490d1368.js";
+} from "./index.6cc31f0d.js";
 import {
     C as z
-} from "./vue-select.6aaeaff8.js";
+} from "./vue-select.9ddbca8a.js";
 
 function pe(n) {
     const o = n == 0 ? 0 : Math.floor(Math.log(n) / Math.log(1024));
     return (n / Math.pow(1024, o)).toFixed(2) + " " + ["B", "kB", "MB", "GB", "TB"][o]
 }
 var d, C, q;
 class he {
@@ -90,18 +90,18 @@
         class: "metadata-dataset"
     },
     Ve = m(() => s("dt", null, "Version", -1)),
     Oe = {
         title: "Version"
     },
     Se = m(() => s("dt", null, "Languages", -1)),
-    Te = {
+    Le = {
         title: "Languages"
     },
-    Le = m(() => s("dt", null, "Pairs", -1)),
+    Te = m(() => s("dt", null, "Pairs", -1)),
     Ce = {
         title: "Sentence pairs"
     },
     Me = m(() => s("dt", null, "Size", -1)),
     $e = {
         title: "Download size"
     },
@@ -128,45 +128,45 @@
                 $ = new Map,
                 k = r(""),
                 D = r(!0),
                 V = r(!0),
                 O = r(!0),
                 i = r(),
                 f = r(),
-                R = r(),
+                F = r(),
                 G = S(() => {
                     if (!i.value) return [];
                     if (!M.has(i.value)) {
                         const a = r([]);
                         M.set(i.value, a), Y(i.value).then(e => {
                             a.value = e
                         })
                     }
                     return M.get(i.value).value
                 }),
-                K = S(() => {
+                H = S(() => {
                     const a = new Intl.DisplayNames([], {
                         type: "language",
                         languageDisplay: "standard"
                     });
-                    return (R.value || []).map(e => {
+                    return (F.value || []).map(e => {
                         try {
                             return {
                                 lang: e,
                                 label: `${a.of(e)} (${e})`
                             }
                         } catch {
                             return {
                                 lang: e,
                                 label: e
                             }
                         }
                     })
                 }),
-                H = S(() => {
+                K = S(() => {
                     const a = new Intl.DisplayNames([], {
                         type: "language",
                         languageDisplay: "standard"
                     });
                     return (G.value || []).map(e => {
                         try {
                             return {
@@ -195,26 +195,26 @@
                         corpus: t,
                         group: u
                     }) => t.toLowerCase().indexOf(k.value.toLowerCase()) !== -1)), e = e.filter(t => t.langs.length > 1 ? O.value : V.value), D.value && (e = Array.from(e.reduce((t, u) => ((!t.has(u.corpus) || t.get(u.corpus).version < u.version) && t.set(u.corpus, u), t), new Map).values())), e.sort(l.value.compare), e
                 }),
                 v = se({});
             ne(async () => {
                 X().then(a => {
-                    R.value = a
-                }), F().then(a => {
+                    F.value = a
+                }), E().then(a => {
                     Object.assign(v, I(a))
                 })
             });
-            let E = new he(1e3, async () => {
-                const a = await F();
+            let R = new he(1e3, async () => {
+                const a = await E();
                 Object.assign(v, I(a))
             });
             oe(v, a => {
                 const e = new Set(["pending", "downloading"]);
-                Object.values(a).some(t => e.has(t.state)) ? E.restart() : E.stop()
+                Object.values(a).some(t => e.has(t.state)) ? R.restart() : R.stop()
             });
 
             function I(a) {
                 return Object.fromEntries(a.map(e => [e.entry.id, e]))
             }
 
             function W(a) {
@@ -235,15 +235,15 @@
             async function Y(a) {
                 return await w(`/api/download/languages/${encodeURIComponent(a)}`)
             }
             async function Z(a, e) {
                 const t = `${a}-${e}`;
                 return await w(`/api/download/by-language/${encodeURIComponent(t)}`)
             }
-            async function F() {
+            async function E() {
                 return await w("/api/download/downloads/")
             }
             async function ee(a) {
                 return await w("/api/download/downloads/", {
                     method: "POST",
                     headers: {
                         "Content-Type": "application/json"
@@ -252,64 +252,64 @@
                         id: e
                     }) => ({
                         id: e
                     })))
                 })
             }
             const te = new Intl.NumberFormat;
-            return (a, e) => (g(), y("div", ve, [ge, s("div", me, [s("label", null, [T(s("input", {
+            return (a, e) => (g(), y("div", ve, [ge, s("div", me, [s("label", null, [L(s("input", {
                 type: "search",
                 placeholder: "Search dataset\u2026",
                 "onUpdate:modelValue": e[0] || (e[0] = t => k.value = t)
             }, null, 512), [
                 [le, k.value]
             ])]), s("label", {
                 class: j(["search-button", {
                     checked: V.value
                 }])
-            }, [T(s("input", {
+            }, [L(s("input", {
                 type: "checkbox",
                 "onUpdate:modelValue": e[1] || (e[1] = t => V.value = t)
             }, null, 512), [
                 [N, V.value]
             ]), h(" Monolingual ")], 2), s("label", {
                 class: j(["search-button", {
                     checked: O.value
                 }])
-            }, [T(s("input", {
+            }, [L(s("input", {
                 type: "checkbox",
                 "onUpdate:modelValue": e[2] || (e[2] = t => O.value = t)
             }, null, 512), [
                 [N, O.value]
             ]), h(" Bilingual ")], 2), s("label", {
                 class: j(["search-button", {
                     checked: D.value
                 }])
-            }, [T(s("input", {
+            }, [L(s("input", {
                 type: "checkbox",
                 "onUpdate:modelValue": e[3] || (e[3] = t => D.value = t)
             }, null, 512), [
                 [N, D.value]
-            ]), h(" Latest only ")], 2), s("label", null, [L(c(z), {
+            ]), h(" Latest only ")], 2), s("label", null, [T(c(z), {
                 modelValue: i.value,
                 "onUpdate:modelValue": e[4] || (e[4] = t => i.value = t),
-                options: c(K),
+                options: c(H),
                 reduce: ({
                     lang: t
                 }) => t,
                 placeholder: "Origin language"
-            }, null, 8, ["modelValue", "options", "reduce"])]), s("label", null, [L(c(z), {
+            }, null, 8, ["modelValue", "options", "reduce"])]), s("label", null, [T(c(z), {
                 modelValue: f.value,
                 "onUpdate:modelValue": e[5] || (e[5] = t => f.value = t),
-                options: c(H),
+                options: c(K),
                 reduce: ({
                     lang: t
                 }) => t,
                 placeholder: "Target language"
-            }, null, 8, ["modelValue", "options", "reduce"])]), s("label", null, [L(c(z), {
+            }, null, 8, ["modelValue", "options", "reduce"])]), s("label", null, [T(c(z), {
                 modelValue: l.value,
                 "onUpdate:modelValue": e[6] || (e[6] = t => l.value = t),
                 options: o,
                 placeholder: "Sort order"
             }, null, 8, ["modelValue"])])]), s("div", _e, [(g(!0), y(P, null, J(c(Q), t => (g(), y("div", {
                 class: "dataset",
                 key: t.id,
@@ -317,17 +317,17 @@
             }, [s("div", we, [s("h3", be, [s("a", {
                 href: `https://opus.nlpl.eu/${t.corpus}-${t.version}.php`,
                 target: "_blank"
             }, p(t.corpus), 9, ye)]), s("button", {
                 class: "download-dataset-button",
                 onClick: u => W(t),
                 disabled: t.id in v || "paths" in t
-            }, [h(" Download "), L(c(ue), {
+            }, [h(" Download "), T(c(ue), {
                 class: "download-icon"
-            })], 8, ke)]), s("dl", De, [Ve, s("dd", Oe, p(t.version), 1), Se, s("dd", Te, p(t.langs.join("\u2192")), 1), Le, s("dd", Ce, p(t.pairs ? c(te).format(t.pairs) : ""), 1), Me, s("dd", $e, p(t.size ? c(pe)(t.size) : ""), 1)])], 8, fe))), 128))]), (g(), re(ie, {
+            })], 8, ke)]), s("dl", De, [Ve, s("dd", Oe, p(t.version), 1), Se, s("dd", Le, p(t.langs.join("\u2192")), 1), Te, s("dd", Ce, p(t.pairs ? c(te).format(t.pairs) : ""), 1), Me, s("dd", $e, p(t.size ? c(pe)(t.size) : ""), 1)])], 8, fe))), 128))]), (g(), re(ie, {
                 to: ".navbar"
             }, [s("details", Ie, [xe, s("ul", null, [(g(!0), y(P, null, J(v, t => (g(), y("li", {
                 key: t.entry.id
             }, [h(p(t.entry.corpus) + " ", 1), s("em", null, p(t.state), 1)]))), 128))])])]))]))
         }
     },
     ze = ae(Be, [
```

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/EditFiltersView.272e0d14.js` & `opuscleaner-0.2/opuscleaner/frontend/assets/EditFiltersView.bc0dd7c3.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1030 +1,1032 @@
 import {
-    B as Tr,
-    D as Ir,
-    G as Pr,
-    H as Cr,
-    I as Dr,
-    J as Ar,
-    K as Rr,
-    L as wr,
-    M as Mr,
-    n as qn,
-    N as Nr,
-    O as jr,
-    Q as Fr,
-    S as Lr,
-    j as $r,
-    z as dn,
-    i as Jt,
-    y as Ur,
-    V as Vr,
-    W as Gr,
-    X as Br,
-    Y as Kr,
-    Z as Hr,
-    $ as Wr,
-    a0 as Xr,
-    u as B,
-    a1 as Yr,
-    a2 as zr,
-    a3 as Be,
-    a4 as Jr,
-    q as Qr,
+    D as jr,
+    G as Fr,
+    H as $r,
+    I as Lr,
+    J as Vr,
+    K as Ur,
+    L as Gr,
+    M as Br,
+    N as Kr,
+    q as lr,
+    O as Hr,
+    Q as Wr,
+    S as Xr,
+    V as Yr,
+    j as zr,
+    l as pn,
+    i as zt,
+    s as Jr,
+    W as Qr,
+    X as Zr,
+    Y as kr,
+    Z as qr,
+    $ as _r,
+    a0 as to,
+    a1 as eo,
+    u as K,
+    a2 as no,
+    a3 as ro,
+    a4 as We,
+    a5 as oo,
+    x as ao,
     t as it,
-    a5 as Zr,
-    a6 as kr,
-    a7 as qr,
-    F as Dt,
-    a8 as _r,
-    a9 as to,
-    aa as eo,
-    T as _n,
-    ab as no,
-    ac as ro,
-    ad as oo,
-    ae as ao,
-    af as io,
-    k as Qt,
-    a as Ke,
-    s as ee,
-    c as Y,
-    d as Z,
-    ag as so,
-    ah as lo,
-    ai as uo,
-    aj as fo,
-    ak as co,
-    f as Zt,
-    b as Mt,
-    al as vo,
-    am as ho,
-    an as po,
-    ao as go,
-    ap as mo,
-    aq as yo,
-    ar as bo,
-    as as So,
-    at as Eo,
-    au as xo,
-    av as Oo,
-    aw as To,
-    ax as Io,
-    ay as Po,
-    az as Co,
-    aA as Do,
-    aB as Ao,
-    aC as Ro,
-    aD as wo,
-    aE as Mo,
-    aF as No,
-    aG as jo,
-    aH as Fo,
-    aI as Lo,
-    aJ as $o,
-    aK as tr,
-    aL as Uo,
-    aM as Vo,
-    aN as Go,
-    aO as er,
-    aP as nr,
-    o as K,
-    h as wn,
-    aQ as Bo,
-    p as Mn,
-    aR as Ko,
-    aS as Ho,
+    a6 as io,
+    a7 as lo,
+    a8 as so,
+    F as bt,
+    a9 as uo,
+    aa as fo,
+    ab as co,
+    T as sr,
+    ac as vo,
+    ad as po,
+    ae as ho,
+    af as mo,
+    ag as go,
+    m as qt,
+    a as ce,
+    y as _t,
+    c as W,
+    d as X,
+    ah as yo,
+    ai as bo,
+    aj as So,
+    ak as Eo,
+    al as xo,
+    f as Bt,
+    b as Tt,
+    am as Oo,
+    an as To,
+    ao as Io,
+    ap as Po,
+    aq as Co,
+    ar as Do,
+    as as Ao,
+    at as Ro,
+    au as wo,
+    av as Mo,
+    aw as No,
+    ax as jo,
+    ay as Fo,
+    az as $o,
+    aA as Lo,
+    aB as Vo,
+    aC as Uo,
+    aD as Te,
+    aE as Go,
+    aF as Bo,
+    aG as Ko,
+    aH as ur,
+    aI as Ho,
+    aJ as Wo,
+    aK as Xo,
+    aL as jn,
+    aM as Yo,
+    aN as zo,
+    aO as Jo,
+    aP as fr,
+    aQ as cr,
+    o as U,
+    h as Fn,
+    aR as Qo,
+    p as $n,
+    aS as Zo,
+    aT as ko,
     r as Gt,
-    aT as He,
-    aU as rr,
-    aV as Wo,
-    aW as or,
-    aX as Xo,
-    aY as Yo,
-    aZ as zo,
-    a_ as Jo,
-    a$ as Qo,
-    b0 as Zo,
-    b1 as ko,
-    b2 as qo,
-    b3 as _o,
-    b4 as ta,
-    b5 as ea,
-    b6 as na,
-    b7 as ra,
-    b8 as oa,
-    b9 as aa,
-    l as ar,
-    ba as ia,
-    bb as sa,
-    bc as la,
-    bd as ua,
-    w as te,
-    be as fa,
-    m as ca,
-    bf as da,
-    bg as va,
-    bh as ha,
-    bi as pa,
-    bj as ga,
-    bk as ma,
-    bl as ya,
-    bm as ba,
-    bn as Sa,
-    bo as Ea,
-    bp as xa,
-    bq as Oa,
-    br as Ta,
-    bs as Ia,
-    v as Pa,
-    bt as Ca,
-    bu as Da,
-    bv as Aa,
-    bw as Ra,
-    bx as wa,
-    by as Ma,
-    bz as Na,
-    _ as xe,
-    bA as ja,
-    bB as Fa,
-    bC as La,
-    bD as $a,
-    A as Ua,
-    U as Va
-} from "./index.490d1368.js";
+    aU as Qt,
+    aV as dr,
+    aW as qo,
+    aX as Xe,
+    aY as _o,
+    aZ as ta,
+    a_ as ea,
+    a$ as na,
+    b0 as ra,
+    b1 as oa,
+    b2 as aa,
+    b3 as ia,
+    b4 as la,
+    b5 as sa,
+    b6 as ua,
+    b7 as fa,
+    b8 as ca,
+    b9 as da,
+    ba as va,
+    k as vr,
+    A as pa,
+    bb as ha,
+    bc as ma,
+    bd as ga,
+    w as Nt,
+    be as ya,
+    n as ba,
+    bf as Sa,
+    bg as Ea,
+    bh as xa,
+    bi as Oa,
+    bj as Ta,
+    bk as Ia,
+    bl as Pa,
+    bm as Ca,
+    bn as Da,
+    bo as Aa,
+    bp as Ra,
+    bq as wa,
+    br as Ma,
+    bs as Na,
+    v as ja,
+    bt as Fa,
+    bu as $a,
+    bv as La,
+    bw as Va,
+    bx as Ua,
+    by as Ga,
+    bz as Ba,
+    _ as ne,
+    bA as Ka,
+    bB as pr,
+    bC as Ha,
+    bD as Wa,
+    bE as Xa,
+    B as Ya,
+    U as za
+} from "./index.6cc31f0d.js";
 import {
-    T as Ga,
-    a as Ba
-} from "./TagsEditor.8b755087.js";
+    d as hr,
+    a as Ja,
+    T as Qa,
+    b as Za
+} from "./TagsEditor.23cf196f.js";
 import {
-    b as ir,
-    g as Ka
-} from "./filtersteps.2a7228ad.js";
+    g as Ln
+} from "./hacks.1ae1ba64.js";
 import {
-    C as Ha
-} from "./vue-select.6aaeaff8.js";
-const Wa = () => {},
-    Xa = Object.freeze(Object.defineProperty({
+    C as ka
+} from "./vue-select.9ddbca8a.js";
+const qa = () => {},
+    _a = Object.freeze(Object.defineProperty({
         __proto__: null,
-        compile: Wa,
-        EffectScope: Tr,
-        ReactiveEffect: Ir,
-        customRef: Pr,
-        effect: Cr,
-        effectScope: Dr,
-        getCurrentScope: Ar,
-        isProxy: Rr,
-        isReactive: wr,
-        isReadonly: Mr,
-        isRef: qn,
-        isShallow: Nr,
-        markRaw: jr,
-        onScopeDispose: Fr,
-        proxyRefs: Lr,
-        reactive: $r,
-        readonly: dn,
-        ref: Jt,
-        shallowReactive: Ur,
-        shallowReadonly: Vr,
-        shallowRef: Gr,
-        stop: Br,
-        toRaw: Kr,
-        toRef: Hr,
-        toRefs: Wr,
-        triggerRef: Xr,
-        unref: B,
-        camelize: Yr,
-        capitalize: zr,
-        normalizeClass: Be,
-        normalizeProps: Jr,
-        normalizeStyle: Qr,
+        compile: qa,
+        EffectScope: jr,
+        ReactiveEffect: Fr,
+        customRef: $r,
+        effect: Lr,
+        effectScope: Vr,
+        getCurrentScope: Ur,
+        isProxy: Gr,
+        isReactive: Br,
+        isReadonly: Kr,
+        isRef: lr,
+        isShallow: Hr,
+        markRaw: Wr,
+        onScopeDispose: Xr,
+        proxyRefs: Yr,
+        reactive: zr,
+        readonly: pn,
+        ref: zt,
+        shallowReactive: Jr,
+        shallowReadonly: Qr,
+        shallowRef: Zr,
+        stop: kr,
+        toRaw: qr,
+        toRef: _r,
+        toRefs: to,
+        triggerRef: eo,
+        unref: K,
+        camelize: no,
+        capitalize: ro,
+        normalizeClass: We,
+        normalizeProps: oo,
+        normalizeStyle: ao,
         toDisplayString: it,
-        toHandlerKey: Zr,
-        BaseTransition: kr,
-        Comment: qr,
-        Fragment: Dt,
-        KeepAlive: _r,
-        Static: to,
-        Suspense: eo,
-        Teleport: _n,
-        Text: no,
-        callWithAsyncErrorHandling: ro,
-        callWithErrorHandling: oo,
-        cloneVNode: ao,
-        compatUtils: io,
-        computed: Qt,
-        createBlock: Ke,
-        createCommentVNode: ee,
-        createElementBlock: Y,
-        createElementVNode: Z,
-        createHydrationRenderer: so,
-        createPropsRestProxy: lo,
-        createRenderer: uo,
-        createSlots: fo,
-        createStaticVNode: co,
-        createTextVNode: Zt,
-        createVNode: Mt,
-        defineAsyncComponent: vo,
-        defineComponent: ho,
-        defineEmits: po,
-        defineExpose: go,
-        defineProps: mo,
+        toHandlerKey: io,
+        BaseTransition: lo,
+        Comment: so,
+        Fragment: bt,
+        KeepAlive: uo,
+        Static: fo,
+        Suspense: co,
+        Teleport: sr,
+        Text: vo,
+        callWithAsyncErrorHandling: po,
+        callWithErrorHandling: ho,
+        cloneVNode: mo,
+        compatUtils: go,
+        computed: qt,
+        createBlock: ce,
+        createCommentVNode: _t,
+        createElementBlock: W,
+        createElementVNode: X,
+        createHydrationRenderer: yo,
+        createPropsRestProxy: bo,
+        createRenderer: So,
+        createSlots: Eo,
+        createStaticVNode: xo,
+        createTextVNode: Bt,
+        createVNode: Tt,
+        defineAsyncComponent: Oo,
+        defineComponent: To,
+        defineEmits: Io,
+        defineExpose: Po,
+        defineProps: Co,
         get devtools() {
-            return yo
+            return Do
         },
-        getCurrentInstance: bo,
-        getTransitionRawChildren: So,
-        guardReactiveProps: Eo,
-        h: xo,
-        handleError: Oo,
-        initCustomFormatter: To,
-        inject: Io,
-        isMemoSame: Po,
-        isRuntimeOnly: Co,
-        isVNode: Do,
-        mergeDefaults: Ao,
-        mergeProps: Ro,
-        nextTick: wo,
-        onActivated: Mo,
-        onBeforeMount: No,
-        onBeforeUnmount: jo,
-        onBeforeUpdate: Fo,
-        onDeactivated: Lo,
-        onErrorCaptured: $o,
-        onMounted: tr,
-        onRenderTracked: Uo,
-        onRenderTriggered: Vo,
-        onServerPrefetch: Go,
-        onUnmounted: er,
-        onUpdated: nr,
-        openBlock: K,
-        popScopeId: wn,
-        provide: Bo,
-        pushScopeId: Mn,
-        queuePostFlushCb: Ko,
-        registerRuntimeCompiler: Ho,
+        getCurrentInstance: Ao,
+        getTransitionRawChildren: Ro,
+        guardReactiveProps: wo,
+        h: Mo,
+        handleError: No,
+        initCustomFormatter: jo,
+        inject: Fo,
+        isMemoSame: $o,
+        isRuntimeOnly: Lo,
+        isVNode: Vo,
+        mergeDefaults: Uo,
+        mergeProps: Te,
+        nextTick: Go,
+        onActivated: Bo,
+        onBeforeMount: Ko,
+        onBeforeUnmount: ur,
+        onBeforeUpdate: Ho,
+        onDeactivated: Wo,
+        onErrorCaptured: Xo,
+        onMounted: jn,
+        onRenderTracked: Yo,
+        onRenderTriggered: zo,
+        onServerPrefetch: Jo,
+        onUnmounted: fr,
+        onUpdated: cr,
+        openBlock: U,
+        popScopeId: Fn,
+        provide: Qo,
+        pushScopeId: $n,
+        queuePostFlushCb: Zo,
+        registerRuntimeCompiler: ko,
         renderList: Gt,
-        renderSlot: He,
-        resolveComponent: rr,
-        resolveDirective: Wo,
-        resolveDynamicComponent: or,
-        resolveFilter: Xo,
-        resolveTransitionHooks: Yo,
-        setBlockTracking: zo,
-        setDevtoolsHook: Jo,
-        setTransitionHooks: Qo,
-        ssrContextKey: Zo,
-        ssrUtils: ko,
-        toHandlers: qo,
-        transformVNodeArgs: _o,
-        useAttrs: ta,
-        useSSRContext: ea,
-        useSlots: na,
-        useTransitionState: ra,
-        version: oa,
-        warn: aa,
-        watch: ar,
-        watchEffect: ia,
-        watchPostEffect: sa,
-        watchSyncEffect: la,
-        withAsyncContext: ua,
-        withCtx: te,
-        withDefaults: fa,
-        withDirectives: ca,
-        withMemo: da,
-        withScopeId: va,
-        Transition: ha,
-        TransitionGroup: pa,
-        VueElement: ga,
-        createApp: ma,
-        createSSRApp: ya,
-        defineCustomElement: ba,
-        defineSSRCustomElement: Sa,
-        hydrate: Ea,
-        initDirectivesForSSR: xa,
-        render: Oa,
-        useCssModule: Ta,
-        useCssVars: Ia,
-        vModelCheckbox: Pa,
-        vModelDynamic: Ca,
-        vModelRadio: Da,
-        vModelSelect: Aa,
-        vModelText: Ra,
-        vShow: wa,
-        withKeys: Ma,
-        withModifiers: Na
+        renderSlot: Qt,
+        resolveComponent: dr,
+        resolveDirective: qo,
+        resolveDynamicComponent: Xe,
+        resolveFilter: _o,
+        resolveTransitionHooks: ta,
+        setBlockTracking: ea,
+        setDevtoolsHook: na,
+        setTransitionHooks: ra,
+        ssrContextKey: oa,
+        ssrUtils: aa,
+        toHandlers: ia,
+        transformVNodeArgs: la,
+        useAttrs: sa,
+        useSSRContext: ua,
+        useSlots: fa,
+        useTransitionState: ca,
+        version: da,
+        warn: va,
+        watch: vr,
+        watchEffect: pa,
+        watchPostEffect: ha,
+        watchSyncEffect: ma,
+        withAsyncContext: ga,
+        withCtx: Nt,
+        withDefaults: ya,
+        withDirectives: ba,
+        withMemo: Sa,
+        withScopeId: Ea,
+        Transition: xa,
+        TransitionGroup: Oa,
+        VueElement: Ta,
+        createApp: Ia,
+        createSSRApp: Pa,
+        defineCustomElement: Ca,
+        defineSSRCustomElement: Da,
+        hydrate: Aa,
+        initDirectivesForSSR: Ra,
+        render: wa,
+        useCssModule: Ma,
+        useCssVars: Na,
+        vModelCheckbox: ja,
+        vModelDynamic: Fa,
+        vModelRadio: $a,
+        vModelSelect: La,
+        vModelText: Va,
+        vShow: Ua,
+        withKeys: Ga,
+        withModifiers: Ba
     }, Symbol.toStringTag, {
         value: "Module"
     }));
-var Ya = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
+var ti = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
 
-function za(a) {
+function ei(a) {
     return a && a.__esModule && Object.prototype.hasOwnProperty.call(a, "default") ? a.default : a
 }
 
-function sr(a) {
+function mr(a) {
     var e = a.default;
     if (typeof e == "function") {
         var n = function() {
             return e.apply(this, arguments)
         };
         n.prototype = e.prototype
     } else n = {};
     return Object.defineProperty(n, "__esModule", {
         value: !0
-    }), Object.keys(a).forEach(function(l) {
-        var r = Object.getOwnPropertyDescriptor(a, l);
-        Object.defineProperty(n, l, r.get ? r : {
+    }), Object.keys(a).forEach(function(i) {
+        var r = Object.getOwnPropertyDescriptor(a, i);
+        Object.defineProperty(n, i, r.get ? r : {
             enumerable: !0,
             get: function() {
-                return a[l]
+                return a[i]
             }
         })
     }), n
 }
-var lr = {
+var gr = {
     exports: {}
 };
-const Ja = sr(Xa);
+const ni = mr(_a);
 /**!
  * Sortable 1.14.0
  * @author	RubaXa   <trash@rubaxa.org>
  * @author	owenm    <owen23355@gmail.com>
  * @license MIT
  */
-function $n(a, e) {
+function Yn(a, e) {
     var n = Object.keys(a);
     if (Object.getOwnPropertySymbols) {
-        var l = Object.getOwnPropertySymbols(a);
-        e && (l = l.filter(function(r) {
+        var i = Object.getOwnPropertySymbols(a);
+        e && (i = i.filter(function(r) {
             return Object.getOwnPropertyDescriptor(a, r).enumerable
-        })), n.push.apply(n, l)
+        })), n.push.apply(n, i)
     }
     return n
 }
 
-function qt(a) {
+function ee(a) {
     for (var e = 1; e < arguments.length; e++) {
         var n = arguments[e] != null ? arguments[e] : {};
-        e % 2 ? $n(Object(n), !0).forEach(function(l) {
-            Qa(a, l, n[l])
-        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(n)) : $n(Object(n)).forEach(function(l) {
-            Object.defineProperty(a, l, Object.getOwnPropertyDescriptor(n, l))
+        e % 2 ? Yn(Object(n), !0).forEach(function(i) {
+            ri(a, i, n[i])
+        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(a, Object.getOwnPropertyDescriptors(n)) : Yn(Object(n)).forEach(function(i) {
+            Object.defineProperty(a, i, Object.getOwnPropertyDescriptor(n, i))
         })
     }
     return a
 }
 
-function tn(a) {
-    return typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? tn = function(e) {
+function nn(a) {
+    return typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? nn = function(e) {
         return typeof e
-    } : tn = function(e) {
+    } : nn = function(e) {
         return e && typeof Symbol == "function" && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-    }, tn(a)
+    }, nn(a)
 }
 
-function Qa(a, e, n) {
+function ri(a, e, n) {
     return e in a ? Object.defineProperty(a, e, {
         value: n,
         enumerable: !0,
         configurable: !0,
         writable: !0
     }) : a[e] = n, a
 }
 
-function Bt() {
-    return Bt = Object.assign || function(a) {
+function Ht() {
+    return Ht = Object.assign || function(a) {
         for (var e = 1; e < arguments.length; e++) {
             var n = arguments[e];
-            for (var l in n) Object.prototype.hasOwnProperty.call(n, l) && (a[l] = n[l])
+            for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (a[i] = n[i])
         }
         return a
-    }, Bt.apply(this, arguments)
+    }, Ht.apply(this, arguments)
 }
 
-function Za(a, e) {
+function oi(a, e) {
     if (a == null) return {};
     var n = {},
-        l = Object.keys(a),
-        r, u;
-    for (u = 0; u < l.length; u++) r = l[u], !(e.indexOf(r) >= 0) && (n[r] = a[r]);
+        i = Object.keys(a),
+        r, s;
+    for (s = 0; s < i.length; s++) r = i[s], !(e.indexOf(r) >= 0) && (n[r] = a[r]);
     return n
 }
 
-function ka(a, e) {
+function ai(a, e) {
     if (a == null) return {};
-    var n = Za(a, e),
-        l, r;
+    var n = oi(a, e),
+        i, r;
     if (Object.getOwnPropertySymbols) {
-        var u = Object.getOwnPropertySymbols(a);
-        for (r = 0; r < u.length; r++) l = u[r], !(e.indexOf(l) >= 0) && (!Object.prototype.propertyIsEnumerable.call(a, l) || (n[l] = a[l]))
+        var s = Object.getOwnPropertySymbols(a);
+        for (r = 0; r < s.length; r++) i = s[r], !(e.indexOf(i) >= 0) && (!Object.prototype.propertyIsEnumerable.call(a, i) || (n[i] = a[i]))
     }
     return n
 }
 
-function qa(a) {
-    return _a(a) || ti(a) || ei(a) || ni()
+function ii(a) {
+    return li(a) || si(a) || ui(a) || fi()
 }
 
-function _a(a) {
-    if (Array.isArray(a)) return Pn(a)
+function li(a) {
+    if (Array.isArray(a)) return Dn(a)
 }
 
-function ti(a) {
+function si(a) {
     if (typeof Symbol < "u" && a[Symbol.iterator] != null || a["@@iterator"] != null) return Array.from(a)
 }
 
-function ei(a, e) {
+function ui(a, e) {
     if (!!a) {
-        if (typeof a == "string") return Pn(a, e);
+        if (typeof a == "string") return Dn(a, e);
         var n = Object.prototype.toString.call(a).slice(8, -1);
         if (n === "Object" && a.constructor && (n = a.constructor.name), n === "Map" || n === "Set") return Array.from(a);
-        if (n === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Pn(a, e)
+        if (n === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Dn(a, e)
     }
 }
 
-function Pn(a, e) {
+function Dn(a, e) {
     (e == null || e > a.length) && (e = a.length);
-    for (var n = 0, l = new Array(e); n < e; n++) l[n] = a[n];
-    return l
+    for (var n = 0, i = new Array(e); n < e; n++) i[n] = a[n];
+    return i
 }
 
-function ni() {
+function fi() {
     throw new TypeError(`Invalid attempt to spread non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
-var ri = "1.14.0";
+var ci = "1.14.0";
 
-function ne(a) {
+function oe(a) {
     if (typeof window < "u" && window.navigator) return !!navigator.userAgent.match(a)
 }
-var re = ne(/(?:Trident.*rv[ :]?11\.|msie|iemobile|Windows Phone)/i),
-    We = ne(/Edge/i),
-    Un = ne(/firefox/i),
-    Le = ne(/safari/i) && !ne(/chrome/i) && !ne(/android/i),
-    ur = ne(/iP(ad|od|hone)/i),
-    oi = ne(/chrome/i) && ne(/android/i),
-    fr = {
+var ae = oe(/(?:Trident.*rv[ :]?11\.|msie|iemobile|Windows Phone)/i),
+    Ye = oe(/Edge/i),
+    zn = oe(/firefox/i),
+    Ue = oe(/safari/i) && !oe(/chrome/i) && !oe(/android/i),
+    yr = oe(/iP(ad|od|hone)/i),
+    di = oe(/chrome/i) && oe(/android/i),
+    br = {
         capture: !1,
         passive: !1
     };
 
 function et(a, e, n) {
-    a.addEventListener(e, n, !re && fr)
+    a.addEventListener(e, n, !ae && br)
 }
 
 function tt(a, e, n) {
-    a.removeEventListener(e, n, !re && fr)
+    a.removeEventListener(e, n, !ae && br)
 }
 
-function sn(a, e) {
+function un(a, e) {
     if (!!e) {
         if (e[0] === ">" && (e = e.substring(1)), a) try {
             if (a.matches) return a.matches(e);
             if (a.msMatchesSelector) return a.msMatchesSelector(e);
             if (a.webkitMatchesSelector) return a.webkitMatchesSelector(e)
         } catch {
             return !1
         }
         return !1
     }
 }
 
-function ai(a) {
+function vi(a) {
     return a.host && a !== document && a.host.nodeType ? a.host : a.parentNode
 }
 
-function Xt(a, e, n, l) {
+function Jt(a, e, n, i) {
     if (a) {
         n = n || document;
         do {
-            if (e != null && (e[0] === ">" ? a.parentNode === n && sn(a, e) : sn(a, e)) || l && a === n) return a;
+            if (e != null && (e[0] === ">" ? a.parentNode === n && un(a, e) : un(a, e)) || i && a === n) return a;
             if (a === n) break
-        } while (a = ai(a))
+        } while (a = vi(a))
     }
     return null
 }
-var Vn = /\s+/g;
+var Jn = /\s+/g;
 
-function dt(a, e, n) {
+function vt(a, e, n) {
     if (a && e)
         if (a.classList) a.classList[n ? "add" : "remove"](e);
         else {
-            var l = (" " + a.className + " ").replace(Vn, " ").replace(" " + e + " ", " ");
-            a.className = (l + (n ? " " + e : "")).replace(Vn, " ")
+            var i = (" " + a.className + " ").replace(Jn, " ").replace(" " + e + " ", " ");
+            a.className = (i + (n ? " " + e : "")).replace(Jn, " ")
         }
 }
 
-function U(a, e, n) {
-    var l = a && a.style;
-    if (l) {
+function G(a, e, n) {
+    var i = a && a.style;
+    if (i) {
         if (n === void 0) return document.defaultView && document.defaultView.getComputedStyle ? n = document.defaultView.getComputedStyle(a, "") : a.currentStyle && (n = a.currentStyle), e === void 0 ? n : n[e];
-        !(e in l) && e.indexOf("webkit") === -1 && (e = "-webkit-" + e), l[e] = n + (typeof n == "string" ? "" : "px")
+        !(e in i) && e.indexOf("webkit") === -1 && (e = "-webkit-" + e), i[e] = n + (typeof n == "string" ? "" : "px")
     }
 }
 
-function he(a, e) {
+function ge(a, e) {
     var n = "";
     if (typeof a == "string") n = a;
     else
         do {
-            var l = U(a, "transform");
-            l && l !== "none" && (n = l + " " + n)
+            var i = G(a, "transform");
+            i && i !== "none" && (n = i + " " + n)
         } while (!e && (a = a.parentNode));
     var r = window.DOMMatrix || window.WebKitCSSMatrix || window.CSSMatrix || window.MSCSSMatrix;
     return r && new r(n)
 }
 
-function cr(a, e, n) {
+function Sr(a, e, n) {
     if (a) {
-        var l = a.getElementsByTagName(e),
+        var i = a.getElementsByTagName(e),
             r = 0,
-            u = l.length;
+            s = i.length;
         if (n)
-            for (; r < u; r++) n(l[r], r);
-        return l
+            for (; r < s; r++) n(i[r], r);
+        return i
     }
     return []
 }
 
-function kt() {
+function te() {
     var a = document.scrollingElement;
     return a || document.documentElement
 }
 
-function ft(a, e, n, l, r) {
+function ft(a, e, n, i, r) {
     if (!(!a.getBoundingClientRect && a !== window)) {
-        var u, t, o, i, s, c, f;
-        if (a !== window && a.parentNode && a !== kt() ? (u = a.getBoundingClientRect(), t = u.top, o = u.left, i = u.bottom, s = u.right, c = u.height, f = u.width) : (t = 0, o = 0, i = window.innerHeight, s = window.innerWidth, c = window.innerHeight, f = window.innerWidth), (e || n) && a !== window && (r = r || a.parentNode, !re))
+        var s, t, o, l, u, f, c;
+        if (a !== window && a.parentNode && a !== te() ? (s = a.getBoundingClientRect(), t = s.top, o = s.left, l = s.bottom, u = s.right, f = s.height, c = s.width) : (t = 0, o = 0, l = window.innerHeight, u = window.innerWidth, f = window.innerHeight, c = window.innerWidth), (e || n) && a !== window && (r = r || a.parentNode, !ae))
             do
-                if (r && r.getBoundingClientRect && (U(r, "transform") !== "none" || n && U(r, "position") !== "static")) {
+                if (r && r.getBoundingClientRect && (G(r, "transform") !== "none" || n && G(r, "position") !== "static")) {
                     var d = r.getBoundingClientRect();
-                    t -= d.top + parseInt(U(r, "border-top-width")), o -= d.left + parseInt(U(r, "border-left-width")), i = t + u.height, s = o + u.width;
+                    t -= d.top + parseInt(G(r, "border-top-width")), o -= d.left + parseInt(G(r, "border-left-width")), l = t + s.height, u = o + s.width;
                     break
                 } while (r = r.parentNode);
-        if (l && a !== window) {
-            var v = he(r || a),
-                h = v && v.a,
-                p = v && v.d;
-            v && (t /= p, o /= h, f /= h, c /= p, i = t + c, s = o + f)
+        if (i && a !== window) {
+            var v = ge(r || a),
+                p = v && v.a,
+                h = v && v.d;
+            v && (t /= h, o /= p, c /= p, f /= h, l = t + f, u = o + c)
         }
         return {
             top: t,
             left: o,
-            bottom: i,
-            right: s,
-            width: f,
-            height: c
+            bottom: l,
+            right: u,
+            width: c,
+            height: f
         }
     }
 }
 
-function Gn(a, e, n) {
-    for (var l = le(a, !0), r = ft(a)[e]; l;) {
-        var u = ft(l)[n],
+function Qn(a, e, n) {
+    for (var i = fe(a, !0), r = ft(a)[e]; i;) {
+        var s = ft(i)[n],
             t = void 0;
-        if (n === "top" || n === "left" ? t = r >= u : t = r <= u, !t) return l;
-        if (l === kt()) break;
-        l = le(l, !1)
+        if (n === "top" || n === "left" ? t = r >= s : t = r <= s, !t) return i;
+        if (i === te()) break;
+        i = fe(i, !1)
     }
     return !1
 }
 
-function Ee(a, e, n, l) {
-    for (var r = 0, u = 0, t = a.children; u < t.length;) {
-        if (t[u].style.display !== "none" && t[u] !== W.ghost && (l || t[u] !== W.dragged) && Xt(t[u], n.draggable, a, !1)) {
-            if (r === e) return t[u];
+function Ie(a, e, n, i) {
+    for (var r = 0, s = 0, t = a.children; s < t.length;) {
+        if (t[s].style.display !== "none" && t[s] !== z.ghost && (i || t[s] !== z.dragged) && Jt(t[s], n.draggable, a, !1)) {
+            if (r === e) return t[s];
             r++
         }
-        u++
+        s++
     }
     return null
 }
 
-function Nn(a, e) {
-    for (var n = a.lastElementChild; n && (n === W.ghost || U(n, "display") === "none" || e && !sn(n, e));) n = n.previousElementSibling;
+function Vn(a, e) {
+    for (var n = a.lastElementChild; n && (n === z.ghost || G(n, "display") === "none" || e && !un(n, e));) n = n.previousElementSibling;
     return n || null
 }
 
-function mt(a, e) {
+function gt(a, e) {
     var n = 0;
     if (!a || !a.parentNode) return -1;
-    for (; a = a.previousElementSibling;) a.nodeName.toUpperCase() !== "TEMPLATE" && a !== W.clone && (!e || sn(a, e)) && n++;
+    for (; a = a.previousElementSibling;) a.nodeName.toUpperCase() !== "TEMPLATE" && a !== z.clone && (!e || un(a, e)) && n++;
     return n
 }
 
-function Bn(a) {
+function Zn(a) {
     var e = 0,
         n = 0,
-        l = kt();
+        i = te();
     if (a)
         do {
-            var r = he(a),
-                u = r.a,
+            var r = ge(a),
+                s = r.a,
                 t = r.d;
-            e += a.scrollLeft * u, n += a.scrollTop * t
-        } while (a !== l && (a = a.parentNode));
+            e += a.scrollLeft * s, n += a.scrollTop * t
+        } while (a !== i && (a = a.parentNode));
     return [e, n]
 }
 
-function ii(a, e) {
+function pi(a, e) {
     for (var n in a)
         if (!!a.hasOwnProperty(n)) {
-            for (var l in e)
-                if (e.hasOwnProperty(l) && e[l] === a[n][l]) return Number(n)
+            for (var i in e)
+                if (e.hasOwnProperty(i) && e[i] === a[n][i]) return Number(n)
         } return -1
 }
 
-function le(a, e) {
-    if (!a || !a.getBoundingClientRect) return kt();
+function fe(a, e) {
+    if (!a || !a.getBoundingClientRect) return te();
     var n = a,
-        l = !1;
+        i = !1;
     do
         if (n.clientWidth < n.scrollWidth || n.clientHeight < n.scrollHeight) {
-            var r = U(n);
+            var r = G(n);
             if (n.clientWidth < n.scrollWidth && (r.overflowX == "auto" || r.overflowX == "scroll") || n.clientHeight < n.scrollHeight && (r.overflowY == "auto" || r.overflowY == "scroll")) {
-                if (!n.getBoundingClientRect || n === document.body) return kt();
-                if (l || e) return n;
-                l = !0
+                if (!n.getBoundingClientRect || n === document.body) return te();
+                if (i || e) return n;
+                i = !0
             }
         } while (n = n.parentNode);
-    return kt()
+    return te()
 }
 
-function si(a, e) {
+function hi(a, e) {
     if (a && e)
         for (var n in e) e.hasOwnProperty(n) && (a[n] = e[n]);
     return a
 }
 
-function gn(a, e) {
+function yn(a, e) {
     return Math.round(a.top) === Math.round(e.top) && Math.round(a.left) === Math.round(e.left) && Math.round(a.height) === Math.round(e.height) && Math.round(a.width) === Math.round(e.width)
 }
-var $e;
+var Ge;
 
-function dr(a, e) {
+function Er(a, e) {
     return function() {
-        if (!$e) {
+        if (!Ge) {
             var n = arguments,
-                l = this;
-            n.length === 1 ? a.call(l, n[0]) : a.apply(l, n), $e = setTimeout(function() {
-                $e = void 0
+                i = this;
+            n.length === 1 ? a.call(i, n[0]) : a.apply(i, n), Ge = setTimeout(function() {
+                Ge = void 0
             }, e)
         }
     }
 }
 
-function li() {
-    clearTimeout($e), $e = void 0
+function mi() {
+    clearTimeout(Ge), Ge = void 0
 }
 
-function vr(a, e, n) {
+function xr(a, e, n) {
     a.scrollLeft += e, a.scrollTop += n
 }
 
-function jn(a) {
+function Un(a) {
     var e = window.Polymer,
         n = window.jQuery || window.Zepto;
     return e && e.dom ? e.dom(a).cloneNode(!0) : n ? n(a).clone(!0)[0] : a.cloneNode(!0)
 }
 
-function Kn(a, e) {
-    U(a, "position", "absolute"), U(a, "top", e.top), U(a, "left", e.left), U(a, "width", e.width), U(a, "height", e.height)
+function kn(a, e) {
+    G(a, "position", "absolute"), G(a, "top", e.top), G(a, "left", e.left), G(a, "width", e.width), G(a, "height", e.height)
 }
 
-function mn(a) {
-    U(a, "position", ""), U(a, "top", ""), U(a, "left", ""), U(a, "width", ""), U(a, "height", "")
+function bn(a) {
+    G(a, "position", ""), G(a, "top", ""), G(a, "left", ""), G(a, "width", ""), G(a, "height", "")
 }
-var At = "Sortable" + new Date().getTime();
+var Rt = "Sortable" + new Date().getTime();
 
-function ui() {
+function gi() {
     var a = [],
         e;
     return {
         captureAnimationState: function() {
             if (a = [], !!this.options.animation) {
-                var l = [].slice.call(this.el.children);
-                l.forEach(function(r) {
-                    if (!(U(r, "display") === "none" || r === W.ghost)) {
+                var i = [].slice.call(this.el.children);
+                i.forEach(function(r) {
+                    if (!(G(r, "display") === "none" || r === z.ghost)) {
                         a.push({
                             target: r,
                             rect: ft(r)
                         });
-                        var u = qt({}, a[a.length - 1].rect);
+                        var s = ee({}, a[a.length - 1].rect);
                         if (r.thisAnimationDuration) {
-                            var t = he(r, !0);
-                            t && (u.top -= t.f, u.left -= t.e)
+                            var t = ge(r, !0);
+                            t && (s.top -= t.f, s.left -= t.e)
                         }
-                        r.fromRect = u
+                        r.fromRect = s
                     }
                 })
             }
         },
-        addAnimationState: function(l) {
-            a.push(l)
+        addAnimationState: function(i) {
+            a.push(i)
         },
-        removeAnimationState: function(l) {
-            a.splice(ii(a, {
-                target: l
+        removeAnimationState: function(i) {
+            a.splice(pi(a, {
+                target: i
             }), 1)
         },
-        animateAll: function(l) {
+        animateAll: function(i) {
             var r = this;
             if (!this.options.animation) {
-                clearTimeout(e), typeof l == "function" && l();
+                clearTimeout(e), typeof i == "function" && i();
                 return
             }
-            var u = !1,
+            var s = !1,
                 t = 0;
             a.forEach(function(o) {
-                var i = 0,
-                    s = o.target,
-                    c = s.fromRect,
-                    f = ft(s),
-                    d = s.prevFromRect,
-                    v = s.prevToRect,
-                    h = o.rect,
-                    p = he(s, !0);
-                p && (f.top -= p.f, f.left -= p.e), s.toRect = f, s.thisAnimationDuration && gn(d, f) && !gn(c, f) && (h.top - f.top) / (h.left - f.left) === (c.top - f.top) / (c.left - f.left) && (i = ci(h, d, v, r.options)), gn(f, c) || (s.prevFromRect = c, s.prevToRect = f, i || (i = r.options.animation), r.animate(s, h, f, i)), i && (u = !0, t = Math.max(t, i), clearTimeout(s.animationResetTimer), s.animationResetTimer = setTimeout(function() {
-                    s.animationTime = 0, s.prevFromRect = null, s.fromRect = null, s.prevToRect = null, s.thisAnimationDuration = null
-                }, i), s.thisAnimationDuration = i)
-            }), clearTimeout(e), u ? e = setTimeout(function() {
-                typeof l == "function" && l()
-            }, t) : typeof l == "function" && l(), a = []
+                var l = 0,
+                    u = o.target,
+                    f = u.fromRect,
+                    c = ft(u),
+                    d = u.prevFromRect,
+                    v = u.prevToRect,
+                    p = o.rect,
+                    h = ge(u, !0);
+                h && (c.top -= h.f, c.left -= h.e), u.toRect = c, u.thisAnimationDuration && yn(d, c) && !yn(f, c) && (p.top - c.top) / (p.left - c.left) === (f.top - c.top) / (f.left - c.left) && (l = bi(p, d, v, r.options)), yn(c, f) || (u.prevFromRect = f, u.prevToRect = c, l || (l = r.options.animation), r.animate(u, p, c, l)), l && (s = !0, t = Math.max(t, l), clearTimeout(u.animationResetTimer), u.animationResetTimer = setTimeout(function() {
+                    u.animationTime = 0, u.prevFromRect = null, u.fromRect = null, u.prevToRect = null, u.thisAnimationDuration = null
+                }, l), u.thisAnimationDuration = l)
+            }), clearTimeout(e), s ? e = setTimeout(function() {
+                typeof i == "function" && i()
+            }, t) : typeof i == "function" && i(), a = []
         },
-        animate: function(l, r, u, t) {
+        animate: function(i, r, s, t) {
             if (t) {
-                U(l, "transition", ""), U(l, "transform", "");
-                var o = he(this.el),
-                    i = o && o.a,
-                    s = o && o.d,
-                    c = (r.left - u.left) / (i || 1),
-                    f = (r.top - u.top) / (s || 1);
-                l.animatingX = !!c, l.animatingY = !!f, U(l, "transform", "translate3d(" + c + "px," + f + "px,0)"), this.forRepaintDummy = fi(l), U(l, "transition", "transform " + t + "ms" + (this.options.easing ? " " + this.options.easing : "")), U(l, "transform", "translate3d(0,0,0)"), typeof l.animated == "number" && clearTimeout(l.animated), l.animated = setTimeout(function() {
-                    U(l, "transition", ""), U(l, "transform", ""), l.animated = !1, l.animatingX = !1, l.animatingY = !1
+                G(i, "transition", ""), G(i, "transform", "");
+                var o = ge(this.el),
+                    l = o && o.a,
+                    u = o && o.d,
+                    f = (r.left - s.left) / (l || 1),
+                    c = (r.top - s.top) / (u || 1);
+                i.animatingX = !!f, i.animatingY = !!c, G(i, "transform", "translate3d(" + f + "px," + c + "px,0)"), this.forRepaintDummy = yi(i), G(i, "transition", "transform " + t + "ms" + (this.options.easing ? " " + this.options.easing : "")), G(i, "transform", "translate3d(0,0,0)"), typeof i.animated == "number" && clearTimeout(i.animated), i.animated = setTimeout(function() {
+                    G(i, "transition", ""), G(i, "transform", ""), i.animated = !1, i.animatingX = !1, i.animatingY = !1
                 }, t)
             }
         }
     }
 }
 
-function fi(a) {
+function yi(a) {
     return a.offsetWidth
 }
 
-function ci(a, e, n, l) {
-    return Math.sqrt(Math.pow(e.top - a.top, 2) + Math.pow(e.left - a.left, 2)) / Math.sqrt(Math.pow(e.top - n.top, 2) + Math.pow(e.left - n.left, 2)) * l.animation
+function bi(a, e, n, i) {
+    return Math.sqrt(Math.pow(e.top - a.top, 2) + Math.pow(e.left - a.left, 2)) / Math.sqrt(Math.pow(e.top - n.top, 2) + Math.pow(e.left - n.left, 2)) * i.animation
 }
-var ge = [],
-    yn = {
+var be = [],
+    Sn = {
         initializeByDefault: !0
     },
-    Xe = {
+    ze = {
         mount: function(e) {
-            for (var n in yn) yn.hasOwnProperty(n) && !(n in e) && (e[n] = yn[n]);
-            ge.forEach(function(l) {
-                if (l.pluginName === e.pluginName) throw "Sortable: Cannot mount plugin ".concat(e.pluginName, " more than once")
-            }), ge.push(e)
+            for (var n in Sn) Sn.hasOwnProperty(n) && !(n in e) && (e[n] = Sn[n]);
+            be.forEach(function(i) {
+                if (i.pluginName === e.pluginName) throw "Sortable: Cannot mount plugin ".concat(e.pluginName, " more than once")
+            }), be.push(e)
         },
-        pluginEvent: function(e, n, l) {
+        pluginEvent: function(e, n, i) {
             var r = this;
-            this.eventCanceled = !1, l.cancel = function() {
+            this.eventCanceled = !1, i.cancel = function() {
                 r.eventCanceled = !0
             };
-            var u = e + "Global";
-            ge.forEach(function(t) {
-                !n[t.pluginName] || (n[t.pluginName][u] && n[t.pluginName][u](qt({
+            var s = e + "Global";
+            be.forEach(function(t) {
+                !n[t.pluginName] || (n[t.pluginName][s] && n[t.pluginName][s](ee({
                     sortable: n
-                }, l)), n.options[t.pluginName] && n[t.pluginName][e] && n[t.pluginName][e](qt({
+                }, i)), n.options[t.pluginName] && n[t.pluginName][e] && n[t.pluginName][e](ee({
                     sortable: n
-                }, l)))
+                }, i)))
             })
         },
-        initializePlugins: function(e, n, l, r) {
-            ge.forEach(function(o) {
-                var i = o.pluginName;
-                if (!(!e.options[i] && !o.initializeByDefault)) {
-                    var s = new o(e, n, e.options);
-                    s.sortable = e, s.options = e.options, e[i] = s, Bt(l, s.defaults)
+        initializePlugins: function(e, n, i, r) {
+            be.forEach(function(o) {
+                var l = o.pluginName;
+                if (!(!e.options[l] && !o.initializeByDefault)) {
+                    var u = new o(e, n, e.options);
+                    u.sortable = e, u.options = e.options, e[l] = u, Ht(i, u.defaults)
                 }
             });
-            for (var u in e.options)
-                if (!!e.options.hasOwnProperty(u)) {
-                    var t = this.modifyOption(e, u, e.options[u]);
-                    typeof t < "u" && (e.options[u] = t)
+            for (var s in e.options)
+                if (!!e.options.hasOwnProperty(s)) {
+                    var t = this.modifyOption(e, s, e.options[s]);
+                    typeof t < "u" && (e.options[s] = t)
                 }
         },
         getEventProperties: function(e, n) {
-            var l = {};
-            return ge.forEach(function(r) {
-                typeof r.eventProperties == "function" && Bt(l, r.eventProperties.call(n[r.pluginName], e))
-            }), l
+            var i = {};
+            return be.forEach(function(r) {
+                typeof r.eventProperties == "function" && Ht(i, r.eventProperties.call(n[r.pluginName], e))
+            }), i
         },
-        modifyOption: function(e, n, l) {
+        modifyOption: function(e, n, i) {
             var r;
-            return ge.forEach(function(u) {
-                !e[u.pluginName] || u.optionListeners && typeof u.optionListeners[n] == "function" && (r = u.optionListeners[n].call(e[u.pluginName], l))
+            return be.forEach(function(s) {
+                !e[s.pluginName] || s.optionListeners && typeof s.optionListeners[n] == "function" && (r = s.optionListeners[n].call(e[s.pluginName], i))
             }), r
         }
     };
 
-function Me(a) {
+function Fe(a) {
     var e = a.sortable,
         n = a.rootEl,
-        l = a.name,
+        i = a.name,
         r = a.targetEl,
-        u = a.cloneEl,
+        s = a.cloneEl,
         t = a.toEl,
         o = a.fromEl,
-        i = a.oldIndex,
-        s = a.newIndex,
-        c = a.oldDraggableIndex,
-        f = a.newDraggableIndex,
+        l = a.oldIndex,
+        u = a.newIndex,
+        f = a.oldDraggableIndex,
+        c = a.newDraggableIndex,
         d = a.originalEvent,
         v = a.putSortable,
-        h = a.extraEventProperties;
-    if (e = e || n && n[At], !!e) {
-        var p, g = e.options,
-            b = "on" + l.charAt(0).toUpperCase() + l.substr(1);
-        window.CustomEvent && !re && !We ? p = new CustomEvent(l, {
+        p = a.extraEventProperties;
+    if (e = e || n && n[Rt], !!e) {
+        var h, m = e.options,
+            g = "on" + i.charAt(0).toUpperCase() + i.substr(1);
+        window.CustomEvent && !ae && !Ye ? h = new CustomEvent(i, {
             bubbles: !0,
             cancelable: !0
-        }) : (p = document.createEvent("Event"), p.initEvent(l, !0, !0)), p.to = t || n, p.from = o || n, p.item = r || n, p.clone = u, p.oldIndex = i, p.newIndex = s, p.oldDraggableIndex = c, p.newDraggableIndex = f, p.originalEvent = d, p.pullMode = v ? v.lastPutMode : void 0;
-        var S = qt(qt({}, h), Xe.getEventProperties(l, e));
-        for (var P in S) p[P] = S[P];
-        n && n.dispatchEvent(p), g[b] && g[b].call(e, p)
+        }) : (h = document.createEvent("Event"), h.initEvent(i, !0, !0)), h.to = t || n, h.from = o || n, h.item = r || n, h.clone = s, h.oldIndex = l, h.newIndex = u, h.oldDraggableIndex = f, h.newDraggableIndex = c, h.originalEvent = d, h.pullMode = v ? v.lastPutMode : void 0;
+        var y = ee(ee({}, p), ze.getEventProperties(i, e));
+        for (var O in y) h[O] = y[O];
+        n && n.dispatchEvent(h), m[g] && m[g].call(e, h)
     }
 }
-var di = ["evt"],
-    jt = function(e, n) {
-        var l = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {},
-            r = l.evt,
-            u = ka(l, di);
-        Xe.pluginEvent.bind(W)(e, n, qt({
-            dragEl: N,
-            parentEl: pt,
-            ghostEl: k,
+var Si = ["evt"],
+    Ft = function(e, n) {
+        var i = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {},
+            r = i.evt,
+            s = ai(i, Si);
+        ze.pluginEvent.bind(z)(e, n, ee({
+            dragEl: w,
+            parentEl: ht,
+            ghostEl: q,
             rootEl: ut,
-            nextEl: ve,
-            lastDownEl: en,
-            cloneEl: gt,
-            cloneHidden: se,
-            dragStarted: Ne,
-            putSortable: Pt,
-            activeSortable: W.active,
+            nextEl: me,
+            lastDownEl: rn,
+            cloneEl: mt,
+            cloneHidden: ue,
+            dragStarted: $e,
+            putSortable: Dt,
+            activeSortable: z.active,
             originalEvent: r,
-            oldIndex: Se,
-            oldDraggableIndex: Ue,
+            oldIndex: Oe,
+            oldDraggableIndex: Be,
             newIndex: Ut,
-            newDraggableIndex: ie,
-            hideGhostForTarget: mr,
-            unhideGhostForTarget: yr,
+            newDraggableIndex: se,
+            hideGhostForTarget: Pr,
+            unhideGhostForTarget: Cr,
             cloneNowHidden: function() {
-                se = !0
+                ue = !0
             },
             cloneNowShown: function() {
-                se = !1
+                ue = !1
             },
             dispatchSortableEvent: function(o) {
-                wt({
+                Mt({
                     sortable: n,
                     name: o,
                     originalEvent: r
                 })
             }
-        }, u))
+        }, s))
     };
 
-function wt(a) {
-    Me(qt({
-        putSortable: Pt,
-        cloneEl: gt,
-        targetEl: N,
+function Mt(a) {
+    Fe(ee({
+        putSortable: Dt,
+        cloneEl: mt,
+        targetEl: w,
         rootEl: ut,
-        oldIndex: Se,
-        oldDraggableIndex: Ue,
+        oldIndex: Oe,
+        oldDraggableIndex: Be,
         newIndex: Ut,
-        newDraggableIndex: ie
+        newDraggableIndex: se
     }, a))
 }
-var N, pt, k, ut, ve, en, gt, se, Se, Ut, Ue, ie, Je, Pt, be = !1,
-    ln = !1,
-    un = [],
-    ce, Ht, bn, Sn, Hn, Wn, Ne, me, Ve, Ge = !1,
-    Qe = !1,
-    nn, Ct, En = [],
-    Cn = !1,
-    fn = [],
-    vn = typeof document < "u",
-    Ze = ur,
-    Xn = We || re ? "cssFloat" : "float",
-    vi = vn && !oi && !ur && "draggable" in document.createElement("div"),
-    hr = function() {
-        if (!!vn) {
-            if (re) return !1;
+var w, ht, q, ut, me, rn, mt, ue, Oe, Ut, Be, se, Ze, Dt, xe = !1,
+    fn = !1,
+    cn = [],
+    pe, Xt, En, xn, qn, _n, $e, Se, Ke, He = !1,
+    ke = !1,
+    on, At, On = [],
+    An = !1,
+    dn = [],
+    hn = typeof document < "u",
+    qe = yr,
+    tr = Ye || ae ? "cssFloat" : "float",
+    Ei = hn && !di && !yr && "draggable" in document.createElement("div"),
+    Or = function() {
+        if (!!hn) {
+            if (ae) return !1;
             var a = document.createElement("x");
             return a.style.cssText = "pointer-events:auto", a.style.pointerEvents === "auto"
         }
     }(),
-    pr = function(e, n) {
-        var l = U(e),
-            r = parseInt(l.width) - parseInt(l.paddingLeft) - parseInt(l.paddingRight) - parseInt(l.borderLeftWidth) - parseInt(l.borderRightWidth),
-            u = Ee(e, 0, n),
-            t = Ee(e, 1, n),
-            o = u && U(u),
-            i = t && U(t),
-            s = o && parseInt(o.marginLeft) + parseInt(o.marginRight) + ft(u).width,
-            c = i && parseInt(i.marginLeft) + parseInt(i.marginRight) + ft(t).width;
-        if (l.display === "flex") return l.flexDirection === "column" || l.flexDirection === "column-reverse" ? "vertical" : "horizontal";
-        if (l.display === "grid") return l.gridTemplateColumns.split(" ").length <= 1 ? "vertical" : "horizontal";
-        if (u && o.float && o.float !== "none") {
-            var f = o.float === "left" ? "left" : "right";
-            return t && (i.clear === "both" || i.clear === f) ? "vertical" : "horizontal"
-        }
-        return u && (o.display === "block" || o.display === "flex" || o.display === "table" || o.display === "grid" || s >= r && l[Xn] === "none" || t && l[Xn] === "none" && s + c > r) ? "vertical" : "horizontal"
-    },
-    hi = function(e, n, l) {
-        var r = l ? e.left : e.top,
-            u = l ? e.right : e.bottom,
-            t = l ? e.width : e.height,
-            o = l ? n.left : n.top,
-            i = l ? n.right : n.bottom,
-            s = l ? n.width : n.height;
-        return r === o || u === i || r + t / 2 === o + s / 2
-    },
-    pi = function(e, n) {
-        var l;
-        return un.some(function(r) {
-            var u = r[At].options.emptyInsertThreshold;
-            if (!(!u || Nn(r))) {
+    Tr = function(e, n) {
+        var i = G(e),
+            r = parseInt(i.width) - parseInt(i.paddingLeft) - parseInt(i.paddingRight) - parseInt(i.borderLeftWidth) - parseInt(i.borderRightWidth),
+            s = Ie(e, 0, n),
+            t = Ie(e, 1, n),
+            o = s && G(s),
+            l = t && G(t),
+            u = o && parseInt(o.marginLeft) + parseInt(o.marginRight) + ft(s).width,
+            f = l && parseInt(l.marginLeft) + parseInt(l.marginRight) + ft(t).width;
+        if (i.display === "flex") return i.flexDirection === "column" || i.flexDirection === "column-reverse" ? "vertical" : "horizontal";
+        if (i.display === "grid") return i.gridTemplateColumns.split(" ").length <= 1 ? "vertical" : "horizontal";
+        if (s && o.float && o.float !== "none") {
+            var c = o.float === "left" ? "left" : "right";
+            return t && (l.clear === "both" || l.clear === c) ? "vertical" : "horizontal"
+        }
+        return s && (o.display === "block" || o.display === "flex" || o.display === "table" || o.display === "grid" || u >= r && i[tr] === "none" || t && i[tr] === "none" && u + f > r) ? "vertical" : "horizontal"
+    },
+    xi = function(e, n, i) {
+        var r = i ? e.left : e.top,
+            s = i ? e.right : e.bottom,
+            t = i ? e.width : e.height,
+            o = i ? n.left : n.top,
+            l = i ? n.right : n.bottom,
+            u = i ? n.width : n.height;
+        return r === o || s === l || r + t / 2 === o + u / 2
+    },
+    Oi = function(e, n) {
+        var i;
+        return cn.some(function(r) {
+            var s = r[Rt].options.emptyInsertThreshold;
+            if (!(!s || Vn(r))) {
                 var t = ft(r),
-                    o = e >= t.left - u && e <= t.right + u,
-                    i = n >= t.top - u && n <= t.bottom + u;
-                if (o && i) return l = r
-            }
-        }), l
-    },
-    gr = function(e) {
-        function n(u, t) {
-            return function(o, i, s, c) {
-                var f = o.options.group.name && i.options.group.name && o.options.group.name === i.options.group.name;
-                if (u == null && (t || f)) return !0;
-                if (u == null || u === !1) return !1;
-                if (t && u === "clone") return u;
-                if (typeof u == "function") return n(u(o, i, s, c), t)(o, i, s, c);
-                var d = (t ? o : i).options.group.name;
-                return u === !0 || typeof u == "string" && u === d || u.join && u.indexOf(d) > -1
+                    o = e >= t.left - s && e <= t.right + s,
+                    l = n >= t.top - s && n <= t.bottom + s;
+                if (o && l) return i = r
+            }
+        }), i
+    },
+    Ir = function(e) {
+        function n(s, t) {
+            return function(o, l, u, f) {
+                var c = o.options.group.name && l.options.group.name && o.options.group.name === l.options.group.name;
+                if (s == null && (t || c)) return !0;
+                if (s == null || s === !1) return !1;
+                if (t && s === "clone") return s;
+                if (typeof s == "function") return n(s(o, l, u, f), t)(o, l, u, f);
+                var d = (t ? o : l).options.group.name;
+                return s === !0 || typeof s == "string" && s === d || s.join && s.indexOf(d) > -1
             }
         }
-        var l = {},
+        var i = {},
             r = e.group;
-        (!r || tn(r) != "object") && (r = {
+        (!r || nn(r) != "object") && (r = {
             name: r
-        }), l.name = r.name, l.checkPull = n(r.pull, !0), l.checkPut = n(r.put), l.revertClone = r.revertClone, e.group = l
+        }), i.name = r.name, i.checkPull = n(r.pull, !0), i.checkPut = n(r.put), i.revertClone = r.revertClone, e.group = i
     },
-    mr = function() {
-        !hr && k && U(k, "display", "none")
+    Pr = function() {
+        !Or && q && G(q, "display", "none")
     },
-    yr = function() {
-        !hr && k && U(k, "display", "")
+    Cr = function() {
+        !Or && q && G(q, "display", "")
     };
-vn && document.addEventListener("click", function(a) {
-    if (ln) return a.preventDefault(), a.stopPropagation && a.stopPropagation(), a.stopImmediatePropagation && a.stopImmediatePropagation(), ln = !1, !1
+hn && document.addEventListener("click", function(a) {
+    if (fn) return a.preventDefault(), a.stopPropagation && a.stopPropagation(), a.stopImmediatePropagation && a.stopImmediatePropagation(), fn = !1, !1
 }, !0);
-var de = function(e) {
-        if (N) {
+var he = function(e) {
+        if (w) {
             e = e.touches ? e.touches[0] : e;
-            var n = pi(e.clientX, e.clientY);
+            var n = Oi(e.clientX, e.clientY);
             if (n) {
-                var l = {};
-                for (var r in e) e.hasOwnProperty(r) && (l[r] = e[r]);
-                l.target = l.rootEl = n, l.preventDefault = void 0, l.stopPropagation = void 0, n[At]._onDragOver(l)
+                var i = {};
+                for (var r in e) e.hasOwnProperty(r) && (i[r] = e[r]);
+                i.target = i.rootEl = n, i.preventDefault = void 0, i.stopPropagation = void 0, n[Rt]._onDragOver(i)
             }
         }
     },
-    gi = function(e) {
-        N && N.parentNode[At]._isOutsideThisEl(e.target)
+    Ti = function(e) {
+        w && w.parentNode[Rt]._isOutsideThisEl(e.target)
     };
 
-function W(a, e) {
+function z(a, e) {
     if (!(a && a.nodeType && a.nodeType === 1)) throw "Sortable: `el` must be an HTMLElement, not ".concat({}.toString.call(a));
-    this.el = a, this.options = e = Bt({}, e), a[At] = this;
+    this.el = a, this.options = e = Ht({}, e), a[Rt] = this;
     var n = {
         group: null,
         sort: !0,
         disabled: !1,
         store: null,
         handle: null,
         draggable: /^[uo]l$/i.test(a.nodeName) ? ">li" : ">*",
         swapThreshold: 1,
         invertSwap: !1,
         invertedSwapThreshold: null,
         removeCloneOnHide: !0,
         direction: function() {
-            return pr(a, this.options)
+            return Tr(a, this.options)
         },
         ghostClass: "sortable-ghost",
         chosenClass: "sortable-chosen",
         dragClass: "sortable-drag",
         ignore: "a, img",
         filter: null,
         preventOnFilter: !0,
@@ -1043,3802 +1045,3802 @@
         fallbackClass: "sortable-fallback",
         fallbackOnBody: !1,
         fallbackTolerance: 0,
         fallbackOffset: {
             x: 0,
             y: 0
         },
-        supportPointer: W.supportPointer !== !1 && "PointerEvent" in window && !Le,
+        supportPointer: z.supportPointer !== !1 && "PointerEvent" in window && !Ue,
         emptyInsertThreshold: 5
     };
-    Xe.initializePlugins(this, a, n);
-    for (var l in n) !(l in e) && (e[l] = n[l]);
-    gr(e);
+    ze.initializePlugins(this, a, n);
+    for (var i in n) !(i in e) && (e[i] = n[i]);
+    Ir(e);
     for (var r in this) r.charAt(0) === "_" && typeof this[r] == "function" && (this[r] = this[r].bind(this));
-    this.nativeDraggable = e.forceFallback ? !1 : vi, this.nativeDraggable && (this.options.touchStartThreshold = 1), e.supportPointer ? et(a, "pointerdown", this._onTapStart) : (et(a, "mousedown", this._onTapStart), et(a, "touchstart", this._onTapStart)), this.nativeDraggable && (et(a, "dragover", this), et(a, "dragenter", this)), un.push(this.el), e.store && e.store.get && this.sort(e.store.get(this) || []), Bt(this, ui())
+    this.nativeDraggable = e.forceFallback ? !1 : Ei, this.nativeDraggable && (this.options.touchStartThreshold = 1), e.supportPointer ? et(a, "pointerdown", this._onTapStart) : (et(a, "mousedown", this._onTapStart), et(a, "touchstart", this._onTapStart)), this.nativeDraggable && (et(a, "dragover", this), et(a, "dragenter", this)), cn.push(this.el), e.store && e.store.get && this.sort(e.store.get(this) || []), Ht(this, gi())
 }
-W.prototype = {
-    constructor: W,
+z.prototype = {
+    constructor: z,
     _isOutsideThisEl: function(e) {
-        !this.el.contains(e) && e !== this.el && (me = null)
+        !this.el.contains(e) && e !== this.el && (Se = null)
     },
     _getDirection: function(e, n) {
-        return typeof this.options.direction == "function" ? this.options.direction.call(this, e, n, N) : this.options.direction
+        return typeof this.options.direction == "function" ? this.options.direction.call(this, e, n, w) : this.options.direction
     },
     _onTapStart: function(e) {
         if (!!e.cancelable) {
             var n = this,
-                l = this.el,
+                i = this.el,
                 r = this.options,
-                u = r.preventOnFilter,
+                s = r.preventOnFilter,
                 t = e.type,
                 o = e.touches && e.touches[0] || e.pointerType && e.pointerType === "touch" && e,
-                i = (o || e).target,
-                s = e.target.shadowRoot && (e.path && e.path[0] || e.composedPath && e.composedPath()[0]) || i,
-                c = r.filter;
-            if (Ti(l), !N && !(/mousedown|pointerdown/.test(t) && e.button !== 0 || r.disabled) && !s.isContentEditable && !(!this.nativeDraggable && Le && i && i.tagName.toUpperCase() === "SELECT") && (i = Xt(i, r.draggable, l, !1), !(i && i.animated) && en !== i)) {
-                if (Se = mt(i), Ue = mt(i, r.draggable), typeof c == "function") {
-                    if (c.call(this, e, i, this)) {
-                        wt({
+                l = (o || e).target,
+                u = e.target.shadowRoot && (e.path && e.path[0] || e.composedPath && e.composedPath()[0]) || l,
+                f = r.filter;
+            if (Mi(i), !w && !(/mousedown|pointerdown/.test(t) && e.button !== 0 || r.disabled) && !u.isContentEditable && !(!this.nativeDraggable && Ue && l && l.tagName.toUpperCase() === "SELECT") && (l = Jt(l, r.draggable, i, !1), !(l && l.animated) && rn !== l)) {
+                if (Oe = gt(l), Be = gt(l, r.draggable), typeof f == "function") {
+                    if (f.call(this, e, l, this)) {
+                        Mt({
                             sortable: n,
-                            rootEl: s,
+                            rootEl: u,
                             name: "filter",
-                            targetEl: i,
-                            toEl: l,
-                            fromEl: l
-                        }), jt("filter", n, {
+                            targetEl: l,
+                            toEl: i,
+                            fromEl: i
+                        }), Ft("filter", n, {
                             evt: e
-                        }), u && e.cancelable && e.preventDefault();
+                        }), s && e.cancelable && e.preventDefault();
                         return
                     }
-                } else if (c && (c = c.split(",").some(function(f) {
-                        if (f = Xt(s, f.trim(), l, !1), f) return wt({
+                } else if (f && (f = f.split(",").some(function(c) {
+                        if (c = Jt(u, c.trim(), i, !1), c) return Mt({
                             sortable: n,
-                            rootEl: f,
+                            rootEl: c,
                             name: "filter",
-                            targetEl: i,
-                            fromEl: l,
-                            toEl: l
-                        }), jt("filter", n, {
+                            targetEl: l,
+                            fromEl: i,
+                            toEl: i
+                        }), Ft("filter", n, {
                             evt: e
                         }), !0
-                    }), c)) {
-                    u && e.cancelable && e.preventDefault();
+                    }), f)) {
+                    s && e.cancelable && e.preventDefault();
                     return
                 }
-                r.handle && !Xt(s, r.handle, l, !1) || this._prepareDragStart(e, o, i)
+                r.handle && !Jt(u, r.handle, i, !1) || this._prepareDragStart(e, o, l)
             }
         }
     },
-    _prepareDragStart: function(e, n, l) {
+    _prepareDragStart: function(e, n, i) {
         var r = this,
-            u = r.el,
+            s = r.el,
             t = r.options,
-            o = u.ownerDocument,
-            i;
-        if (l && !N && l.parentNode === u) {
-            var s = ft(l);
-            if (ut = u, N = l, pt = N.parentNode, ve = N.nextSibling, en = l, Je = t.group, W.dragged = N, ce = {
-                    target: N,
+            o = s.ownerDocument,
+            l;
+        if (i && !w && i.parentNode === s) {
+            var u = ft(i);
+            if (ut = s, w = i, ht = w.parentNode, me = w.nextSibling, rn = i, Ze = t.group, z.dragged = w, pe = {
+                    target: w,
                     clientX: (n || e).clientX,
                     clientY: (n || e).clientY
-                }, Hn = ce.clientX - s.left, Wn = ce.clientY - s.top, this._lastX = (n || e).clientX, this._lastY = (n || e).clientY, N.style["will-change"] = "all", i = function() {
-                    if (jt("delayEnded", r, {
+                }, qn = pe.clientX - u.left, _n = pe.clientY - u.top, this._lastX = (n || e).clientX, this._lastY = (n || e).clientY, w.style["will-change"] = "all", l = function() {
+                    if (Ft("delayEnded", r, {
                             evt: e
-                        }), W.eventCanceled) {
+                        }), z.eventCanceled) {
                         r._onDrop();
                         return
                     }
-                    r._disableDelayedDragEvents(), !Un && r.nativeDraggable && (N.draggable = !0), r._triggerDragStart(e, n), wt({
+                    r._disableDelayedDragEvents(), !zn && r.nativeDraggable && (w.draggable = !0), r._triggerDragStart(e, n), Mt({
                         sortable: r,
                         name: "choose",
                         originalEvent: e
-                    }), dt(N, t.chosenClass, !0)
-                }, t.ignore.split(",").forEach(function(c) {
-                    cr(N, c.trim(), xn)
-                }), et(o, "dragover", de), et(o, "mousemove", de), et(o, "touchmove", de), et(o, "mouseup", r._onDrop), et(o, "touchend", r._onDrop), et(o, "touchcancel", r._onDrop), Un && this.nativeDraggable && (this.options.touchStartThreshold = 4, N.draggable = !0), jt("delayStart", this, {
+                    }), vt(w, t.chosenClass, !0)
+                }, t.ignore.split(",").forEach(function(f) {
+                    Sr(w, f.trim(), Tn)
+                }), et(o, "dragover", he), et(o, "mousemove", he), et(o, "touchmove", he), et(o, "mouseup", r._onDrop), et(o, "touchend", r._onDrop), et(o, "touchcancel", r._onDrop), zn && this.nativeDraggable && (this.options.touchStartThreshold = 4, w.draggable = !0), Ft("delayStart", this, {
                     evt: e
-                }), t.delay && (!t.delayOnTouchOnly || n) && (!this.nativeDraggable || !(We || re))) {
-                if (W.eventCanceled) {
+                }), t.delay && (!t.delayOnTouchOnly || n) && (!this.nativeDraggable || !(Ye || ae))) {
+                if (z.eventCanceled) {
                     this._onDrop();
                     return
                 }
-                et(o, "mouseup", r._disableDelayedDrag), et(o, "touchend", r._disableDelayedDrag), et(o, "touchcancel", r._disableDelayedDrag), et(o, "mousemove", r._delayedDragTouchMoveHandler), et(o, "touchmove", r._delayedDragTouchMoveHandler), t.supportPointer && et(o, "pointermove", r._delayedDragTouchMoveHandler), r._dragStartTimer = setTimeout(i, t.delay)
-            } else i()
+                et(o, "mouseup", r._disableDelayedDrag), et(o, "touchend", r._disableDelayedDrag), et(o, "touchcancel", r._disableDelayedDrag), et(o, "mousemove", r._delayedDragTouchMoveHandler), et(o, "touchmove", r._delayedDragTouchMoveHandler), t.supportPointer && et(o, "pointermove", r._delayedDragTouchMoveHandler), r._dragStartTimer = setTimeout(l, t.delay)
+            } else l()
         }
     },
     _delayedDragTouchMoveHandler: function(e) {
         var n = e.touches ? e.touches[0] : e;
         Math.max(Math.abs(n.clientX - this._lastX), Math.abs(n.clientY - this._lastY)) >= Math.floor(this.options.touchStartThreshold / (this.nativeDraggable && window.devicePixelRatio || 1)) && this._disableDelayedDrag()
     },
     _disableDelayedDrag: function() {
-        N && xn(N), clearTimeout(this._dragStartTimer), this._disableDelayedDragEvents()
+        w && Tn(w), clearTimeout(this._dragStartTimer), this._disableDelayedDragEvents()
     },
     _disableDelayedDragEvents: function() {
         var e = this.el.ownerDocument;
         tt(e, "mouseup", this._disableDelayedDrag), tt(e, "touchend", this._disableDelayedDrag), tt(e, "touchcancel", this._disableDelayedDrag), tt(e, "mousemove", this._delayedDragTouchMoveHandler), tt(e, "touchmove", this._delayedDragTouchMoveHandler), tt(e, "pointermove", this._delayedDragTouchMoveHandler)
     },
     _triggerDragStart: function(e, n) {
-        n = n || e.pointerType == "touch" && e, !this.nativeDraggable || n ? this.options.supportPointer ? et(document, "pointermove", this._onTouchMove) : n ? et(document, "touchmove", this._onTouchMove) : et(document, "mousemove", this._onTouchMove) : (et(N, "dragend", this), et(ut, "dragstart", this._onDragStart));
+        n = n || e.pointerType == "touch" && e, !this.nativeDraggable || n ? this.options.supportPointer ? et(document, "pointermove", this._onTouchMove) : n ? et(document, "touchmove", this._onTouchMove) : et(document, "mousemove", this._onTouchMove) : (et(w, "dragend", this), et(ut, "dragstart", this._onDragStart));
         try {
-            document.selection ? rn(function() {
+            document.selection ? an(function() {
                 document.selection.empty()
             }) : window.getSelection().removeAllRanges()
         } catch {}
     },
     _dragStarted: function(e, n) {
-        if (be = !1, ut && N) {
-            jt("dragStarted", this, {
+        if (xe = !1, ut && w) {
+            Ft("dragStarted", this, {
                 evt: n
-            }), this.nativeDraggable && et(document, "dragover", gi);
-            var l = this.options;
-            !e && dt(N, l.dragClass, !1), dt(N, l.ghostClass, !0), W.active = this, e && this._appendGhost(), wt({
+            }), this.nativeDraggable && et(document, "dragover", Ti);
+            var i = this.options;
+            !e && vt(w, i.dragClass, !1), vt(w, i.ghostClass, !0), z.active = this, e && this._appendGhost(), Mt({
                 sortable: this,
                 name: "start",
                 originalEvent: n
             })
         } else this._nulling()
     },
     _emulateDragOver: function() {
-        if (Ht) {
-            this._lastX = Ht.clientX, this._lastY = Ht.clientY, mr();
-            for (var e = document.elementFromPoint(Ht.clientX, Ht.clientY), n = e; e && e.shadowRoot && (e = e.shadowRoot.elementFromPoint(Ht.clientX, Ht.clientY), e !== n);) n = e;
-            if (N.parentNode[At]._isOutsideThisEl(e), n)
+        if (Xt) {
+            this._lastX = Xt.clientX, this._lastY = Xt.clientY, Pr();
+            for (var e = document.elementFromPoint(Xt.clientX, Xt.clientY), n = e; e && e.shadowRoot && (e = e.shadowRoot.elementFromPoint(Xt.clientX, Xt.clientY), e !== n);) n = e;
+            if (w.parentNode[Rt]._isOutsideThisEl(e), n)
                 do {
-                    if (n[At]) {
-                        var l = void 0;
-                        if (l = n[At]._onDragOver({
-                                clientX: Ht.clientX,
-                                clientY: Ht.clientY,
+                    if (n[Rt]) {
+                        var i = void 0;
+                        if (i = n[Rt]._onDragOver({
+                                clientX: Xt.clientX,
+                                clientY: Xt.clientY,
                                 target: e,
                                 rootEl: n
-                            }), l && !this.options.dragoverBubble) break
+                            }), i && !this.options.dragoverBubble) break
                     }
                     e = n
                 } while (n = n.parentNode);
-            yr()
+            Cr()
         }
     },
     _onTouchMove: function(e) {
-        if (ce) {
+        if (pe) {
             var n = this.options,
-                l = n.fallbackTolerance,
+                i = n.fallbackTolerance,
                 r = n.fallbackOffset,
-                u = e.touches ? e.touches[0] : e,
-                t = k && he(k, !0),
-                o = k && t && t.a,
-                i = k && t && t.d,
-                s = Ze && Ct && Bn(Ct),
-                c = (u.clientX - ce.clientX + r.x) / (o || 1) + (s ? s[0] - En[0] : 0) / (o || 1),
-                f = (u.clientY - ce.clientY + r.y) / (i || 1) + (s ? s[1] - En[1] : 0) / (i || 1);
-            if (!W.active && !be) {
-                if (l && Math.max(Math.abs(u.clientX - this._lastX), Math.abs(u.clientY - this._lastY)) < l) return;
+                s = e.touches ? e.touches[0] : e,
+                t = q && ge(q, !0),
+                o = q && t && t.a,
+                l = q && t && t.d,
+                u = qe && At && Zn(At),
+                f = (s.clientX - pe.clientX + r.x) / (o || 1) + (u ? u[0] - On[0] : 0) / (o || 1),
+                c = (s.clientY - pe.clientY + r.y) / (l || 1) + (u ? u[1] - On[1] : 0) / (l || 1);
+            if (!z.active && !xe) {
+                if (i && Math.max(Math.abs(s.clientX - this._lastX), Math.abs(s.clientY - this._lastY)) < i) return;
                 this._onDragStart(e, !0)
             }
-            if (k) {
-                t ? (t.e += c - (bn || 0), t.f += f - (Sn || 0)) : t = {
+            if (q) {
+                t ? (t.e += f - (En || 0), t.f += c - (xn || 0)) : t = {
                     a: 1,
                     b: 0,
                     c: 0,
                     d: 1,
-                    e: c,
-                    f
+                    e: f,
+                    f: c
                 };
                 var d = "matrix(".concat(t.a, ",").concat(t.b, ",").concat(t.c, ",").concat(t.d, ",").concat(t.e, ",").concat(t.f, ")");
-                U(k, "webkitTransform", d), U(k, "mozTransform", d), U(k, "msTransform", d), U(k, "transform", d), bn = c, Sn = f, Ht = u
+                G(q, "webkitTransform", d), G(q, "mozTransform", d), G(q, "msTransform", d), G(q, "transform", d), En = f, xn = c, Xt = s
             }
             e.cancelable && e.preventDefault()
         }
     },
     _appendGhost: function() {
-        if (!k) {
+        if (!q) {
             var e = this.options.fallbackOnBody ? document.body : ut,
-                n = ft(N, !0, Ze, !0, e),
-                l = this.options;
-            if (Ze) {
-                for (Ct = e; U(Ct, "position") === "static" && U(Ct, "transform") === "none" && Ct !== document;) Ct = Ct.parentNode;
-                Ct !== document.body && Ct !== document.documentElement ? (Ct === document && (Ct = kt()), n.top += Ct.scrollTop, n.left += Ct.scrollLeft) : Ct = kt(), En = Bn(Ct)
+                n = ft(w, !0, qe, !0, e),
+                i = this.options;
+            if (qe) {
+                for (At = e; G(At, "position") === "static" && G(At, "transform") === "none" && At !== document;) At = At.parentNode;
+                At !== document.body && At !== document.documentElement ? (At === document && (At = te()), n.top += At.scrollTop, n.left += At.scrollLeft) : At = te(), On = Zn(At)
             }
-            k = N.cloneNode(!0), dt(k, l.ghostClass, !1), dt(k, l.fallbackClass, !0), dt(k, l.dragClass, !0), U(k, "transition", ""), U(k, "transform", ""), U(k, "box-sizing", "border-box"), U(k, "margin", 0), U(k, "top", n.top), U(k, "left", n.left), U(k, "width", n.width), U(k, "height", n.height), U(k, "opacity", "0.8"), U(k, "position", Ze ? "absolute" : "fixed"), U(k, "zIndex", "100000"), U(k, "pointerEvents", "none"), W.ghost = k, e.appendChild(k), U(k, "transform-origin", Hn / parseInt(k.style.width) * 100 + "% " + Wn / parseInt(k.style.height) * 100 + "%")
+            q = w.cloneNode(!0), vt(q, i.ghostClass, !1), vt(q, i.fallbackClass, !0), vt(q, i.dragClass, !0), G(q, "transition", ""), G(q, "transform", ""), G(q, "box-sizing", "border-box"), G(q, "margin", 0), G(q, "top", n.top), G(q, "left", n.left), G(q, "width", n.width), G(q, "height", n.height), G(q, "opacity", "0.8"), G(q, "position", qe ? "absolute" : "fixed"), G(q, "zIndex", "100000"), G(q, "pointerEvents", "none"), z.ghost = q, e.appendChild(q), G(q, "transform-origin", qn / parseInt(q.style.width) * 100 + "% " + _n / parseInt(q.style.height) * 100 + "%")
         }
     },
     _onDragStart: function(e, n) {
-        var l = this,
+        var i = this,
             r = e.dataTransfer,
-            u = l.options;
-        if (jt("dragStart", this, {
+            s = i.options;
+        if (Ft("dragStart", this, {
                 evt: e
-            }), W.eventCanceled) {
+            }), z.eventCanceled) {
             this._onDrop();
             return
         }
-        jt("setupClone", this), W.eventCanceled || (gt = jn(N), gt.draggable = !1, gt.style["will-change"] = "", this._hideClone(), dt(gt, this.options.chosenClass, !1), W.clone = gt), l.cloneId = rn(function() {
-            jt("clone", l), !W.eventCanceled && (l.options.removeCloneOnHide || ut.insertBefore(gt, N), l._hideClone(), wt({
-                sortable: l,
+        Ft("setupClone", this), z.eventCanceled || (mt = Un(w), mt.draggable = !1, mt.style["will-change"] = "", this._hideClone(), vt(mt, this.options.chosenClass, !1), z.clone = mt), i.cloneId = an(function() {
+            Ft("clone", i), !z.eventCanceled && (i.options.removeCloneOnHide || ut.insertBefore(mt, w), i._hideClone(), Mt({
+                sortable: i,
                 name: "clone"
             }))
-        }), !n && dt(N, u.dragClass, !0), n ? (ln = !0, l._loopId = setInterval(l._emulateDragOver, 50)) : (tt(document, "mouseup", l._onDrop), tt(document, "touchend", l._onDrop), tt(document, "touchcancel", l._onDrop), r && (r.effectAllowed = "move", u.setData && u.setData.call(l, r, N)), et(document, "drop", l), U(N, "transform", "translateZ(0)")), be = !0, l._dragStartId = rn(l._dragStarted.bind(l, n, e)), et(document, "selectstart", l), Ne = !0, Le && U(document.body, "user-select", "none")
+        }), !n && vt(w, s.dragClass, !0), n ? (fn = !0, i._loopId = setInterval(i._emulateDragOver, 50)) : (tt(document, "mouseup", i._onDrop), tt(document, "touchend", i._onDrop), tt(document, "touchcancel", i._onDrop), r && (r.effectAllowed = "move", s.setData && s.setData.call(i, r, w)), et(document, "drop", i), G(w, "transform", "translateZ(0)")), xe = !0, i._dragStartId = an(i._dragStarted.bind(i, n, e)), et(document, "selectstart", i), $e = !0, Ue && G(document.body, "user-select", "none")
     },
     _onDragOver: function(e) {
         var n = this.el,
-            l = e.target,
-            r, u, t, o = this.options,
-            i = o.group,
-            s = W.active,
-            c = Je === i,
-            f = o.sort,
-            d = Pt || s,
-            v, h = this,
-            p = !1;
-        if (Cn) return;
+            i = e.target,
+            r, s, t, o = this.options,
+            l = o.group,
+            u = z.active,
+            f = Ze === l,
+            c = o.sort,
+            d = Dt || u,
+            v, p = this,
+            h = !1;
+        if (An) return;
 
-        function g(_, at) {
-            jt(_, h, qt({
+        function m(k, ot) {
+            Ft(k, p, ee({
                 evt: e,
-                isOwner: c,
+                isOwner: f,
                 axis: v ? "vertical" : "horizontal",
                 revert: t,
                 dragRect: r,
-                targetRect: u,
-                canSort: f,
+                targetRect: s,
+                canSort: c,
                 fromSortable: d,
-                target: l,
-                completed: S,
-                onMove: function(vt, ht) {
-                    return ke(ut, n, N, r, vt, ft(vt), e, ht)
+                target: i,
+                completed: y,
+                onMove: function(ct, pt) {
+                    return _e(ut, n, w, r, ct, ft(ct), e, pt)
                 },
-                changed: P
-            }, at))
+                changed: O
+            }, ot))
         }
 
-        function b() {
-            g("dragOverAnimationCapture"), h.captureAnimationState(), h !== d && d.captureAnimationState()
+        function g() {
+            m("dragOverAnimationCapture"), p.captureAnimationState(), p !== d && d.captureAnimationState()
         }
 
-        function S(_) {
-            return g("dragOverCompleted", {
-                insertion: _
-            }), _ && (c ? s._hideClone() : s._showClone(h), h !== d && (dt(N, Pt ? Pt.options.ghostClass : s.options.ghostClass, !1), dt(N, o.ghostClass, !0)), Pt !== h && h !== W.active ? Pt = h : h === W.active && Pt && (Pt = null), d === h && (h._ignoreWhileAnimating = l), h.animateAll(function() {
-                g("dragOverAnimationComplete"), h._ignoreWhileAnimating = null
-            }), h !== d && (d.animateAll(), d._ignoreWhileAnimating = null)), (l === N && !N.animated || l === n && !l.animated) && (me = null), !o.dragoverBubble && !e.rootEl && l !== document && (N.parentNode[At]._isOutsideThisEl(e.target), !_ && de(e)), !o.dragoverBubble && e.stopPropagation && e.stopPropagation(), p = !0
+        function y(k) {
+            return m("dragOverCompleted", {
+                insertion: k
+            }), k && (f ? u._hideClone() : u._showClone(p), p !== d && (vt(w, Dt ? Dt.options.ghostClass : u.options.ghostClass, !1), vt(w, o.ghostClass, !0)), Dt !== p && p !== z.active ? Dt = p : p === z.active && Dt && (Dt = null), d === p && (p._ignoreWhileAnimating = i), p.animateAll(function() {
+                m("dragOverAnimationComplete"), p._ignoreWhileAnimating = null
+            }), p !== d && (d.animateAll(), d._ignoreWhileAnimating = null)), (i === w && !w.animated || i === n && !i.animated) && (Se = null), !o.dragoverBubble && !e.rootEl && i !== document && (w.parentNode[Rt]._isOutsideThisEl(e.target), !k && he(e)), !o.dragoverBubble && e.stopPropagation && e.stopPropagation(), h = !0
         }
 
-        function P() {
-            Ut = mt(N), ie = mt(N, o.draggable), wt({
-                sortable: h,
+        function O() {
+            Ut = gt(w), se = gt(w, o.draggable), Mt({
+                sortable: p,
                 name: "change",
                 toEl: n,
                 newIndex: Ut,
-                newDraggableIndex: ie,
+                newDraggableIndex: se,
                 originalEvent: e
             })
         }
-        if (e.preventDefault !== void 0 && e.cancelable && e.preventDefault(), l = Xt(l, o.draggable, n, !0), g("dragOver"), W.eventCanceled) return p;
-        if (N.contains(e.target) || l.animated && l.animatingX && l.animatingY || h._ignoreWhileAnimating === l) return S(!1);
-        if (ln = !1, s && !o.disabled && (c ? f || (t = pt !== ut) : Pt === this || (this.lastPutMode = Je.checkPull(this, s, N, e)) && i.checkPut(this, s, N, e))) {
-            if (v = this._getDirection(e, l) === "vertical", r = ft(N), g("dragOverValid"), W.eventCanceled) return p;
-            if (t) return pt = ut, b(), this._hideClone(), g("revert"), W.eventCanceled || (ve ? ut.insertBefore(N, ve) : ut.appendChild(N)), S(!0);
-            var x = Nn(n, o.draggable);
-            if (!x || Si(e, v, this) && !x.animated) {
-                if (x === N) return S(!1);
-                if (x && n === e.target && (l = x), l && (u = ft(l)), ke(ut, n, N, r, l, u, e, !!l) !== !1) return b(), n.appendChild(N), pt = n, P(), S(!0)
-            } else if (x && bi(e, v, this)) {
-                var C = Ee(n, 0, o, !0);
-                if (C === N) return S(!1);
-                if (l = C, u = ft(l), ke(ut, n, N, r, l, u, e, !1) !== !1) return b(), n.insertBefore(N, C), pt = n, P(), S(!0)
-            } else if (l.parentNode === n) {
-                u = ft(l);
-                var I = 0,
-                    j, L = N.parentNode !== n,
-                    T = !hi(N.animated && N.toRect || r, l.animated && l.toRect || u, v),
-                    O = v ? "top" : "left",
-                    D = Gn(l, "top", "top") || Gn(N, "top", "top"),
-                    G = D ? D.scrollTop : void 0;
-                me !== l && (j = u[O], Ge = !1, Qe = !T && o.invertSwap || L), I = Ei(e, l, u, v, T ? 1 : o.swapThreshold, o.invertedSwapThreshold == null ? o.swapThreshold : o.invertedSwapThreshold, Qe, me === l);
-                var A;
-                if (I !== 0) {
-                    var M = mt(N);
-                    do M -= I, A = pt.children[M]; while (A && (U(A, "display") === "none" || A === k))
-                }
-                if (I === 0 || A === l) return S(!1);
-                me = l, Ve = I;
-                var X = l.nextElementSibling,
-                    R = !1;
-                R = I === 1;
-                var F = ke(ut, n, N, r, l, u, e, R);
-                if (F !== !1) return (F === 1 || F === -1) && (R = F === 1), Cn = !0, setTimeout(yi, 30), b(), R && !X ? n.appendChild(N) : l.parentNode.insertBefore(N, R ? X : l), D && vr(D, 0, G - D.scrollTop), pt = N.parentNode, j !== void 0 && !Qe && (nn = Math.abs(j - ft(l)[O])), P(), S(!0)
+        if (e.preventDefault !== void 0 && e.cancelable && e.preventDefault(), i = Jt(i, o.draggable, n, !0), m("dragOver"), z.eventCanceled) return h;
+        if (w.contains(e.target) || i.animated && i.animatingX && i.animatingY || p._ignoreWhileAnimating === i) return y(!1);
+        if (fn = !1, u && !o.disabled && (f ? c || (t = ht !== ut) : Dt === this || (this.lastPutMode = Ze.checkPull(this, u, w, e)) && l.checkPut(this, u, w, e))) {
+            if (v = this._getDirection(e, i) === "vertical", r = ft(w), m("dragOverValid"), z.eventCanceled) return h;
+            if (t) return ht = ut, g(), this._hideClone(), m("revert"), z.eventCanceled || (me ? ut.insertBefore(w, me) : ut.appendChild(w)), y(!0);
+            var E = Vn(n, o.draggable);
+            if (!E || Di(e, v, this) && !E.animated) {
+                if (E === w) return y(!1);
+                if (E && n === e.target && (i = E), i && (s = ft(i)), _e(ut, n, w, r, i, s, e, !!i) !== !1) return g(), n.appendChild(w), ht = n, O(), y(!0)
+            } else if (E && Ci(e, v, this)) {
+                var C = Ie(n, 0, o, !0);
+                if (C === w) return y(!1);
+                if (i = C, s = ft(i), _e(ut, n, w, r, i, s, e, !1) !== !1) return g(), n.insertBefore(w, C), ht = n, O(), y(!0)
+            } else if (i.parentNode === n) {
+                s = ft(i);
+                var T = 0,
+                    $, L = w.parentNode !== n,
+                    I = !xi(w.animated && w.toRect || r, i.animated && i.toRect || s, v),
+                    j = v ? "top" : "left",
+                    P = Qn(i, "top", "top") || Qn(w, "top", "top"),
+                    M = P ? P.scrollTop : void 0;
+                Se !== i && ($ = s[j], He = !1, ke = !I && o.invertSwap || L), T = Ai(e, i, s, v, I ? 1 : o.swapThreshold, o.invertedSwapThreshold == null ? o.swapThreshold : o.invertedSwapThreshold, ke, Se === i);
+                var D;
+                if (T !== 0) {
+                    var R = gt(w);
+                    do R -= T, D = ht.children[R]; while (D && (G(D, "display") === "none" || D === q))
+                }
+                if (T === 0 || D === i) return y(!1);
+                Se = i, Ke = T;
+                var H = i.nextElementSibling,
+                    F = !1;
+                F = T === 1;
+                var N = _e(ut, n, w, r, i, s, e, F);
+                if (N !== !1) return (N === 1 || N === -1) && (F = N === 1), An = !0, setTimeout(Pi, 30), g(), F && !H ? n.appendChild(w) : i.parentNode.insertBefore(w, F ? H : i), P && xr(P, 0, M - P.scrollTop), ht = w.parentNode, $ !== void 0 && !ke && (on = Math.abs($ - ft(i)[j])), O(), y(!0)
             }
-            if (n.contains(N)) return S(!1)
+            if (n.contains(w)) return y(!1)
         }
         return !1
     },
     _ignoreWhileAnimating: null,
     _offMoveEvents: function() {
-        tt(document, "mousemove", this._onTouchMove), tt(document, "touchmove", this._onTouchMove), tt(document, "pointermove", this._onTouchMove), tt(document, "dragover", de), tt(document, "mousemove", de), tt(document, "touchmove", de)
+        tt(document, "mousemove", this._onTouchMove), tt(document, "touchmove", this._onTouchMove), tt(document, "pointermove", this._onTouchMove), tt(document, "dragover", he), tt(document, "mousemove", he), tt(document, "touchmove", he)
     },
     _offUpEvents: function() {
         var e = this.el.ownerDocument;
         tt(e, "mouseup", this._onDrop), tt(e, "touchend", this._onDrop), tt(e, "pointerup", this._onDrop), tt(e, "touchcancel", this._onDrop), tt(document, "selectstart", this)
     },
     _onDrop: function(e) {
         var n = this.el,
-            l = this.options;
-        if (Ut = mt(N), ie = mt(N, l.draggable), jt("drop", this, {
+            i = this.options;
+        if (Ut = gt(w), se = gt(w, i.draggable), Ft("drop", this, {
                 evt: e
-            }), pt = N && N.parentNode, Ut = mt(N), ie = mt(N, l.draggable), W.eventCanceled) {
+            }), ht = w && w.parentNode, Ut = gt(w), se = gt(w, i.draggable), z.eventCanceled) {
             this._nulling();
             return
         }
-        be = !1, Qe = !1, Ge = !1, clearInterval(this._loopId), clearTimeout(this._dragStartTimer), Dn(this.cloneId), Dn(this._dragStartId), this.nativeDraggable && (tt(document, "drop", this), tt(n, "dragstart", this._onDragStart)), this._offMoveEvents(), this._offUpEvents(), Le && U(document.body, "user-select", ""), U(N, "transform", ""), e && (Ne && (e.cancelable && e.preventDefault(), !l.dropBubble && e.stopPropagation()), k && k.parentNode && k.parentNode.removeChild(k), (ut === pt || Pt && Pt.lastPutMode !== "clone") && gt && gt.parentNode && gt.parentNode.removeChild(gt), N && (this.nativeDraggable && tt(N, "dragend", this), xn(N), N.style["will-change"] = "", Ne && !be && dt(N, Pt ? Pt.options.ghostClass : this.options.ghostClass, !1), dt(N, this.options.chosenClass, !1), wt({
+        xe = !1, ke = !1, He = !1, clearInterval(this._loopId), clearTimeout(this._dragStartTimer), Rn(this.cloneId), Rn(this._dragStartId), this.nativeDraggable && (tt(document, "drop", this), tt(n, "dragstart", this._onDragStart)), this._offMoveEvents(), this._offUpEvents(), Ue && G(document.body, "user-select", ""), G(w, "transform", ""), e && ($e && (e.cancelable && e.preventDefault(), !i.dropBubble && e.stopPropagation()), q && q.parentNode && q.parentNode.removeChild(q), (ut === ht || Dt && Dt.lastPutMode !== "clone") && mt && mt.parentNode && mt.parentNode.removeChild(mt), w && (this.nativeDraggable && tt(w, "dragend", this), Tn(w), w.style["will-change"] = "", $e && !xe && vt(w, Dt ? Dt.options.ghostClass : this.options.ghostClass, !1), vt(w, this.options.chosenClass, !1), Mt({
             sortable: this,
             name: "unchoose",
-            toEl: pt,
+            toEl: ht,
             newIndex: null,
             newDraggableIndex: null,
             originalEvent: e
-        }), ut !== pt ? (Ut >= 0 && (wt({
-            rootEl: pt,
+        }), ut !== ht ? (Ut >= 0 && (Mt({
+            rootEl: ht,
             name: "add",
-            toEl: pt,
+            toEl: ht,
             fromEl: ut,
             originalEvent: e
-        }), wt({
+        }), Mt({
             sortable: this,
             name: "remove",
-            toEl: pt,
+            toEl: ht,
             originalEvent: e
-        }), wt({
-            rootEl: pt,
+        }), Mt({
+            rootEl: ht,
             name: "sort",
-            toEl: pt,
+            toEl: ht,
             fromEl: ut,
             originalEvent: e
-        }), wt({
+        }), Mt({
             sortable: this,
             name: "sort",
-            toEl: pt,
+            toEl: ht,
             originalEvent: e
-        })), Pt && Pt.save()) : Ut !== Se && Ut >= 0 && (wt({
+        })), Dt && Dt.save()) : Ut !== Oe && Ut >= 0 && (Mt({
             sortable: this,
             name: "update",
-            toEl: pt,
+            toEl: ht,
             originalEvent: e
-        }), wt({
+        }), Mt({
             sortable: this,
             name: "sort",
-            toEl: pt,
+            toEl: ht,
             originalEvent: e
-        })), W.active && ((Ut == null || Ut === -1) && (Ut = Se, ie = Ue), wt({
+        })), z.active && ((Ut == null || Ut === -1) && (Ut = Oe, se = Be), Mt({
             sortable: this,
             name: "end",
-            toEl: pt,
+            toEl: ht,
             originalEvent: e
         }), this.save()))), this._nulling()
     },
     _nulling: function() {
-        jt("nulling", this), ut = N = pt = k = ve = gt = en = se = ce = Ht = Ne = Ut = ie = Se = Ue = me = Ve = Pt = Je = W.dragged = W.ghost = W.clone = W.active = null, fn.forEach(function(e) {
+        Ft("nulling", this), ut = w = ht = q = me = mt = rn = ue = pe = Xt = $e = Ut = se = Oe = Be = Se = Ke = Dt = Ze = z.dragged = z.ghost = z.clone = z.active = null, dn.forEach(function(e) {
             e.checked = !0
-        }), fn.length = bn = Sn = 0
+        }), dn.length = En = xn = 0
     },
     handleEvent: function(e) {
         switch (e.type) {
             case "drop":
             case "dragend":
                 this._onDrop(e);
                 break;
             case "dragenter":
             case "dragover":
-                N && (this._onDragOver(e), mi(e));
+                w && (this._onDragOver(e), Ii(e));
                 break;
             case "selectstart":
                 e.preventDefault();
                 break
         }
     },
     toArray: function() {
-        for (var e = [], n, l = this.el.children, r = 0, u = l.length, t = this.options; r < u; r++) n = l[r], Xt(n, t.draggable, this.el, !1) && e.push(n.getAttribute(t.dataIdAttr) || Oi(n));
+        for (var e = [], n, i = this.el.children, r = 0, s = i.length, t = this.options; r < s; r++) n = i[r], Jt(n, t.draggable, this.el, !1) && e.push(n.getAttribute(t.dataIdAttr) || wi(n));
         return e
     },
     sort: function(e, n) {
-        var l = {},
+        var i = {},
             r = this.el;
-        this.toArray().forEach(function(u, t) {
+        this.toArray().forEach(function(s, t) {
             var o = r.children[t];
-            Xt(o, this.options.draggable, r, !1) && (l[u] = o)
-        }, this), n && this.captureAnimationState(), e.forEach(function(u) {
-            l[u] && (r.removeChild(l[u]), r.appendChild(l[u]))
+            Jt(o, this.options.draggable, r, !1) && (i[s] = o)
+        }, this), n && this.captureAnimationState(), e.forEach(function(s) {
+            i[s] && (r.removeChild(i[s]), r.appendChild(i[s]))
         }), n && this.animateAll()
     },
     save: function() {
         var e = this.options.store;
         e && e.set && e.set(this)
     },
     closest: function(e, n) {
-        return Xt(e, n || this.options.draggable, this.el, !1)
+        return Jt(e, n || this.options.draggable, this.el, !1)
     },
     option: function(e, n) {
-        var l = this.options;
-        if (n === void 0) return l[e];
-        var r = Xe.modifyOption(this, e, n);
-        typeof r < "u" ? l[e] = r : l[e] = n, e === "group" && gr(l)
+        var i = this.options;
+        if (n === void 0) return i[e];
+        var r = ze.modifyOption(this, e, n);
+        typeof r < "u" ? i[e] = r : i[e] = n, e === "group" && Ir(i)
     },
     destroy: function() {
-        jt("destroy", this);
+        Ft("destroy", this);
         var e = this.el;
-        e[At] = null, tt(e, "mousedown", this._onTapStart), tt(e, "touchstart", this._onTapStart), tt(e, "pointerdown", this._onTapStart), this.nativeDraggable && (tt(e, "dragover", this), tt(e, "dragenter", this)), Array.prototype.forEach.call(e.querySelectorAll("[draggable]"), function(n) {
+        e[Rt] = null, tt(e, "mousedown", this._onTapStart), tt(e, "touchstart", this._onTapStart), tt(e, "pointerdown", this._onTapStart), this.nativeDraggable && (tt(e, "dragover", this), tt(e, "dragenter", this)), Array.prototype.forEach.call(e.querySelectorAll("[draggable]"), function(n) {
             n.removeAttribute("draggable")
-        }), this._onDrop(), this._disableDelayedDragEvents(), un.splice(un.indexOf(this.el), 1), this.el = e = null
+        }), this._onDrop(), this._disableDelayedDragEvents(), cn.splice(cn.indexOf(this.el), 1), this.el = e = null
     },
     _hideClone: function() {
-        if (!se) {
-            if (jt("hideClone", this), W.eventCanceled) return;
-            U(gt, "display", "none"), this.options.removeCloneOnHide && gt.parentNode && gt.parentNode.removeChild(gt), se = !0
+        if (!ue) {
+            if (Ft("hideClone", this), z.eventCanceled) return;
+            G(mt, "display", "none"), this.options.removeCloneOnHide && mt.parentNode && mt.parentNode.removeChild(mt), ue = !0
         }
     },
     _showClone: function(e) {
         if (e.lastPutMode !== "clone") {
             this._hideClone();
             return
         }
-        if (se) {
-            if (jt("showClone", this), W.eventCanceled) return;
-            N.parentNode == ut && !this.options.group.revertClone ? ut.insertBefore(gt, N) : ve ? ut.insertBefore(gt, ve) : ut.appendChild(gt), this.options.group.revertClone && this.animate(N, gt), U(gt, "display", ""), se = !1
+        if (ue) {
+            if (Ft("showClone", this), z.eventCanceled) return;
+            w.parentNode == ut && !this.options.group.revertClone ? ut.insertBefore(mt, w) : me ? ut.insertBefore(mt, me) : ut.appendChild(mt), this.options.group.revertClone && this.animate(w, mt), G(mt, "display", ""), ue = !1
         }
     }
 };
 
-function mi(a) {
+function Ii(a) {
     a.dataTransfer && (a.dataTransfer.dropEffect = "move"), a.cancelable && a.preventDefault()
 }
 
-function ke(a, e, n, l, r, u, t, o) {
-    var i, s = a[At],
-        c = s.options.onMove,
-        f;
-    return window.CustomEvent && !re && !We ? i = new CustomEvent("move", {
+function _e(a, e, n, i, r, s, t, o) {
+    var l, u = a[Rt],
+        f = u.options.onMove,
+        c;
+    return window.CustomEvent && !ae && !Ye ? l = new CustomEvent("move", {
         bubbles: !0,
         cancelable: !0
-    }) : (i = document.createEvent("Event"), i.initEvent("move", !0, !0)), i.to = e, i.from = a, i.dragged = n, i.draggedRect = l, i.related = r || e, i.relatedRect = u || ft(e), i.willInsertAfter = o, i.originalEvent = t, a.dispatchEvent(i), c && (f = c.call(s, i, t)), f
+    }) : (l = document.createEvent("Event"), l.initEvent("move", !0, !0)), l.to = e, l.from = a, l.dragged = n, l.draggedRect = i, l.related = r || e, l.relatedRect = s || ft(e), l.willInsertAfter = o, l.originalEvent = t, a.dispatchEvent(l), f && (c = f.call(u, l, t)), c
 }
 
-function xn(a) {
+function Tn(a) {
     a.draggable = !1
 }
 
-function yi() {
-    Cn = !1
+function Pi() {
+    An = !1
 }
 
-function bi(a, e, n) {
-    var l = ft(Ee(n.el, 0, n.options, !0)),
+function Ci(a, e, n) {
+    var i = ft(Ie(n.el, 0, n.options, !0)),
         r = 10;
-    return e ? a.clientX < l.left - r || a.clientY < l.top && a.clientX < l.right : a.clientY < l.top - r || a.clientY < l.bottom && a.clientX < l.left
+    return e ? a.clientX < i.left - r || a.clientY < i.top && a.clientX < i.right : a.clientY < i.top - r || a.clientY < i.bottom && a.clientX < i.left
 }
 
-function Si(a, e, n) {
-    var l = ft(Nn(n.el, n.options.draggable)),
+function Di(a, e, n) {
+    var i = ft(Vn(n.el, n.options.draggable)),
         r = 10;
-    return e ? a.clientX > l.right + r || a.clientX <= l.right && a.clientY > l.bottom && a.clientX >= l.left : a.clientX > l.right && a.clientY > l.top || a.clientX <= l.right && a.clientY > l.bottom + r
+    return e ? a.clientX > i.right + r || a.clientX <= i.right && a.clientY > i.bottom && a.clientX >= i.left : a.clientX > i.right && a.clientY > i.top || a.clientX <= i.right && a.clientY > i.bottom + r
 }
 
-function Ei(a, e, n, l, r, u, t, o) {
-    var i = l ? a.clientY : a.clientX,
-        s = l ? n.height : n.width,
-        c = l ? n.top : n.left,
-        f = l ? n.bottom : n.right,
+function Ai(a, e, n, i, r, s, t, o) {
+    var l = i ? a.clientY : a.clientX,
+        u = i ? n.height : n.width,
+        f = i ? n.top : n.left,
+        c = i ? n.bottom : n.right,
         d = !1;
     if (!t) {
-        if (o && nn < s * r) {
-            if (!Ge && (Ve === 1 ? i > c + s * u / 2 : i < f - s * u / 2) && (Ge = !0), Ge) d = !0;
-            else if (Ve === 1 ? i < c + nn : i > f - nn) return -Ve
-        } else if (i > c + s * (1 - r) / 2 && i < f - s * (1 - r) / 2) return xi(e)
+        if (o && on < u * r) {
+            if (!He && (Ke === 1 ? l > f + u * s / 2 : l < c - u * s / 2) && (He = !0), He) d = !0;
+            else if (Ke === 1 ? l < f + on : l > c - on) return -Ke
+        } else if (l > f + u * (1 - r) / 2 && l < c - u * (1 - r) / 2) return Ri(e)
     }
-    return d = d || t, d && (i < c + s * u / 2 || i > f - s * u / 2) ? i > c + s / 2 ? 1 : -1 : 0
+    return d = d || t, d && (l < f + u * s / 2 || l > c - u * s / 2) ? l > f + u / 2 ? 1 : -1 : 0
 }
 
-function xi(a) {
-    return mt(N) < mt(a) ? 1 : -1
+function Ri(a) {
+    return gt(w) < gt(a) ? 1 : -1
 }
 
-function Oi(a) {
-    for (var e = a.tagName + a.className + a.src + a.href + a.textContent, n = e.length, l = 0; n--;) l += e.charCodeAt(n);
-    return l.toString(36)
+function wi(a) {
+    for (var e = a.tagName + a.className + a.src + a.href + a.textContent, n = e.length, i = 0; n--;) i += e.charCodeAt(n);
+    return i.toString(36)
 }
 
-function Ti(a) {
-    fn.length = 0;
+function Mi(a) {
+    dn.length = 0;
     for (var e = a.getElementsByTagName("input"), n = e.length; n--;) {
-        var l = e[n];
-        l.checked && fn.push(l)
+        var i = e[n];
+        i.checked && dn.push(i)
     }
 }
 
-function rn(a) {
+function an(a) {
     return setTimeout(a, 0)
 }
 
-function Dn(a) {
+function Rn(a) {
     return clearTimeout(a)
 }
-vn && et(document, "touchmove", function(a) {
-    (W.active || be) && a.cancelable && a.preventDefault()
+hn && et(document, "touchmove", function(a) {
+    (z.active || xe) && a.cancelable && a.preventDefault()
 });
-W.utils = {
+z.utils = {
     on: et,
     off: tt,
-    css: U,
-    find: cr,
+    css: G,
+    find: Sr,
     is: function(e, n) {
-        return !!Xt(e, n, e, !1)
+        return !!Jt(e, n, e, !1)
     },
-    extend: si,
-    throttle: dr,
-    closest: Xt,
-    toggleClass: dt,
-    clone: jn,
-    index: mt,
-    nextTick: rn,
-    cancelNextTick: Dn,
-    detectDirection: pr,
-    getChild: Ee
+    extend: hi,
+    throttle: Er,
+    closest: Jt,
+    toggleClass: vt,
+    clone: Un,
+    index: gt,
+    nextTick: an,
+    cancelNextTick: Rn,
+    detectDirection: Tr,
+    getChild: Ie
 };
-W.get = function(a) {
-    return a[At]
+z.get = function(a) {
+    return a[Rt]
 };
-W.mount = function() {
+z.mount = function() {
     for (var a = arguments.length, e = new Array(a), n = 0; n < a; n++) e[n] = arguments[n];
-    e[0].constructor === Array && (e = e[0]), e.forEach(function(l) {
-        if (!l.prototype || !l.prototype.constructor) throw "Sortable: Mounted plugin must be a constructor function, not ".concat({}.toString.call(l));
-        l.utils && (W.utils = qt(qt({}, W.utils), l.utils)), Xe.mount(l)
+    e[0].constructor === Array && (e = e[0]), e.forEach(function(i) {
+        if (!i.prototype || !i.prototype.constructor) throw "Sortable: Mounted plugin must be a constructor function, not ".concat({}.toString.call(i));
+        i.utils && (z.utils = ee(ee({}, z.utils), i.utils)), ze.mount(i)
     })
 };
-W.create = function(a, e) {
-    return new W(a, e)
+z.create = function(a, e) {
+    return new z(a, e)
 };
-W.version = ri;
-var St = [],
-    je, An, Rn = !1,
-    On, Tn, cn, Fe;
+z.version = ci;
+var xt = [],
+    Le, wn, Mn = !1,
+    In, Pn, vn, Ve;
 
-function Ii() {
+function Ni() {
     function a() {
         this.defaults = {
             scroll: !0,
             forceAutoScrollFallback: !1,
             scrollSensitivity: 30,
             scrollSpeed: 10,
             bubbleScroll: !0
         };
         for (var e in this) e.charAt(0) === "_" && typeof this[e] == "function" && (this[e] = this[e].bind(this))
     }
     return a.prototype = {
         dragStarted: function(n) {
-            var l = n.originalEvent;
-            this.sortable.nativeDraggable ? et(document, "dragover", this._handleAutoScroll) : this.options.supportPointer ? et(document, "pointermove", this._handleFallbackAutoScroll) : l.touches ? et(document, "touchmove", this._handleFallbackAutoScroll) : et(document, "mousemove", this._handleFallbackAutoScroll)
+            var i = n.originalEvent;
+            this.sortable.nativeDraggable ? et(document, "dragover", this._handleAutoScroll) : this.options.supportPointer ? et(document, "pointermove", this._handleFallbackAutoScroll) : i.touches ? et(document, "touchmove", this._handleFallbackAutoScroll) : et(document, "mousemove", this._handleFallbackAutoScroll)
         },
         dragOverCompleted: function(n) {
-            var l = n.originalEvent;
-            !this.options.dragOverBubble && !l.rootEl && this._handleAutoScroll(l)
+            var i = n.originalEvent;
+            !this.options.dragOverBubble && !i.rootEl && this._handleAutoScroll(i)
         },
         drop: function() {
-            this.sortable.nativeDraggable ? tt(document, "dragover", this._handleAutoScroll) : (tt(document, "pointermove", this._handleFallbackAutoScroll), tt(document, "touchmove", this._handleFallbackAutoScroll), tt(document, "mousemove", this._handleFallbackAutoScroll)), Yn(), on(), li()
+            this.sortable.nativeDraggable ? tt(document, "dragover", this._handleAutoScroll) : (tt(document, "pointermove", this._handleFallbackAutoScroll), tt(document, "touchmove", this._handleFallbackAutoScroll), tt(document, "mousemove", this._handleFallbackAutoScroll)), er(), ln(), mi()
         },
         nulling: function() {
-            cn = An = je = Rn = Fe = On = Tn = null, St.length = 0
+            vn = wn = Le = Mn = Ve = In = Pn = null, xt.length = 0
         },
         _handleFallbackAutoScroll: function(n) {
             this._handleAutoScroll(n, !0)
         },
-        _handleAutoScroll: function(n, l) {
+        _handleAutoScroll: function(n, i) {
             var r = this,
-                u = (n.touches ? n.touches[0] : n).clientX,
+                s = (n.touches ? n.touches[0] : n).clientX,
                 t = (n.touches ? n.touches[0] : n).clientY,
-                o = document.elementFromPoint(u, t);
-            if (cn = n, l || this.options.forceAutoScrollFallback || We || re || Le) {
-                In(n, this.options, o, l);
-                var i = le(o, !0);
-                Rn && (!Fe || u !== On || t !== Tn) && (Fe && Yn(), Fe = setInterval(function() {
-                    var s = le(document.elementFromPoint(u, t), !0);
-                    s !== i && (i = s, on()), In(n, r.options, s, l)
-                }, 10), On = u, Tn = t)
+                o = document.elementFromPoint(s, t);
+            if (vn = n, i || this.options.forceAutoScrollFallback || Ye || ae || Ue) {
+                Cn(n, this.options, o, i);
+                var l = fe(o, !0);
+                Mn && (!Ve || s !== In || t !== Pn) && (Ve && er(), Ve = setInterval(function() {
+                    var u = fe(document.elementFromPoint(s, t), !0);
+                    u !== l && (l = u, ln()), Cn(n, r.options, u, i)
+                }, 10), In = s, Pn = t)
             } else {
-                if (!this.options.bubbleScroll || le(o, !0) === kt()) {
-                    on();
+                if (!this.options.bubbleScroll || fe(o, !0) === te()) {
+                    ln();
                     return
                 }
-                In(n, this.options, le(o, !1), !1)
+                Cn(n, this.options, fe(o, !1), !1)
             }
         }
-    }, Bt(a, {
+    }, Ht(a, {
         pluginName: "scroll",
         initializeByDefault: !0
     })
 }
 
-function on() {
-    St.forEach(function(a) {
+function ln() {
+    xt.forEach(function(a) {
         clearInterval(a.pid)
-    }), St = []
+    }), xt = []
 }
 
-function Yn() {
-    clearInterval(Fe)
+function er() {
+    clearInterval(Ve)
 }
-var In = dr(function(a, e, n, l) {
+var Cn = Er(function(a, e, n, i) {
         if (!!e.scroll) {
             var r = (a.touches ? a.touches[0] : a).clientX,
-                u = (a.touches ? a.touches[0] : a).clientY,
+                s = (a.touches ? a.touches[0] : a).clientY,
                 t = e.scrollSensitivity,
                 o = e.scrollSpeed,
-                i = kt(),
-                s = !1,
-                c;
-            An !== n && (An = n, on(), je = e.scroll, c = e.scrollFn, je === !0 && (je = le(n, !0)));
-            var f = 0,
-                d = je;
+                l = te(),
+                u = !1,
+                f;
+            wn !== n && (wn = n, ln(), Le = e.scroll, f = e.scrollFn, Le === !0 && (Le = fe(n, !0)));
+            var c = 0,
+                d = Le;
             do {
                 var v = d,
-                    h = ft(v),
-                    p = h.top,
-                    g = h.bottom,
-                    b = h.left,
-                    S = h.right,
-                    P = h.width,
-                    x = h.height,
+                    p = ft(v),
+                    h = p.top,
+                    m = p.bottom,
+                    g = p.left,
+                    y = p.right,
+                    O = p.width,
+                    E = p.height,
                     C = void 0,
-                    I = void 0,
-                    j = v.scrollWidth,
+                    T = void 0,
+                    $ = v.scrollWidth,
                     L = v.scrollHeight,
-                    T = U(v),
-                    O = v.scrollLeft,
-                    D = v.scrollTop;
-                v === i ? (C = P < j && (T.overflowX === "auto" || T.overflowX === "scroll" || T.overflowX === "visible"), I = x < L && (T.overflowY === "auto" || T.overflowY === "scroll" || T.overflowY === "visible")) : (C = P < j && (T.overflowX === "auto" || T.overflowX === "scroll"), I = x < L && (T.overflowY === "auto" || T.overflowY === "scroll"));
-                var G = C && (Math.abs(S - r) <= t && O + P < j) - (Math.abs(b - r) <= t && !!O),
-                    A = I && (Math.abs(g - u) <= t && D + x < L) - (Math.abs(p - u) <= t && !!D);
-                if (!St[f])
-                    for (var M = 0; M <= f; M++) St[M] || (St[M] = {});
-                (St[f].vx != G || St[f].vy != A || St[f].el !== v) && (St[f].el = v, St[f].vx = G, St[f].vy = A, clearInterval(St[f].pid), (G != 0 || A != 0) && (s = !0, St[f].pid = setInterval(function() {
-                    l && this.layer === 0 && W.active._onTouchMove(cn);
-                    var X = St[this.layer].vy ? St[this.layer].vy * o : 0,
-                        R = St[this.layer].vx ? St[this.layer].vx * o : 0;
-                    typeof c == "function" && c.call(W.dragged.parentNode[At], R, X, a, cn, St[this.layer].el) !== "continue" || vr(St[this.layer].el, R, X)
+                    I = G(v),
+                    j = v.scrollLeft,
+                    P = v.scrollTop;
+                v === l ? (C = O < $ && (I.overflowX === "auto" || I.overflowX === "scroll" || I.overflowX === "visible"), T = E < L && (I.overflowY === "auto" || I.overflowY === "scroll" || I.overflowY === "visible")) : (C = O < $ && (I.overflowX === "auto" || I.overflowX === "scroll"), T = E < L && (I.overflowY === "auto" || I.overflowY === "scroll"));
+                var M = C && (Math.abs(y - r) <= t && j + O < $) - (Math.abs(g - r) <= t && !!j),
+                    D = T && (Math.abs(m - s) <= t && P + E < L) - (Math.abs(h - s) <= t && !!P);
+                if (!xt[c])
+                    for (var R = 0; R <= c; R++) xt[R] || (xt[R] = {});
+                (xt[c].vx != M || xt[c].vy != D || xt[c].el !== v) && (xt[c].el = v, xt[c].vx = M, xt[c].vy = D, clearInterval(xt[c].pid), (M != 0 || D != 0) && (u = !0, xt[c].pid = setInterval(function() {
+                    i && this.layer === 0 && z.active._onTouchMove(vn);
+                    var H = xt[this.layer].vy ? xt[this.layer].vy * o : 0,
+                        F = xt[this.layer].vx ? xt[this.layer].vx * o : 0;
+                    typeof f == "function" && f.call(z.dragged.parentNode[Rt], F, H, a, vn, xt[this.layer].el) !== "continue" || xr(xt[this.layer].el, F, H)
                 }.bind({
-                    layer: f
-                }), 24))), f++
-            } while (e.bubbleScroll && d !== i && (d = le(d, !1)));
-            Rn = s
+                    layer: c
+                }), 24))), c++
+            } while (e.bubbleScroll && d !== l && (d = fe(d, !1)));
+            Mn = u
         }
     }, 30),
-    br = function(e) {
+    Dr = function(e) {
         var n = e.originalEvent,
-            l = e.putSortable,
+            i = e.putSortable,
             r = e.dragEl,
-            u = e.activeSortable,
+            s = e.activeSortable,
             t = e.dispatchSortableEvent,
             o = e.hideGhostForTarget,
-            i = e.unhideGhostForTarget;
+            l = e.unhideGhostForTarget;
         if (!!n) {
-            var s = l || u;
+            var u = i || s;
             o();
-            var c = n.changedTouches && n.changedTouches.length ? n.changedTouches[0] : n,
-                f = document.elementFromPoint(c.clientX, c.clientY);
-            i(), s && !s.el.contains(f) && (t("spill"), this.onSpill({
+            var f = n.changedTouches && n.changedTouches.length ? n.changedTouches[0] : n,
+                c = document.elementFromPoint(f.clientX, f.clientY);
+            l(), u && !u.el.contains(c) && (t("spill"), this.onSpill({
                 dragEl: r,
-                putSortable: l
+                putSortable: i
             }))
         }
     };
 
-function Fn() {}
-Fn.prototype = {
+function Gn() {}
+Gn.prototype = {
     startIndex: null,
     dragStart: function(e) {
         var n = e.oldDraggableIndex;
         this.startIndex = n
     },
     onSpill: function(e) {
         var n = e.dragEl,
-            l = e.putSortable;
-        this.sortable.captureAnimationState(), l && l.captureAnimationState();
-        var r = Ee(this.sortable.el, this.startIndex, this.options);
-        r ? this.sortable.el.insertBefore(n, r) : this.sortable.el.appendChild(n), this.sortable.animateAll(), l && l.animateAll()
+            i = e.putSortable;
+        this.sortable.captureAnimationState(), i && i.captureAnimationState();
+        var r = Ie(this.sortable.el, this.startIndex, this.options);
+        r ? this.sortable.el.insertBefore(n, r) : this.sortable.el.appendChild(n), this.sortable.animateAll(), i && i.animateAll()
     },
-    drop: br
+    drop: Dr
 };
-Bt(Fn, {
+Ht(Gn, {
     pluginName: "revertOnSpill"
 });
 
-function Ln() {}
-Ln.prototype = {
+function Bn() {}
+Bn.prototype = {
     onSpill: function(e) {
         var n = e.dragEl,
-            l = e.putSortable,
-            r = l || this.sortable;
+            i = e.putSortable,
+            r = i || this.sortable;
         r.captureAnimationState(), n.parentNode && n.parentNode.removeChild(n), r.animateAll()
     },
-    drop: br
+    drop: Dr
 };
-Bt(Ln, {
+Ht(Bn, {
     pluginName: "removeOnSpill"
 });
-var Vt;
+var Kt;
 
-function Pi() {
+function ji() {
     function a() {
         this.defaults = {
             swapClass: "sortable-swap-highlight"
         }
     }
     return a.prototype = {
         dragStart: function(n) {
-            var l = n.dragEl;
-            Vt = l
+            var i = n.dragEl;
+            Kt = i
         },
         dragOverValid: function(n) {
-            var l = n.completed,
+            var i = n.completed,
                 r = n.target,
-                u = n.onMove,
+                s = n.onMove,
                 t = n.activeSortable,
                 o = n.changed,
-                i = n.cancel;
+                l = n.cancel;
             if (!!t.options.swap) {
-                var s = this.sortable.el,
-                    c = this.options;
-                if (r && r !== s) {
-                    var f = Vt;
-                    u(r) !== !1 ? (dt(r, c.swapClass, !0), Vt = r) : Vt = null, f && f !== Vt && dt(f, c.swapClass, !1)
+                var u = this.sortable.el,
+                    f = this.options;
+                if (r && r !== u) {
+                    var c = Kt;
+                    s(r) !== !1 ? (vt(r, f.swapClass, !0), Kt = r) : Kt = null, c && c !== Kt && vt(c, f.swapClass, !1)
                 }
-                o(), l(!0), i()
+                o(), i(!0), l()
             }
         },
         drop: function(n) {
-            var l = n.activeSortable,
+            var i = n.activeSortable,
                 r = n.putSortable,
-                u = n.dragEl,
+                s = n.dragEl,
                 t = r || this.sortable,
                 o = this.options;
-            Vt && dt(Vt, o.swapClass, !1), Vt && (o.swap || r && r.options.swap) && u !== Vt && (t.captureAnimationState(), t !== l && l.captureAnimationState(), Ci(u, Vt), t.animateAll(), t !== l && l.animateAll())
+            Kt && vt(Kt, o.swapClass, !1), Kt && (o.swap || r && r.options.swap) && s !== Kt && (t.captureAnimationState(), t !== i && i.captureAnimationState(), Fi(s, Kt), t.animateAll(), t !== i && i.animateAll())
         },
         nulling: function() {
-            Vt = null
+            Kt = null
         }
-    }, Bt(a, {
+    }, Ht(a, {
         pluginName: "swap",
         eventProperties: function() {
             return {
-                swapItem: Vt
+                swapItem: Kt
             }
         }
     })
 }
 
-function Ci(a, e) {
+function Fi(a, e) {
     var n = a.parentNode,
-        l = e.parentNode,
-        r, u;
-    !n || !l || n.isEqualNode(e) || l.isEqualNode(a) || (r = mt(a), u = mt(e), n.isEqualNode(l) && r < u && u++, n.insertBefore(e, n.children[r]), l.insertBefore(a, l.children[u]))
-}
-var Q = [],
-    $t = [],
-    Ae, Wt, Re = !1,
-    Ft = !1,
-    ye = !1,
-    st, we, qe;
+        i = e.parentNode,
+        r, s;
+    !n || !i || n.isEqualNode(e) || i.isEqualNode(a) || (r = gt(a), s = gt(e), n.isEqualNode(i) && r < s && s++, n.insertBefore(e, n.children[r]), i.insertBefore(a, i.children[s]))
+}
+var Z = [],
+    Vt = [],
+    Me, Yt, Ne = !1,
+    $t = !1,
+    Ee = !1,
+    lt, je, tn;
 
-function Di() {
+function $i() {
     function a(e) {
         for (var n in this) n.charAt(0) === "_" && typeof this[n] == "function" && (this[n] = this[n].bind(this));
         e.options.supportPointer ? et(document, "pointerup", this._deselectMultiDrag) : (et(document, "mouseup", this._deselectMultiDrag), et(document, "touchend", this._deselectMultiDrag)), et(document, "keydown", this._checkKeyDown), et(document, "keyup", this._checkKeyUp), this.defaults = {
             selectedClass: "sortable-selected",
             multiDragKey: null,
-            setData: function(r, u) {
+            setData: function(r, s) {
                 var t = "";
-                Q.length && Wt === e ? Q.forEach(function(o, i) {
-                    t += (i ? ", " : "") + o.textContent
-                }) : t = u.textContent, r.setData("Text", t)
+                Z.length && Yt === e ? Z.forEach(function(o, l) {
+                    t += (l ? ", " : "") + o.textContent
+                }) : t = s.textContent, r.setData("Text", t)
             }
         }
     }
     return a.prototype = {
         multiDragKeyDown: !1,
         isMultiDrag: !1,
         delayStartGlobal: function(n) {
-            var l = n.dragEl;
-            st = l
+            var i = n.dragEl;
+            lt = i
         },
         delayEnded: function() {
-            this.isMultiDrag = ~Q.indexOf(st)
+            this.isMultiDrag = ~Z.indexOf(lt)
         },
         setupClone: function(n) {
-            var l = n.sortable,
+            var i = n.sortable,
                 r = n.cancel;
             if (!!this.isMultiDrag) {
-                for (var u = 0; u < Q.length; u++) $t.push(jn(Q[u])), $t[u].sortableIndex = Q[u].sortableIndex, $t[u].draggable = !1, $t[u].style["will-change"] = "", dt($t[u], this.options.selectedClass, !1), Q[u] === st && dt($t[u], this.options.chosenClass, !1);
-                l._hideClone(), r()
+                for (var s = 0; s < Z.length; s++) Vt.push(Un(Z[s])), Vt[s].sortableIndex = Z[s].sortableIndex, Vt[s].draggable = !1, Vt[s].style["will-change"] = "", vt(Vt[s], this.options.selectedClass, !1), Z[s] === lt && vt(Vt[s], this.options.chosenClass, !1);
+                i._hideClone(), r()
             }
         },
         clone: function(n) {
-            var l = n.sortable,
+            var i = n.sortable,
                 r = n.rootEl,
-                u = n.dispatchSortableEvent,
+                s = n.dispatchSortableEvent,
                 t = n.cancel;
-            !this.isMultiDrag || this.options.removeCloneOnHide || Q.length && Wt === l && (zn(!0, r), u("clone"), t())
+            !this.isMultiDrag || this.options.removeCloneOnHide || Z.length && Yt === i && (nr(!0, r), s("clone"), t())
         },
         showClone: function(n) {
-            var l = n.cloneNowShown,
+            var i = n.cloneNowShown,
                 r = n.rootEl,
-                u = n.cancel;
-            !this.isMultiDrag || (zn(!1, r), $t.forEach(function(t) {
-                U(t, "display", "")
-            }), l(), qe = !1, u())
+                s = n.cancel;
+            !this.isMultiDrag || (nr(!1, r), Vt.forEach(function(t) {
+                G(t, "display", "")
+            }), i(), tn = !1, s())
         },
         hideClone: function(n) {
-            var l = this;
+            var i = this;
             n.sortable;
             var r = n.cloneNowHidden,
-                u = n.cancel;
-            !this.isMultiDrag || ($t.forEach(function(t) {
-                U(t, "display", "none"), l.options.removeCloneOnHide && t.parentNode && t.parentNode.removeChild(t)
-            }), r(), qe = !0, u())
+                s = n.cancel;
+            !this.isMultiDrag || (Vt.forEach(function(t) {
+                G(t, "display", "none"), i.options.removeCloneOnHide && t.parentNode && t.parentNode.removeChild(t)
+            }), r(), tn = !0, s())
         },
         dragStartGlobal: function(n) {
-            n.sortable, !this.isMultiDrag && Wt && Wt.multiDrag._deselectMultiDrag(), Q.forEach(function(l) {
-                l.sortableIndex = mt(l)
-            }), Q = Q.sort(function(l, r) {
-                return l.sortableIndex - r.sortableIndex
-            }), ye = !0
+            n.sortable, !this.isMultiDrag && Yt && Yt.multiDrag._deselectMultiDrag(), Z.forEach(function(i) {
+                i.sortableIndex = gt(i)
+            }), Z = Z.sort(function(i, r) {
+                return i.sortableIndex - r.sortableIndex
+            }), Ee = !0
         },
         dragStarted: function(n) {
-            var l = this,
+            var i = this,
                 r = n.sortable;
             if (!!this.isMultiDrag) {
                 if (this.options.sort && (r.captureAnimationState(), this.options.animation)) {
-                    Q.forEach(function(t) {
-                        t !== st && U(t, "position", "absolute")
+                    Z.forEach(function(t) {
+                        t !== lt && G(t, "position", "absolute")
                     });
-                    var u = ft(st, !1, !0, !0);
-                    Q.forEach(function(t) {
-                        t !== st && Kn(t, u)
-                    }), Ft = !0, Re = !0
+                    var s = ft(lt, !1, !0, !0);
+                    Z.forEach(function(t) {
+                        t !== lt && kn(t, s)
+                    }), $t = !0, Ne = !0
                 }
                 r.animateAll(function() {
-                    Ft = !1, Re = !1, l.options.animation && Q.forEach(function(t) {
-                        mn(t)
-                    }), l.options.sort && _e()
+                    $t = !1, Ne = !1, i.options.animation && Z.forEach(function(t) {
+                        bn(t)
+                    }), i.options.sort && en()
                 })
             }
         },
         dragOver: function(n) {
-            var l = n.target,
+            var i = n.target,
                 r = n.completed,
-                u = n.cancel;
-            Ft && ~Q.indexOf(l) && (r(!1), u())
+                s = n.cancel;
+            $t && ~Z.indexOf(i) && (r(!1), s())
         },
         revert: function(n) {
-            var l = n.fromSortable,
+            var i = n.fromSortable,
                 r = n.rootEl,
-                u = n.sortable,
+                s = n.sortable,
                 t = n.dragRect;
-            Q.length > 1 && (Q.forEach(function(o) {
-                u.addAnimationState({
+            Z.length > 1 && (Z.forEach(function(o) {
+                s.addAnimationState({
                     target: o,
-                    rect: Ft ? ft(o) : t
-                }), mn(o), o.fromRect = t, l.removeAnimationState(o)
-            }), Ft = !1, Ai(!this.options.removeCloneOnHide, r))
+                    rect: $t ? ft(o) : t
+                }), bn(o), o.fromRect = t, i.removeAnimationState(o)
+            }), $t = !1, Li(!this.options.removeCloneOnHide, r))
         },
         dragOverCompleted: function(n) {
-            var l = n.sortable,
+            var i = n.sortable,
                 r = n.isOwner,
-                u = n.insertion,
+                s = n.insertion,
                 t = n.activeSortable,
                 o = n.parentEl,
-                i = n.putSortable,
-                s = this.options;
-            if (u) {
-                if (r && t._hideClone(), Re = !1, s.animation && Q.length > 1 && (Ft || !r && !t.options.sort && !i)) {
-                    var c = ft(st, !1, !0, !0);
-                    Q.forEach(function(d) {
-                        d !== st && (Kn(d, c), o.appendChild(d))
-                    }), Ft = !0
+                l = n.putSortable,
+                u = this.options;
+            if (s) {
+                if (r && t._hideClone(), Ne = !1, u.animation && Z.length > 1 && ($t || !r && !t.options.sort && !l)) {
+                    var f = ft(lt, !1, !0, !0);
+                    Z.forEach(function(d) {
+                        d !== lt && (kn(d, f), o.appendChild(d))
+                    }), $t = !0
                 }
                 if (!r)
-                    if (Ft || _e(), Q.length > 1) {
-                        var f = qe;
-                        t._showClone(l), t.options.animation && !qe && f && $t.forEach(function(d) {
+                    if ($t || en(), Z.length > 1) {
+                        var c = tn;
+                        t._showClone(i), t.options.animation && !tn && c && Vt.forEach(function(d) {
                             t.addAnimationState({
                                 target: d,
-                                rect: we
-                            }), d.fromRect = we, d.thisAnimationDuration = null
+                                rect: je
+                            }), d.fromRect = je, d.thisAnimationDuration = null
                         })
-                    } else t._showClone(l)
+                    } else t._showClone(i)
             }
         },
         dragOverAnimationCapture: function(n) {
-            var l = n.dragRect,
+            var i = n.dragRect,
                 r = n.isOwner,
-                u = n.activeSortable;
-            if (Q.forEach(function(o) {
+                s = n.activeSortable;
+            if (Z.forEach(function(o) {
                     o.thisAnimationDuration = null
-                }), u.options.animation && !r && u.multiDrag.isMultiDrag) {
-                we = Bt({}, l);
-                var t = he(st, !0);
-                we.top -= t.f, we.left -= t.e
+                }), s.options.animation && !r && s.multiDrag.isMultiDrag) {
+                je = Ht({}, i);
+                var t = ge(lt, !0);
+                je.top -= t.f, je.left -= t.e
             }
         },
         dragOverAnimationComplete: function() {
-            Ft && (Ft = !1, _e())
+            $t && ($t = !1, en())
         },
         drop: function(n) {
-            var l = n.originalEvent,
+            var i = n.originalEvent,
                 r = n.rootEl,
-                u = n.parentEl,
+                s = n.parentEl,
                 t = n.sortable,
                 o = n.dispatchSortableEvent,
-                i = n.oldIndex,
-                s = n.putSortable,
-                c = s || this.sortable;
-            if (!!l) {
-                var f = this.options,
-                    d = u.children;
-                if (!ye)
-                    if (f.multiDragKey && !this.multiDragKeyDown && this._deselectMultiDrag(), dt(st, f.selectedClass, !~Q.indexOf(st)), ~Q.indexOf(st)) Q.splice(Q.indexOf(st), 1), Ae = null, Me({
+                l = n.oldIndex,
+                u = n.putSortable,
+                f = u || this.sortable;
+            if (!!i) {
+                var c = this.options,
+                    d = s.children;
+                if (!Ee)
+                    if (c.multiDragKey && !this.multiDragKeyDown && this._deselectMultiDrag(), vt(lt, c.selectedClass, !~Z.indexOf(lt)), ~Z.indexOf(lt)) Z.splice(Z.indexOf(lt), 1), Me = null, Fe({
                         sortable: t,
                         rootEl: r,
                         name: "deselect",
-                        targetEl: st,
-                        originalEvt: l
+                        targetEl: lt,
+                        originalEvt: i
                     });
                     else {
-                        if (Q.push(st), Me({
+                        if (Z.push(lt), Fe({
                                 sortable: t,
                                 rootEl: r,
                                 name: "select",
-                                targetEl: st,
-                                originalEvt: l
-                            }), l.shiftKey && Ae && t.el.contains(Ae)) {
-                            var v = mt(Ae),
-                                h = mt(st);
-                            if (~v && ~h && v !== h) {
-                                var p, g;
-                                for (h > v ? (g = v, p = h) : (g = h, p = v + 1); g < p; g++) ~Q.indexOf(d[g]) || (dt(d[g], f.selectedClass, !0), Q.push(d[g]), Me({
+                                targetEl: lt,
+                                originalEvt: i
+                            }), i.shiftKey && Me && t.el.contains(Me)) {
+                            var v = gt(Me),
+                                p = gt(lt);
+                            if (~v && ~p && v !== p) {
+                                var h, m;
+                                for (p > v ? (m = v, h = p) : (m = p, h = v + 1); m < h; m++) ~Z.indexOf(d[m]) || (vt(d[m], c.selectedClass, !0), Z.push(d[m]), Fe({
                                     sortable: t,
                                     rootEl: r,
                                     name: "select",
-                                    targetEl: d[g],
-                                    originalEvt: l
+                                    targetEl: d[m],
+                                    originalEvt: i
                                 }))
                             }
-                        } else Ae = st;
-                        Wt = c
-                    } if (ye && this.isMultiDrag) {
-                    if (Ft = !1, (u[At].options.sort || u !== r) && Q.length > 1) {
-                        var b = ft(st),
-                            S = mt(st, ":not(." + this.options.selectedClass + ")");
-                        if (!Re && f.animation && (st.thisAnimationDuration = null), c.captureAnimationState(), !Re && (f.animation && (st.fromRect = b, Q.forEach(function(x) {
-                                if (x.thisAnimationDuration = null, x !== st) {
-                                    var C = Ft ? ft(x) : b;
-                                    x.fromRect = C, c.addAnimationState({
-                                        target: x,
+                        } else Me = lt;
+                        Yt = f
+                    } if (Ee && this.isMultiDrag) {
+                    if ($t = !1, (s[Rt].options.sort || s !== r) && Z.length > 1) {
+                        var g = ft(lt),
+                            y = gt(lt, ":not(." + this.options.selectedClass + ")");
+                        if (!Ne && c.animation && (lt.thisAnimationDuration = null), f.captureAnimationState(), !Ne && (c.animation && (lt.fromRect = g, Z.forEach(function(E) {
+                                if (E.thisAnimationDuration = null, E !== lt) {
+                                    var C = $t ? ft(E) : g;
+                                    E.fromRect = C, f.addAnimationState({
+                                        target: E,
                                         rect: C
                                     })
                                 }
-                            })), _e(), Q.forEach(function(x) {
-                                d[S] ? u.insertBefore(x, d[S]) : u.appendChild(x), S++
-                            }), i === mt(st))) {
-                            var P = !1;
-                            Q.forEach(function(x) {
-                                if (x.sortableIndex !== mt(x)) {
-                                    P = !0;
+                            })), en(), Z.forEach(function(E) {
+                                d[y] ? s.insertBefore(E, d[y]) : s.appendChild(E), y++
+                            }), l === gt(lt))) {
+                            var O = !1;
+                            Z.forEach(function(E) {
+                                if (E.sortableIndex !== gt(E)) {
+                                    O = !0;
                                     return
                                 }
-                            }), P && o("update")
+                            }), O && o("update")
                         }
-                        Q.forEach(function(x) {
-                            mn(x)
-                        }), c.animateAll()
-                    }
-                    Wt = c
-                }(r === u || s && s.lastPutMode !== "clone") && $t.forEach(function(x) {
-                    x.parentNode && x.parentNode.removeChild(x)
+                        Z.forEach(function(E) {
+                            bn(E)
+                        }), f.animateAll()
+                    }
+                    Yt = f
+                }(r === s || u && u.lastPutMode !== "clone") && Vt.forEach(function(E) {
+                    E.parentNode && E.parentNode.removeChild(E)
                 })
             }
         },
         nullingGlobal: function() {
-            this.isMultiDrag = ye = !1, $t.length = 0
+            this.isMultiDrag = Ee = !1, Vt.length = 0
         },
         destroyGlobal: function() {
             this._deselectMultiDrag(), tt(document, "pointerup", this._deselectMultiDrag), tt(document, "mouseup", this._deselectMultiDrag), tt(document, "touchend", this._deselectMultiDrag), tt(document, "keydown", this._checkKeyDown), tt(document, "keyup", this._checkKeyUp)
         },
         _deselectMultiDrag: function(n) {
-            if (!(typeof ye < "u" && ye) && Wt === this.sortable && !(n && Xt(n.target, this.options.draggable, this.sortable.el, !1)) && !(n && n.button !== 0))
-                for (; Q.length;) {
-                    var l = Q[0];
-                    dt(l, this.options.selectedClass, !1), Q.shift(), Me({
+            if (!(typeof Ee < "u" && Ee) && Yt === this.sortable && !(n && Jt(n.target, this.options.draggable, this.sortable.el, !1)) && !(n && n.button !== 0))
+                for (; Z.length;) {
+                    var i = Z[0];
+                    vt(i, this.options.selectedClass, !1), Z.shift(), Fe({
                         sortable: this.sortable,
                         rootEl: this.sortable.el,
                         name: "deselect",
-                        targetEl: l,
+                        targetEl: i,
                         originalEvt: n
                     })
                 }
         },
         _checkKeyDown: function(n) {
             n.key === this.options.multiDragKey && (this.multiDragKeyDown = !0)
         },
         _checkKeyUp: function(n) {
             n.key === this.options.multiDragKey && (this.multiDragKeyDown = !1)
         }
-    }, Bt(a, {
+    }, Ht(a, {
         pluginName: "multiDrag",
         utils: {
             select: function(n) {
-                var l = n.parentNode[At];
-                !l || !l.options.multiDrag || ~Q.indexOf(n) || (Wt && Wt !== l && (Wt.multiDrag._deselectMultiDrag(), Wt = l), dt(n, l.options.selectedClass, !0), Q.push(n))
+                var i = n.parentNode[Rt];
+                !i || !i.options.multiDrag || ~Z.indexOf(n) || (Yt && Yt !== i && (Yt.multiDrag._deselectMultiDrag(), Yt = i), vt(n, i.options.selectedClass, !0), Z.push(n))
             },
             deselect: function(n) {
-                var l = n.parentNode[At],
-                    r = Q.indexOf(n);
-                !l || !l.options.multiDrag || !~r || (dt(n, l.options.selectedClass, !1), Q.splice(r, 1))
+                var i = n.parentNode[Rt],
+                    r = Z.indexOf(n);
+                !i || !i.options.multiDrag || !~r || (vt(n, i.options.selectedClass, !1), Z.splice(r, 1))
             }
         },
         eventProperties: function() {
             var n = this,
-                l = [],
+                i = [],
                 r = [];
-            return Q.forEach(function(u) {
-                l.push({
-                    multiDragElement: u,
-                    index: u.sortableIndex
+            return Z.forEach(function(s) {
+                i.push({
+                    multiDragElement: s,
+                    index: s.sortableIndex
                 });
                 var t;
-                Ft && u !== st ? t = -1 : Ft ? t = mt(u, ":not(." + n.options.selectedClass + ")") : t = mt(u), r.push({
-                    multiDragElement: u,
+                $t && s !== lt ? t = -1 : $t ? t = gt(s, ":not(." + n.options.selectedClass + ")") : t = gt(s), r.push({
+                    multiDragElement: s,
                     index: t
                 })
             }), {
-                items: qa(Q),
-                clones: [].concat($t),
-                oldIndicies: l,
+                items: ii(Z),
+                clones: [].concat(Vt),
+                oldIndicies: i,
                 newIndicies: r
             }
         },
         optionListeners: {
             multiDragKey: function(n) {
                 return n = n.toLowerCase(), n === "ctrl" ? n = "Control" : n.length > 1 && (n = n.charAt(0).toUpperCase() + n.substr(1)), n
             }
         }
     })
 }
 
-function Ai(a, e) {
-    Q.forEach(function(n, l) {
-        var r = e.children[n.sortableIndex + (a ? Number(l) : 0)];
+function Li(a, e) {
+    Z.forEach(function(n, i) {
+        var r = e.children[n.sortableIndex + (a ? Number(i) : 0)];
         r ? e.insertBefore(n, r) : e.appendChild(n)
     })
 }
 
-function zn(a, e) {
-    $t.forEach(function(n, l) {
-        var r = e.children[n.sortableIndex + (a ? Number(l) : 0)];
+function nr(a, e) {
+    Vt.forEach(function(n, i) {
+        var r = e.children[n.sortableIndex + (a ? Number(i) : 0)];
         r ? e.insertBefore(n, r) : e.appendChild(n)
     })
 }
 
-function _e() {
-    Q.forEach(function(a) {
-        a !== st && a.parentNode && a.parentNode.removeChild(a)
+function en() {
+    Z.forEach(function(a) {
+        a !== lt && a.parentNode && a.parentNode.removeChild(a)
     })
 }
-W.mount(new Ii);
-W.mount(Ln, Fn);
-const Ri = Object.freeze(Object.defineProperty({
+z.mount(new Ni);
+z.mount(Bn, Gn);
+const Vi = Object.freeze(Object.defineProperty({
         __proto__: null,
-        default: W,
-        MultiDrag: Di,
-        Sortable: W,
-        Swap: Pi
+        default: z,
+        MultiDrag: $i,
+        Sortable: z,
+        Swap: ji
     }, Symbol.toStringTag, {
         value: "Module"
     })),
-    wi = sr(Ri);
+    Ui = mr(Vi);
 (function(a, e) {
-    (function(l, r) {
-        a.exports = r(Ja, wi)
-    })(typeof self < "u" ? self : Ya, function(n, l) {
+    (function(i, r) {
+        a.exports = r(ni, Ui)
+    })(typeof self < "u" ? self : ti, function(n, i) {
         return function(r) {
-            var u = {};
+            var s = {};
 
             function t(o) {
-                if (u[o]) return u[o].exports;
-                var i = u[o] = {
+                if (s[o]) return s[o].exports;
+                var l = s[o] = {
                     i: o,
                     l: !1,
                     exports: {}
                 };
-                return r[o].call(i.exports, i, i.exports, t), i.l = !0, i.exports
+                return r[o].call(l.exports, l, l.exports, t), l.l = !0, l.exports
             }
-            return t.m = r, t.c = u, t.d = function(o, i, s) {
-                t.o(o, i) || Object.defineProperty(o, i, {
+            return t.m = r, t.c = s, t.d = function(o, l, u) {
+                t.o(o, l) || Object.defineProperty(o, l, {
                     enumerable: !0,
-                    get: s
+                    get: u
                 })
             }, t.r = function(o) {
                 typeof Symbol < "u" && Symbol.toStringTag && Object.defineProperty(o, Symbol.toStringTag, {
                     value: "Module"
                 }), Object.defineProperty(o, "__esModule", {
                     value: !0
                 })
-            }, t.t = function(o, i) {
-                if (i & 1 && (o = t(o)), i & 8 || i & 4 && typeof o == "object" && o && o.__esModule) return o;
-                var s = Object.create(null);
-                if (t.r(s), Object.defineProperty(s, "default", {
+            }, t.t = function(o, l) {
+                if (l & 1 && (o = t(o)), l & 8 || l & 4 && typeof o == "object" && o && o.__esModule) return o;
+                var u = Object.create(null);
+                if (t.r(u), Object.defineProperty(u, "default", {
                         enumerable: !0,
                         value: o
-                    }), i & 2 && typeof o != "string")
-                    for (var c in o) t.d(s, c, function(f) {
-                        return o[f]
-                    }.bind(null, c));
-                return s
+                    }), l & 2 && typeof o != "string")
+                    for (var f in o) t.d(u, f, function(c) {
+                        return o[c]
+                    }.bind(null, f));
+                return u
             }, t.n = function(o) {
-                var i = o && o.__esModule ? function() {
+                var l = o && o.__esModule ? function() {
                     return o.default
                 } : function() {
                     return o
                 };
-                return t.d(i, "a", i), i
-            }, t.o = function(o, i) {
-                return Object.prototype.hasOwnProperty.call(o, i)
+                return t.d(l, "a", l), l
+            }, t.o = function(o, l) {
+                return Object.prototype.hasOwnProperty.call(o, l)
             }, t.p = "", t(t.s = "fb15")
         }({
-            "00ee": function(r, u, t) {
+            "00ee": function(r, s, t) {
                 var o = t("b622"),
-                    i = o("toStringTag"),
-                    s = {};
-                s[i] = "z", r.exports = String(s) === "[object z]"
+                    l = o("toStringTag"),
+                    u = {};
+                u[l] = "z", r.exports = String(u) === "[object z]"
             },
-            "0366": function(r, u, t) {
+            "0366": function(r, s, t) {
                 var o = t("1c0b");
-                r.exports = function(i, s, c) {
-                    if (o(i), s === void 0) return i;
-                    switch (c) {
+                r.exports = function(l, u, f) {
+                    if (o(l), u === void 0) return l;
+                    switch (f) {
                         case 0:
                             return function() {
-                                return i.call(s)
+                                return l.call(u)
                             };
                         case 1:
-                            return function(f) {
-                                return i.call(s, f)
+                            return function(c) {
+                                return l.call(u, c)
                             };
                         case 2:
-                            return function(f, d) {
-                                return i.call(s, f, d)
+                            return function(c, d) {
+                                return l.call(u, c, d)
                             };
                         case 3:
-                            return function(f, d, v) {
-                                return i.call(s, f, d, v)
+                            return function(c, d, v) {
+                                return l.call(u, c, d, v)
                             }
                     }
                     return function() {
-                        return i.apply(s, arguments)
+                        return l.apply(u, arguments)
                     }
                 }
             },
-            "057f": function(r, u, t) {
+            "057f": function(r, s, t) {
                 var o = t("fc6a"),
-                    i = t("241c").f,
-                    s = {}.toString,
-                    c = typeof window == "object" && window && Object.getOwnPropertyNames ? Object.getOwnPropertyNames(window) : [],
-                    f = function(d) {
+                    l = t("241c").f,
+                    u = {}.toString,
+                    f = typeof window == "object" && window && Object.getOwnPropertyNames ? Object.getOwnPropertyNames(window) : [],
+                    c = function(d) {
                         try {
-                            return i(d)
+                            return l(d)
                         } catch {
-                            return c.slice()
+                            return f.slice()
                         }
                     };
                 r.exports.f = function(v) {
-                    return c && s.call(v) == "[object Window]" ? f(v) : i(o(v))
+                    return f && u.call(v) == "[object Window]" ? c(v) : l(o(v))
                 }
             },
-            "06cf": function(r, u, t) {
+            "06cf": function(r, s, t) {
                 var o = t("83ab"),
-                    i = t("d1e7"),
-                    s = t("5c6c"),
-                    c = t("fc6a"),
-                    f = t("c04e"),
+                    l = t("d1e7"),
+                    u = t("5c6c"),
+                    f = t("fc6a"),
+                    c = t("c04e"),
                     d = t("5135"),
                     v = t("0cfb"),
-                    h = Object.getOwnPropertyDescriptor;
-                u.f = o ? h : function(g, b) {
-                    if (g = c(g), b = f(b, !0), v) try {
-                        return h(g, b)
+                    p = Object.getOwnPropertyDescriptor;
+                s.f = o ? p : function(m, g) {
+                    if (m = f(m), g = c(g, !0), v) try {
+                        return p(m, g)
                     } catch {}
-                    if (d(g, b)) return s(!i.f.call(g, b), g[b])
+                    if (d(m, g)) return u(!l.f.call(m, g), m[g])
                 }
             },
-            "0cfb": function(r, u, t) {
+            "0cfb": function(r, s, t) {
                 var o = t("83ab"),
-                    i = t("d039"),
-                    s = t("cc12");
-                r.exports = !o && !i(function() {
-                    return Object.defineProperty(s("div"), "a", {
+                    l = t("d039"),
+                    u = t("cc12");
+                r.exports = !o && !l(function() {
+                    return Object.defineProperty(u("div"), "a", {
                         get: function() {
                             return 7
                         }
                     }).a != 7
                 })
             },
-            "13d5": function(r, u, t) {
+            "13d5": function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("d58f").left,
-                    s = t("a640"),
-                    c = t("ae40"),
-                    f = s("reduce"),
-                    d = c("reduce", {
+                    l = t("d58f").left,
+                    u = t("a640"),
+                    f = t("ae40"),
+                    c = u("reduce"),
+                    d = f("reduce", {
                         1: 0
                     });
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: !f || !d
+                    forced: !c || !d
                 }, {
-                    reduce: function(h) {
-                        return i(this, h, arguments.length, arguments.length > 1 ? arguments[1] : void 0)
+                    reduce: function(p) {
+                        return l(this, p, arguments.length, arguments.length > 1 ? arguments[1] : void 0)
                     }
                 })
             },
-            "14c3": function(r, u, t) {
+            "14c3": function(r, s, t) {
                 var o = t("c6b6"),
-                    i = t("9263");
-                r.exports = function(s, c) {
-                    var f = s.exec;
-                    if (typeof f == "function") {
-                        var d = f.call(s, c);
+                    l = t("9263");
+                r.exports = function(u, f) {
+                    var c = u.exec;
+                    if (typeof c == "function") {
+                        var d = c.call(u, f);
                         if (typeof d != "object") throw TypeError("RegExp exec method returned something other than an Object or null");
                         return d
                     }
-                    if (o(s) !== "RegExp") throw TypeError("RegExp#exec called on incompatible receiver");
-                    return i.call(s, c)
+                    if (o(u) !== "RegExp") throw TypeError("RegExp#exec called on incompatible receiver");
+                    return l.call(u, f)
                 }
             },
-            "159b": function(r, u, t) {
+            "159b": function(r, s, t) {
                 var o = t("da84"),
-                    i = t("fdbc"),
-                    s = t("17c2"),
-                    c = t("9112");
-                for (var f in i) {
-                    var d = o[f],
+                    l = t("fdbc"),
+                    u = t("17c2"),
+                    f = t("9112");
+                for (var c in l) {
+                    var d = o[c],
                         v = d && d.prototype;
-                    if (v && v.forEach !== s) try {
-                        c(v, "forEach", s)
+                    if (v && v.forEach !== u) try {
+                        f(v, "forEach", u)
                     } catch {
-                        v.forEach = s
+                        v.forEach = u
                     }
                 }
             },
-            "17c2": function(r, u, t) {
+            "17c2": function(r, s, t) {
                 var o = t("b727").forEach,
-                    i = t("a640"),
-                    s = t("ae40"),
-                    c = i("forEach"),
-                    f = s("forEach");
-                r.exports = !c || !f ? function(v) {
+                    l = t("a640"),
+                    u = t("ae40"),
+                    f = l("forEach"),
+                    c = u("forEach");
+                r.exports = !f || !c ? function(v) {
                     return o(this, v, arguments.length > 1 ? arguments[1] : void 0)
                 } : [].forEach
             },
-            "1be4": function(r, u, t) {
+            "1be4": function(r, s, t) {
                 var o = t("d066");
                 r.exports = o("document", "documentElement")
             },
-            "1c0b": function(r, u) {
+            "1c0b": function(r, s) {
                 r.exports = function(t) {
                     if (typeof t != "function") throw TypeError(String(t) + " is not a function");
                     return t
                 }
             },
-            "1c7e": function(r, u, t) {
+            "1c7e": function(r, s, t) {
                 var o = t("b622"),
-                    i = o("iterator"),
-                    s = !1;
+                    l = o("iterator"),
+                    u = !1;
                 try {
-                    var c = 0,
-                        f = {
+                    var f = 0,
+                        c = {
                             next: function() {
                                 return {
-                                    done: !!c++
+                                    done: !!f++
                                 }
                             },
                             return: function() {
-                                s = !0
+                                u = !0
                             }
                         };
-                    f[i] = function() {
+                    c[l] = function() {
                         return this
-                    }, Array.from(f, function() {
+                    }, Array.from(c, function() {
                         throw 2
                     })
                 } catch {}
                 r.exports = function(d, v) {
-                    if (!v && !s) return !1;
-                    var h = !1;
+                    if (!v && !u) return !1;
+                    var p = !1;
                     try {
-                        var p = {};
-                        p[i] = function() {
+                        var h = {};
+                        h[l] = function() {
                             return {
                                 next: function() {
                                     return {
-                                        done: h = !0
+                                        done: p = !0
                                     }
                                 }
                             }
-                        }, d(p)
+                        }, d(h)
                     } catch {}
-                    return h
+                    return p
                 }
             },
-            "1d80": function(r, u) {
+            "1d80": function(r, s) {
                 r.exports = function(t) {
                     if (t == null) throw TypeError("Can't call method on " + t);
                     return t
                 }
             },
-            "1dde": function(r, u, t) {
+            "1dde": function(r, s, t) {
                 var o = t("d039"),
-                    i = t("b622"),
-                    s = t("2d00"),
-                    c = i("species");
-                r.exports = function(f) {
-                    return s >= 51 || !o(function() {
+                    l = t("b622"),
+                    u = t("2d00"),
+                    f = l("species");
+                r.exports = function(c) {
+                    return u >= 51 || !o(function() {
                         var d = [],
                             v = d.constructor = {};
-                        return v[c] = function() {
+                        return v[f] = function() {
                             return {
                                 foo: 1
                             }
-                        }, d[f](Boolean).foo !== 1
+                        }, d[c](Boolean).foo !== 1
                     })
                 }
             },
-            "23cb": function(r, u, t) {
+            "23cb": function(r, s, t) {
                 var o = t("a691"),
-                    i = Math.max,
-                    s = Math.min;
-                r.exports = function(c, f) {
-                    var d = o(c);
-                    return d < 0 ? i(d + f, 0) : s(d, f)
+                    l = Math.max,
+                    u = Math.min;
+                r.exports = function(f, c) {
+                    var d = o(f);
+                    return d < 0 ? l(d + c, 0) : u(d, c)
                 }
             },
-            "23e7": function(r, u, t) {
+            "23e7": function(r, s, t) {
                 var o = t("da84"),
-                    i = t("06cf").f,
-                    s = t("9112"),
-                    c = t("6eeb"),
-                    f = t("ce4e"),
+                    l = t("06cf").f,
+                    u = t("9112"),
+                    f = t("6eeb"),
+                    c = t("ce4e"),
                     d = t("e893"),
                     v = t("94ca");
-                r.exports = function(h, p) {
-                    var g = h.target,
-                        b = h.global,
-                        S = h.stat,
-                        P, x, C, I, j, L;
-                    if (b ? x = o : S ? x = o[g] || f(g, {}) : x = (o[g] || {}).prototype, x)
-                        for (C in p) {
-                            if (j = p[C], h.noTargetGet ? (L = i(x, C), I = L && L.value) : I = x[C], P = v(b ? C : g + (S ? "." : "#") + C, h.forced), !P && I !== void 0) {
-                                if (typeof j == typeof I) continue;
-                                d(j, I)
-                            }(h.sham || I && I.sham) && s(j, "sham", !0), c(x, C, j, h)
+                r.exports = function(p, h) {
+                    var m = p.target,
+                        g = p.global,
+                        y = p.stat,
+                        O, E, C, T, $, L;
+                    if (g ? E = o : y ? E = o[m] || c(m, {}) : E = (o[m] || {}).prototype, E)
+                        for (C in h) {
+                            if ($ = h[C], p.noTargetGet ? (L = l(E, C), T = L && L.value) : T = E[C], O = v(g ? C : m + (y ? "." : "#") + C, p.forced), !O && T !== void 0) {
+                                if (typeof $ == typeof T) continue;
+                                d($, T)
+                            }(p.sham || T && T.sham) && u($, "sham", !0), f(E, C, $, p)
                         }
                 }
             },
-            "241c": function(r, u, t) {
+            "241c": function(r, s, t) {
                 var o = t("ca84"),
-                    i = t("7839"),
-                    s = i.concat("length", "prototype");
-                u.f = Object.getOwnPropertyNames || function(f) {
-                    return o(f, s)
+                    l = t("7839"),
+                    u = l.concat("length", "prototype");
+                s.f = Object.getOwnPropertyNames || function(c) {
+                    return o(c, u)
                 }
             },
-            "25f0": function(r, u, t) {
+            "25f0": function(r, s, t) {
                 var o = t("6eeb"),
-                    i = t("825a"),
-                    s = t("d039"),
-                    c = t("ad6d"),
-                    f = "toString",
+                    l = t("825a"),
+                    u = t("d039"),
+                    f = t("ad6d"),
+                    c = "toString",
                     d = RegExp.prototype,
-                    v = d[f],
-                    h = s(function() {
+                    v = d[c],
+                    p = u(function() {
                         return v.call({
                             source: "a",
                             flags: "b"
                         }) != "/a/b"
                     }),
-                    p = v.name != f;
-                (h || p) && o(RegExp.prototype, f, function() {
-                    var b = i(this),
-                        S = String(b.source),
-                        P = b.flags,
-                        x = String(P === void 0 && b instanceof RegExp && !("flags" in d) ? c.call(b) : P);
-                    return "/" + S + "/" + x
+                    h = v.name != c;
+                (p || h) && o(RegExp.prototype, c, function() {
+                    var g = l(this),
+                        y = String(g.source),
+                        O = g.flags,
+                        E = String(O === void 0 && g instanceof RegExp && !("flags" in d) ? f.call(g) : O);
+                    return "/" + y + "/" + E
                 }, {
                     unsafe: !0
                 })
             },
-            "2ca0": function(r, u, t) {
+            "2ca0": function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("06cf").f,
-                    s = t("50c4"),
-                    c = t("5a34"),
-                    f = t("1d80"),
+                    l = t("06cf").f,
+                    u = t("50c4"),
+                    f = t("5a34"),
+                    c = t("1d80"),
                     d = t("ab13"),
                     v = t("c430"),
-                    h = "".startsWith,
-                    p = Math.min,
-                    g = d("startsWith"),
-                    b = !v && !g && !! function() {
-                        var S = i(String.prototype, "startsWith");
-                        return S && !S.writable
+                    p = "".startsWith,
+                    h = Math.min,
+                    m = d("startsWith"),
+                    g = !v && !m && !! function() {
+                        var y = l(String.prototype, "startsWith");
+                        return y && !y.writable
                     }();
                 o({
                     target: "String",
                     proto: !0,
-                    forced: !b && !g
+                    forced: !g && !m
                 }, {
-                    startsWith: function(P) {
-                        var x = String(f(this));
-                        c(P);
-                        var C = s(p(arguments.length > 1 ? arguments[1] : void 0, x.length)),
-                            I = String(P);
-                        return h ? h.call(x, I, C) : x.slice(C, C + I.length) === I
+                    startsWith: function(O) {
+                        var E = String(c(this));
+                        f(O);
+                        var C = u(h(arguments.length > 1 ? arguments[1] : void 0, E.length)),
+                            T = String(O);
+                        return p ? p.call(E, T, C) : E.slice(C, C + T.length) === T
                     }
                 })
             },
-            "2d00": function(r, u, t) {
+            "2d00": function(r, s, t) {
                 var o = t("da84"),
-                    i = t("342f"),
-                    s = o.process,
-                    c = s && s.versions,
-                    f = c && c.v8,
+                    l = t("342f"),
+                    u = o.process,
+                    f = u && u.versions,
+                    c = f && f.v8,
                     d, v;
-                f ? (d = f.split("."), v = d[0] + d[1]) : i && (d = i.match(/Edge\/(\d+)/), (!d || d[1] >= 74) && (d = i.match(/Chrome\/(\d+)/), d && (v = d[1]))), r.exports = v && +v
+                c ? (d = c.split("."), v = d[0] + d[1]) : l && (d = l.match(/Edge\/(\d+)/), (!d || d[1] >= 74) && (d = l.match(/Chrome\/(\d+)/), d && (v = d[1]))), r.exports = v && +v
             },
-            "342f": function(r, u, t) {
+            "342f": function(r, s, t) {
                 var o = t("d066");
                 r.exports = o("navigator", "userAgent") || ""
             },
-            "35a1": function(r, u, t) {
+            "35a1": function(r, s, t) {
                 var o = t("f5df"),
-                    i = t("3f8c"),
-                    s = t("b622"),
-                    c = s("iterator");
-                r.exports = function(f) {
-                    if (f != null) return f[c] || f["@@iterator"] || i[o(f)]
+                    l = t("3f8c"),
+                    u = t("b622"),
+                    f = u("iterator");
+                r.exports = function(c) {
+                    if (c != null) return c[f] || c["@@iterator"] || l[o(c)]
                 }
             },
-            "37e8": function(r, u, t) {
+            "37e8": function(r, s, t) {
                 var o = t("83ab"),
-                    i = t("9bf2"),
-                    s = t("825a"),
-                    c = t("df75");
+                    l = t("9bf2"),
+                    u = t("825a"),
+                    f = t("df75");
                 r.exports = o ? Object.defineProperties : function(d, v) {
-                    s(d);
-                    for (var h = c(v), p = h.length, g = 0, b; p > g;) i.f(d, b = h[g++], v[b]);
+                    u(d);
+                    for (var p = f(v), h = p.length, m = 0, g; h > m;) l.f(d, g = p[m++], v[g]);
                     return d
                 }
             },
-            "3bbe": function(r, u, t) {
+            "3bbe": function(r, s, t) {
                 var o = t("861d");
-                r.exports = function(i) {
-                    if (!o(i) && i !== null) throw TypeError("Can't set " + String(i) + " as a prototype");
-                    return i
+                r.exports = function(l) {
+                    if (!o(l) && l !== null) throw TypeError("Can't set " + String(l) + " as a prototype");
+                    return l
                 }
             },
-            "3ca3": function(r, u, t) {
+            "3ca3": function(r, s, t) {
                 var o = t("6547").charAt,
-                    i = t("69f3"),
-                    s = t("7dd0"),
-                    c = "String Iterator",
-                    f = i.set,
-                    d = i.getterFor(c);
-                s(String, "String", function(v) {
-                    f(this, {
-                        type: c,
+                    l = t("69f3"),
+                    u = t("7dd0"),
+                    f = "String Iterator",
+                    c = l.set,
+                    d = l.getterFor(f);
+                u(String, "String", function(v) {
+                    c(this, {
+                        type: f,
                         string: String(v),
                         index: 0
                     })
                 }, function() {
-                    var h = d(this),
-                        p = h.string,
-                        g = h.index,
-                        b;
-                    return g >= p.length ? {
+                    var p = d(this),
+                        h = p.string,
+                        m = p.index,
+                        g;
+                    return m >= h.length ? {
                         value: void 0,
                         done: !0
-                    } : (b = o(p, g), h.index += b.length, {
-                        value: b,
+                    } : (g = o(h, m), p.index += g.length, {
+                        value: g,
                         done: !1
                     })
                 })
             },
-            "3f8c": function(r, u) {
+            "3f8c": function(r, s) {
                 r.exports = {}
             },
-            4160: function(r, u, t) {
+            4160: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("17c2");
+                    l = t("17c2");
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: [].forEach != i
+                    forced: [].forEach != l
                 }, {
-                    forEach: i
+                    forEach: l
                 })
             },
-            "428f": function(r, u, t) {
+            "428f": function(r, s, t) {
                 var o = t("da84");
                 r.exports = o
             },
-            "44ad": function(r, u, t) {
+            "44ad": function(r, s, t) {
                 var o = t("d039"),
-                    i = t("c6b6"),
-                    s = "".split;
+                    l = t("c6b6"),
+                    u = "".split;
                 r.exports = o(function() {
                     return !Object("z").propertyIsEnumerable(0)
-                }) ? function(c) {
-                    return i(c) == "String" ? s.call(c, "") : Object(c)
+                }) ? function(f) {
+                    return l(f) == "String" ? u.call(f, "") : Object(f)
                 } : Object
             },
-            "44d2": function(r, u, t) {
+            "44d2": function(r, s, t) {
                 var o = t("b622"),
-                    i = t("7c73"),
-                    s = t("9bf2"),
-                    c = o("unscopables"),
-                    f = Array.prototype;
-                f[c] == null && s.f(f, c, {
+                    l = t("7c73"),
+                    u = t("9bf2"),
+                    f = o("unscopables"),
+                    c = Array.prototype;
+                c[f] == null && u.f(c, f, {
                     configurable: !0,
-                    value: i(null)
+                    value: l(null)
                 }), r.exports = function(d) {
-                    f[c][d] = !0
+                    c[f][d] = !0
                 }
             },
-            "44e7": function(r, u, t) {
+            "44e7": function(r, s, t) {
                 var o = t("861d"),
-                    i = t("c6b6"),
-                    s = t("b622"),
-                    c = s("match");
-                r.exports = function(f) {
+                    l = t("c6b6"),
+                    u = t("b622"),
+                    f = u("match");
+                r.exports = function(c) {
                     var d;
-                    return o(f) && ((d = f[c]) !== void 0 ? !!d : i(f) == "RegExp")
+                    return o(c) && ((d = c[f]) !== void 0 ? !!d : l(c) == "RegExp")
                 }
             },
-            4930: function(r, u, t) {
+            4930: function(r, s, t) {
                 var o = t("d039");
                 r.exports = !!Object.getOwnPropertySymbols && !o(function() {
                     return !String(Symbol())
                 })
             },
-            "4d64": function(r, u, t) {
+            "4d64": function(r, s, t) {
                 var o = t("fc6a"),
-                    i = t("50c4"),
-                    s = t("23cb"),
-                    c = function(f) {
-                        return function(d, v, h) {
-                            var p = o(d),
-                                g = i(p.length),
-                                b = s(h, g),
-                                S;
-                            if (f && v != v) {
-                                for (; g > b;)
-                                    if (S = p[b++], S != S) return !0
+                    l = t("50c4"),
+                    u = t("23cb"),
+                    f = function(c) {
+                        return function(d, v, p) {
+                            var h = o(d),
+                                m = l(h.length),
+                                g = u(p, m),
+                                y;
+                            if (c && v != v) {
+                                for (; m > g;)
+                                    if (y = h[g++], y != y) return !0
                             } else
-                                for (; g > b; b++)
-                                    if ((f || b in p) && p[b] === v) return f || b || 0;
-                            return !f && -1
+                                for (; m > g; g++)
+                                    if ((c || g in h) && h[g] === v) return c || g || 0;
+                            return !c && -1
                         }
                     };
                 r.exports = {
-                    includes: c(!0),
-                    indexOf: c(!1)
+                    includes: f(!0),
+                    indexOf: f(!1)
                 }
             },
-            "4de4": function(r, u, t) {
+            "4de4": function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("b727").filter,
-                    s = t("1dde"),
-                    c = t("ae40"),
-                    f = s("filter"),
-                    d = c("filter");
+                    l = t("b727").filter,
+                    u = t("1dde"),
+                    f = t("ae40"),
+                    c = u("filter"),
+                    d = f("filter");
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: !f || !d
+                    forced: !c || !d
                 }, {
-                    filter: function(h) {
-                        return i(this, h, arguments.length > 1 ? arguments[1] : void 0)
+                    filter: function(p) {
+                        return l(this, p, arguments.length > 1 ? arguments[1] : void 0)
                     }
                 })
             },
-            "4df4": function(r, u, t) {
+            "4df4": function(r, s, t) {
                 var o = t("0366"),
-                    i = t("7b0b"),
-                    s = t("9bdd"),
-                    c = t("e95a"),
-                    f = t("50c4"),
+                    l = t("7b0b"),
+                    u = t("9bdd"),
+                    f = t("e95a"),
+                    c = t("50c4"),
                     d = t("8418"),
                     v = t("35a1");
-                r.exports = function(p) {
-                    var g = i(p),
-                        b = typeof this == "function" ? this : Array,
-                        S = arguments.length,
-                        P = S > 1 ? arguments[1] : void 0,
-                        x = P !== void 0,
-                        C = v(g),
-                        I = 0,
-                        j, L, T, O, D, G;
-                    if (x && (P = o(P, S > 2 ? arguments[2] : void 0, 2)), C != null && !(b == Array && c(C)))
-                        for (O = C.call(g), D = O.next, L = new b; !(T = D.call(O)).done; I++) G = x ? s(O, P, [T.value, I], !0) : T.value, d(L, I, G);
+                r.exports = function(h) {
+                    var m = l(h),
+                        g = typeof this == "function" ? this : Array,
+                        y = arguments.length,
+                        O = y > 1 ? arguments[1] : void 0,
+                        E = O !== void 0,
+                        C = v(m),
+                        T = 0,
+                        $, L, I, j, P, M;
+                    if (E && (O = o(O, y > 2 ? arguments[2] : void 0, 2)), C != null && !(g == Array && f(C)))
+                        for (j = C.call(m), P = j.next, L = new g; !(I = P.call(j)).done; T++) M = E ? u(j, O, [I.value, T], !0) : I.value, d(L, T, M);
                     else
-                        for (j = f(g.length), L = new b(j); j > I; I++) G = x ? P(g[I], I) : g[I], d(L, I, G);
-                    return L.length = I, L
+                        for ($ = c(m.length), L = new g($); $ > T; T++) M = E ? O(m[T], T) : m[T], d(L, T, M);
+                    return L.length = T, L
                 }
             },
-            "4fad": function(r, u, t) {
+            "4fad": function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("6f53").entries;
+                    l = t("6f53").entries;
                 o({
                     target: "Object",
                     stat: !0
                 }, {
-                    entries: function(c) {
-                        return i(c)
+                    entries: function(f) {
+                        return l(f)
                     }
                 })
             },
-            "50c4": function(r, u, t) {
+            "50c4": function(r, s, t) {
                 var o = t("a691"),
-                    i = Math.min;
-                r.exports = function(s) {
-                    return s > 0 ? i(o(s), 9007199254740991) : 0
+                    l = Math.min;
+                r.exports = function(u) {
+                    return u > 0 ? l(o(u), 9007199254740991) : 0
                 }
             },
-            5135: function(r, u) {
+            5135: function(r, s) {
                 var t = {}.hasOwnProperty;
-                r.exports = function(o, i) {
-                    return t.call(o, i)
+                r.exports = function(o, l) {
+                    return t.call(o, l)
                 }
             },
-            5319: function(r, u, t) {
+            5319: function(r, s, t) {
                 var o = t("d784"),
-                    i = t("825a"),
-                    s = t("7b0b"),
-                    c = t("50c4"),
-                    f = t("a691"),
+                    l = t("825a"),
+                    u = t("7b0b"),
+                    f = t("50c4"),
+                    c = t("a691"),
                     d = t("1d80"),
                     v = t("8aa5"),
-                    h = t("14c3"),
-                    p = Math.max,
-                    g = Math.min,
-                    b = Math.floor,
-                    S = /\$([$&'`]|\d\d?|<[^>]*>)/g,
-                    P = /\$([$&'`]|\d\d?)/g,
-                    x = function(C) {
+                    p = t("14c3"),
+                    h = Math.max,
+                    m = Math.min,
+                    g = Math.floor,
+                    y = /\$([$&'`]|\d\d?|<[^>]*>)/g,
+                    O = /\$([$&'`]|\d\d?)/g,
+                    E = function(C) {
                         return C === void 0 ? C : String(C)
                     };
-                o("replace", 2, function(C, I, j, L) {
-                    var T = L.REGEXP_REPLACE_SUBSTITUTES_UNDEFINED_CAPTURE,
-                        O = L.REPLACE_KEEPS_$0,
-                        D = T ? "$" : "$0";
-                    return [function(M, X) {
-                        var R = d(this),
-                            F = M == null ? void 0 : M[C];
-                        return F !== void 0 ? F.call(M, R, X) : I.call(String(R), M, X)
-                    }, function(A, M) {
-                        if (!T && O || typeof M == "string" && M.indexOf(D) === -1) {
-                            var X = j(I, A, this, M);
-                            if (X.done) return X.value
+                o("replace", 2, function(C, T, $, L) {
+                    var I = L.REGEXP_REPLACE_SUBSTITUTES_UNDEFINED_CAPTURE,
+                        j = L.REPLACE_KEEPS_$0,
+                        P = I ? "$" : "$0";
+                    return [function(R, H) {
+                        var F = d(this),
+                            N = R == null ? void 0 : R[C];
+                        return N !== void 0 ? N.call(R, F, H) : T.call(String(F), R, H)
+                    }, function(D, R) {
+                        if (!I && j || typeof R == "string" && R.indexOf(P) === -1) {
+                            var H = $(T, D, this, R);
+                            if (H.done) return H.value
                         }
-                        var R = i(A),
-                            F = String(this),
-                            _ = typeof M == "function";
-                        _ || (M = String(M));
-                        var at = R.global;
-                        if (at) {
-                            var xt = R.unicode;
-                            R.lastIndex = 0
+                        var F = l(D),
+                            N = String(this),
+                            k = typeof R == "function";
+                        k || (R = String(R));
+                        var ot = F.global;
+                        if (ot) {
+                            var St = F.unicode;
+                            F.lastIndex = 0
                         }
-                        for (var vt = [];;) {
-                            var ht = h(R, F);
-                            if (ht === null || (vt.push(ht), !at)) break;
-                            var Et = String(ht[0]);
-                            Et === "" && (R.lastIndex = v(F, c(R.lastIndex), xt))
+                        for (var ct = [];;) {
+                            var pt = p(F, N);
+                            if (pt === null || (ct.push(pt), !ot)) break;
+                            var Ot = String(pt[0]);
+                            Ot === "" && (F.lastIndex = v(N, f(F.lastIndex), St))
                         }
-                        for (var Ot = "", bt = 0, lt = 0; lt < vt.length; lt++) {
-                            ht = vt[lt];
-                            for (var ct = String(ht[0]), Lt = p(g(f(ht.index), F.length), 0), Rt = [], _t = 1; _t < ht.length; _t++) Rt.push(x(ht[_t]));
-                            var ue = ht.groups;
-                            if (_) {
-                                var oe = [ct].concat(Rt, Lt, F);
-                                ue !== void 0 && oe.push(ue);
-                                var Tt = String(M.apply(void 0, oe))
-                            } else Tt = G(ct, F, Lt, Rt, ue, M);
-                            Lt >= bt && (Ot += F.slice(bt, Lt) + Tt, bt = Lt + ct.length)
+                        for (var It = "", Et = 0, st = 0; st < ct.length; st++) {
+                            pt = ct[st];
+                            for (var dt = String(pt[0]), Lt = h(m(c(pt.index), N.length), 0), wt = [], re = 1; re < pt.length; re++) wt.push(E(pt[re]));
+                            var de = pt.groups;
+                            if (k) {
+                                var ie = [dt].concat(wt, Lt, N);
+                                de !== void 0 && ie.push(de);
+                                var Pt = String(R.apply(void 0, ie))
+                            } else Pt = M(dt, N, Lt, wt, de, R);
+                            Lt >= Et && (It += N.slice(Et, Lt) + Pt, Et = Lt + dt.length)
                         }
-                        return Ot + F.slice(bt)
+                        return It + N.slice(Et)
                     }];
 
-                    function G(A, M, X, R, F, _) {
-                        var at = X + A.length,
-                            xt = R.length,
-                            vt = P;
-                        return F !== void 0 && (F = s(F), vt = S), I.call(_, vt, function(ht, Et) {
-                            var Ot;
-                            switch (Et.charAt(0)) {
+                    function M(D, R, H, F, N, k) {
+                        var ot = H + D.length,
+                            St = F.length,
+                            ct = O;
+                        return N !== void 0 && (N = u(N), ct = y), T.call(k, ct, function(pt, Ot) {
+                            var It;
+                            switch (Ot.charAt(0)) {
                                 case "$":
                                     return "$";
                                 case "&":
-                                    return A;
+                                    return D;
                                 case "`":
-                                    return M.slice(0, X);
+                                    return R.slice(0, H);
                                 case "'":
-                                    return M.slice(at);
+                                    return R.slice(ot);
                                 case "<":
-                                    Ot = F[Et.slice(1, -1)];
+                                    It = N[Ot.slice(1, -1)];
                                     break;
                                 default:
-                                    var bt = +Et;
-                                    if (bt === 0) return ht;
-                                    if (bt > xt) {
-                                        var lt = b(bt / 10);
-                                        return lt === 0 ? ht : lt <= xt ? R[lt - 1] === void 0 ? Et.charAt(1) : R[lt - 1] + Et.charAt(1) : ht
+                                    var Et = +Ot;
+                                    if (Et === 0) return pt;
+                                    if (Et > St) {
+                                        var st = g(Et / 10);
+                                        return st === 0 ? pt : st <= St ? F[st - 1] === void 0 ? Ot.charAt(1) : F[st - 1] + Ot.charAt(1) : pt
                                     }
-                                    Ot = R[bt - 1]
+                                    It = F[Et - 1]
                             }
-                            return Ot === void 0 ? "" : Ot
+                            return It === void 0 ? "" : It
                         })
                     }
                 })
             },
-            5692: function(r, u, t) {
+            5692: function(r, s, t) {
                 var o = t("c430"),
-                    i = t("c6cd");
-                (r.exports = function(s, c) {
-                    return i[s] || (i[s] = c !== void 0 ? c : {})
+                    l = t("c6cd");
+                (r.exports = function(u, f) {
+                    return l[u] || (l[u] = f !== void 0 ? f : {})
                 })("versions", []).push({
                     version: "3.6.5",
                     mode: o ? "pure" : "global",
                     copyright: "\xA9 2020 Denis Pushkarev (zloirock.ru)"
                 })
             },
-            "56ef": function(r, u, t) {
+            "56ef": function(r, s, t) {
                 var o = t("d066"),
-                    i = t("241c"),
-                    s = t("7418"),
-                    c = t("825a");
+                    l = t("241c"),
+                    u = t("7418"),
+                    f = t("825a");
                 r.exports = o("Reflect", "ownKeys") || function(d) {
-                    var v = i.f(c(d)),
-                        h = s.f;
-                    return h ? v.concat(h(d)) : v
+                    var v = l.f(f(d)),
+                        p = u.f;
+                    return p ? v.concat(p(d)) : v
                 }
             },
-            "5a34": function(r, u, t) {
+            "5a34": function(r, s, t) {
                 var o = t("44e7");
-                r.exports = function(i) {
-                    if (o(i)) throw TypeError("The method doesn't accept regular expressions");
-                    return i
+                r.exports = function(l) {
+                    if (o(l)) throw TypeError("The method doesn't accept regular expressions");
+                    return l
                 }
             },
-            "5c6c": function(r, u) {
+            "5c6c": function(r, s) {
                 r.exports = function(t, o) {
                     return {
                         enumerable: !(t & 1),
                         configurable: !(t & 2),
                         writable: !(t & 4),
                         value: o
                     }
                 }
             },
-            "5db7": function(r, u, t) {
+            "5db7": function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("a2bf"),
-                    s = t("7b0b"),
-                    c = t("50c4"),
-                    f = t("1c0b"),
+                    l = t("a2bf"),
+                    u = t("7b0b"),
+                    f = t("50c4"),
+                    c = t("1c0b"),
                     d = t("65f0");
                 o({
                     target: "Array",
                     proto: !0
                 }, {
-                    flatMap: function(h) {
-                        var p = s(this),
-                            g = c(p.length),
-                            b;
-                        return f(h), b = d(p, 0), b.length = i(b, p, p, g, 0, 1, h, arguments.length > 1 ? arguments[1] : void 0), b
+                    flatMap: function(p) {
+                        var h = u(this),
+                            m = f(h.length),
+                            g;
+                        return c(p), g = d(h, 0), g.length = l(g, h, h, m, 0, 1, p, arguments.length > 1 ? arguments[1] : void 0), g
                     }
                 })
             },
-            6547: function(r, u, t) {
+            6547: function(r, s, t) {
                 var o = t("a691"),
-                    i = t("1d80"),
-                    s = function(c) {
-                        return function(f, d) {
-                            var v = String(i(f)),
-                                h = o(d),
-                                p = v.length,
-                                g, b;
-                            return h < 0 || h >= p ? c ? "" : void 0 : (g = v.charCodeAt(h), g < 55296 || g > 56319 || h + 1 === p || (b = v.charCodeAt(h + 1)) < 56320 || b > 57343 ? c ? v.charAt(h) : g : c ? v.slice(h, h + 2) : (g - 55296 << 10) + (b - 56320) + 65536)
+                    l = t("1d80"),
+                    u = function(f) {
+                        return function(c, d) {
+                            var v = String(l(c)),
+                                p = o(d),
+                                h = v.length,
+                                m, g;
+                            return p < 0 || p >= h ? f ? "" : void 0 : (m = v.charCodeAt(p), m < 55296 || m > 56319 || p + 1 === h || (g = v.charCodeAt(p + 1)) < 56320 || g > 57343 ? f ? v.charAt(p) : m : f ? v.slice(p, p + 2) : (m - 55296 << 10) + (g - 56320) + 65536)
                         }
                     };
                 r.exports = {
-                    codeAt: s(!1),
-                    charAt: s(!0)
+                    codeAt: u(!1),
+                    charAt: u(!0)
                 }
             },
-            "65f0": function(r, u, t) {
+            "65f0": function(r, s, t) {
                 var o = t("861d"),
-                    i = t("e8b5"),
-                    s = t("b622"),
-                    c = s("species");
-                r.exports = function(f, d) {
+                    l = t("e8b5"),
+                    u = t("b622"),
+                    f = u("species");
+                r.exports = function(c, d) {
                     var v;
-                    return i(f) && (v = f.constructor, typeof v == "function" && (v === Array || i(v.prototype)) ? v = void 0 : o(v) && (v = v[c], v === null && (v = void 0))), new(v === void 0 ? Array : v)(d === 0 ? 0 : d)
+                    return l(c) && (v = c.constructor, typeof v == "function" && (v === Array || l(v.prototype)) ? v = void 0 : o(v) && (v = v[f], v === null && (v = void 0))), new(v === void 0 ? Array : v)(d === 0 ? 0 : d)
                 }
             },
-            "69f3": function(r, u, t) {
+            "69f3": function(r, s, t) {
                 var o = t("7f9a"),
-                    i = t("da84"),
-                    s = t("861d"),
-                    c = t("9112"),
-                    f = t("5135"),
+                    l = t("da84"),
+                    u = t("861d"),
+                    f = t("9112"),
+                    c = t("5135"),
                     d = t("f772"),
                     v = t("d012"),
-                    h = i.WeakMap,
-                    p, g, b, S = function(T) {
-                        return b(T) ? g(T) : p(T, {})
+                    p = l.WeakMap,
+                    h, m, g, y = function(I) {
+                        return g(I) ? m(I) : h(I, {})
                     },
-                    P = function(T) {
-                        return function(O) {
-                            var D;
-                            if (!s(O) || (D = g(O)).type !== T) throw TypeError("Incompatible receiver, " + T + " required");
-                            return D
+                    O = function(I) {
+                        return function(j) {
+                            var P;
+                            if (!u(j) || (P = m(j)).type !== I) throw TypeError("Incompatible receiver, " + I + " required");
+                            return P
                         }
                     };
                 if (o) {
-                    var x = new h,
-                        C = x.get,
-                        I = x.has,
-                        j = x.set;
-                    p = function(T, O) {
-                        return j.call(x, T, O), O
-                    }, g = function(T) {
-                        return C.call(x, T) || {}
-                    }, b = function(T) {
-                        return I.call(x, T)
+                    var E = new p,
+                        C = E.get,
+                        T = E.has,
+                        $ = E.set;
+                    h = function(I, j) {
+                        return $.call(E, I, j), j
+                    }, m = function(I) {
+                        return C.call(E, I) || {}
+                    }, g = function(I) {
+                        return T.call(E, I)
                     }
                 } else {
                     var L = d("state");
-                    v[L] = !0, p = function(T, O) {
-                        return c(T, L, O), O
-                    }, g = function(T) {
-                        return f(T, L) ? T[L] : {}
-                    }, b = function(T) {
-                        return f(T, L)
+                    v[L] = !0, h = function(I, j) {
+                        return f(I, L, j), j
+                    }, m = function(I) {
+                        return c(I, L) ? I[L] : {}
+                    }, g = function(I) {
+                        return c(I, L)
                     }
                 }
                 r.exports = {
-                    set: p,
-                    get: g,
-                    has: b,
-                    enforce: S,
-                    getterFor: P
+                    set: h,
+                    get: m,
+                    has: g,
+                    enforce: y,
+                    getterFor: O
                 }
             },
-            "6eeb": function(r, u, t) {
+            "6eeb": function(r, s, t) {
                 var o = t("da84"),
-                    i = t("9112"),
-                    s = t("5135"),
-                    c = t("ce4e"),
-                    f = t("8925"),
+                    l = t("9112"),
+                    u = t("5135"),
+                    f = t("ce4e"),
+                    c = t("8925"),
                     d = t("69f3"),
                     v = d.get,
-                    h = d.enforce,
-                    p = String(String).split("String");
-                (r.exports = function(g, b, S, P) {
-                    var x = P ? !!P.unsafe : !1,
-                        C = P ? !!P.enumerable : !1,
-                        I = P ? !!P.noTargetGet : !1;
-                    if (typeof S == "function" && (typeof b == "string" && !s(S, "name") && i(S, "name", b), h(S).source = p.join(typeof b == "string" ? b : "")), g === o) {
-                        C ? g[b] = S : c(b, S);
+                    p = d.enforce,
+                    h = String(String).split("String");
+                (r.exports = function(m, g, y, O) {
+                    var E = O ? !!O.unsafe : !1,
+                        C = O ? !!O.enumerable : !1,
+                        T = O ? !!O.noTargetGet : !1;
+                    if (typeof y == "function" && (typeof g == "string" && !u(y, "name") && l(y, "name", g), p(y).source = h.join(typeof g == "string" ? g : "")), m === o) {
+                        C ? m[g] = y : f(g, y);
                         return
-                    } else x ? !I && g[b] && (C = !0) : delete g[b];
-                    C ? g[b] = S : i(g, b, S)
+                    } else E ? !T && m[g] && (C = !0) : delete m[g];
+                    C ? m[g] = y : l(m, g, y)
                 })(Function.prototype, "toString", function() {
-                    return typeof this == "function" && v(this).source || f(this)
+                    return typeof this == "function" && v(this).source || c(this)
                 })
             },
-            "6f53": function(r, u, t) {
+            "6f53": function(r, s, t) {
                 var o = t("83ab"),
-                    i = t("df75"),
-                    s = t("fc6a"),
-                    c = t("d1e7").f,
-                    f = function(d) {
+                    l = t("df75"),
+                    u = t("fc6a"),
+                    f = t("d1e7").f,
+                    c = function(d) {
                         return function(v) {
-                            for (var h = s(v), p = i(h), g = p.length, b = 0, S = [], P; g > b;) P = p[b++], (!o || c.call(h, P)) && S.push(d ? [P, h[P]] : h[P]);
-                            return S
+                            for (var p = u(v), h = l(p), m = h.length, g = 0, y = [], O; m > g;) O = h[g++], (!o || f.call(p, O)) && y.push(d ? [O, p[O]] : p[O]);
+                            return y
                         }
                     };
                 r.exports = {
-                    entries: f(!0),
-                    values: f(!1)
+                    entries: c(!0),
+                    values: c(!1)
                 }
             },
-            "73d9": function(r, u, t) {
+            "73d9": function(r, s, t) {
                 var o = t("44d2");
                 o("flatMap")
             },
-            7418: function(r, u) {
-                u.f = Object.getOwnPropertySymbols
+            7418: function(r, s) {
+                s.f = Object.getOwnPropertySymbols
             },
-            "746f": function(r, u, t) {
+            "746f": function(r, s, t) {
                 var o = t("428f"),
-                    i = t("5135"),
-                    s = t("e538"),
-                    c = t("9bf2").f;
-                r.exports = function(f) {
+                    l = t("5135"),
+                    u = t("e538"),
+                    f = t("9bf2").f;
+                r.exports = function(c) {
                     var d = o.Symbol || (o.Symbol = {});
-                    i(d, f) || c(d, f, {
-                        value: s.f(f)
+                    l(d, c) || f(d, c, {
+                        value: u.f(c)
                     })
                 }
             },
-            7839: function(r, u) {
+            7839: function(r, s) {
                 r.exports = ["constructor", "hasOwnProperty", "isPrototypeOf", "propertyIsEnumerable", "toLocaleString", "toString", "valueOf"]
             },
-            "7b0b": function(r, u, t) {
+            "7b0b": function(r, s, t) {
                 var o = t("1d80");
-                r.exports = function(i) {
-                    return Object(o(i))
+                r.exports = function(l) {
+                    return Object(o(l))
                 }
             },
-            "7c73": function(r, u, t) {
+            "7c73": function(r, s, t) {
                 var o = t("825a"),
-                    i = t("37e8"),
-                    s = t("7839"),
-                    c = t("d012"),
-                    f = t("1be4"),
+                    l = t("37e8"),
+                    u = t("7839"),
+                    f = t("d012"),
+                    c = t("1be4"),
                     d = t("cc12"),
                     v = t("f772"),
-                    h = ">",
-                    p = "<",
-                    g = "prototype",
-                    b = "script",
-                    S = v("IE_PROTO"),
-                    P = function() {},
-                    x = function(T) {
-                        return p + b + h + T + p + "/" + b + h
+                    p = ">",
+                    h = "<",
+                    m = "prototype",
+                    g = "script",
+                    y = v("IE_PROTO"),
+                    O = function() {},
+                    E = function(I) {
+                        return h + g + p + I + h + "/" + g + p
                     },
-                    C = function(T) {
-                        T.write(x("")), T.close();
-                        var O = T.parentWindow.Object;
-                        return T = null, O
+                    C = function(I) {
+                        I.write(E("")), I.close();
+                        var j = I.parentWindow.Object;
+                        return I = null, j
                     },
-                    I = function() {
-                        var T = d("iframe"),
-                            O = "java" + b + ":",
-                            D;
-                        return T.style.display = "none", f.appendChild(T), T.src = String(O), D = T.contentWindow.document, D.open(), D.write(x("document.F=Object")), D.close(), D.F
+                    T = function() {
+                        var I = d("iframe"),
+                            j = "java" + g + ":",
+                            P;
+                        return I.style.display = "none", c.appendChild(I), I.src = String(j), P = I.contentWindow.document, P.open(), P.write(E("document.F=Object")), P.close(), P.F
                     },
-                    j, L = function() {
+                    $, L = function() {
                         try {
-                            j = document.domain && new ActiveXObject("htmlfile")
+                            $ = document.domain && new ActiveXObject("htmlfile")
                         } catch {}
-                        L = j ? C(j) : I();
-                        for (var T = s.length; T--;) delete L[g][s[T]];
+                        L = $ ? C($) : T();
+                        for (var I = u.length; I--;) delete L[m][u[I]];
                         return L()
                     };
-                c[S] = !0, r.exports = Object.create || function(O, D) {
-                    var G;
-                    return O !== null ? (P[g] = o(O), G = new P, P[g] = null, G[S] = O) : G = L(), D === void 0 ? G : i(G, D)
+                f[y] = !0, r.exports = Object.create || function(j, P) {
+                    var M;
+                    return j !== null ? (O[m] = o(j), M = new O, O[m] = null, M[y] = j) : M = L(), P === void 0 ? M : l(M, P)
                 }
             },
-            "7dd0": function(r, u, t) {
+            "7dd0": function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("9ed3"),
-                    s = t("e163"),
-                    c = t("d2bb"),
-                    f = t("d44e"),
+                    l = t("9ed3"),
+                    u = t("e163"),
+                    f = t("d2bb"),
+                    c = t("d44e"),
                     d = t("9112"),
                     v = t("6eeb"),
-                    h = t("b622"),
-                    p = t("c430"),
-                    g = t("3f8c"),
-                    b = t("ae93"),
-                    S = b.IteratorPrototype,
-                    P = b.BUGGY_SAFARI_ITERATORS,
-                    x = h("iterator"),
+                    p = t("b622"),
+                    h = t("c430"),
+                    m = t("3f8c"),
+                    g = t("ae93"),
+                    y = g.IteratorPrototype,
+                    O = g.BUGGY_SAFARI_ITERATORS,
+                    E = p("iterator"),
                     C = "keys",
-                    I = "values",
-                    j = "entries",
+                    T = "values",
+                    $ = "entries",
                     L = function() {
                         return this
                     };
-                r.exports = function(T, O, D, G, A, M, X) {
-                    i(D, O, G);
-                    var R = function(lt) {
-                            if (lt === A && vt) return vt;
-                            if (!P && lt in at) return at[lt];
-                            switch (lt) {
+                r.exports = function(I, j, P, M, D, R, H) {
+                    l(P, j, M);
+                    var F = function(st) {
+                            if (st === D && ct) return ct;
+                            if (!O && st in ot) return ot[st];
+                            switch (st) {
                                 case C:
                                     return function() {
-                                        return new D(this, lt)
+                                        return new P(this, st)
                                     };
-                                case I:
+                                case T:
                                     return function() {
-                                        return new D(this, lt)
+                                        return new P(this, st)
                                     };
-                                case j:
+                                case $:
                                     return function() {
-                                        return new D(this, lt)
+                                        return new P(this, st)
                                     }
                             }
                             return function() {
-                                return new D(this)
+                                return new P(this)
                             }
                         },
-                        F = O + " Iterator",
-                        _ = !1,
-                        at = T.prototype,
-                        xt = at[x] || at["@@iterator"] || A && at[A],
-                        vt = !P && xt || R(A),
-                        ht = O == "Array" && at.entries || xt,
-                        Et, Ot, bt;
-                    if (ht && (Et = s(ht.call(new T)), S !== Object.prototype && Et.next && (!p && s(Et) !== S && (c ? c(Et, S) : typeof Et[x] != "function" && d(Et, x, L)), f(Et, F, !0, !0), p && (g[F] = L))), A == I && xt && xt.name !== I && (_ = !0, vt = function() {
-                            return xt.call(this)
-                        }), (!p || X) && at[x] !== vt && d(at, x, vt), g[O] = vt, A)
-                        if (Ot = {
-                                values: R(I),
-                                keys: M ? vt : R(C),
-                                entries: R(j)
-                            }, X)
-                            for (bt in Ot)(P || _ || !(bt in at)) && v(at, bt, Ot[bt]);
+                        N = j + " Iterator",
+                        k = !1,
+                        ot = I.prototype,
+                        St = ot[E] || ot["@@iterator"] || D && ot[D],
+                        ct = !O && St || F(D),
+                        pt = j == "Array" && ot.entries || St,
+                        Ot, It, Et;
+                    if (pt && (Ot = u(pt.call(new I)), y !== Object.prototype && Ot.next && (!h && u(Ot) !== y && (f ? f(Ot, y) : typeof Ot[E] != "function" && d(Ot, E, L)), c(Ot, N, !0, !0), h && (m[N] = L))), D == T && St && St.name !== T && (k = !0, ct = function() {
+                            return St.call(this)
+                        }), (!h || H) && ot[E] !== ct && d(ot, E, ct), m[j] = ct, D)
+                        if (It = {
+                                values: F(T),
+                                keys: R ? ct : F(C),
+                                entries: F($)
+                            }, H)
+                            for (Et in It)(O || k || !(Et in ot)) && v(ot, Et, It[Et]);
                         else o({
-                            target: O,
+                            target: j,
                             proto: !0,
-                            forced: P || _
-                        }, Ot);
-                    return Ot
+                            forced: O || k
+                        }, It);
+                    return It
                 }
             },
-            "7f9a": function(r, u, t) {
+            "7f9a": function(r, s, t) {
                 var o = t("da84"),
-                    i = t("8925"),
-                    s = o.WeakMap;
-                r.exports = typeof s == "function" && /native code/.test(i(s))
+                    l = t("8925"),
+                    u = o.WeakMap;
+                r.exports = typeof u == "function" && /native code/.test(l(u))
             },
-            "825a": function(r, u, t) {
+            "825a": function(r, s, t) {
                 var o = t("861d");
-                r.exports = function(i) {
-                    if (!o(i)) throw TypeError(String(i) + " is not an object");
-                    return i
+                r.exports = function(l) {
+                    if (!o(l)) throw TypeError(String(l) + " is not an object");
+                    return l
                 }
             },
-            "83ab": function(r, u, t) {
+            "83ab": function(r, s, t) {
                 var o = t("d039");
                 r.exports = !o(function() {
                     return Object.defineProperty({}, 1, {
                         get: function() {
                             return 7
                         }
                     })[1] != 7
                 })
             },
-            8418: function(r, u, t) {
+            8418: function(r, s, t) {
                 var o = t("c04e"),
-                    i = t("9bf2"),
-                    s = t("5c6c");
-                r.exports = function(c, f, d) {
-                    var v = o(f);
-                    v in c ? i.f(c, v, s(0, d)) : c[v] = d
+                    l = t("9bf2"),
+                    u = t("5c6c");
+                r.exports = function(f, c, d) {
+                    var v = o(c);
+                    v in f ? l.f(f, v, u(0, d)) : f[v] = d
                 }
             },
-            "861d": function(r, u) {
+            "861d": function(r, s) {
                 r.exports = function(t) {
                     return typeof t == "object" ? t !== null : typeof t == "function"
                 }
             },
-            8875: function(r, u, t) {
-                var o, i, s;
-                (function(c, f) {
-                    i = [], o = f, s = typeof o == "function" ? o.apply(u, i) : o, s !== void 0 && (r.exports = s)
+            8875: function(r, s, t) {
+                var o, l, u;
+                (function(f, c) {
+                    l = [], o = c, u = typeof o == "function" ? o.apply(s, l) : o, u !== void 0 && (r.exports = u)
                 })(typeof self < "u" ? self : this, function() {
-                    function c() {
-                        var f = Object.getOwnPropertyDescriptor(document, "currentScript");
-                        if (!f && "currentScript" in document && document.currentScript || f && f.get !== c && document.currentScript) return document.currentScript;
+                    function f() {
+                        var c = Object.getOwnPropertyDescriptor(document, "currentScript");
+                        if (!c && "currentScript" in document && document.currentScript || c && c.get !== f && document.currentScript) return document.currentScript;
                         try {
                             throw new Error
-                        } catch (j) {
+                        } catch ($) {
                             var d = /.*at [^(]*\((.*):(.+):(.+)\)$/ig,
                                 v = /@([^@]*):(\d+):(\d+)\s*$/ig,
-                                h = d.exec(j.stack) || v.exec(j.stack),
-                                p = h && h[1] || !1,
-                                g = h && h[2] || !1,
-                                b = document.location.href.replace(document.location.hash, ""),
-                                S, P, x, C = document.getElementsByTagName("script");
-                            p === b && (S = document.documentElement.outerHTML, P = new RegExp("(?:[^\\n]+?\\n){0," + (g - 2) + "}[^<]*<script>([\\d\\D]*?)<\\/script>[\\d\\D]*", "i"), x = S.replace(P, "$1").trim());
-                            for (var I = 0; I < C.length; I++)
-                                if (C[I].readyState === "interactive" || C[I].src === p || p === b && C[I].innerHTML && C[I].innerHTML.trim() === x) return C[I];
+                                p = d.exec($.stack) || v.exec($.stack),
+                                h = p && p[1] || !1,
+                                m = p && p[2] || !1,
+                                g = document.location.href.replace(document.location.hash, ""),
+                                y, O, E, C = document.getElementsByTagName("script");
+                            h === g && (y = document.documentElement.outerHTML, O = new RegExp("(?:[^\\n]+?\\n){0," + (m - 2) + "}[^<]*<script>([\\d\\D]*?)<\\/script>[\\d\\D]*", "i"), E = y.replace(O, "$1").trim());
+                            for (var T = 0; T < C.length; T++)
+                                if (C[T].readyState === "interactive" || C[T].src === h || h === g && C[T].innerHTML && C[T].innerHTML.trim() === E) return C[T];
                             return null
                         }
                     }
-                    return c
+                    return f
                 })
             },
-            8925: function(r, u, t) {
+            8925: function(r, s, t) {
                 var o = t("c6cd"),
-                    i = Function.toString;
-                typeof o.inspectSource != "function" && (o.inspectSource = function(s) {
-                    return i.call(s)
+                    l = Function.toString;
+                typeof o.inspectSource != "function" && (o.inspectSource = function(u) {
+                    return l.call(u)
                 }), r.exports = o.inspectSource
             },
-            "8aa5": function(r, u, t) {
+            "8aa5": function(r, s, t) {
                 var o = t("6547").charAt;
-                r.exports = function(i, s, c) {
-                    return s + (c ? o(i, s).length : 1)
+                r.exports = function(l, u, f) {
+                    return u + (f ? o(l, u).length : 1)
                 }
             },
-            "8bbf": function(r, u) {
+            "8bbf": function(r, s) {
                 r.exports = n
             },
-            "90e3": function(r, u) {
+            "90e3": function(r, s) {
                 var t = 0,
                     o = Math.random();
-                r.exports = function(i) {
-                    return "Symbol(" + String(i === void 0 ? "" : i) + ")_" + (++t + o).toString(36)
+                r.exports = function(l) {
+                    return "Symbol(" + String(l === void 0 ? "" : l) + ")_" + (++t + o).toString(36)
                 }
             },
-            9112: function(r, u, t) {
+            9112: function(r, s, t) {
                 var o = t("83ab"),
-                    i = t("9bf2"),
-                    s = t("5c6c");
-                r.exports = o ? function(c, f, d) {
-                    return i.f(c, f, s(1, d))
-                } : function(c, f, d) {
-                    return c[f] = d, c
+                    l = t("9bf2"),
+                    u = t("5c6c");
+                r.exports = o ? function(f, c, d) {
+                    return l.f(f, c, u(1, d))
+                } : function(f, c, d) {
+                    return f[c] = d, f
                 }
             },
-            9263: function(r, u, t) {
+            9263: function(r, s, t) {
                 var o = t("ad6d"),
-                    i = t("9f7f"),
-                    s = RegExp.prototype.exec,
-                    c = String.prototype.replace,
-                    f = s,
+                    l = t("9f7f"),
+                    u = RegExp.prototype.exec,
+                    f = String.prototype.replace,
+                    c = u,
                     d = function() {
-                        var g = /a/,
-                            b = /b*/g;
-                        return s.call(g, "a"), s.call(b, "a"), g.lastIndex !== 0 || b.lastIndex !== 0
+                        var m = /a/,
+                            g = /b*/g;
+                        return u.call(m, "a"), u.call(g, "a"), m.lastIndex !== 0 || g.lastIndex !== 0
                     }(),
-                    v = i.UNSUPPORTED_Y || i.BROKEN_CARET,
-                    h = /()??/.exec("")[1] !== void 0,
-                    p = d || h || v;
-                p && (f = function(b) {
-                    var S = this,
-                        P, x, C, I, j = v && S.sticky,
-                        L = o.call(S),
-                        T = S.source,
-                        O = 0,
-                        D = b;
-                    return j && (L = L.replace("y", ""), L.indexOf("g") === -1 && (L += "g"), D = String(b).slice(S.lastIndex), S.lastIndex > 0 && (!S.multiline || S.multiline && b[S.lastIndex - 1] !== `
-`) && (T = "(?: " + T + ")", D = " " + D, O++), x = new RegExp("^(?:" + T + ")", L)), h && (x = new RegExp("^" + T + "$(?!\\s)", L)), d && (P = S.lastIndex), C = s.call(j ? x : S, D), j ? C ? (C.input = C.input.slice(O), C[0] = C[0].slice(O), C.index = S.lastIndex, S.lastIndex += C[0].length) : S.lastIndex = 0 : d && C && (S.lastIndex = S.global ? C.index + C[0].length : P), h && C && C.length > 1 && c.call(C[0], x, function() {
-                        for (I = 1; I < arguments.length - 2; I++) arguments[I] === void 0 && (C[I] = void 0)
+                    v = l.UNSUPPORTED_Y || l.BROKEN_CARET,
+                    p = /()??/.exec("")[1] !== void 0,
+                    h = d || p || v;
+                h && (c = function(g) {
+                    var y = this,
+                        O, E, C, T, $ = v && y.sticky,
+                        L = o.call(y),
+                        I = y.source,
+                        j = 0,
+                        P = g;
+                    return $ && (L = L.replace("y", ""), L.indexOf("g") === -1 && (L += "g"), P = String(g).slice(y.lastIndex), y.lastIndex > 0 && (!y.multiline || y.multiline && g[y.lastIndex - 1] !== `
+`) && (I = "(?: " + I + ")", P = " " + P, j++), E = new RegExp("^(?:" + I + ")", L)), p && (E = new RegExp("^" + I + "$(?!\\s)", L)), d && (O = y.lastIndex), C = u.call($ ? E : y, P), $ ? C ? (C.input = C.input.slice(j), C[0] = C[0].slice(j), C.index = y.lastIndex, y.lastIndex += C[0].length) : y.lastIndex = 0 : d && C && (y.lastIndex = y.global ? C.index + C[0].length : O), p && C && C.length > 1 && f.call(C[0], E, function() {
+                        for (T = 1; T < arguments.length - 2; T++) arguments[T] === void 0 && (C[T] = void 0)
                     }), C
-                }), r.exports = f
+                }), r.exports = c
             },
-            "94ca": function(r, u, t) {
+            "94ca": function(r, s, t) {
                 var o = t("d039"),
-                    i = /#|\.prototype\./,
-                    s = function(h, p) {
-                        var g = f[c(h)];
-                        return g == v ? !0 : g == d ? !1 : typeof p == "function" ? o(p) : !!p
+                    l = /#|\.prototype\./,
+                    u = function(p, h) {
+                        var m = c[f(p)];
+                        return m == v ? !0 : m == d ? !1 : typeof h == "function" ? o(h) : !!h
                     },
-                    c = s.normalize = function(h) {
-                        return String(h).replace(i, ".").toLowerCase()
+                    f = u.normalize = function(p) {
+                        return String(p).replace(l, ".").toLowerCase()
                     },
-                    f = s.data = {},
-                    d = s.NATIVE = "N",
-                    v = s.POLYFILL = "P";
-                r.exports = s
+                    c = u.data = {},
+                    d = u.NATIVE = "N",
+                    v = u.POLYFILL = "P";
+                r.exports = u
             },
-            "99af": function(r, u, t) {
+            "99af": function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("d039"),
-                    s = t("e8b5"),
-                    c = t("861d"),
-                    f = t("7b0b"),
+                    l = t("d039"),
+                    u = t("e8b5"),
+                    f = t("861d"),
+                    c = t("7b0b"),
                     d = t("50c4"),
                     v = t("8418"),
-                    h = t("65f0"),
-                    p = t("1dde"),
-                    g = t("b622"),
-                    b = t("2d00"),
-                    S = g("isConcatSpreadable"),
-                    P = 9007199254740991,
-                    x = "Maximum allowed index exceeded",
-                    C = b >= 51 || !i(function() {
-                        var T = [];
-                        return T[S] = !1, T.concat()[0] !== T
+                    p = t("65f0"),
+                    h = t("1dde"),
+                    m = t("b622"),
+                    g = t("2d00"),
+                    y = m("isConcatSpreadable"),
+                    O = 9007199254740991,
+                    E = "Maximum allowed index exceeded",
+                    C = g >= 51 || !l(function() {
+                        var I = [];
+                        return I[y] = !1, I.concat()[0] !== I
                     }),
-                    I = p("concat"),
-                    j = function(T) {
-                        if (!c(T)) return !1;
-                        var O = T[S];
-                        return O !== void 0 ? !!O : s(T)
+                    T = h("concat"),
+                    $ = function(I) {
+                        if (!f(I)) return !1;
+                        var j = I[y];
+                        return j !== void 0 ? !!j : u(I)
                     },
-                    L = !C || !I;
+                    L = !C || !T;
                 o({
                     target: "Array",
                     proto: !0,
                     forced: L
                 }, {
-                    concat: function(O) {
-                        var D = f(this),
-                            G = h(D, 0),
-                            A = 0,
-                            M, X, R, F, _;
-                        for (M = -1, R = arguments.length; M < R; M++)
-                            if (_ = M === -1 ? D : arguments[M], j(_)) {
-                                if (F = d(_.length), A + F > P) throw TypeError(x);
-                                for (X = 0; X < F; X++, A++) X in _ && v(G, A, _[X])
+                    concat: function(j) {
+                        var P = c(this),
+                            M = p(P, 0),
+                            D = 0,
+                            R, H, F, N, k;
+                        for (R = -1, F = arguments.length; R < F; R++)
+                            if (k = R === -1 ? P : arguments[R], $(k)) {
+                                if (N = d(k.length), D + N > O) throw TypeError(E);
+                                for (H = 0; H < N; H++, D++) H in k && v(M, D, k[H])
                             } else {
-                                if (A >= P) throw TypeError(x);
-                                v(G, A++, _)
-                            } return G.length = A, G
+                                if (D >= O) throw TypeError(E);
+                                v(M, D++, k)
+                            } return M.length = D, M
                     }
                 })
             },
-            "9bdd": function(r, u, t) {
+            "9bdd": function(r, s, t) {
                 var o = t("825a");
-                r.exports = function(i, s, c, f) {
+                r.exports = function(l, u, f, c) {
                     try {
-                        return f ? s(o(c)[0], c[1]) : s(c)
+                        return c ? u(o(f)[0], f[1]) : u(f)
                     } catch (v) {
-                        var d = i.return;
-                        throw d !== void 0 && o(d.call(i)), v
+                        var d = l.return;
+                        throw d !== void 0 && o(d.call(l)), v
                     }
                 }
             },
-            "9bf2": function(r, u, t) {
+            "9bf2": function(r, s, t) {
                 var o = t("83ab"),
-                    i = t("0cfb"),
-                    s = t("825a"),
-                    c = t("c04e"),
-                    f = Object.defineProperty;
-                u.f = o ? f : function(v, h, p) {
-                    if (s(v), h = c(h, !0), s(p), i) try {
-                        return f(v, h, p)
+                    l = t("0cfb"),
+                    u = t("825a"),
+                    f = t("c04e"),
+                    c = Object.defineProperty;
+                s.f = o ? c : function(v, p, h) {
+                    if (u(v), p = f(p, !0), u(h), l) try {
+                        return c(v, p, h)
                     } catch {}
-                    if ("get" in p || "set" in p) throw TypeError("Accessors not supported");
-                    return "value" in p && (v[h] = p.value), v
+                    if ("get" in h || "set" in h) throw TypeError("Accessors not supported");
+                    return "value" in h && (v[p] = h.value), v
                 }
             },
-            "9ed3": function(r, u, t) {
+            "9ed3": function(r, s, t) {
                 var o = t("ae93").IteratorPrototype,
-                    i = t("7c73"),
-                    s = t("5c6c"),
-                    c = t("d44e"),
-                    f = t("3f8c"),
+                    l = t("7c73"),
+                    u = t("5c6c"),
+                    f = t("d44e"),
+                    c = t("3f8c"),
                     d = function() {
                         return this
                     };
-                r.exports = function(v, h, p) {
-                    var g = h + " Iterator";
-                    return v.prototype = i(o, {
-                        next: s(1, p)
-                    }), c(v, g, !1, !0), f[g] = d, v
+                r.exports = function(v, p, h) {
+                    var m = p + " Iterator";
+                    return v.prototype = l(o, {
+                        next: u(1, h)
+                    }), f(v, m, !1, !0), c[m] = d, v
                 }
             },
-            "9f7f": function(r, u, t) {
+            "9f7f": function(r, s, t) {
                 var o = t("d039");
 
-                function i(s, c) {
-                    return RegExp(s, c)
+                function l(u, f) {
+                    return RegExp(u, f)
                 }
-                u.UNSUPPORTED_Y = o(function() {
-                    var s = i("a", "y");
-                    return s.lastIndex = 2, s.exec("abcd") != null
-                }), u.BROKEN_CARET = o(function() {
-                    var s = i("^r", "gy");
-                    return s.lastIndex = 2, s.exec("str") != null
+                s.UNSUPPORTED_Y = o(function() {
+                    var u = l("a", "y");
+                    return u.lastIndex = 2, u.exec("abcd") != null
+                }), s.BROKEN_CARET = o(function() {
+                    var u = l("^r", "gy");
+                    return u.lastIndex = 2, u.exec("str") != null
                 })
             },
-            a2bf: function(r, u, t) {
+            a2bf: function(r, s, t) {
                 var o = t("e8b5"),
-                    i = t("50c4"),
-                    s = t("0366"),
-                    c = function(f, d, v, h, p, g, b, S) {
-                        for (var P = p, x = 0, C = b ? s(b, S, 3) : !1, I; x < h;) {
-                            if (x in v) {
-                                if (I = C ? C(v[x], x, d) : v[x], g > 0 && o(I)) P = c(f, d, I, i(I.length), P, g - 1) - 1;
+                    l = t("50c4"),
+                    u = t("0366"),
+                    f = function(c, d, v, p, h, m, g, y) {
+                        for (var O = h, E = 0, C = g ? u(g, y, 3) : !1, T; E < p;) {
+                            if (E in v) {
+                                if (T = C ? C(v[E], E, d) : v[E], m > 0 && o(T)) O = f(c, d, T, l(T.length), O, m - 1) - 1;
                                 else {
-                                    if (P >= 9007199254740991) throw TypeError("Exceed the acceptable array length");
-                                    f[P] = I
+                                    if (O >= 9007199254740991) throw TypeError("Exceed the acceptable array length");
+                                    c[O] = T
                                 }
-                                P++
+                                O++
                             }
-                            x++
+                            E++
                         }
-                        return P
+                        return O
                     };
-                r.exports = c
+                r.exports = f
             },
-            a352: function(r, u) {
-                r.exports = l
+            a352: function(r, s) {
+                r.exports = i
             },
-            a434: function(r, u, t) {
+            a434: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("23cb"),
-                    s = t("a691"),
-                    c = t("50c4"),
-                    f = t("7b0b"),
+                    l = t("23cb"),
+                    u = t("a691"),
+                    f = t("50c4"),
+                    c = t("7b0b"),
                     d = t("65f0"),
                     v = t("8418"),
-                    h = t("1dde"),
-                    p = t("ae40"),
-                    g = h("splice"),
-                    b = p("splice", {
+                    p = t("1dde"),
+                    h = t("ae40"),
+                    m = p("splice"),
+                    g = h("splice", {
                         ACCESSORS: !0,
                         0: 0,
                         1: 2
                     }),
-                    S = Math.max,
-                    P = Math.min,
-                    x = 9007199254740991,
+                    y = Math.max,
+                    O = Math.min,
+                    E = 9007199254740991,
                     C = "Maximum allowed length exceeded";
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: !g || !b
+                    forced: !m || !g
                 }, {
-                    splice: function(j, L) {
-                        var T = f(this),
-                            O = c(T.length),
-                            D = i(j, O),
-                            G = arguments.length,
-                            A, M, X, R, F, _;
-                        if (G === 0 ? A = M = 0 : G === 1 ? (A = 0, M = O - D) : (A = G - 2, M = P(S(s(L), 0), O - D)), O + A - M > x) throw TypeError(C);
-                        for (X = d(T, M), R = 0; R < M; R++) F = D + R, F in T && v(X, R, T[F]);
-                        if (X.length = M, A < M) {
-                            for (R = D; R < O - M; R++) F = R + M, _ = R + A, F in T ? T[_] = T[F] : delete T[_];
-                            for (R = O; R > O - M + A; R--) delete T[R - 1]
-                        } else if (A > M)
-                            for (R = O - M; R > D; R--) F = R + M - 1, _ = R + A - 1, F in T ? T[_] = T[F] : delete T[_];
-                        for (R = 0; R < A; R++) T[R + D] = arguments[R + 2];
-                        return T.length = O - M + A, X
+                    splice: function($, L) {
+                        var I = c(this),
+                            j = f(I.length),
+                            P = l($, j),
+                            M = arguments.length,
+                            D, R, H, F, N, k;
+                        if (M === 0 ? D = R = 0 : M === 1 ? (D = 0, R = j - P) : (D = M - 2, R = O(y(u(L), 0), j - P)), j + D - R > E) throw TypeError(C);
+                        for (H = d(I, R), F = 0; F < R; F++) N = P + F, N in I && v(H, F, I[N]);
+                        if (H.length = R, D < R) {
+                            for (F = P; F < j - R; F++) N = F + R, k = F + D, N in I ? I[k] = I[N] : delete I[k];
+                            for (F = j; F > j - R + D; F--) delete I[F - 1]
+                        } else if (D > R)
+                            for (F = j - R; F > P; F--) N = F + R - 1, k = F + D - 1, N in I ? I[k] = I[N] : delete I[k];
+                        for (F = 0; F < D; F++) I[F + P] = arguments[F + 2];
+                        return I.length = j - R + D, H
                     }
                 })
             },
-            a4d3: function(r, u, t) {
+            a4d3: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("da84"),
-                    s = t("d066"),
-                    c = t("c430"),
-                    f = t("83ab"),
+                    l = t("da84"),
+                    u = t("d066"),
+                    f = t("c430"),
+                    c = t("83ab"),
                     d = t("4930"),
                     v = t("fdbf"),
-                    h = t("d039"),
-                    p = t("5135"),
-                    g = t("e8b5"),
-                    b = t("861d"),
-                    S = t("825a"),
-                    P = t("7b0b"),
-                    x = t("fc6a"),
+                    p = t("d039"),
+                    h = t("5135"),
+                    m = t("e8b5"),
+                    g = t("861d"),
+                    y = t("825a"),
+                    O = t("7b0b"),
+                    E = t("fc6a"),
                     C = t("c04e"),
-                    I = t("5c6c"),
-                    j = t("7c73"),
+                    T = t("5c6c"),
+                    $ = t("7c73"),
                     L = t("df75"),
-                    T = t("241c"),
-                    O = t("057f"),
-                    D = t("7418"),
-                    G = t("06cf"),
-                    A = t("9bf2"),
-                    M = t("d1e7"),
-                    X = t("9112"),
-                    R = t("6eeb"),
-                    F = t("5692"),
-                    _ = t("f772"),
-                    at = t("d012"),
-                    xt = t("90e3"),
-                    vt = t("b622"),
-                    ht = t("e538"),
-                    Et = t("746f"),
-                    Ot = t("d44e"),
-                    bt = t("69f3"),
-                    lt = t("b727").forEach,
-                    ct = _("hidden"),
+                    I = t("241c"),
+                    j = t("057f"),
+                    P = t("7418"),
+                    M = t("06cf"),
+                    D = t("9bf2"),
+                    R = t("d1e7"),
+                    H = t("9112"),
+                    F = t("6eeb"),
+                    N = t("5692"),
+                    k = t("f772"),
+                    ot = t("d012"),
+                    St = t("90e3"),
+                    ct = t("b622"),
+                    pt = t("e538"),
+                    Ot = t("746f"),
+                    It = t("d44e"),
+                    Et = t("69f3"),
+                    st = t("b727").forEach,
+                    dt = k("hidden"),
                     Lt = "Symbol",
-                    Rt = "prototype",
-                    _t = vt("toPrimitive"),
-                    ue = bt.set,
-                    oe = bt.getterFor(Lt),
-                    Tt = Object[Rt],
-                    It = i.Symbol,
-                    fe = s("JSON", "stringify"),
-                    Yt = G.f,
-                    zt = A.f,
-                    Ye = O.f,
-                    hn = M.f,
-                    Kt = F("symbols"),
-                    ae = F("op-symbols"),
-                    pe = F("string-to-symbol-registry"),
-                    Oe = F("symbol-to-string-registry"),
-                    Te = F("wks"),
-                    Ie = i.QObject,
-                    Pe = !Ie || !Ie[Rt] || !Ie[Rt].findChild,
-                    Ce = f && h(function() {
-                        return j(zt({}, "a", {
+                    wt = "prototype",
+                    re = ct("toPrimitive"),
+                    de = Et.set,
+                    ie = Et.getterFor(Lt),
+                    Pt = Object[wt],
+                    Ct = l.Symbol,
+                    ve = u("JSON", "stringify"),
+                    Zt = M.f,
+                    kt = D.f,
+                    Je = j.f,
+                    mn = R.f,
+                    Wt = N("symbols"),
+                    le = N("op-symbols"),
+                    ye = N("string-to-symbol-registry"),
+                    Pe = N("symbol-to-string-registry"),
+                    Ce = N("wks"),
+                    De = l.QObject,
+                    Ae = !De || !De[wt] || !De[wt].findChild,
+                    Re = c && p(function() {
+                        return $(kt({}, "a", {
                             get: function() {
-                                return zt(this, "a", {
+                                return kt(this, "a", {
                                     value: 7
                                 }).a
                             }
                         })).a != 7
-                    }) ? function(J, V, H) {
-                        var nt = Yt(Tt, V);
-                        nt && delete Tt[V], zt(J, V, H), nt && J !== Tt && zt(Tt, V, nt)
-                    } : zt,
-                    De = function(J, V) {
-                        var H = Kt[J] = j(It[Rt]);
-                        return ue(H, {
+                    }) ? function(Q, B, Y) {
+                        var nt = Zt(Pt, B);
+                        nt && delete Pt[B], kt(Q, B, Y), nt && Q !== Pt && kt(Pt, B, nt)
+                    } : kt,
+                    we = function(Q, B) {
+                        var Y = Wt[Q] = $(Ct[wt]);
+                        return de(Y, {
                             type: Lt,
-                            tag: J,
-                            description: V
-                        }), f || (H.description = V), H
+                            tag: Q,
+                            description: B
+                        }), c || (Y.description = B), Y
                     },
-                    y = v ? function(J) {
-                        return typeof J == "symbol"
-                    } : function(J) {
-                        return Object(J) instanceof It
+                    S = v ? function(Q) {
+                        return typeof Q == "symbol"
+                    } : function(Q) {
+                        return Object(Q) instanceof Ct
                     },
-                    m = function(V, H, nt) {
-                        V === Tt && m(ae, H, nt), S(V);
-                        var rt = C(H, !0);
-                        return S(nt), p(Kt, rt) ? (nt.enumerable ? (p(V, ct) && V[ct][rt] && (V[ct][rt] = !1), nt = j(nt, {
-                            enumerable: I(0, !1)
-                        })) : (p(V, ct) || zt(V, ct, I(1, {})), V[ct][rt] = !0), Ce(V, rt, nt)) : zt(V, rt, nt)
+                    b = function(B, Y, nt) {
+                        B === Pt && b(le, Y, nt), y(B);
+                        var rt = C(Y, !0);
+                        return y(nt), h(Wt, rt) ? (nt.enumerable ? (h(B, dt) && B[dt][rt] && (B[dt][rt] = !1), nt = $(nt, {
+                            enumerable: T(0, !1)
+                        })) : (h(B, dt) || kt(B, dt, T(1, {})), B[dt][rt] = !0), Re(B, rt, nt)) : kt(B, rt, nt)
                     },
-                    E = function(V, H) {
-                        S(V);
-                        var nt = x(H),
-                            rt = L(nt).concat(ot(nt));
-                        return lt(rt, function(Nt) {
-                            (!f || $.call(nt, Nt)) && m(V, Nt, nt[Nt])
-                        }), V
+                    x = function(B, Y) {
+                        y(B);
+                        var nt = E(Y),
+                            rt = L(nt).concat(at(nt));
+                        return st(rt, function(jt) {
+                            (!c || V.call(nt, jt)) && b(B, jt, nt[jt])
+                        }), B
                     },
-                    w = function(V, H) {
-                        return H === void 0 ? j(V) : E(j(V), H)
+                    A = function(B, Y) {
+                        return Y === void 0 ? $(B) : x($(B), Y)
                     },
-                    $ = function(V) {
-                        var H = C(V, !0),
-                            nt = hn.call(this, H);
-                        return this === Tt && p(Kt, H) && !p(ae, H) ? !1 : nt || !p(this, H) || !p(Kt, H) || p(this, ct) && this[ct][H] ? nt : !0
+                    V = function(B) {
+                        var Y = C(B, !0),
+                            nt = mn.call(this, Y);
+                        return this === Pt && h(Wt, Y) && !h(le, Y) ? !1 : nt || !h(this, Y) || !h(Wt, Y) || h(this, dt) && this[dt][Y] ? nt : !0
                     },
-                    z = function(V, H) {
-                        var nt = x(V),
-                            rt = C(H, !0);
-                        if (!(nt === Tt && p(Kt, rt) && !p(ae, rt))) {
-                            var Nt = Yt(nt, rt);
-                            return Nt && p(Kt, rt) && !(p(nt, ct) && nt[ct][rt]) && (Nt.enumerable = !0), Nt
+                    J = function(B, Y) {
+                        var nt = E(B),
+                            rt = C(Y, !0);
+                        if (!(nt === Pt && h(Wt, rt) && !h(le, rt))) {
+                            var jt = Zt(nt, rt);
+                            return jt && h(Wt, rt) && !(h(nt, dt) && nt[dt][rt]) && (jt.enumerable = !0), jt
                         }
                     },
-                    q = function(V) {
-                        var H = Ye(x(V)),
+                    _ = function(B) {
+                        var Y = Je(E(B)),
                             nt = [];
-                        return lt(H, function(rt) {
-                            !p(Kt, rt) && !p(at, rt) && nt.push(rt)
+                        return st(Y, function(rt) {
+                            !h(Wt, rt) && !h(ot, rt) && nt.push(rt)
                         }), nt
                     },
-                    ot = function(V) {
-                        var H = V === Tt,
-                            nt = Ye(H ? ae : x(V)),
+                    at = function(B) {
+                        var Y = B === Pt,
+                            nt = Je(Y ? le : E(B)),
                             rt = [];
-                        return lt(nt, function(Nt) {
-                            p(Kt, Nt) && (!H || p(Tt, Nt)) && rt.push(Kt[Nt])
+                        return st(nt, function(jt) {
+                            h(Wt, jt) && (!Y || h(Pt, jt)) && rt.push(Wt[jt])
                         }), rt
                     };
-                if (d || (It = function() {
-                        if (this instanceof It) throw TypeError("Symbol is not a constructor");
-                        var V = !arguments.length || arguments[0] === void 0 ? void 0 : String(arguments[0]),
-                            H = xt(V),
+                if (d || (Ct = function() {
+                        if (this instanceof Ct) throw TypeError("Symbol is not a constructor");
+                        var B = !arguments.length || arguments[0] === void 0 ? void 0 : String(arguments[0]),
+                            Y = St(B),
                             nt = function(rt) {
-                                this === Tt && nt.call(ae, rt), p(this, ct) && p(this[ct], H) && (this[ct][H] = !1), Ce(this, H, I(1, rt))
+                                this === Pt && nt.call(le, rt), h(this, dt) && h(this[dt], Y) && (this[dt][Y] = !1), Re(this, Y, T(1, rt))
                             };
-                        return f && Pe && Ce(Tt, H, {
+                        return c && Ae && Re(Pt, Y, {
                             configurable: !0,
                             set: nt
-                        }), De(H, V)
-                    }, R(It[Rt], "toString", function() {
-                        return oe(this).tag
-                    }), R(It, "withoutSetter", function(J) {
-                        return De(xt(J), J)
-                    }), M.f = $, A.f = m, G.f = z, T.f = O.f = q, D.f = ot, ht.f = function(J) {
-                        return De(vt(J), J)
-                    }, f && (zt(It[Rt], "description", {
+                        }), we(Y, B)
+                    }, F(Ct[wt], "toString", function() {
+                        return ie(this).tag
+                    }), F(Ct, "withoutSetter", function(Q) {
+                        return we(St(Q), Q)
+                    }), R.f = V, D.f = b, M.f = J, I.f = j.f = _, P.f = at, pt.f = function(Q) {
+                        return we(ct(Q), Q)
+                    }, c && (kt(Ct[wt], "description", {
                         configurable: !0,
                         get: function() {
-                            return oe(this).description
+                            return ie(this).description
                         }
-                    }), c || R(Tt, "propertyIsEnumerable", $, {
+                    }), f || F(Pt, "propertyIsEnumerable", V, {
                         unsafe: !0
                     }))), o({
                         global: !0,
                         wrap: !0,
                         forced: !d,
                         sham: !d
                     }, {
-                        Symbol: It
-                    }), lt(L(Te), function(J) {
-                        Et(J)
+                        Symbol: Ct
+                    }), st(L(Ce), function(Q) {
+                        Ot(Q)
                     }), o({
                         target: Lt,
                         stat: !0,
                         forced: !d
                     }, {
-                        for: function(J) {
-                            var V = String(J);
-                            if (p(pe, V)) return pe[V];
-                            var H = It(V);
-                            return pe[V] = H, Oe[H] = V, H
+                        for: function(Q) {
+                            var B = String(Q);
+                            if (h(ye, B)) return ye[B];
+                            var Y = Ct(B);
+                            return ye[B] = Y, Pe[Y] = B, Y
                         },
-                        keyFor: function(V) {
-                            if (!y(V)) throw TypeError(V + " is not a symbol");
-                            if (p(Oe, V)) return Oe[V]
+                        keyFor: function(B) {
+                            if (!S(B)) throw TypeError(B + " is not a symbol");
+                            if (h(Pe, B)) return Pe[B]
                         },
                         useSetter: function() {
-                            Pe = !0
+                            Ae = !0
                         },
                         useSimple: function() {
-                            Pe = !1
+                            Ae = !1
                         }
                     }), o({
                         target: "Object",
                         stat: !0,
                         forced: !d,
-                        sham: !f
+                        sham: !c
                     }, {
-                        create: w,
-                        defineProperty: m,
-                        defineProperties: E,
-                        getOwnPropertyDescriptor: z
+                        create: A,
+                        defineProperty: b,
+                        defineProperties: x,
+                        getOwnPropertyDescriptor: J
                     }), o({
                         target: "Object",
                         stat: !0,
                         forced: !d
                     }, {
-                        getOwnPropertyNames: q,
-                        getOwnPropertySymbols: ot
+                        getOwnPropertyNames: _,
+                        getOwnPropertySymbols: at
                     }), o({
                         target: "Object",
                         stat: !0,
-                        forced: h(function() {
-                            D.f(1)
+                        forced: p(function() {
+                            P.f(1)
                         })
                     }, {
-                        getOwnPropertySymbols: function(V) {
-                            return D.f(P(V))
+                        getOwnPropertySymbols: function(B) {
+                            return P.f(O(B))
                         }
-                    }), fe) {
-                    var yt = !d || h(function() {
-                        var J = It();
-                        return fe([J]) != "[null]" || fe({
-                            a: J
-                        }) != "{}" || fe(Object(J)) != "{}"
+                    }), ve) {
+                    var yt = !d || p(function() {
+                        var Q = Ct();
+                        return ve([Q]) != "[null]" || ve({
+                            a: Q
+                        }) != "{}" || ve(Object(Q)) != "{}"
                     });
                     o({
                         target: "JSON",
                         stat: !0,
                         forced: yt
                     }, {
-                        stringify: function(V, H, nt) {
-                            for (var rt = [V], Nt = 1, pn; arguments.length > Nt;) rt.push(arguments[Nt++]);
-                            if (pn = H, !(!b(H) && V === void 0 || y(V))) return g(H) || (H = function(Or, ze) {
-                                if (typeof pn == "function" && (ze = pn.call(this, Or, ze)), !y(ze)) return ze
-                            }), rt[1] = H, fe.apply(null, rt)
+                        stringify: function(B, Y, nt) {
+                            for (var rt = [B], jt = 1, gn; arguments.length > jt;) rt.push(arguments[jt++]);
+                            if (gn = Y, !(!g(Y) && B === void 0 || S(B))) return m(Y) || (Y = function(Nr, Qe) {
+                                if (typeof gn == "function" && (Qe = gn.call(this, Nr, Qe)), !S(Qe)) return Qe
+                            }), rt[1] = Y, ve.apply(null, rt)
                         }
                     })
                 }
-                It[Rt][_t] || X(It[Rt], _t, It[Rt].valueOf), Ot(It, Lt), at[ct] = !0
+                Ct[wt][re] || H(Ct[wt], re, Ct[wt].valueOf), It(Ct, Lt), ot[dt] = !0
             },
-            a630: function(r, u, t) {
+            a630: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("4df4"),
-                    s = t("1c7e"),
-                    c = !s(function(f) {
-                        Array.from(f)
+                    l = t("4df4"),
+                    u = t("1c7e"),
+                    f = !u(function(c) {
+                        Array.from(c)
                     });
                 o({
                     target: "Array",
                     stat: !0,
-                    forced: c
+                    forced: f
                 }, {
-                    from: i
+                    from: l
                 })
             },
-            a640: function(r, u, t) {
+            a640: function(r, s, t) {
                 var o = t("d039");
-                r.exports = function(i, s) {
-                    var c = [][i];
-                    return !!c && o(function() {
-                        c.call(null, s || function() {
+                r.exports = function(l, u) {
+                    var f = [][l];
+                    return !!f && o(function() {
+                        f.call(null, u || function() {
                             throw 1
                         }, 1)
                     })
                 }
             },
-            a691: function(r, u) {
+            a691: function(r, s) {
                 var t = Math.ceil,
                     o = Math.floor;
-                r.exports = function(i) {
-                    return isNaN(i = +i) ? 0 : (i > 0 ? o : t)(i)
+                r.exports = function(l) {
+                    return isNaN(l = +l) ? 0 : (l > 0 ? o : t)(l)
                 }
             },
-            ab13: function(r, u, t) {
+            ab13: function(r, s, t) {
                 var o = t("b622"),
-                    i = o("match");
-                r.exports = function(s) {
-                    var c = /./;
+                    l = o("match");
+                r.exports = function(u) {
+                    var f = /./;
                     try {
-                        "/./" [s](c)
+                        "/./" [u](f)
                     } catch {
                         try {
-                            return c[i] = !1, "/./" [s](c)
+                            return f[l] = !1, "/./" [u](f)
                         } catch {}
                     }
                     return !1
                 }
             },
-            ac1f: function(r, u, t) {
+            ac1f: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("9263");
+                    l = t("9263");
                 o({
                     target: "RegExp",
                     proto: !0,
-                    forced: /./.exec !== i
+                    forced: /./.exec !== l
                 }, {
-                    exec: i
+                    exec: l
                 })
             },
-            ad6d: function(r, u, t) {
+            ad6d: function(r, s, t) {
                 var o = t("825a");
                 r.exports = function() {
-                    var i = o(this),
-                        s = "";
-                    return i.global && (s += "g"), i.ignoreCase && (s += "i"), i.multiline && (s += "m"), i.dotAll && (s += "s"), i.unicode && (s += "u"), i.sticky && (s += "y"), s
+                    var l = o(this),
+                        u = "";
+                    return l.global && (u += "g"), l.ignoreCase && (u += "i"), l.multiline && (u += "m"), l.dotAll && (u += "s"), l.unicode && (u += "u"), l.sticky && (u += "y"), u
                 }
             },
-            ae40: function(r, u, t) {
+            ae40: function(r, s, t) {
                 var o = t("83ab"),
-                    i = t("d039"),
-                    s = t("5135"),
-                    c = Object.defineProperty,
-                    f = {},
+                    l = t("d039"),
+                    u = t("5135"),
+                    f = Object.defineProperty,
+                    c = {},
                     d = function(v) {
                         throw v
                     };
-                r.exports = function(v, h) {
-                    if (s(f, v)) return f[v];
-                    h || (h = {});
-                    var p = [][v],
-                        g = s(h, "ACCESSORS") ? h.ACCESSORS : !1,
-                        b = s(h, 0) ? h[0] : d,
-                        S = s(h, 1) ? h[1] : void 0;
-                    return f[v] = !!p && !i(function() {
-                        if (g && !o) return !0;
-                        var P = {
+                r.exports = function(v, p) {
+                    if (u(c, v)) return c[v];
+                    p || (p = {});
+                    var h = [][v],
+                        m = u(p, "ACCESSORS") ? p.ACCESSORS : !1,
+                        g = u(p, 0) ? p[0] : d,
+                        y = u(p, 1) ? p[1] : void 0;
+                    return c[v] = !!h && !l(function() {
+                        if (m && !o) return !0;
+                        var O = {
                             length: -1
                         };
-                        g ? c(P, 1, {
+                        m ? f(O, 1, {
                             enumerable: !0,
                             get: d
-                        }) : P[1] = 1, p.call(P, b, S)
+                        }) : O[1] = 1, h.call(O, g, y)
                     })
                 }
             },
-            ae93: function(r, u, t) {
+            ae93: function(r, s, t) {
                 var o = t("e163"),
-                    i = t("9112"),
-                    s = t("5135"),
-                    c = t("b622"),
-                    f = t("c430"),
-                    d = c("iterator"),
+                    l = t("9112"),
+                    u = t("5135"),
+                    f = t("b622"),
+                    c = t("c430"),
+                    d = f("iterator"),
                     v = !1,
-                    h = function() {
+                    p = function() {
                         return this
                     },
-                    p, g, b;
-                [].keys && (b = [].keys(), "next" in b ? (g = o(o(b)), g !== Object.prototype && (p = g)) : v = !0), p == null && (p = {}), !f && !s(p, d) && i(p, d, h), r.exports = {
-                    IteratorPrototype: p,
+                    h, m, g;
+                [].keys && (g = [].keys(), "next" in g ? (m = o(o(g)), m !== Object.prototype && (h = m)) : v = !0), h == null && (h = {}), !c && !u(h, d) && l(h, d, p), r.exports = {
+                    IteratorPrototype: h,
                     BUGGY_SAFARI_ITERATORS: v
                 }
             },
-            b041: function(r, u, t) {
+            b041: function(r, s, t) {
                 var o = t("00ee"),
-                    i = t("f5df");
+                    l = t("f5df");
                 r.exports = o ? {}.toString : function() {
-                    return "[object " + i(this) + "]"
+                    return "[object " + l(this) + "]"
                 }
             },
-            b0c0: function(r, u, t) {
+            b0c0: function(r, s, t) {
                 var o = t("83ab"),
-                    i = t("9bf2").f,
-                    s = Function.prototype,
-                    c = s.toString,
-                    f = /^\s*function ([^ (]*)/,
+                    l = t("9bf2").f,
+                    u = Function.prototype,
+                    f = u.toString,
+                    c = /^\s*function ([^ (]*)/,
                     d = "name";
-                o && !(d in s) && i(s, d, {
+                o && !(d in u) && l(u, d, {
                     configurable: !0,
                     get: function() {
                         try {
-                            return c.call(this).match(f)[1]
+                            return f.call(this).match(c)[1]
                         } catch {
                             return ""
                         }
                     }
                 })
             },
-            b622: function(r, u, t) {
+            b622: function(r, s, t) {
                 var o = t("da84"),
-                    i = t("5692"),
-                    s = t("5135"),
-                    c = t("90e3"),
-                    f = t("4930"),
+                    l = t("5692"),
+                    u = t("5135"),
+                    f = t("90e3"),
+                    c = t("4930"),
                     d = t("fdbf"),
-                    v = i("wks"),
-                    h = o.Symbol,
-                    p = d ? h : h && h.withoutSetter || c;
-                r.exports = function(g) {
-                    return s(v, g) || (f && s(h, g) ? v[g] = h[g] : v[g] = p("Symbol." + g)), v[g]
+                    v = l("wks"),
+                    p = o.Symbol,
+                    h = d ? p : p && p.withoutSetter || f;
+                r.exports = function(m) {
+                    return u(v, m) || (c && u(p, m) ? v[m] = p[m] : v[m] = h("Symbol." + m)), v[m]
                 }
             },
-            b64b: function(r, u, t) {
+            b64b: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("7b0b"),
-                    s = t("df75"),
-                    c = t("d039"),
-                    f = c(function() {
-                        s(1)
+                    l = t("7b0b"),
+                    u = t("df75"),
+                    f = t("d039"),
+                    c = f(function() {
+                        u(1)
                     });
                 o({
                     target: "Object",
                     stat: !0,
-                    forced: f
+                    forced: c
                 }, {
                     keys: function(v) {
-                        return s(i(v))
+                        return u(l(v))
                     }
                 })
             },
-            b727: function(r, u, t) {
+            b727: function(r, s, t) {
                 var o = t("0366"),
-                    i = t("44ad"),
-                    s = t("7b0b"),
-                    c = t("50c4"),
-                    f = t("65f0"),
+                    l = t("44ad"),
+                    u = t("7b0b"),
+                    f = t("50c4"),
+                    c = t("65f0"),
                     d = [].push,
-                    v = function(h) {
-                        var p = h == 1,
-                            g = h == 2,
-                            b = h == 3,
-                            S = h == 4,
-                            P = h == 6,
-                            x = h == 5 || P;
-                        return function(C, I, j, L) {
-                            for (var T = s(C), O = i(T), D = o(I, j, 3), G = c(O.length), A = 0, M = L || f, X = p ? M(C, G) : g ? M(C, 0) : void 0, R, F; G > A; A++)
-                                if ((x || A in O) && (R = O[A], F = D(R, A, T), h)) {
-                                    if (p) X[A] = F;
-                                    else if (F) switch (h) {
+                    v = function(p) {
+                        var h = p == 1,
+                            m = p == 2,
+                            g = p == 3,
+                            y = p == 4,
+                            O = p == 6,
+                            E = p == 5 || O;
+                        return function(C, T, $, L) {
+                            for (var I = u(C), j = l(I), P = o(T, $, 3), M = f(j.length), D = 0, R = L || c, H = h ? R(C, M) : m ? R(C, 0) : void 0, F, N; M > D; D++)
+                                if ((E || D in j) && (F = j[D], N = P(F, D, I), p)) {
+                                    if (h) H[D] = N;
+                                    else if (N) switch (p) {
                                         case 3:
                                             return !0;
                                         case 5:
-                                            return R;
+                                            return F;
                                         case 6:
-                                            return A;
+                                            return D;
                                         case 2:
-                                            d.call(X, R)
-                                    } else if (S) return !1
-                                } return P ? -1 : b || S ? S : X
+                                            d.call(H, F)
+                                    } else if (y) return !1
+                                } return O ? -1 : g || y ? y : H
                         }
                     };
                 r.exports = {
                     forEach: v(0),
                     map: v(1),
                     filter: v(2),
                     some: v(3),
                     every: v(4),
                     find: v(5),
                     findIndex: v(6)
                 }
             },
-            c04e: function(r, u, t) {
+            c04e: function(r, s, t) {
                 var o = t("861d");
-                r.exports = function(i, s) {
-                    if (!o(i)) return i;
-                    var c, f;
-                    if (s && typeof(c = i.toString) == "function" && !o(f = c.call(i)) || typeof(c = i.valueOf) == "function" && !o(f = c.call(i)) || !s && typeof(c = i.toString) == "function" && !o(f = c.call(i))) return f;
+                r.exports = function(l, u) {
+                    if (!o(l)) return l;
+                    var f, c;
+                    if (u && typeof(f = l.toString) == "function" && !o(c = f.call(l)) || typeof(f = l.valueOf) == "function" && !o(c = f.call(l)) || !u && typeof(f = l.toString) == "function" && !o(c = f.call(l))) return c;
                     throw TypeError("Can't convert object to primitive value")
                 }
             },
-            c430: function(r, u) {
+            c430: function(r, s) {
                 r.exports = !1
             },
-            c6b6: function(r, u) {
+            c6b6: function(r, s) {
                 var t = {}.toString;
                 r.exports = function(o) {
                     return t.call(o).slice(8, -1)
                 }
             },
-            c6cd: function(r, u, t) {
+            c6cd: function(r, s, t) {
                 var o = t("da84"),
-                    i = t("ce4e"),
-                    s = "__core-js_shared__",
-                    c = o[s] || i(s, {});
-                r.exports = c
+                    l = t("ce4e"),
+                    u = "__core-js_shared__",
+                    f = o[u] || l(u, {});
+                r.exports = f
             },
-            c740: function(r, u, t) {
+            c740: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("b727").findIndex,
-                    s = t("44d2"),
-                    c = t("ae40"),
-                    f = "findIndex",
+                    l = t("b727").findIndex,
+                    u = t("44d2"),
+                    f = t("ae40"),
+                    c = "findIndex",
                     d = !0,
-                    v = c(f);
-                f in [] && Array(1)[f](function() {
+                    v = f(c);
+                c in [] && Array(1)[c](function() {
                     d = !1
                 }), o({
                     target: "Array",
                     proto: !0,
                     forced: d || !v
                 }, {
-                    findIndex: function(p) {
-                        return i(this, p, arguments.length > 1 ? arguments[1] : void 0)
+                    findIndex: function(h) {
+                        return l(this, h, arguments.length > 1 ? arguments[1] : void 0)
                     }
-                }), s(f)
+                }), u(c)
             },
-            c8ba: function(r, u) {
+            c8ba: function(r, s) {
                 var t;
                 t = function() {
                     return this
                 }();
                 try {
                     t = t || new Function("return this")()
                 } catch {
                     typeof window == "object" && (t = window)
                 }
                 r.exports = t
             },
-            c975: function(r, u, t) {
+            c975: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("4d64").indexOf,
-                    s = t("a640"),
-                    c = t("ae40"),
-                    f = [].indexOf,
-                    d = !!f && 1 / [1].indexOf(1, -0) < 0,
-                    v = s("indexOf"),
-                    h = c("indexOf", {
+                    l = t("4d64").indexOf,
+                    u = t("a640"),
+                    f = t("ae40"),
+                    c = [].indexOf,
+                    d = !!c && 1 / [1].indexOf(1, -0) < 0,
+                    v = u("indexOf"),
+                    p = f("indexOf", {
                         ACCESSORS: !0,
                         1: 0
                     });
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: d || !v || !h
+                    forced: d || !v || !p
                 }, {
-                    indexOf: function(g) {
-                        return d ? f.apply(this, arguments) || 0 : i(this, g, arguments.length > 1 ? arguments[1] : void 0)
+                    indexOf: function(m) {
+                        return d ? c.apply(this, arguments) || 0 : l(this, m, arguments.length > 1 ? arguments[1] : void 0)
                     }
                 })
             },
-            ca84: function(r, u, t) {
+            ca84: function(r, s, t) {
                 var o = t("5135"),
-                    i = t("fc6a"),
-                    s = t("4d64").indexOf,
-                    c = t("d012");
-                r.exports = function(f, d) {
-                    var v = i(f),
-                        h = 0,
-                        p = [],
-                        g;
-                    for (g in v) !o(c, g) && o(v, g) && p.push(g);
-                    for (; d.length > h;) o(v, g = d[h++]) && (~s(p, g) || p.push(g));
-                    return p
+                    l = t("fc6a"),
+                    u = t("4d64").indexOf,
+                    f = t("d012");
+                r.exports = function(c, d) {
+                    var v = l(c),
+                        p = 0,
+                        h = [],
+                        m;
+                    for (m in v) !o(f, m) && o(v, m) && h.push(m);
+                    for (; d.length > p;) o(v, m = d[p++]) && (~u(h, m) || h.push(m));
+                    return h
                 }
             },
-            caad: function(r, u, t) {
+            caad: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("4d64").includes,
-                    s = t("44d2"),
-                    c = t("ae40"),
-                    f = c("indexOf", {
+                    l = t("4d64").includes,
+                    u = t("44d2"),
+                    f = t("ae40"),
+                    c = f("indexOf", {
                         ACCESSORS: !0,
                         1: 0
                     });
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: !f
+                    forced: !c
                 }, {
                     includes: function(v) {
-                        return i(this, v, arguments.length > 1 ? arguments[1] : void 0)
+                        return l(this, v, arguments.length > 1 ? arguments[1] : void 0)
                     }
-                }), s("includes")
+                }), u("includes")
             },
-            cc12: function(r, u, t) {
+            cc12: function(r, s, t) {
                 var o = t("da84"),
-                    i = t("861d"),
-                    s = o.document,
-                    c = i(s) && i(s.createElement);
-                r.exports = function(f) {
-                    return c ? s.createElement(f) : {}
+                    l = t("861d"),
+                    u = o.document,
+                    f = l(u) && l(u.createElement);
+                r.exports = function(c) {
+                    return f ? u.createElement(c) : {}
                 }
             },
-            ce4e: function(r, u, t) {
+            ce4e: function(r, s, t) {
                 var o = t("da84"),
-                    i = t("9112");
-                r.exports = function(s, c) {
+                    l = t("9112");
+                r.exports = function(u, f) {
                     try {
-                        i(o, s, c)
+                        l(o, u, f)
                     } catch {
-                        o[s] = c
+                        o[u] = f
                     }
-                    return c
+                    return f
                 }
             },
-            d012: function(r, u) {
+            d012: function(r, s) {
                 r.exports = {}
             },
-            d039: function(r, u) {
+            d039: function(r, s) {
                 r.exports = function(t) {
                     try {
                         return !!t()
                     } catch {
                         return !0
                     }
                 }
             },
-            d066: function(r, u, t) {
+            d066: function(r, s, t) {
                 var o = t("428f"),
-                    i = t("da84"),
-                    s = function(c) {
-                        return typeof c == "function" ? c : void 0
+                    l = t("da84"),
+                    u = function(f) {
+                        return typeof f == "function" ? f : void 0
                     };
-                r.exports = function(c, f) {
-                    return arguments.length < 2 ? s(o[c]) || s(i[c]) : o[c] && o[c][f] || i[c] && i[c][f]
+                r.exports = function(f, c) {
+                    return arguments.length < 2 ? u(o[f]) || u(l[f]) : o[f] && o[f][c] || l[f] && l[f][c]
                 }
             },
-            d1e7: function(r, u, t) {
+            d1e7: function(r, s, t) {
                 var o = {}.propertyIsEnumerable,
-                    i = Object.getOwnPropertyDescriptor,
-                    s = i && !o.call({
+                    l = Object.getOwnPropertyDescriptor,
+                    u = l && !o.call({
                         1: 2
                     }, 1);
-                u.f = s ? function(f) {
-                    var d = i(this, f);
+                s.f = u ? function(c) {
+                    var d = l(this, c);
                     return !!d && d.enumerable
                 } : o
             },
-            d28b: function(r, u, t) {
+            d28b: function(r, s, t) {
                 var o = t("746f");
                 o("iterator")
             },
-            d2bb: function(r, u, t) {
+            d2bb: function(r, s, t) {
                 var o = t("825a"),
-                    i = t("3bbe");
+                    l = t("3bbe");
                 r.exports = Object.setPrototypeOf || ("__proto__" in {} ? function() {
-                    var s = !1,
-                        c = {},
-                        f;
+                    var u = !1,
+                        f = {},
+                        c;
                     try {
-                        f = Object.getOwnPropertyDescriptor(Object.prototype, "__proto__").set, f.call(c, []), s = c instanceof Array
+                        c = Object.getOwnPropertyDescriptor(Object.prototype, "__proto__").set, c.call(f, []), u = f instanceof Array
                     } catch {}
-                    return function(v, h) {
-                        return o(v), i(h), s ? f.call(v, h) : v.__proto__ = h, v
+                    return function(v, p) {
+                        return o(v), l(p), u ? c.call(v, p) : v.__proto__ = p, v
                     }
                 }() : void 0)
             },
-            d3b7: function(r, u, t) {
+            d3b7: function(r, s, t) {
                 var o = t("00ee"),
-                    i = t("6eeb"),
-                    s = t("b041");
-                o || i(Object.prototype, "toString", s, {
+                    l = t("6eeb"),
+                    u = t("b041");
+                o || l(Object.prototype, "toString", u, {
                     unsafe: !0
                 })
             },
-            d44e: function(r, u, t) {
+            d44e: function(r, s, t) {
                 var o = t("9bf2").f,
-                    i = t("5135"),
-                    s = t("b622"),
-                    c = s("toStringTag");
-                r.exports = function(f, d, v) {
-                    f && !i(f = v ? f : f.prototype, c) && o(f, c, {
+                    l = t("5135"),
+                    u = t("b622"),
+                    f = u("toStringTag");
+                r.exports = function(c, d, v) {
+                    c && !l(c = v ? c : c.prototype, f) && o(c, f, {
                         configurable: !0,
                         value: d
                     })
                 }
             },
-            d58f: function(r, u, t) {
+            d58f: function(r, s, t) {
                 var o = t("1c0b"),
-                    i = t("7b0b"),
-                    s = t("44ad"),
-                    c = t("50c4"),
-                    f = function(d) {
-                        return function(v, h, p, g) {
-                            o(h);
-                            var b = i(v),
-                                S = s(b),
-                                P = c(b.length),
-                                x = d ? P - 1 : 0,
+                    l = t("7b0b"),
+                    u = t("44ad"),
+                    f = t("50c4"),
+                    c = function(d) {
+                        return function(v, p, h, m) {
+                            o(p);
+                            var g = l(v),
+                                y = u(g),
+                                O = f(g.length),
+                                E = d ? O - 1 : 0,
                                 C = d ? -1 : 1;
-                            if (p < 2)
+                            if (h < 2)
                                 for (;;) {
-                                    if (x in S) {
-                                        g = S[x], x += C;
+                                    if (E in y) {
+                                        m = y[E], E += C;
                                         break
                                     }
-                                    if (x += C, d ? x < 0 : P <= x) throw TypeError("Reduce of empty array with no initial value")
+                                    if (E += C, d ? E < 0 : O <= E) throw TypeError("Reduce of empty array with no initial value")
                                 }
-                            for (; d ? x >= 0 : P > x; x += C) x in S && (g = h(g, S[x], x, b));
-                            return g
+                            for (; d ? E >= 0 : O > E; E += C) E in y && (m = p(m, y[E], E, g));
+                            return m
                         }
                     };
                 r.exports = {
-                    left: f(!1),
-                    right: f(!0)
+                    left: c(!1),
+                    right: c(!0)
                 }
             },
-            d784: function(r, u, t) {
+            d784: function(r, s, t) {
                 t("ac1f");
                 var o = t("6eeb"),
-                    i = t("d039"),
-                    s = t("b622"),
-                    c = t("9263"),
-                    f = t("9112"),
-                    d = s("species"),
-                    v = !i(function() {
-                        var S = /./;
-                        return S.exec = function() {
-                            var P = [];
-                            return P.groups = {
+                    l = t("d039"),
+                    u = t("b622"),
+                    f = t("9263"),
+                    c = t("9112"),
+                    d = u("species"),
+                    v = !l(function() {
+                        var y = /./;
+                        return y.exec = function() {
+                            var O = [];
+                            return O.groups = {
                                 a: "7"
-                            }, P
-                        }, "".replace(S, "$<a>") !== "7"
+                            }, O
+                        }, "".replace(y, "$<a>") !== "7"
                     }),
-                    h = function() {
+                    p = function() {
                         return "a".replace(/./, "$0") === "$0"
                     }(),
-                    p = s("replace"),
-                    g = function() {
-                        return /./ [p] ? /./ [p]("a", "$0") === "" : !1
+                    h = u("replace"),
+                    m = function() {
+                        return /./ [h] ? /./ [h]("a", "$0") === "" : !1
                     }(),
-                    b = !i(function() {
-                        var S = /(?:)/,
-                            P = S.exec;
-                        S.exec = function() {
-                            return P.apply(this, arguments)
+                    g = !l(function() {
+                        var y = /(?:)/,
+                            O = y.exec;
+                        y.exec = function() {
+                            return O.apply(this, arguments)
                         };
-                        var x = "ab".split(S);
-                        return x.length !== 2 || x[0] !== "a" || x[1] !== "b"
+                        var E = "ab".split(y);
+                        return E.length !== 2 || E[0] !== "a" || E[1] !== "b"
                     });
-                r.exports = function(S, P, x, C) {
-                    var I = s(S),
-                        j = !i(function() {
-                            var A = {};
-                            return A[I] = function() {
+                r.exports = function(y, O, E, C) {
+                    var T = u(y),
+                        $ = !l(function() {
+                            var D = {};
+                            return D[T] = function() {
                                 return 7
-                            }, "" [S](A) != 7
+                            }, "" [y](D) != 7
                         }),
-                        L = j && !i(function() {
-                            var A = !1,
-                                M = /a/;
-                            return S === "split" && (M = {}, M.constructor = {}, M.constructor[d] = function() {
-                                return M
-                            }, M.flags = "", M[I] = /./ [I]), M.exec = function() {
-                                return A = !0, null
-                            }, M[I](""), !A
+                        L = $ && !l(function() {
+                            var D = !1,
+                                R = /a/;
+                            return y === "split" && (R = {}, R.constructor = {}, R.constructor[d] = function() {
+                                return R
+                            }, R.flags = "", R[T] = /./ [T]), R.exec = function() {
+                                return D = !0, null
+                            }, R[T](""), !D
                         });
-                    if (!j || !L || S === "replace" && !(v && h && !g) || S === "split" && !b) {
-                        var T = /./ [I],
-                            O = x(I, "" [S], function(A, M, X, R, F) {
-                                return M.exec === c ? j && !F ? {
+                    if (!$ || !L || y === "replace" && !(v && p && !m) || y === "split" && !g) {
+                        var I = /./ [T],
+                            j = E(T, "" [y], function(D, R, H, F, N) {
+                                return R.exec === f ? $ && !N ? {
                                     done: !0,
-                                    value: T.call(M, X, R)
+                                    value: I.call(R, H, F)
                                 } : {
                                     done: !0,
-                                    value: A.call(X, M, R)
+                                    value: D.call(H, R, F)
                                 } : {
                                     done: !1
                                 }
                             }, {
-                                REPLACE_KEEPS_$0: h,
-                                REGEXP_REPLACE_SUBSTITUTES_UNDEFINED_CAPTURE: g
+                                REPLACE_KEEPS_$0: p,
+                                REGEXP_REPLACE_SUBSTITUTES_UNDEFINED_CAPTURE: m
                             }),
-                            D = O[0],
-                            G = O[1];
-                        o(String.prototype, S, D), o(RegExp.prototype, I, P == 2 ? function(A, M) {
-                            return G.call(A, this, M)
-                        } : function(A) {
-                            return G.call(A, this)
+                            P = j[0],
+                            M = j[1];
+                        o(String.prototype, y, P), o(RegExp.prototype, T, O == 2 ? function(D, R) {
+                            return M.call(D, this, R)
+                        } : function(D) {
+                            return M.call(D, this)
                         })
                     }
-                    C && f(RegExp.prototype[I], "sham", !0)
+                    C && c(RegExp.prototype[T], "sham", !0)
                 }
             },
-            d81d: function(r, u, t) {
+            d81d: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("b727").map,
-                    s = t("1dde"),
-                    c = t("ae40"),
-                    f = s("map"),
-                    d = c("map");
+                    l = t("b727").map,
+                    u = t("1dde"),
+                    f = t("ae40"),
+                    c = u("map"),
+                    d = f("map");
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: !f || !d
+                    forced: !c || !d
                 }, {
-                    map: function(h) {
-                        return i(this, h, arguments.length > 1 ? arguments[1] : void 0)
+                    map: function(p) {
+                        return l(this, p, arguments.length > 1 ? arguments[1] : void 0)
                     }
                 })
             },
-            da84: function(r, u, t) {
+            da84: function(r, s, t) {
                 (function(o) {
-                    var i = function(s) {
-                        return s && s.Math == Math && s
+                    var l = function(u) {
+                        return u && u.Math == Math && u
                     };
-                    r.exports = i(typeof globalThis == "object" && globalThis) || i(typeof window == "object" && window) || i(typeof self == "object" && self) || i(typeof o == "object" && o) || Function("return this")()
+                    r.exports = l(typeof globalThis == "object" && globalThis) || l(typeof window == "object" && window) || l(typeof self == "object" && self) || l(typeof o == "object" && o) || Function("return this")()
                 }).call(this, t("c8ba"))
             },
-            dbb4: function(r, u, t) {
+            dbb4: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("83ab"),
-                    s = t("56ef"),
-                    c = t("fc6a"),
-                    f = t("06cf"),
+                    l = t("83ab"),
+                    u = t("56ef"),
+                    f = t("fc6a"),
+                    c = t("06cf"),
                     d = t("8418");
                 o({
                     target: "Object",
                     stat: !0,
-                    sham: !i
+                    sham: !l
                 }, {
-                    getOwnPropertyDescriptors: function(h) {
-                        for (var p = c(h), g = f.f, b = s(p), S = {}, P = 0, x, C; b.length > P;) C = g(p, x = b[P++]), C !== void 0 && d(S, x, C);
-                        return S
+                    getOwnPropertyDescriptors: function(p) {
+                        for (var h = f(p), m = c.f, g = u(h), y = {}, O = 0, E, C; g.length > O;) C = m(h, E = g[O++]), C !== void 0 && d(y, E, C);
+                        return y
                     }
                 })
             },
-            dbf1: function(r, u, t) {
+            dbf1: function(r, s, t) {
                 (function(o) {
-                    t.d(u, "a", function() {
-                        return s
+                    t.d(s, "a", function() {
+                        return u
                     });
 
-                    function i() {
+                    function l() {
                         return typeof window < "u" ? window.console : o.console
                     }
-                    var s = i()
+                    var u = l()
                 }).call(this, t("c8ba"))
             },
-            ddb0: function(r, u, t) {
+            ddb0: function(r, s, t) {
                 var o = t("da84"),
-                    i = t("fdbc"),
-                    s = t("e260"),
-                    c = t("9112"),
-                    f = t("b622"),
-                    d = f("iterator"),
-                    v = f("toStringTag"),
-                    h = s.values;
-                for (var p in i) {
-                    var g = o[p],
-                        b = g && g.prototype;
-                    if (b) {
-                        if (b[d] !== h) try {
-                            c(b, d, h)
+                    l = t("fdbc"),
+                    u = t("e260"),
+                    f = t("9112"),
+                    c = t("b622"),
+                    d = c("iterator"),
+                    v = c("toStringTag"),
+                    p = u.values;
+                for (var h in l) {
+                    var m = o[h],
+                        g = m && m.prototype;
+                    if (g) {
+                        if (g[d] !== p) try {
+                            f(g, d, p)
                         } catch {
-                            b[d] = h
+                            g[d] = p
                         }
-                        if (b[v] || c(b, v, p), i[p]) {
-                            for (var S in s)
-                                if (b[S] !== s[S]) try {
-                                    c(b, S, s[S])
+                        if (g[v] || f(g, v, h), l[h]) {
+                            for (var y in u)
+                                if (g[y] !== u[y]) try {
+                                    f(g, y, u[y])
                                 } catch {
-                                    b[S] = s[S]
+                                    g[y] = u[y]
                                 }
                         }
                     }
                 }
             },
-            df75: function(r, u, t) {
+            df75: function(r, s, t) {
                 var o = t("ca84"),
-                    i = t("7839");
-                r.exports = Object.keys || function(c) {
-                    return o(c, i)
+                    l = t("7839");
+                r.exports = Object.keys || function(f) {
+                    return o(f, l)
                 }
             },
-            e01a: function(r, u, t) {
+            e01a: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("83ab"),
-                    s = t("da84"),
-                    c = t("5135"),
-                    f = t("861d"),
+                    l = t("83ab"),
+                    u = t("da84"),
+                    f = t("5135"),
+                    c = t("861d"),
                     d = t("9bf2").f,
                     v = t("e893"),
-                    h = s.Symbol;
-                if (i && typeof h == "function" && (!("description" in h.prototype) || h().description !== void 0)) {
-                    var p = {},
-                        g = function() {
-                            var I = arguments.length < 1 || arguments[0] === void 0 ? void 0 : String(arguments[0]),
-                                j = this instanceof g ? new h(I) : I === void 0 ? h() : h(I);
-                            return I === "" && (p[j] = !0), j
+                    p = u.Symbol;
+                if (l && typeof p == "function" && (!("description" in p.prototype) || p().description !== void 0)) {
+                    var h = {},
+                        m = function() {
+                            var T = arguments.length < 1 || arguments[0] === void 0 ? void 0 : String(arguments[0]),
+                                $ = this instanceof m ? new p(T) : T === void 0 ? p() : p(T);
+                            return T === "" && (h[$] = !0), $
                         };
-                    v(g, h);
-                    var b = g.prototype = h.prototype;
-                    b.constructor = g;
-                    var S = b.toString,
-                        P = String(h("test")) == "Symbol(test)",
-                        x = /^Symbol\((.*)\)[^)]+$/;
-                    d(b, "description", {
+                    v(m, p);
+                    var g = m.prototype = p.prototype;
+                    g.constructor = m;
+                    var y = g.toString,
+                        O = String(p("test")) == "Symbol(test)",
+                        E = /^Symbol\((.*)\)[^)]+$/;
+                    d(g, "description", {
                         configurable: !0,
                         get: function() {
-                            var I = f(this) ? this.valueOf() : this,
-                                j = S.call(I);
-                            if (c(p, I)) return "";
-                            var L = P ? j.slice(7, -1) : j.replace(x, "$1");
+                            var T = c(this) ? this.valueOf() : this,
+                                $ = y.call(T);
+                            if (f(h, T)) return "";
+                            var L = O ? $.slice(7, -1) : $.replace(E, "$1");
                             return L === "" ? void 0 : L
                         }
                     }), o({
                         global: !0,
                         forced: !0
                     }, {
-                        Symbol: g
+                        Symbol: m
                     })
                 }
             },
-            e163: function(r, u, t) {
+            e163: function(r, s, t) {
                 var o = t("5135"),
-                    i = t("7b0b"),
-                    s = t("f772"),
-                    c = t("e177"),
-                    f = s("IE_PROTO"),
+                    l = t("7b0b"),
+                    u = t("f772"),
+                    f = t("e177"),
+                    c = u("IE_PROTO"),
                     d = Object.prototype;
-                r.exports = c ? Object.getPrototypeOf : function(v) {
-                    return v = i(v), o(v, f) ? v[f] : typeof v.constructor == "function" && v instanceof v.constructor ? v.constructor.prototype : v instanceof Object ? d : null
+                r.exports = f ? Object.getPrototypeOf : function(v) {
+                    return v = l(v), o(v, c) ? v[c] : typeof v.constructor == "function" && v instanceof v.constructor ? v.constructor.prototype : v instanceof Object ? d : null
                 }
             },
-            e177: function(r, u, t) {
+            e177: function(r, s, t) {
                 var o = t("d039");
                 r.exports = !o(function() {
-                    function i() {}
-                    return i.prototype.constructor = null, Object.getPrototypeOf(new i) !== i.prototype
+                    function l() {}
+                    return l.prototype.constructor = null, Object.getPrototypeOf(new l) !== l.prototype
                 })
             },
-            e260: function(r, u, t) {
+            e260: function(r, s, t) {
                 var o = t("fc6a"),
-                    i = t("44d2"),
-                    s = t("3f8c"),
-                    c = t("69f3"),
-                    f = t("7dd0"),
+                    l = t("44d2"),
+                    u = t("3f8c"),
+                    f = t("69f3"),
+                    c = t("7dd0"),
                     d = "Array Iterator",
-                    v = c.set,
-                    h = c.getterFor(d);
-                r.exports = f(Array, "Array", function(p, g) {
+                    v = f.set,
+                    p = f.getterFor(d);
+                r.exports = c(Array, "Array", function(h, m) {
                     v(this, {
                         type: d,
-                        target: o(p),
+                        target: o(h),
                         index: 0,
-                        kind: g
+                        kind: m
                     })
                 }, function() {
-                    var p = h(this),
-                        g = p.target,
-                        b = p.kind,
-                        S = p.index++;
-                    return !g || S >= g.length ? (p.target = void 0, {
+                    var h = p(this),
+                        m = h.target,
+                        g = h.kind,
+                        y = h.index++;
+                    return !m || y >= m.length ? (h.target = void 0, {
                         value: void 0,
                         done: !0
-                    }) : b == "keys" ? {
-                        value: S,
+                    }) : g == "keys" ? {
+                        value: y,
                         done: !1
-                    } : b == "values" ? {
-                        value: g[S],
+                    } : g == "values" ? {
+                        value: m[y],
                         done: !1
                     } : {
-                        value: [S, g[S]],
+                        value: [y, m[y]],
                         done: !1
                     }
-                }, "values"), s.Arguments = s.Array, i("keys"), i("values"), i("entries")
+                }, "values"), u.Arguments = u.Array, l("keys"), l("values"), l("entries")
             },
-            e439: function(r, u, t) {
+            e439: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("d039"),
-                    s = t("fc6a"),
-                    c = t("06cf").f,
-                    f = t("83ab"),
-                    d = i(function() {
-                        c(1)
+                    l = t("d039"),
+                    u = t("fc6a"),
+                    f = t("06cf").f,
+                    c = t("83ab"),
+                    d = l(function() {
+                        f(1)
                     }),
-                    v = !f || d;
+                    v = !c || d;
                 o({
                     target: "Object",
                     stat: !0,
                     forced: v,
-                    sham: !f
+                    sham: !c
                 }, {
-                    getOwnPropertyDescriptor: function(p, g) {
-                        return c(s(p), g)
+                    getOwnPropertyDescriptor: function(h, m) {
+                        return f(u(h), m)
                     }
                 })
             },
-            e538: function(r, u, t) {
+            e538: function(r, s, t) {
                 var o = t("b622");
-                u.f = o
+                s.f = o
             },
-            e893: function(r, u, t) {
+            e893: function(r, s, t) {
                 var o = t("5135"),
-                    i = t("56ef"),
-                    s = t("06cf"),
-                    c = t("9bf2");
-                r.exports = function(f, d) {
-                    for (var v = i(d), h = c.f, p = s.f, g = 0; g < v.length; g++) {
-                        var b = v[g];
-                        o(f, b) || h(f, b, p(d, b))
+                    l = t("56ef"),
+                    u = t("06cf"),
+                    f = t("9bf2");
+                r.exports = function(c, d) {
+                    for (var v = l(d), p = f.f, h = u.f, m = 0; m < v.length; m++) {
+                        var g = v[m];
+                        o(c, g) || p(c, g, h(d, g))
                     }
                 }
             },
-            e8b5: function(r, u, t) {
+            e8b5: function(r, s, t) {
                 var o = t("c6b6");
-                r.exports = Array.isArray || function(s) {
-                    return o(s) == "Array"
+                r.exports = Array.isArray || function(u) {
+                    return o(u) == "Array"
                 }
             },
-            e95a: function(r, u, t) {
+            e95a: function(r, s, t) {
                 var o = t("b622"),
-                    i = t("3f8c"),
-                    s = o("iterator"),
-                    c = Array.prototype;
-                r.exports = function(f) {
-                    return f !== void 0 && (i.Array === f || c[s] === f)
+                    l = t("3f8c"),
+                    u = o("iterator"),
+                    f = Array.prototype;
+                r.exports = function(c) {
+                    return c !== void 0 && (l.Array === c || f[u] === c)
                 }
             },
-            f5df: function(r, u, t) {
+            f5df: function(r, s, t) {
                 var o = t("00ee"),
-                    i = t("c6b6"),
-                    s = t("b622"),
-                    c = s("toStringTag"),
-                    f = i(function() {
+                    l = t("c6b6"),
+                    u = t("b622"),
+                    f = u("toStringTag"),
+                    c = l(function() {
                         return arguments
                     }()) == "Arguments",
-                    d = function(v, h) {
+                    d = function(v, p) {
                         try {
-                            return v[h]
+                            return v[p]
                         } catch {}
                     };
-                r.exports = o ? i : function(v) {
-                    var h, p, g;
-                    return v === void 0 ? "Undefined" : v === null ? "Null" : typeof(p = d(h = Object(v), c)) == "string" ? p : f ? i(h) : (g = i(h)) == "Object" && typeof h.callee == "function" ? "Arguments" : g
+                r.exports = o ? l : function(v) {
+                    var p, h, m;
+                    return v === void 0 ? "Undefined" : v === null ? "Null" : typeof(h = d(p = Object(v), f)) == "string" ? h : c ? l(p) : (m = l(p)) == "Object" && typeof p.callee == "function" ? "Arguments" : m
                 }
             },
-            f772: function(r, u, t) {
+            f772: function(r, s, t) {
                 var o = t("5692"),
-                    i = t("90e3"),
-                    s = o("keys");
-                r.exports = function(c) {
-                    return s[c] || (s[c] = i(c))
+                    l = t("90e3"),
+                    u = o("keys");
+                r.exports = function(f) {
+                    return u[f] || (u[f] = l(f))
                 }
             },
-            fb15: function(r, u, t) {
-                if (t.r(u), typeof window < "u") {
+            fb15: function(r, s, t) {
+                if (t.r(s), typeof window < "u") {
                     var o = window.document.currentScript; {
-                        var i = t("8875");
-                        o = i(), "currentScript" in document || Object.defineProperty(document, "currentScript", {
-                            get: i
+                        var l = t("8875");
+                        o = l(), "currentScript" in document || Object.defineProperty(document, "currentScript", {
+                            get: l
                         })
                     }
-                    var s = o && o.src.match(/(.+\/)[^/]+\.js(\?.*)?$/);
-                    s && (t.p = s[1])
+                    var u = o && o.src.match(/(.+\/)[^/]+\.js(\?.*)?$/);
+                    u && (t.p = u[1])
                 }
                 t("99af"), t("4de4"), t("4160"), t("c975"), t("d81d"), t("a434"), t("159b"), t("a4d3"), t("e439"), t("dbb4"), t("b64b");
 
-                function c(y, m, E) {
-                    return m in y ? Object.defineProperty(y, m, {
-                        value: E,
+                function f(S, b, x) {
+                    return b in S ? Object.defineProperty(S, b, {
+                        value: x,
                         enumerable: !0,
                         configurable: !0,
                         writable: !0
-                    }) : y[m] = E, y
+                    }) : S[b] = x, S
                 }
 
-                function f(y, m) {
-                    var E = Object.keys(y);
+                function c(S, b) {
+                    var x = Object.keys(S);
                     if (Object.getOwnPropertySymbols) {
-                        var w = Object.getOwnPropertySymbols(y);
-                        m && (w = w.filter(function($) {
-                            return Object.getOwnPropertyDescriptor(y, $).enumerable
-                        })), E.push.apply(E, w)
-                    }
-                    return E
+                        var A = Object.getOwnPropertySymbols(S);
+                        b && (A = A.filter(function(V) {
+                            return Object.getOwnPropertyDescriptor(S, V).enumerable
+                        })), x.push.apply(x, A)
+                    }
+                    return x
                 }
 
-                function d(y) {
-                    for (var m = 1; m < arguments.length; m++) {
-                        var E = arguments[m] != null ? arguments[m] : {};
-                        m % 2 ? f(Object(E), !0).forEach(function(w) {
-                            c(y, w, E[w])
-                        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(y, Object.getOwnPropertyDescriptors(E)) : f(Object(E)).forEach(function(w) {
-                            Object.defineProperty(y, w, Object.getOwnPropertyDescriptor(E, w))
+                function d(S) {
+                    for (var b = 1; b < arguments.length; b++) {
+                        var x = arguments[b] != null ? arguments[b] : {};
+                        b % 2 ? c(Object(x), !0).forEach(function(A) {
+                            f(S, A, x[A])
+                        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(S, Object.getOwnPropertyDescriptors(x)) : c(Object(x)).forEach(function(A) {
+                            Object.defineProperty(S, A, Object.getOwnPropertyDescriptor(x, A))
                         })
                     }
-                    return y
+                    return S
                 }
 
-                function v(y) {
-                    if (Array.isArray(y)) return y
+                function v(S) {
+                    if (Array.isArray(S)) return S
                 }
                 t("e01a"), t("d28b"), t("e260"), t("d3b7"), t("3ca3"), t("ddb0");
 
-                function h(y, m) {
-                    if (!(typeof Symbol > "u" || !(Symbol.iterator in Object(y)))) {
-                        var E = [],
-                            w = !0,
-                            $ = !1,
-                            z = void 0;
+                function p(S, b) {
+                    if (!(typeof Symbol > "u" || !(Symbol.iterator in Object(S)))) {
+                        var x = [],
+                            A = !0,
+                            V = !1,
+                            J = void 0;
                         try {
-                            for (var q = y[Symbol.iterator](), ot; !(w = (ot = q.next()).done) && (E.push(ot.value), !(m && E.length === m)); w = !0);
+                            for (var _ = S[Symbol.iterator](), at; !(A = (at = _.next()).done) && (x.push(at.value), !(b && x.length === b)); A = !0);
                         } catch (yt) {
-                            $ = !0, z = yt
+                            V = !0, J = yt
                         } finally {
                             try {
-                                !w && q.return != null && q.return()
+                                !A && _.return != null && _.return()
                             } finally {
-                                if ($) throw z
+                                if (V) throw J
                             }
                         }
-                        return E
+                        return x
                     }
                 }
                 t("a630"), t("fb6a"), t("b0c0"), t("25f0");
 
-                function p(y, m) {
-                    (m == null || m > y.length) && (m = y.length);
-                    for (var E = 0, w = new Array(m); E < m; E++) w[E] = y[E];
-                    return w
+                function h(S, b) {
+                    (b == null || b > S.length) && (b = S.length);
+                    for (var x = 0, A = new Array(b); x < b; x++) A[x] = S[x];
+                    return A
                 }
 
-                function g(y, m) {
-                    if (!!y) {
-                        if (typeof y == "string") return p(y, m);
-                        var E = Object.prototype.toString.call(y).slice(8, -1);
-                        if (E === "Object" && y.constructor && (E = y.constructor.name), E === "Map" || E === "Set") return Array.from(y);
-                        if (E === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(E)) return p(y, m)
+                function m(S, b) {
+                    if (!!S) {
+                        if (typeof S == "string") return h(S, b);
+                        var x = Object.prototype.toString.call(S).slice(8, -1);
+                        if (x === "Object" && S.constructor && (x = S.constructor.name), x === "Map" || x === "Set") return Array.from(S);
+                        if (x === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(x)) return h(S, b)
                     }
                 }
 
-                function b() {
+                function g() {
                     throw new TypeError(`Invalid attempt to destructure non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
                 }
 
-                function S(y, m) {
-                    return v(y) || h(y, m) || g(y, m) || b()
+                function y(S, b) {
+                    return v(S) || p(S, b) || m(S, b) || g()
                 }
 
-                function P(y) {
-                    if (Array.isArray(y)) return p(y)
+                function O(S) {
+                    if (Array.isArray(S)) return h(S)
                 }
 
-                function x(y) {
-                    if (typeof Symbol < "u" && Symbol.iterator in Object(y)) return Array.from(y)
+                function E(S) {
+                    if (typeof Symbol < "u" && Symbol.iterator in Object(S)) return Array.from(S)
                 }
 
                 function C() {
                     throw new TypeError(`Invalid attempt to spread non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
                 }
 
-                function I(y) {
-                    return P(y) || x(y) || g(y) || C()
+                function T(S) {
+                    return O(S) || E(S) || m(S) || C()
                 }
-                var j = t("a352"),
-                    L = t.n(j);
+                var $ = t("a352"),
+                    L = t.n($);
 
-                function T(y) {
-                    y.parentElement !== null && y.parentElement.removeChild(y)
+                function I(S) {
+                    S.parentElement !== null && S.parentElement.removeChild(S)
                 }
 
-                function O(y, m, E) {
-                    var w = E === 0 ? y.children[0] : y.children[E - 1].nextSibling;
-                    y.insertBefore(m, w)
+                function j(S, b, x) {
+                    var A = x === 0 ? S.children[0] : S.children[x - 1].nextSibling;
+                    S.insertBefore(b, A)
                 }
-                var D = t("dbf1");
+                var P = t("dbf1");
                 t("13d5"), t("4fad"), t("ac1f"), t("5319");
 
-                function G(y) {
-                    var m = Object.create(null);
-                    return function(w) {
-                        var $ = m[w];
-                        return $ || (m[w] = y(w))
+                function M(S) {
+                    var b = Object.create(null);
+                    return function(A) {
+                        var V = b[A];
+                        return V || (b[A] = S(A))
                     }
                 }
-                var A = /-(\w)/g,
-                    M = G(function(y) {
-                        return y.replace(A, function(m, E) {
-                            return E.toUpperCase()
+                var D = /-(\w)/g,
+                    R = M(function(S) {
+                        return S.replace(D, function(b, x) {
+                            return x.toUpperCase()
                         })
                     });
                 t("5db7"), t("73d9");
-                var X = ["Start", "Add", "Remove", "Update", "End"],
-                    R = ["Choose", "Unchoose", "Sort", "Filter", "Clone"],
-                    F = ["Move"],
-                    _ = [F, X, R].flatMap(function(y) {
-                        return y
-                    }).map(function(y) {
-                        return "on".concat(y)
+                var H = ["Start", "Add", "Remove", "Update", "End"],
+                    F = ["Choose", "Unchoose", "Sort", "Filter", "Clone"],
+                    N = ["Move"],
+                    k = [N, H, F].flatMap(function(S) {
+                        return S
+                    }).map(function(S) {
+                        return "on".concat(S)
                     }),
-                    at = {
-                        manage: F,
-                        manageAndEmit: X,
-                        emit: R
+                    ot = {
+                        manage: N,
+                        manageAndEmit: H,
+                        emit: F
                     };
 
-                function xt(y) {
-                    return _.indexOf(y) !== -1
+                function St(S) {
+                    return k.indexOf(S) !== -1
                 }
                 t("caad"), t("2ca0");
-                var vt = ["a", "abbr", "address", "area", "article", "aside", "audio", "b", "base", "bdi", "bdo", "blockquote", "body", "br", "button", "canvas", "caption", "cite", "code", "col", "colgroup", "data", "datalist", "dd", "del", "details", "dfn", "dialog", "div", "dl", "dt", "em", "embed", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hgroup", "hr", "html", "i", "iframe", "img", "input", "ins", "kbd", "label", "legend", "li", "link", "main", "map", "mark", "math", "menu", "menuitem", "meta", "meter", "nav", "noscript", "object", "ol", "optgroup", "option", "output", "p", "param", "picture", "pre", "progress", "q", "rb", "rp", "rt", "rtc", "ruby", "s", "samp", "script", "section", "select", "slot", "small", "source", "span", "strong", "style", "sub", "summary", "sup", "svg", "table", "tbody", "td", "template", "textarea", "tfoot", "th", "thead", "time", "title", "tr", "track", "u", "ul", "var", "video", "wbr"];
+                var ct = ["a", "abbr", "address", "area", "article", "aside", "audio", "b", "base", "bdi", "bdo", "blockquote", "body", "br", "button", "canvas", "caption", "cite", "code", "col", "colgroup", "data", "datalist", "dd", "del", "details", "dfn", "dialog", "div", "dl", "dt", "em", "embed", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hgroup", "hr", "html", "i", "iframe", "img", "input", "ins", "kbd", "label", "legend", "li", "link", "main", "map", "mark", "math", "menu", "menuitem", "meta", "meter", "nav", "noscript", "object", "ol", "optgroup", "option", "output", "p", "param", "picture", "pre", "progress", "q", "rb", "rp", "rt", "rtc", "ruby", "s", "samp", "script", "section", "select", "slot", "small", "source", "span", "strong", "style", "sub", "summary", "sup", "svg", "table", "tbody", "td", "template", "textarea", "tfoot", "th", "thead", "time", "title", "tr", "track", "u", "ul", "var", "video", "wbr"];
 
-                function ht(y) {
-                    return vt.includes(y)
+                function pt(S) {
+                    return ct.includes(S)
                 }
 
-                function Et(y) {
-                    return ["transition-group", "TransitionGroup"].includes(y)
+                function Ot(S) {
+                    return ["transition-group", "TransitionGroup"].includes(S)
                 }
 
-                function Ot(y) {
-                    return ["id", "class", "role", "style"].includes(y) || y.startsWith("data-") || y.startsWith("aria-") || y.startsWith("on")
+                function It(S) {
+                    return ["id", "class", "role", "style"].includes(S) || S.startsWith("data-") || S.startsWith("aria-") || S.startsWith("on")
                 }
 
-                function bt(y) {
-                    return y.reduce(function(m, E) {
-                        var w = S(E, 2),
-                            $ = w[0],
-                            z = w[1];
-                        return m[$] = z, m
+                function Et(S) {
+                    return S.reduce(function(b, x) {
+                        var A = y(x, 2),
+                            V = A[0],
+                            J = A[1];
+                        return b[V] = J, b
                     }, {})
                 }
 
-                function lt(y) {
-                    var m = y.$attrs,
-                        E = y.componentData,
-                        w = E === void 0 ? {} : E,
-                        $ = bt(Object.entries(m).filter(function(z) {
-                            var q = S(z, 2),
-                                ot = q[0];
-                            return q[1], Ot(ot)
+                function st(S) {
+                    var b = S.$attrs,
+                        x = S.componentData,
+                        A = x === void 0 ? {} : x,
+                        V = Et(Object.entries(b).filter(function(J) {
+                            var _ = y(J, 2),
+                                at = _[0];
+                            return _[1], It(at)
                         }));
-                    return d(d({}, $), w)
+                    return d(d({}, V), A)
                 }
 
-                function ct(y) {
-                    var m = y.$attrs,
-                        E = y.callBackBuilder,
-                        w = bt(Lt(m));
-                    Object.entries(E).forEach(function(z) {
-                        var q = S(z, 2),
-                            ot = q[0],
-                            yt = q[1];
-                        at[ot].forEach(function(J) {
-                            w["on".concat(J)] = yt(J)
+                function dt(S) {
+                    var b = S.$attrs,
+                        x = S.callBackBuilder,
+                        A = Et(Lt(b));
+                    Object.entries(x).forEach(function(J) {
+                        var _ = y(J, 2),
+                            at = _[0],
+                            yt = _[1];
+                        ot[at].forEach(function(Q) {
+                            A["on".concat(Q)] = yt(Q)
                         })
                     });
-                    var $ = "[data-draggable]".concat(w.draggable || "");
-                    return d(d({}, w), {}, {
-                        draggable: $
+                    var V = "[data-draggable]".concat(A.draggable || "");
+                    return d(d({}, A), {}, {
+                        draggable: V
                     })
                 }
 
-                function Lt(y) {
-                    return Object.entries(y).filter(function(m) {
-                        var E = S(m, 2),
-                            w = E[0];
-                        return E[1], !Ot(w)
-                    }).map(function(m) {
-                        var E = S(m, 2),
-                            w = E[0],
-                            $ = E[1];
-                        return [M(w), $]
-                    }).filter(function(m) {
-                        var E = S(m, 2),
-                            w = E[0];
-                        return E[1], !xt(w)
+                function Lt(S) {
+                    return Object.entries(S).filter(function(b) {
+                        var x = y(b, 2),
+                            A = x[0];
+                        return x[1], !It(A)
+                    }).map(function(b) {
+                        var x = y(b, 2),
+                            A = x[0],
+                            V = x[1];
+                        return [R(A), V]
+                    }).filter(function(b) {
+                        var x = y(b, 2),
+                            A = x[0];
+                        return x[1], !St(A)
                     })
                 }
                 t("c740");
 
-                function Rt(y, m) {
-                    if (!(y instanceof m)) throw new TypeError("Cannot call a class as a function")
+                function wt(S, b) {
+                    if (!(S instanceof b)) throw new TypeError("Cannot call a class as a function")
                 }
 
-                function _t(y, m) {
-                    for (var E = 0; E < m.length; E++) {
-                        var w = m[E];
-                        w.enumerable = w.enumerable || !1, w.configurable = !0, "value" in w && (w.writable = !0), Object.defineProperty(y, w.key, w)
+                function re(S, b) {
+                    for (var x = 0; x < b.length; x++) {
+                        var A = b[x];
+                        A.enumerable = A.enumerable || !1, A.configurable = !0, "value" in A && (A.writable = !0), Object.defineProperty(S, A.key, A)
                     }
                 }
 
-                function ue(y, m, E) {
-                    return m && _t(y.prototype, m), E && _t(y, E), y
+                function de(S, b, x) {
+                    return b && re(S.prototype, b), x && re(S, x), S
                 }
-                var oe = function(m) {
-                        var E = m.el;
-                        return E
+                var ie = function(b) {
+                        var x = b.el;
+                        return x
                     },
-                    Tt = function(m, E) {
-                        return m.__draggable_context = E
+                    Pt = function(b, x) {
+                        return b.__draggable_context = x
                     },
-                    It = function(m) {
-                        return m.__draggable_context
+                    Ct = function(b) {
+                        return b.__draggable_context
                     },
-                    fe = function() {
-                        function y(m) {
-                            var E = m.nodes,
-                                w = E.header,
-                                $ = E.default,
-                                z = E.footer,
-                                q = m.root,
-                                ot = m.realList;
-                            Rt(this, y), this.defaultNodes = $, this.children = [].concat(I(w), I($), I(z)), this.externalComponent = q.externalComponent, this.rootTransition = q.transition, this.tag = q.tag, this.realList = ot
+                    ve = function() {
+                        function S(b) {
+                            var x = b.nodes,
+                                A = x.header,
+                                V = x.default,
+                                J = x.footer,
+                                _ = b.root,
+                                at = b.realList;
+                            wt(this, S), this.defaultNodes = V, this.children = [].concat(T(A), T(V), T(J)), this.externalComponent = _.externalComponent, this.rootTransition = _.transition, this.tag = _.tag, this.realList = at
                         }
-                        return ue(y, [{
+                        return de(S, [{
                             key: "render",
-                            value: function(E, w) {
-                                var $ = this.tag,
-                                    z = this.children,
-                                    q = this._isRootComponent,
-                                    ot = q ? {
+                            value: function(x, A) {
+                                var V = this.tag,
+                                    J = this.children,
+                                    _ = this._isRootComponent,
+                                    at = _ ? {
                                         default: function() {
-                                            return z
+                                            return J
                                         }
-                                    } : z;
-                                return E($, w, ot)
+                                    } : J;
+                                return x(V, A, at)
                             }
                         }, {
                             key: "updated",
                             value: function() {
-                                var E = this.defaultNodes,
-                                    w = this.realList;
-                                E.forEach(function($, z) {
-                                    Tt(oe($), {
-                                        element: w[z],
-                                        index: z
+                                var x = this.defaultNodes,
+                                    A = this.realList;
+                                x.forEach(function(V, J) {
+                                    Pt(ie(V), {
+                                        element: A[J],
+                                        index: J
                                     })
                                 })
                             }
                         }, {
                             key: "getUnderlyingVm",
-                            value: function(E) {
-                                return It(E)
+                            value: function(x) {
+                                return Ct(x)
                             }
                         }, {
                             key: "getVmIndexFromDomIndex",
-                            value: function(E, w) {
-                                var $ = this.defaultNodes,
-                                    z = $.length,
-                                    q = w.children,
-                                    ot = q.item(E);
-                                if (ot === null) return z;
-                                var yt = It(ot);
+                            value: function(x, A) {
+                                var V = this.defaultNodes,
+                                    J = V.length,
+                                    _ = A.children,
+                                    at = _.item(x);
+                                if (at === null) return J;
+                                var yt = Ct(at);
                                 if (yt) return yt.index;
-                                if (z === 0) return 0;
-                                var J = oe($[0]),
-                                    V = I(q).findIndex(function(H) {
-                                        return H === J
+                                if (J === 0) return 0;
+                                var Q = ie(V[0]),
+                                    B = T(_).findIndex(function(Y) {
+                                        return Y === Q
                                     });
-                                return E < V ? 0 : z
+                                return x < B ? 0 : J
                             }
                         }, {
                             key: "_isRootComponent",
                             get: function() {
                                 return this.externalComponent || this.rootTransition
                             }
-                        }]), y
+                        }]), S
                     }(),
-                    Yt = t("8bbf");
+                    Zt = t("8bbf");
 
-                function zt(y, m) {
-                    var E = y[m];
-                    return E ? E() : []
+                function kt(S, b) {
+                    var x = S[b];
+                    return x ? x() : []
                 }
 
-                function Ye(y) {
-                    var m = y.$slots,
-                        E = y.realList,
-                        w = y.getKey,
-                        $ = E || [],
-                        z = ["header", "footer"].map(function(H) {
-                            return zt(m, H)
+                function Je(S) {
+                    var b = S.$slots,
+                        x = S.realList,
+                        A = S.getKey,
+                        V = x || [],
+                        J = ["header", "footer"].map(function(Y) {
+                            return kt(b, Y)
                         }),
-                        q = S(z, 2),
-                        ot = q[0],
-                        yt = q[1],
-                        J = m.item;
-                    if (!J) throw new Error("draggable element must have an item slot");
-                    var V = $.flatMap(function(H, nt) {
-                        return J({
-                            element: H,
+                        _ = y(J, 2),
+                        at = _[0],
+                        yt = _[1],
+                        Q = b.item;
+                    if (!Q) throw new Error("draggable element must have an item slot");
+                    var B = V.flatMap(function(Y, nt) {
+                        return Q({
+                            element: Y,
                             index: nt
                         }).map(function(rt) {
-                            return rt.key = w(H), rt.props = d(d({}, rt.props || {}), {}, {
+                            return rt.key = A(Y), rt.props = d(d({}, rt.props || {}), {}, {
                                 "data-draggable": !0
                             }), rt
                         })
                     });
-                    if (V.length !== $.length) throw new Error("Item slot must have only one child");
+                    if (B.length !== V.length) throw new Error("Item slot must have only one child");
                     return {
-                        header: ot,
+                        header: at,
                         footer: yt,
-                        default: V
+                        default: B
                     }
                 }
 
-                function hn(y) {
-                    var m = Et(y),
-                        E = !ht(y) && !m;
+                function mn(S) {
+                    var b = Ot(S),
+                        x = !pt(S) && !b;
                     return {
-                        transition: m,
-                        externalComponent: E,
-                        tag: E ? Object(Yt.resolveComponent)(y) : m ? Yt.TransitionGroup : y
+                        transition: b,
+                        externalComponent: x,
+                        tag: x ? Object(Zt.resolveComponent)(S) : b ? Zt.TransitionGroup : S
                     }
                 }
 
-                function Kt(y) {
-                    var m = y.$slots,
-                        E = y.tag,
-                        w = y.realList,
-                        $ = y.getKey,
-                        z = Ye({
-                            $slots: m,
-                            realList: w,
-                            getKey: $
+                function Wt(S) {
+                    var b = S.$slots,
+                        x = S.tag,
+                        A = S.realList,
+                        V = S.getKey,
+                        J = Je({
+                            $slots: b,
+                            realList: A,
+                            getKey: V
                         }),
-                        q = hn(E);
-                    return new fe({
-                        nodes: z,
-                        root: q,
-                        realList: w
+                        _ = mn(x);
+                    return new ve({
+                        nodes: J,
+                        root: _,
+                        realList: A
                     })
                 }
 
-                function ae(y, m) {
-                    var E = this;
-                    Object(Yt.nextTick)(function() {
-                        return E.$emit(y.toLowerCase(), m)
+                function le(S, b) {
+                    var x = this;
+                    Object(Zt.nextTick)(function() {
+                        return x.$emit(S.toLowerCase(), b)
                     })
                 }
 
-                function pe(y) {
-                    var m = this;
-                    return function(E, w) {
-                        if (m.realList !== null) return m["onDrag".concat(y)](E, w)
+                function ye(S) {
+                    var b = this;
+                    return function(x, A) {
+                        if (b.realList !== null) return b["onDrag".concat(S)](x, A)
                     }
                 }
 
-                function Oe(y) {
-                    var m = this,
-                        E = pe.call(this, y);
-                    return function(w, $) {
-                        E.call(m, w, $), ae.call(m, y, w)
+                function Pe(S) {
+                    var b = this,
+                        x = ye.call(this, S);
+                    return function(A, V) {
+                        x.call(b, A, V), le.call(b, S, A)
                     }
                 }
-                var Te = null,
-                    Ie = {
+                var Ce = null,
+                    De = {
                         list: {
                             type: Array,
                             required: !1,
                             default: null
                         },
                         modelValue: {
                             type: Array,
@@ -4847,16 +4849,16 @@
                         },
                         itemKey: {
                             type: [String, Function],
                             required: !0
                         },
                         clone: {
                             type: Function,
-                            default: function(m) {
-                                return m
+                            default: function(b) {
+                                return b
                             }
                         },
                         tag: {
                             type: String,
                             default: "div"
                         },
                         move: {
@@ -4865,298 +4867,298 @@
                         },
                         componentData: {
                             type: Object,
                             required: !1,
                             default: null
                         }
                     },
-                    Pe = ["update:modelValue", "change"].concat(I([].concat(I(at.manageAndEmit), I(at.emit)).map(function(y) {
-                        return y.toLowerCase()
+                    Ae = ["update:modelValue", "change"].concat(T([].concat(T(ot.manageAndEmit), T(ot.emit)).map(function(S) {
+                        return S.toLowerCase()
                     }))),
-                    Ce = Object(Yt.defineComponent)({
+                    Re = Object(Zt.defineComponent)({
                         name: "draggable",
                         inheritAttrs: !1,
-                        props: Ie,
-                        emits: Pe,
+                        props: De,
+                        emits: Ae,
                         data: function() {
                             return {
                                 error: !1
                             }
                         },
                         render: function() {
                             try {
                                 this.error = !1;
-                                var m = this.$slots,
-                                    E = this.$attrs,
-                                    w = this.tag,
-                                    $ = this.componentData,
-                                    z = this.realList,
-                                    q = this.getKey,
-                                    ot = Kt({
-                                        $slots: m,
-                                        tag: w,
-                                        realList: z,
-                                        getKey: q
+                                var b = this.$slots,
+                                    x = this.$attrs,
+                                    A = this.tag,
+                                    V = this.componentData,
+                                    J = this.realList,
+                                    _ = this.getKey,
+                                    at = Wt({
+                                        $slots: b,
+                                        tag: A,
+                                        realList: J,
+                                        getKey: _
                                     });
-                                this.componentStructure = ot;
-                                var yt = lt({
-                                    $attrs: E,
-                                    componentData: $
+                                this.componentStructure = at;
+                                var yt = st({
+                                    $attrs: x,
+                                    componentData: V
                                 });
-                                return ot.render(Yt.h, yt)
-                            } catch (J) {
-                                return this.error = !0, Object(Yt.h)("pre", {
+                                return at.render(Zt.h, yt)
+                            } catch (Q) {
+                                return this.error = !0, Object(Zt.h)("pre", {
                                     style: {
                                         color: "red"
                                     }
-                                }, J.stack)
+                                }, Q.stack)
                             }
                         },
                         created: function() {
-                            this.list !== null && this.modelValue !== null && D.a.error("modelValue and list props are mutually exclusive! Please set one or another.")
+                            this.list !== null && this.modelValue !== null && P.a.error("modelValue and list props are mutually exclusive! Please set one or another.")
                         },
                         mounted: function() {
-                            var m = this;
+                            var b = this;
                             if (!this.error) {
-                                var E = this.$attrs,
-                                    w = this.$el,
-                                    $ = this.componentStructure;
-                                $.updated();
-                                var z = ct({
-                                        $attrs: E,
+                                var x = this.$attrs,
+                                    A = this.$el,
+                                    V = this.componentStructure;
+                                V.updated();
+                                var J = dt({
+                                        $attrs: x,
                                         callBackBuilder: {
                                             manageAndEmit: function(yt) {
-                                                return Oe.call(m, yt)
+                                                return Pe.call(b, yt)
                                             },
                                             emit: function(yt) {
-                                                return ae.bind(m, yt)
+                                                return le.bind(b, yt)
                                             },
                                             manage: function(yt) {
-                                                return pe.call(m, yt)
+                                                return ye.call(b, yt)
                                             }
                                         }
                                     }),
-                                    q = w.nodeType === 1 ? w : w.parentElement;
-                                this._sortable = new L.a(q, z), this.targetDomElement = q, q.__draggable_component__ = this
+                                    _ = A.nodeType === 1 ? A : A.parentElement;
+                                this._sortable = new L.a(_, J), this.targetDomElement = _, _.__draggable_component__ = this
                             }
                         },
                         updated: function() {
                             this.componentStructure.updated()
                         },
                         beforeUnmount: function() {
                             this._sortable !== void 0 && this._sortable.destroy()
                         },
                         computed: {
                             realList: function() {
-                                var m = this.list;
-                                return m || this.modelValue
+                                var b = this.list;
+                                return b || this.modelValue
                             },
                             getKey: function() {
-                                var m = this.itemKey;
-                                return typeof m == "function" ? m : function(E) {
-                                    return E[m]
+                                var b = this.itemKey;
+                                return typeof b == "function" ? b : function(x) {
+                                    return x[b]
                                 }
                             }
                         },
                         watch: {
                             $attrs: {
-                                handler: function(m) {
-                                    var E = this._sortable;
-                                    !E || Lt(m).forEach(function(w) {
-                                        var $ = S(w, 2),
-                                            z = $[0],
-                                            q = $[1];
-                                        E.option(z, q)
+                                handler: function(b) {
+                                    var x = this._sortable;
+                                    !x || Lt(b).forEach(function(A) {
+                                        var V = y(A, 2),
+                                            J = V[0],
+                                            _ = V[1];
+                                        x.option(J, _)
                                     })
                                 },
                                 deep: !0
                             }
                         },
                         methods: {
-                            getUnderlyingVm: function(m) {
-                                return this.componentStructure.getUnderlyingVm(m) || null
+                            getUnderlyingVm: function(b) {
+                                return this.componentStructure.getUnderlyingVm(b) || null
                             },
-                            getUnderlyingPotencialDraggableComponent: function(m) {
-                                return m.__draggable_component__
+                            getUnderlyingPotencialDraggableComponent: function(b) {
+                                return b.__draggable_component__
                             },
-                            emitChanges: function(m) {
-                                var E = this;
-                                Object(Yt.nextTick)(function() {
-                                    return E.$emit("change", m)
+                            emitChanges: function(b) {
+                                var x = this;
+                                Object(Zt.nextTick)(function() {
+                                    return x.$emit("change", b)
                                 })
                             },
-                            alterList: function(m) {
+                            alterList: function(b) {
                                 if (this.list) {
-                                    m(this.list);
+                                    b(this.list);
                                     return
                                 }
-                                var E = I(this.modelValue);
-                                m(E), this.$emit("update:modelValue", E)
+                                var x = T(this.modelValue);
+                                b(x), this.$emit("update:modelValue", x)
                             },
                             spliceList: function() {
-                                var m = arguments,
-                                    E = function($) {
-                                        return $.splice.apply($, I(m))
+                                var b = arguments,
+                                    x = function(V) {
+                                        return V.splice.apply(V, T(b))
                                     };
-                                this.alterList(E)
+                                this.alterList(x)
                             },
-                            updatePosition: function(m, E) {
-                                var w = function(z) {
-                                    return z.splice(E, 0, z.splice(m, 1)[0])
+                            updatePosition: function(b, x) {
+                                var A = function(J) {
+                                    return J.splice(x, 0, J.splice(b, 1)[0])
                                 };
-                                this.alterList(w)
+                                this.alterList(A)
                             },
-                            getRelatedContextFromMoveEvent: function(m) {
-                                var E = m.to,
-                                    w = m.related,
-                                    $ = this.getUnderlyingPotencialDraggableComponent(E);
-                                if (!$) return {
-                                    component: $
+                            getRelatedContextFromMoveEvent: function(b) {
+                                var x = b.to,
+                                    A = b.related,
+                                    V = this.getUnderlyingPotencialDraggableComponent(x);
+                                if (!V) return {
+                                    component: V
                                 };
-                                var z = $.realList,
-                                    q = {
-                                        list: z,
-                                        component: $
+                                var J = V.realList,
+                                    _ = {
+                                        list: J,
+                                        component: V
                                     };
-                                if (E !== w && z) {
-                                    var ot = $.getUnderlyingVm(w) || {};
-                                    return d(d({}, ot), q)
+                                if (x !== A && J) {
+                                    var at = V.getUnderlyingVm(A) || {};
+                                    return d(d({}, at), _)
                                 }
-                                return q
+                                return _
                             },
-                            getVmIndexFromDomIndex: function(m) {
-                                return this.componentStructure.getVmIndexFromDomIndex(m, this.targetDomElement)
+                            getVmIndexFromDomIndex: function(b) {
+                                return this.componentStructure.getVmIndexFromDomIndex(b, this.targetDomElement)
                             },
-                            onDragStart: function(m) {
-                                this.context = this.getUnderlyingVm(m.item), m.item._underlying_vm_ = this.clone(this.context.element), Te = m.item
+                            onDragStart: function(b) {
+                                this.context = this.getUnderlyingVm(b.item), b.item._underlying_vm_ = this.clone(this.context.element), Ce = b.item
                             },
-                            onDragAdd: function(m) {
-                                var E = m.item._underlying_vm_;
-                                if (E !== void 0) {
-                                    T(m.item);
-                                    var w = this.getVmIndexFromDomIndex(m.newIndex);
-                                    this.spliceList(w, 0, E);
-                                    var $ = {
-                                        element: E,
-                                        newIndex: w
+                            onDragAdd: function(b) {
+                                var x = b.item._underlying_vm_;
+                                if (x !== void 0) {
+                                    I(b.item);
+                                    var A = this.getVmIndexFromDomIndex(b.newIndex);
+                                    this.spliceList(A, 0, x);
+                                    var V = {
+                                        element: x,
+                                        newIndex: A
                                     };
                                     this.emitChanges({
-                                        added: $
+                                        added: V
                                     })
                                 }
                             },
-                            onDragRemove: function(m) {
-                                if (O(this.$el, m.item, m.oldIndex), m.pullMode === "clone") {
-                                    T(m.clone);
+                            onDragRemove: function(b) {
+                                if (j(this.$el, b.item, b.oldIndex), b.pullMode === "clone") {
+                                    I(b.clone);
                                     return
                                 }
-                                var E = this.context,
-                                    w = E.index,
-                                    $ = E.element;
-                                this.spliceList(w, 1);
-                                var z = {
-                                    element: $,
-                                    oldIndex: w
+                                var x = this.context,
+                                    A = x.index,
+                                    V = x.element;
+                                this.spliceList(A, 1);
+                                var J = {
+                                    element: V,
+                                    oldIndex: A
                                 };
                                 this.emitChanges({
-                                    removed: z
+                                    removed: J
                                 })
                             },
-                            onDragUpdate: function(m) {
-                                T(m.item), O(m.from, m.item, m.oldIndex);
-                                var E = this.context.index,
-                                    w = this.getVmIndexFromDomIndex(m.newIndex);
-                                this.updatePosition(E, w);
-                                var $ = {
+                            onDragUpdate: function(b) {
+                                I(b.item), j(b.from, b.item, b.oldIndex);
+                                var x = this.context.index,
+                                    A = this.getVmIndexFromDomIndex(b.newIndex);
+                                this.updatePosition(x, A);
+                                var V = {
                                     element: this.context.element,
-                                    oldIndex: E,
-                                    newIndex: w
+                                    oldIndex: x,
+                                    newIndex: A
                                 };
                                 this.emitChanges({
-                                    moved: $
+                                    moved: V
                                 })
                             },
-                            computeFutureIndex: function(m, E) {
-                                if (!m.element) return 0;
-                                var w = I(E.to.children).filter(function(ot) {
-                                        return ot.style.display !== "none"
+                            computeFutureIndex: function(b, x) {
+                                if (!b.element) return 0;
+                                var A = T(x.to.children).filter(function(at) {
+                                        return at.style.display !== "none"
                                     }),
-                                    $ = w.indexOf(E.related),
-                                    z = m.component.getVmIndexFromDomIndex($),
-                                    q = w.indexOf(Te) !== -1;
-                                return q || !E.willInsertAfter ? z : z + 1
+                                    V = A.indexOf(x.related),
+                                    J = b.component.getVmIndexFromDomIndex(V),
+                                    _ = A.indexOf(Ce) !== -1;
+                                return _ || !x.willInsertAfter ? J : J + 1
                             },
-                            onDragMove: function(m, E) {
-                                var w = this.move,
-                                    $ = this.realList;
-                                if (!w || !$) return !0;
-                                var z = this.getRelatedContextFromMoveEvent(m),
-                                    q = this.computeFutureIndex(z, m),
-                                    ot = d(d({}, this.context), {}, {
-                                        futureIndex: q
+                            onDragMove: function(b, x) {
+                                var A = this.move,
+                                    V = this.realList;
+                                if (!A || !V) return !0;
+                                var J = this.getRelatedContextFromMoveEvent(b),
+                                    _ = this.computeFutureIndex(J, b),
+                                    at = d(d({}, this.context), {}, {
+                                        futureIndex: _
                                     }),
-                                    yt = d(d({}, m), {}, {
-                                        relatedContext: z,
-                                        draggedContext: ot
+                                    yt = d(d({}, b), {}, {
+                                        relatedContext: J,
+                                        draggedContext: at
                                     });
-                                return w(yt, E)
+                                return A(yt, x)
                             },
                             onDragEnd: function() {
-                                Te = null
+                                Ce = null
                             }
                         }
                     }),
-                    De = Ce;
-                u.default = De
+                    we = Re;
+                s.default = we
             },
-            fb6a: function(r, u, t) {
+            fb6a: function(r, s, t) {
                 var o = t("23e7"),
-                    i = t("861d"),
-                    s = t("e8b5"),
-                    c = t("23cb"),
-                    f = t("50c4"),
+                    l = t("861d"),
+                    u = t("e8b5"),
+                    f = t("23cb"),
+                    c = t("50c4"),
                     d = t("fc6a"),
                     v = t("8418"),
-                    h = t("b622"),
-                    p = t("1dde"),
-                    g = t("ae40"),
-                    b = p("slice"),
-                    S = g("slice", {
+                    p = t("b622"),
+                    h = t("1dde"),
+                    m = t("ae40"),
+                    g = h("slice"),
+                    y = m("slice", {
                         ACCESSORS: !0,
                         0: 0,
                         1: 2
                     }),
-                    P = h("species"),
-                    x = [].slice,
+                    O = p("species"),
+                    E = [].slice,
                     C = Math.max;
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: !b || !S
+                    forced: !g || !y
                 }, {
-                    slice: function(j, L) {
-                        var T = d(this),
-                            O = f(T.length),
-                            D = c(j, O),
-                            G = c(L === void 0 ? O : L, O),
-                            A, M, X;
-                        if (s(T) && (A = T.constructor, typeof A == "function" && (A === Array || s(A.prototype)) ? A = void 0 : i(A) && (A = A[P], A === null && (A = void 0)), A === Array || A === void 0)) return x.call(T, D, G);
-                        for (M = new(A === void 0 ? Array : A)(C(G - D, 0)), X = 0; D < G; D++, X++) D in T && v(M, X, T[D]);
-                        return M.length = X, M
+                    slice: function($, L) {
+                        var I = d(this),
+                            j = c(I.length),
+                            P = f($, j),
+                            M = f(L === void 0 ? j : L, j),
+                            D, R, H;
+                        if (u(I) && (D = I.constructor, typeof D == "function" && (D === Array || u(D.prototype)) ? D = void 0 : l(D) && (D = D[O], D === null && (D = void 0)), D === Array || D === void 0)) return E.call(I, P, M);
+                        for (R = new(D === void 0 ? Array : D)(C(M - P, 0)), H = 0; P < M; P++, H++) P in I && v(R, H, I[P]);
+                        return R.length = H, R
                     }
                 })
             },
-            fc6a: function(r, u, t) {
+            fc6a: function(r, s, t) {
                 var o = t("44ad"),
-                    i = t("1d80");
-                r.exports = function(s) {
-                    return o(i(s))
+                    l = t("1d80");
+                r.exports = function(u) {
+                    return o(l(u))
                 }
             },
-            fdbc: function(r, u) {
+            fdbc: function(r, s) {
                 r.exports = {
                     CSSRuleList: 0,
                     CSSStyleDeclaration: 0,
                     CSSValueList: 0,
                     ClientRectList: 0,
                     DOMRectList: 0,
                     DOMStringList: 0,
@@ -5183,389 +5185,522 @@
                     SourceBufferList: 0,
                     StyleSheetList: 0,
                     TextTrackCueList: 0,
                     TextTrackList: 0,
                     TouchList: 0
                 }
             },
-            fdbf: function(r, u, t) {
+            fdbf: function(r, s, t) {
                 var o = t("4930");
                 r.exports = o && !Symbol.sham && typeof Symbol.iterator == "symbol"
             }
         }).default
     })
-})(lr);
-const Jn = za(lr.exports);
-async function* Mi(a) {
+})(gr);
+const Nn = ei(gr.exports);
+async function* Gi(a) {
     const e = new TextDecoder("utf-8");
     let {
         value: n,
-        done: l
+        done: i
     } = await a.read();
     n = n ? e.decode(n, {
         stream: !0
     }) : "";
     const r = /\r\n|\n|\r/gm;
-    let u = 0;
+    let s = 0;
     for (;;) {
         let t = r.exec(n);
         if (t) {
-            yield n.substring(u, t.index), u = r.lastIndex;
+            yield n.substring(s, t.index), s = r.lastIndex;
             continue
         }
-        if (l) break;
-        let o = n.substr(u);
+        if (i) break;
+        let o = n.substr(s);
         ({
             value: n,
-            done: l
+            done: i
         } = await a.read()), n = o + (n ? e.decode(n, {
             stream: !0
-        }) : ""), u = 0, r.lastIndex = 0
+        }) : ""), s = 0, r.lastIndex = 0
     }
-    u < n.length && (yield n.substr(u))
+    s < n.length && (yield n.substr(s))
 }
-async function* Ni(a, e) {
+async function* Bi(a, e) {
     const n = await fetch(a, e);
     if (!n.ok) throw new Error(await n.text());
-    const l = n.body.getReader();
-    for await (let r of Mi(l)) yield JSON.parse(r)
+    const i = n.body.getReader();
+    for await (let r of Gi(i)) yield JSON.parse(r)
 }
-const an = Jt([]);
-async function ji() {
+const sn = zt([]);
+async function Ki() {
     const e = await (await fetch("/api/filters/")).json();
-    return Array.from(Object.entries(e), ([l, r]) => Object.assign(r, {
-        name: l
-    })).sort((l, r) => l.name.localeCompare(r.name))
+    return Array.from(Object.entries(e), ([i, r]) => Object.assign(r, {
+        name: i
+    })).sort((i, r) => i.name.localeCompare(r.name))
 }
-let Qn = null;
+let rr = null;
 
-function Fi() {
-    return Qn || (Qn = ji().then(a => {
-        an.value.splice(0, an.length, ...dn(a))
-    })), an
+function Hi() {
+    return rr || (rr = Ki().then(a => {
+        sn.value.splice(0, sn.length, ...pn(a))
+    })), sn
 }
 
-function Sr(a) {
-    return an.value.find(e => e.name === a.filter)
+function Ar(a) {
+    return sn.value.find(e => e.name === a.filter)
 }
 
-function Er(a) {
+function Rr(a) {
     var e;
-    return ((e = Sr(a)) == null ? void 0 : e.type) == "monolingual"
+    return ((e = Ar(a)) == null ? void 0 : e.type) == "monolingual"
 }
-const Li = a => (Mn("data-v-c95e23ce"), a = a(), wn(), a),
-    $i = {
+const Wi = a => ($n("data-v-c95e23ce"), a = a(), Fn(), a),
+    Xi = {
         class: "container"
     },
-    Ui = ["checked"],
-    Vi = Li(() => Z("span", {
+    Yi = ["checked"],
+    zi = Wi(() => X("span", {
         class: "checkmark"
     }, null, -1)),
-    Gi = {
+    Ji = {
         __name: "Checkbox",
         props: {
             modelValue: {
                 type: Boolean
             }
         },
         emits: ["update:modelValue"],
         setup(a) {
-            return (e, n) => (K(), Y("label", $i, [Z("input", {
+            return (e, n) => (U(), W("label", Xi, [X("input", {
                 type: "checkbox",
                 checked: a.modelValue,
-                onInput: n[0] || (n[0] = l => e.$emit("update:modelValue", l.target.checked))
-            }, null, 40, Ui), Vi, He(e.$slots, "default", {}, void 0, !0)]))
+                onInput: n[0] || (n[0] = i => e.$emit("update:modelValue", i.target.checked))
+            }, null, 40, Yi), zi, Qt(e.$slots, "default", {}, void 0, !0)]))
         }
     },
-    Bi = xe(Gi, [
+    or = ne(Ji, [
         ["__scopeId", "data-v-c95e23ce"]
     ]);
-const Ki = {
+const Qi = {
         class: "segmented-control"
     },
-    Hi = ["onInput", "checked"],
-    Wi = {
+    Zi = ["onInput", "checked"],
+    ki = {
         __name: "SegmentedControl",
         props: {
             options: {
                 type: Array
             },
             modelValue: {}
         },
         emits: ["update:modelValue"],
         setup(a) {
-            return (e, n) => (K(), Y("div", Ki, [(K(!0), Y(Dt, null, Gt(a.options, l => (K(), Y("label", {
-                key: l,
-                class: Be({
-                    selected: a.modelValue === l
+            return (e, n) => (U(), W("div", Qi, [(U(!0), W(bt, null, Gt(a.options, i => (U(), W("label", {
+                key: i,
+                class: We({
+                    selected: a.modelValue === i
                 })
-            }, [Z("input", {
+            }, [X("input", {
                 type: "radio",
-                onInput: r => e.$emit("update:modelValue", l),
-                checked: a.modelValue === l
-            }, null, 40, Hi), Z("span", null, [He(e.$slots, "default", {
-                option: l
-            }, () => [Zt(it(l), 1)], !0)])], 2))), 128))]))
+                onInput: r => e.$emit("update:modelValue", i),
+                checked: a.modelValue === i
+            }, null, 40, Zi), X("span", null, [Qt(e.$slots, "default", {
+                option: i
+            }, () => [Bt(it(i), 1)], !0)])], 2))), 128))]))
         }
     },
-    Xi = xe(Wi, [
+    qi = ne(ki, [
         ["__scopeId", "data-v-3ae3bbf6"]
-    ]);
-const Yi = ["open"],
-    zi = {
+    ]),
+    _i = {
+        props: ["parameter", "modelValue"],
+        emits: ["update:modelValue"]
+    },
+    tl = ["value", "min", "max"];
+
+function el(a, e, n, i, r, s) {
+    return U(), W(bt, null, [Qt(a.$slots, "default"), X("input", Te({
+        type: "number"
+    }, a.$attrs, {
+        value: n.modelValue,
+        onInput: e[0] || (e[0] = t => a.$emit("update:modelValue", t.target.value)),
+        min: n.parameter.min,
+        max: n.parameter.max,
+        step: 1
+    }), null, 16, tl)], 64)
+}
+const Kn = ne(_i, [
+        ["render", el]
+    ]),
+    nl = {
+        props: ["parameter", "modelValue"],
+        emits: ["update:modelValue"]
+    },
+    rl = ["value", "min", "max", "step"];
+
+function ol(a, e, n, i, r, s) {
+    return U(), W(bt, null, [Qt(a.$slots, "default"), X("input", Te({
+        type: "number"
+    }, a.$attrs, {
+        value: n.modelValue,
+        onInput: e[0] || (e[0] = t => a.$emit("update:modelValue", t.target.value)),
+        min: n.parameter.min,
+        max: n.parameter.max,
+        step: .1
+    }), null, 16, rl)], 64)
+}
+const Hn = ne(nl, [
+        ["render", ol]
+    ]),
+    al = {
+        props: ["parameter", "modelValue"],
+        emits: ["update:modelValue"]
+    },
+    il = ["value"],
+    ll = ["value"],
+    sl = ["value"];
+
+function ul(a, e, n, i, r, s) {
+    return U(), W(bt, null, [Qt(a.$slots, "default"), n.parameter.allowed_values ? (U(), W("select", Te({
         key: 0
+    }, a.$attrs, {
+        value: n.modelValue,
+        onInput: e[0] || (e[0] = t => a.$emit("update:modelValue", t.target.value))
+    }), [(U(!0), W(bt, null, Gt(n.parameter.allowed_values, t => (U(), W("option", {
+        value: t,
+        key: t
+    }, it(t), 9, ll))), 128))], 16, il)) : (U(), W("input", Te({
+        key: 1,
+        type: "text"
+    }, a.$attrs, {
+        value: n.modelValue,
+        onInput: e[1] || (e[1] = t => a.$emit("update:modelValue", t.target.value))
+    }), null, 16, sl))], 64)
+}
+const Wn = ne(al, [
+        ["render", ul]
+    ]),
+    fl = {
+        props: ["parameter", "modelValue"],
+        emits: ["update:modelValue"]
+    },
+    cl = ["value"];
+
+function dl(a, e, n, i, r, s) {
+    return U(), W(bt, null, [Qt(a.$slots, "default"), X("input", Te({
+        type: "checkbox"
+    }, a.$attrs, {
+        value: n.modelValue,
+        onInput: e[0] || (e[0] = t => a.$emit("update:modelValue", t.target.value))
+    }), null, 16, cl)], 64)
+}
+const Xn = ne(fl, [
+        ["render", dl]
+    ]),
+    vl = {
+        class: "property-list"
     },
-    Ji = ["for"],
-    Qi = ["id", "value"],
-    Zi = ["for"],
-    ki = ["id", "value", "onInput"],
-    qi = ["value"],
-    _i = ["id", "checked", "onInput"],
-    ts = ["id", "min", "max", "step", "value", "onInput"],
-    es = ["id", "value", "onInput"],
-    ns = {
-        key: 4,
+    pl = ["for"],
+    wr = {
+        __name: "TupleParameter",
+        props: ["parameter", "modelValue"],
+        emits: ["update:modelValue"],
+        setup(a) {
+            const e = {
+                    int: Kn,
+                    float: Hn,
+                    str: Wn,
+                    bool: Xn
+                },
+                n = Ln();
+            return (i, r) => (U(), W("fieldset", vl, [X("legend", null, [Qt(i.$slots, "default")]), (U(!0), W(bt, null, Gt(a.parameter.parameters || [], (s, t) => (U(), W("div", {
+                key: t
+            }, [(U(), ce(Xe(e[s.type]), {
+                id: `tuple-${K(n)}-${t}`,
+                parameter: s,
+                modelValue: a.modelValue[t],
+                "onUpdate:modelValue": o => i.$emit("update:modelValue", [...a.modelValue.slice(0, t), o, ...a.modelValue.slice(t + 1)])
+            }, {
+                default: Nt(() => [s.help ? (U(), W("label", {
+                    key: 0,
+                    for: `tuple-${K(n)}-${t}`
+                }, it(s.help), 9, pl)) : _t("", !0)]),
+                _: 2
+            }, 1032, ["id", "parameter", "modelValue", "onUpdate:modelValue"]))]))), 128))]))
+        }
+    };
+const hl = ["onClick"],
+    ml = {
+        __name: "ListParameter",
+        props: ["parameter", "modelValue"],
+        emits: ["update:modelValue"],
+        setup(a) {
+            const e = a,
+                n = {
+                    int: Kn,
+                    float: Hn,
+                    str: Wn,
+                    bool: Xn,
+                    tuple: wr,
+                    list: void 0
+                };
+
+            function i(r) {
+                return e.modelValue.indexOf(r).toString()
+            }
+            return (r, s) => (U(), W("fieldset", null, [X("legend", null, [Qt(r.$slots, "default", {}, void 0, !0)]), Tt(K(Nn), {
+                tag: "ol",
+                class: "parameter-list",
+                "item-key": i,
+                modelValue: e.modelValue,
+                "onUpdate:modelValue": s[1] || (s[1] = t => r.$emit("update:modelValue", t))
+            }, {
+                item: Nt(({
+                    element: t,
+                    index: o
+                }) => [X("li", null, [(U(), ce(Xe(n[a.parameter.parameter.type]), {
+                    parameter: a.parameter.parameter,
+                    modelValue: t,
+                    "onUpdate:modelValue": l => r.$emit("update:modelValue", [...e.modelValue.slice(0, o), l, ...e.modelValue.slice(o + 1)])
+                }, {
+                    default: Nt(() => [Bt(" Item " + it(o + 1) + " ", 1), X("button", {
+                        class: "icon-button",
+                        onClick: l => r.$emit("update:modelValue", [...e.modelValue.slice(0, o), ...e.modelValue.slice(o + 1)])
+                    }, [Tt(K(Ka), {
+                        size: "16"
+                    })], 8, hl)]),
+                    _: 2
+                }, 1032, ["parameter", "modelValue", "onUpdate:modelValue"]))])]),
+                footer: Nt(() => [X("li", null, [X("button", {
+                    class: "add-item-button",
+                    onClick: s[0] || (s[0] = t => r.$emit("update:modelValue", [...e.modelValue, K(hr)(a.parameter.parameter)]))
+                }, [Tt(K(pr), {
+                    size: "16"
+                }), Bt(" Add item")])])]),
+                _: 1
+            }, 8, ["modelValue"])]))
+        }
+    },
+    gl = ne(ml, [
+        ["__scopeId", "data-v-b762df52"]
+    ]),
+    yl = ["open"],
+    bl = {
+        key: 0
+    },
+    Sl = ["for"],
+    El = ["id", "value"],
+    xl = ["for"],
+    Ol = {
+        key: 0,
         class: "property-list-description"
     },
-    rs = {
+    Tl = {
         __name: "FilterStep",
         props: {
             open: Boolean,
             languages: Array,
             modelValue: Object
         },
         emits: ["update:modelValue", "update:open"],
         setup(a) {
-            const e = ir();
-            return (n, l) => {
-                var r;
-                return K(), Y("li", null, [Z("details", {
+            const e = {
+                    int: Kn,
+                    float: Hn,
+                    str: Wn,
+                    bool: Xn,
+                    list: gl,
+                    tuple: wr
+                },
+                n = Ln();
+            return (i, r) => {
+                var s;
+                return U(), W("li", null, [X("details", {
                     class: "property-list",
-                    onToggle: l[1] || (l[1] = u => n.$emit("update:open", u.target.open)),
+                    onToggle: r[1] || (r[1] = t => i.$emit("update:open", t.target.open)),
                     open: a.open
-                }, [Z("summary", null, [He(n.$slots, "header", {}, void 0, !0)]), B(Er)(a.modelValue) ? (K(), Y("div", zi, [Z("label", {
-                    for: `step-${B(e)}-column`
-                }, "Column", 8, Ji), Z("select", {
-                    id: `step-${B(e)}-column`,
+                }, [X("summary", null, [Qt(i.$slots, "header")]), K(Rr)(a.modelValue) ? (U(), W("div", bl, [X("label", {
+                    for: `step-${K(n)}-column`
+                }, "Column", 8, Sl), X("select", {
+                    id: `step-${K(n)}-column`,
                     value: a.modelValue.language,
-                    onInput: l[0] || (l[0] = u => n.$emit("update:modelValue", {
+                    onInput: r[0] || (r[0] = t => i.$emit("update:modelValue", {
                         ...a.modelValue,
-                        language: u.target.value
+                        language: t.target.value
                     }))
-                }, [(K(!0), Y(Dt, null, Gt(a.languages, u => (K(), Y("option", {
-                    key: u
-                }, it(u), 1))), 128))], 40, Qi)])) : ee("", !0), (K(!0), Y(Dt, null, Gt(((r = B(Sr)(a.modelValue)) == null ? void 0 : r.parameters) || {}, (u, t) => (K(), Y("div", {
+                }, [(U(!0), W(bt, null, Gt(a.languages, t => (U(), W("option", {
                     key: t
-                }, [Z("label", {
-                    for: `step-${B(e)}-${t}`
-                }, it(t), 9, Zi), u.type == "str" && u.allowed_values ? (K(), Y("select", {
-                    key: 0,
-                    id: `step-${B(e)}-${t}`,
-                    value: a.modelValue.parameters[t],
-                    onInput: o => n.$emit("update:modelValue", {
+                }, it(t), 1))), 128))], 40, El)])) : _t("", !0), (U(!0), W(bt, null, Gt(((s = K(Ar)(a.modelValue)) == null ? void 0 : s.parameters) || {}, (t, o) => (U(), W("div", {
+                    key: o
+                }, [(U(), ce(Xe(e[t.type]), {
+                    id: `step-${K(n)}-${o}`,
+                    parameter: t,
+                    modelValue: a.modelValue.parameters[o],
+                    "onUpdate:modelValue": l => i.$emit("update:modelValue", {
                         ...a.modelValue,
                         parameters: {
                             ...a.modelValue.parameters,
-                            [t]: o.target.value
+                            [o]: l
                         }
                     })
-                }, [(K(!0), Y(Dt, null, Gt(u.allowed_values, o => (K(), Y("option", {
-                    key: o,
-                    value: o
-                }, it(o), 9, qi))), 128))], 40, ki)) : u.type == "bool" ? (K(), Y("input", {
-                    key: 1,
-                    type: "checkbox",
-                    id: `step-${B(e)}-${t}`,
-                    checked: a.modelValue.parameters[t],
-                    onInput: o => n.$emit("update:modelValue", {
-                        ...a.modelValue,
-                        parameters: {
-                            ...a.modelValue.parameters,
-                            [t]: o.target.checked
-                        }
-                    })
-                }, null, 40, _i)) : u.type == "int" || u.type == "float" ? (K(), Y("input", {
-                    key: 2,
-                    type: "number",
-                    id: `step-${B(e)}-${t}`,
-                    min: u.min,
-                    max: u.max,
-                    step: u.type == "int" ? 1 : .1,
-                    value: a.modelValue.parameters[t],
-                    onInput: o => n.$emit("update:modelValue", {
-                        ...a.modelValue,
-                        parameters: {
-                            ...a.modelValue.parameters,
-                            [t]: o.target.value
-                        }
-                    })
-                }, null, 40, ts)) : (K(), Y("input", {
-                    key: 3,
-                    type: "text",
-                    id: `step-${B(e)}-${t}`,
-                    value: a.modelValue.parameters[t],
-                    onInput: o => n.$emit("update:modelValue", {
-                        ...a.modelValue,
-                        parameters: {
-                            ...a.modelValue.parameters,
-                            [t]: o.target.value
-                        }
-                    })
-                }, null, 40, es)), u.help ? (K(), Y("small", ns, it(u.help), 1)) : ee("", !0)]))), 128)), Z("footer", null, [He(n.$slots, "footer", {}, void 0, !0)])], 40, Yi)])
+                }, {
+                    default: Nt(() => [X("label", {
+                        for: `step-${K(n)}-${o}`
+                    }, it(o), 9, xl)]),
+                    _: 2
+                }, 1032, ["id", "parameter", "modelValue", "onUpdate:modelValue"])), t.help ? (U(), W("small", Ol, it(t.help), 1)) : _t("", !0)]))), 128)), X("footer", null, [Qt(i.$slots, "footer")])], 40, yl)])
             }
         }
-    },
-    os = xe(rs, [
-        ["__scopeId", "data-v-336c341c"]
-    ]);
+    };
 
-function xr(a, e, n = {
-    equals(l, r) {
-        return l == r
+function Mr(a, e, n = {
+    equals(i, r) {
+        return i == r
     }
 }) {
-    let l = e.length,
+    let i = e.length,
         r = a.length,
-        u = 1,
-        t = l + r;
+        s = 1,
+        t = i + r;
     n.maxEditLength && (t = Math.min(t, n.maxEditLength));
     let o = [{
             newPos: -1,
             components: []
         }],
-        i = Zn(n, o[0], e, a, 0);
-    if (o[0].newPos + 1 >= l && i + 1 >= r) return [{
+        l = ar(n, o[0], e, a, 0);
+    if (o[0].newPos + 1 >= i && l + 1 >= r) return [{
         value: e,
         count: e.length
     }];
-    for (u = 1; u <= t; ++u)
-        for (let s = -1 * u; s <= u; s += 2) {
-            let c, f = o[s - 1],
-                d = o[s + 1],
-                v = (d ? d.newPos : 0) - s;
-            f && (o[s - 1] = void 0);
-            let h = f && f.newPos + 1 < l,
-                p = d && 0 <= v && v < r;
-            if (!h && !p) {
-                o[s] = void 0;
+    for (s = 1; s <= t; ++s)
+        for (let u = -1 * s; u <= s; u += 2) {
+            let f, c = o[u - 1],
+                d = o[u + 1],
+                v = (d ? d.newPos : 0) - u;
+            c && (o[u - 1] = void 0);
+            let p = c && c.newPos + 1 < i,
+                h = d && 0 <= v && v < r;
+            if (!p && !h) {
+                o[u] = void 0;
                 continue
             }
-            if (!h || p && f.newPos < d.newPos ? (c = is(d), kn(c.components, void 0, !0)) : (c = f, c.newPos++, kn(c.components, !0, void 0)), v = Zn(n, c, e, a, s), c.newPos + 1 >= l && v + 1 >= r) return as(n, c.components, e, a);
-            o[s] = c
+            if (!p || h && c.newPos < d.newPos ? (f = Pl(d), ir(f.components, void 0, !0)) : (f = c, f.newPos++, ir(f.components, !0, void 0)), v = ar(n, f, e, a, u), f.newPos + 1 >= i && v + 1 >= r) return Il(n, f.components, e, a);
+            o[u] = f
         }
 }
 
-function Zn({
+function ar({
     equals: a
-}, e, n, l, r) {
-    let u = n.length,
-        t = l.length,
+}, e, n, i, r) {
+    let s = n.length,
+        t = i.length,
         o = e.newPos,
-        i = o - r,
-        s = 0;
-    for (; o + 1 < u && i + 1 < t && a(n[o + 1], l[i + 1]);) o++, i++, s++;
-    return s && e.components.push({
-        count: s
-    }), e.newPos = o, i
+        l = o - r,
+        u = 0;
+    for (; o + 1 < s && l + 1 < t && a(n[o + 1], i[l + 1]);) o++, l++, u++;
+    return u && e.components.push({
+        count: u
+    }), e.newPos = o, l
 }
 
-function kn(a, e, n) {
-    let l = a[a.length - 1];
-    l && l.added === e && l.removed === n ? a[a.length - 1] = {
-        count: l.count + 1,
+function ir(a, e, n) {
+    let i = a[a.length - 1];
+    i && i.added === e && i.removed === n ? a[a.length - 1] = {
+        count: i.count + 1,
         added: e,
         removed: n
     } : a.push({
         count: 1,
         added: e,
         removed: n
     })
 }
 
-function as({
+function Il({
     equals: a,
     useLongestToken: e
-}, n, l, r) {
-    let u = 0,
+}, n, i, r) {
+    let s = 0,
         t = n.length,
         o = 0,
-        i = 0;
-    for (; u < t; u++) {
-        let c = n[u];
-        if (c.removed) {
-            if (c.value = r.slice(i, i + c.count), i += c.count, u && n[u - 1].added) {
-                let f = n[u - 1];
-                n[u - 1] = n[u], n[u] = f
+        l = 0;
+    for (; s < t; s++) {
+        let f = n[s];
+        if (f.removed) {
+            if (f.value = r.slice(l, l + f.count), l += f.count, s && n[s - 1].added) {
+                let c = n[s - 1];
+                n[s - 1] = n[s], n[s] = c
             }
         } else {
-            if (!c.added && e) {
-                let f = l.slice(o, o + c.count);
-                f = f.map(function(d, v) {
-                    let h = r[i + v];
-                    return h.length > d.length ? h : d
-                }), c.value = f
-            } else c.value = l.slice(o, o + c.count);
-            o += c.count, c.added || (i += c.count)
+            if (!f.added && e) {
+                let c = i.slice(o, o + f.count);
+                c = c.map(function(d, v) {
+                    let p = r[l + v];
+                    return p.length > d.length ? p : d
+                }), f.value = c
+            } else f.value = i.slice(o, o + f.count);
+            o += f.count, f.added || (l += f.count)
         }
     }
-    let s = n[t - 1];
-    return t > 1 && typeof s.value == "string" && (s.added || s.removed) && a("", s.value) && (n[t - 2].value += s.value, n.pop()), n
+    let u = n[t - 1];
+    return t > 1 && typeof u.value == "string" && (u.added || u.removed) && a("", u.value) && (n[t - 2].value += u.value, n.pop()), n
 }
 
-function is(a) {
+function Pl(a) {
     return {
         newPos: a.newPos,
         components: a.components.slice(0)
     }
 }
 
-function ss(a, e, n) {
-    const l = (o, i) => !a.every(s => o[s] !== i[s]),
-        r = (o, i) => a.every(s => o[s] === i[s]),
-        u = xr(e || [], n || [], {
-            equals: l
+function Cl(a, e, n) {
+    const i = (o, l) => !a.every(u => o[u] !== l[u]),
+        r = (o, l) => a.every(u => o[u] === l[u]),
+        s = Mr(e || [], n || [], {
+            equals: i
         });
     let t = 0;
-    for (let o = 0; o < u.length; ++o) {
-        if (console.assert(u[o].count === u[o].value.length), u[o].added) continue;
-        if (u[o].removed) {
-            t += u[o].count;
+    for (let o = 0; o < s.length; ++o) {
+        if (console.assert(s[o].count === s[o].value.length), s[o].added) continue;
+        if (s[o].removed) {
+            t += s[o].count;
             continue
         }
-        let i, s;
-        for (i = 0; i < u[o].value.length && r(e[t + i], u[o].value[i]); ++i);
-        if (i == u[o].value.length) {
-            t += u[o].count;
+        let l, u;
+        for (l = 0; l < s[o].value.length && r(e[t + l], s[o].value[l]); ++l);
+        if (l == s[o].value.length) {
+            t += s[o].count;
             continue
         }
-        for (s = i + 1; s < u[o].value.length && !r(e[t + s], u[o].value[s]); ++s);
-        if (console.assert(s <= u[o].value.length), i > 0 && (u.splice(o, 0, {
-                count: i,
-                value: u[o].value.slice(0, i)
-            }), ++o), u[o].value = u[o].value.slice(i), u[o].count = s - i, u[o].changed = !0, s - i < u[o].value.length) {
-            const c = u[o].value.length - (s - i);
-            u.splice(o + 1, 0, {
-                count: c,
-                value: u[o].value.slice(s - i)
-            }), u[o].value = u[o].value.slice(0, s - i)
-        }
-        console.assert(u[o].value.every((c, f) => !r(e[t + i + f], c))), u[o].differences = u[o].value.map((c, f) => ({
-            previous: e[t + i + f],
-            current: c
-        })), t += s
+        for (u = l + 1; u < s[o].value.length && !r(e[t + u], s[o].value[u]); ++u);
+        if (console.assert(u <= s[o].value.length), l > 0 && (s.splice(o, 0, {
+                count: l,
+                value: s[o].value.slice(0, l)
+            }), ++o), s[o].value = s[o].value.slice(l), s[o].count = u - l, s[o].changed = !0, u - l < s[o].value.length) {
+            const f = s[o].value.length - (u - l);
+            s.splice(o + 1, 0, {
+                count: f,
+                value: s[o].value.slice(u - l)
+            }), s[o].value = s[o].value.slice(0, u - l)
+        }
+        console.assert(s[o].value.every((f, c) => !r(e[t + l + c], f))), s[o].differences = s[o].value.map((f, c) => ({
+            previous: e[t + l + c],
+            current: f
+        })), t += u
     }
-    return u
+    return s
 }
-const ls = {
+const Dl = {
         key: 0
     },
-    us = {
+    Al = {
         key: 1
     },
-    fs = {
+    Rl = {
         __name: "InlineDiff",
         props: {
             current: {
                 type: String,
                 required: !0
             },
             previous: {
@@ -5573,52 +5708,52 @@
                 required: !0
             }
         },
         setup(a) {
             const {
                 current: e,
                 previous: n
-            } = a, l = Qt(() => xr(n.split(""), e.split(""), {
-                equals: (r, u) => r == u,
+            } = a, i = qt(() => Mr(n.split(""), e.split(""), {
+                equals: (r, s) => r == s,
                 maxEditLength: Math.max(n.length, e.length) * .5
             }));
-            return (r, u) => B(l) ? (K(), Y("span", us, [(K(!0), Y(Dt, null, Gt(B(l), t => (K(), Y(Dt, null, [t.added || t.removed ? (K(), Ke(or(t.added ? "ins" : "del"), {
+            return (r, s) => K(i) ? (U(), W("span", Al, [(U(!0), W(bt, null, Gt(K(i), t => (U(), W(bt, null, [t.added || t.removed ? (U(), ce(Xe(t.added ? "ins" : "del"), {
                 key: 0
             }, {
-                default: te(() => [Zt(it(t.value.join("")), 1)]),
+                default: Nt(() => [Bt(it(t.value.join("")), 1)]),
                 _: 2
-            }, 1024)) : (K(), Y(Dt, {
+            }, 1024)) : (U(), W(bt, {
                 key: 1
-            }, [Zt(it(t.value.join("")), 1)], 64))], 64))), 256))])) : (K(), Y("span", ls, [Z("del", null, it(a.previous), 1), Z("ins", null, it(a.current), 1)]))
+            }, [Bt(it(t.value.join("")), 1)], 64))], 64))), 256))])) : (U(), W("span", Dl, [X("del", null, it(a.previous), 1), X("ins", null, it(a.current), 1)]))
         }
     };
-const cs = {
+const wl = {
         class: "filter-output-table"
     },
-    ds = {
+    Ml = {
         key: 0
     },
-    vs = {
+    Nl = {
         key: 0
     },
-    hs = ["colspan"],
-    ps = {
+    jl = ["colspan"],
+    Fl = {
         key: 0,
         class: "controls"
     },
-    gs = {
+    $l = {
         key: 0,
         class: "table-diff"
     },
-    ms = ["lang"],
-    ys = {
+    Ll = ["lang"],
+    Vl = {
         key: 1
     },
-    bs = ["lang"],
-    Ss = {
+    Ul = ["lang"],
+    Gl = {
         __name: "FilterOutputTable",
         props: {
             languages: {
                 type: Array
             },
             rows: {
                 type: Array
@@ -5626,448 +5761,476 @@
             refRows: {
                 type: Array,
                 default: null
             },
             displayAsRows: {
                 type: Boolean,
                 default: !1
+            },
+            displayWhitespace: {
+                type: Boolean,
+                default: !1
             }
         },
         setup(a) {
             const e = a,
-                n = Jt(),
-                l = Qt(() => e.refRows !== null),
-                r = Qt(() => dn(e.refRows !== null ? ss(e.languages, e.refRows, e.rows) : [])),
-                u = Qt(() => {
-                    let s = 0,
-                        c = 0,
-                        f = 0;
+                n = zt(),
+                i = qt(() => e.refRows !== null),
+                r = qt(() => pn(e.refRows !== null ? Cl(e.languages, e.refRows, e.rows) : [])),
+                s = qt(() => {
+                    let p = 0,
+                        h = 0,
+                        m = 0;
                     return r.value.forEach(({
-                        added: d,
-                        removed: v,
-                        changed: h,
-                        count: p
+                        added: g,
+                        removed: y,
+                        changed: O,
+                        count: E
                     }) => {
-                        d ? s += p : v ? c += p : h && (f += p)
+                        g ? p += E : y ? h += E : O && (m += E)
                     }), {
-                        additions: s,
-                        deletions: c,
-                        changes: f
+                        additions: p,
+                        deletions: h,
+                        changes: m
                     }
                 });
 
             function t() {
-                const s = n.value.querySelectorAll("tr.added, tr.removed, tr.changed");
-                let c = 0;
-                for (; c < s.length && !(s[c].offsetTop > n.value.clientHeight + n.value.scrollTop); ++c);
-                const f = s[(s.length + c) % s.length];
+                const p = n.value.querySelectorAll("tr.added, tr.removed, tr.changed");
+                let h = 0;
+                for (; h < p.length && !(p[h].offsetTop > n.value.clientHeight + n.value.scrollTop); ++h);
+                const m = p[(p.length + h) % p.length];
                 n.value.scrollTo({
-                    top: f.offsetTop + f.offsetHeight - n.value.clientHeight,
+                    top: m.offsetTop + m.offsetHeight - n.value.clientHeight,
                     behavior: "smooth"
                 })
             }
 
-            function o(s) {
-                const c = new Intl.DisplayNames([], {
+            function o(p) {
+                const h = new Intl.DisplayNames([], {
                     type: "language"
                 });
                 try {
-                    return c.of(s)
+                    return h.of(p)
                 } catch {
-                    return s
+                    return p
                 }
             }
-            const i = Jt();
-            return nr(() => {
-                if (i.value.hidden = !l.value) return;
-                const s = n.value.clientHeight,
-                    c = n.value.firstElementChild.clientHeight;
-                i.value.width = 16, i.value.height = s;
-                const f = i.value.getContext("2d"),
+            const l = zt();
+
+            function u() {
+                if (l.value.hidden = !i.value) return;
+                const p = n.value.clientHeight,
+                    h = n.value.firstElementChild.clientHeight;
+                l.value.width = 16, l.value.height = p;
+                const m = l.value.getContext("2d"),
                     {
-                        width: d,
-                        height: v
-                    } = i.value;
-                f.clearRect(0, 0, d, v);
-                const h = {
+                        width: g,
+                        height: y
+                    } = l.value;
+                m.clearRect(0, 0, g, y);
+                const O = {
                     added: "green",
                     removed: "red",
                     changed: "yellow"
                 };
-                n.value.querySelectorAll("tbody tr:is(.added, .removed, .changed)").forEach(p => {
-                    f.fillStyle = h[p.className], f.fillRect(0, p.offsetTop / c * s, d, Math.max(p.offsetHeight / c, 1))
+                n.value.querySelectorAll("tbody tr:is(.added, .removed, .changed)").forEach(E => {
+                    m.fillStyle = O[E.className], m.fillRect(0, E.offsetTop / h * p, g, Math.max(E.offsetHeight / h * p, 1))
                 })
-            }), (s, c) => (K(), Y("div", cs, [Z("div", {
+            }
+            cr(u);
+            const f = new ResizeObserver(u);
+            jn(() => f.observe(n.value)), ur(() => f.unobserve(n.value));
+            const c = {
+                    "\xA0": "\u2423",
+                    "\u202F": "\u2423",
+                    "\u2007": "\u2423",
+                    "\u2060": "\u2423",
+                    " ": "\xB7"
+                },
+                d = new RegExp(Object.keys(c).join("|"), "g");
+
+            function v(p) {
+                return e.displayWhitespace ? p.replace(d, h => c[h]) : p
+            }
+            return (p, h) => (U(), W("div", wl, [X("div", {
                 ref_key: "outputElement",
                 ref: n,
-                class: Be(["sample", {
+                class: We(["sample", {
                     "display-as-rows": e.displayAsRows
                 }])
-            }, [a.rows ? (K(), Y("table", ds, [Z("thead", null, [Z("tr", null, [(K(!0), Y(Dt, null, Gt(e.languages, f => (K(), Y("th", {
-                key: f
-            }, it(o(f)), 1))), 128))]), B(l) ? (K(), Y("tr", vs, [Z("td", {
+            }, [a.rows ? (U(), W("table", Ml, [X("thead", null, [X("tr", null, [(U(!0), W(bt, null, Gt(e.languages, m => (U(), W("th", {
+                key: m
+            }, it(o(m)), 1))), 128))]), K(i) ? (U(), W("tr", Nl, [X("td", {
                 colspan: e.languages.length
-            }, [B(u).additions || B(u).deletions || B(u).changes ? (K(), Y("div", ps, [Z("span", null, "Comparing sample to the filtered sample: " + it(B(u).additions) + " lines added, " + it(B(u).deletions) + " lines removed, and " + it(B(u).changes) + " lines changed.", 1), Z("button", {
-                onClick: c[0] || (c[0] = f => t()),
+            }, [K(s).additions || K(s).deletions || K(s).changes ? (U(), W("div", Fl, [X("span", null, "Comparing sample to the filtered sample: " + it(K(s).additions) + " lines added, " + it(K(s).deletions) + " lines removed, and " + it(K(s).changes) + " lines changed.", 1), X("button", {
+                onClick: h[0] || (h[0] = m => t()),
                 title: "Scroll to next difference"
-            }, "Next")])) : ee("", !0)], 8, hs)])) : ee("", !0)]), B(l) ? (K(), Y("tbody", gs, [(K(!0), Y(Dt, null, Gt(B(r), (f, d) => (K(), Y(Dt, null, [(K(!0), Y(Dt, null, Gt(f.value, (v, h) => (K(), Y("tr", {
-                key: `${d}:${h}`,
-                class: Be({
-                    added: f.added,
-                    removed: f.removed,
-                    changed: f.changed
+            }, "Next")])) : _t("", !0)], 8, jl)])) : _t("", !0)]), K(i) ? (U(), W("tbody", $l, [(U(!0), W(bt, null, Gt(K(r), (m, g) => (U(), W(bt, null, [(U(!0), W(bt, null, Gt(m.value, (y, O) => (U(), W("tr", {
+                key: `${g}:${O}`,
+                class: We({
+                    added: m.added,
+                    removed: m.removed,
+                    changed: m.changed
                 })
-            }, [(K(!0), Y(Dt, null, Gt(e.languages, p => (K(), Y("td", {
-                key: p,
-                lang: p
-            }, [f.changed ? (K(), Ke(fs, {
+            }, [(U(!0), W(bt, null, Gt(e.languages, E => (U(), W("td", {
+                key: E,
+                lang: E
+            }, [m.changed ? (U(), ce(Rl, {
                 key: 0,
                 class: "inline-diff",
-                current: v[p],
-                previous: f.differences[h].previous[p]
-            }, null, 8, ["current", "previous"])) : (K(), Y(Dt, {
+                current: v(y[E]),
+                previous: v(m.differences[O].previous[E])
+            }, null, 8, ["current", "previous"])) : (U(), W(bt, {
                 key: 1
-            }, [Zt(it(v[p]), 1)], 64))], 8, ms))), 128))], 2))), 128))], 64))), 256))])) : (K(), Y("tbody", ys, [(K(!0), Y(Dt, null, Gt(e.rows, (f, d) => (K(), Y("tr", {
-                key: d
-            }, [(K(!0), Y(Dt, null, Gt(e.languages, v => (K(), Y("td", {
-                key: v,
-                lang: v
-            }, it(f[v]), 9, bs))), 128))]))), 128))]))])) : ee("", !0), Z("canvas", {
+            }, [Bt(it(v(y[E])), 1)], 64))], 8, Ll))), 128))], 2))), 128))], 64))), 256))])) : (U(), W("tbody", Vl, [(U(!0), W(bt, null, Gt(e.rows, (m, g) => (U(), W("tr", {
+                key: g
+            }, [(U(!0), W(bt, null, Gt(e.languages, y => (U(), W("td", {
+                key: y,
+                lang: y
+            }, it(v(m[y])), 9, Ul))), 128))]))), 128))]))])) : _t("", !0), X("canvas", {
                 class: "gutter",
                 ref_key: "gutter",
-                ref: i,
+                ref: l,
                 width: "16"
             }, null, 512)], 2)]))
         }
     },
-    Es = xe(Ss, [
-        ["__scopeId", "data-v-3cc6db50"]
+    Bl = ne(Gl, [
+        ["__scopeId", "data-v-7fccf6d5"]
     ]);
-const xs = a => (Mn("data-v-2f50d990"), a = a(), wn(), a),
-    Os = {
+const Kl = a => ($n("data-v-d9732d88"), a = a(), Fn(), a),
+    Hl = {
         class: "clean-corpus-container"
     },
-    Ts = {
+    Wl = {
         class: "output-panel"
     },
-    Is = {
+    Xl = {
         class: "controls"
     },
-    Ps = {
+    Yl = {
         class: "button-group"
     },
-    Cs = ["disabled"],
-    Ds = ["disabled"],
-    As = {
+    zl = ["disabled"],
+    Jl = ["disabled"],
+    Ql = {
         key: 0,
         class: "line-count",
         title: "Number of lines in sample"
     },
-    Rs = {
+    Zl = {
         class: "filter-output"
     },
-    ws = {
+    kl = {
         key: 0,
         class: "filter-error",
         translate: "no"
     },
-    Ms = {
+    ql = {
         class: "filter-container"
     },
-    Ns = {
+    _l = {
         class: "filter-input"
     },
-    js = ["title"],
-    Fs = xs(() => Z("br", null, null, -1)),
-    Ls = {
+    ts = ["title"],
+    es = Kl(() => X("br", null, null, -1)),
+    ns = {
         class: "filter-name"
     },
-    $s = {
+    rs = {
         key: 0,
         class: "line-count",
         title: "Line count"
     },
-    Us = ["onClick"],
-    Vs = {
+    os = ["onClick"],
+    as = {
         class: "filter"
     },
-    Gs = {
+    is = {
         class: "property-list"
     },
-    Bs = ["title"],
-    Ks = ["onClick"],
-    Hs = {
+    ls = ["title"],
+    ss = ["onClick"],
+    us = {
         __name: "FilterEditor",
         props: {
             dataset: Object
         },
         setup(a) {
             const {
                 dataset: e
-            } = a, n = navigator.platform.match(/^(Mac|iPhone$)/) ? "Meta" : "Control", l = 1e3, r = Jt(!1), u = ["original", "clean", "changes"], t = Jt("clean"), o = Jt(!1), i = Fi(), s = Ka(e), c = Qt(() => {
+            } = a, n = navigator.platform.match(/^(Mac|iPhone$)/) ? "Meta" : "Control", i = 1e3, r = zt(!1), s = zt(!1), t = ["original", "clean", "changes"], o = zt("clean"), l = zt(!1), u = Hi(), f = Ja(e), c = qt(() => {
                 if (!(e != null && e.columns)) return [];
-                const O = Array.from(Object.keys(e.columns)).sort();
-                return e.name.includes(O.reverse().join("-")) || O.reverse(), O
-            }), f = Jt([]), d = Qt(() => f.value.length > 0 ? f.value[f.value.length - 1] : null), v = Qt(() => f.value.length > 0 ? f.value[0] : null);
-            async function h(O, D, {
-                signal: G
+                const P = Array.from(Object.keys(e.columns)).sort();
+                return e.name.includes(P.reverse().join("-")) || P.reverse(), P
+            }), d = zt([]), v = qt(() => d.value.length > 0 ? d.value[d.value.length - 1] : null), p = qt(() => d.value.length > 0 ? d.value[0] : null);
+            async function h(P, M, {
+                signal: D
             }) {
-                o.value = !0, f.value = [];
+                l.value = !0, d.value = [];
                 try {
-                    const A = Ni(`/api/datasets/${encodeURIComponent(O.name)}/sample`, {
+                    const R = Bi(`/api/datasets/${encodeURIComponent(P.name)}/sample`, {
                         method: "POST",
-                        signal: G,
+                        signal: D,
                         headers: {
                             "Content-Type": "application/json",
                             Accept: "application/json"
                         },
-                        body: JSON.stringify(D, null, 2)
+                        body: JSON.stringify(M, null, 2)
                     });
-                    for await (let M of A) G.aborted || f.value.push(dn(M))
-                } catch (A) {
-                    if (A.toString().indexOf("The operation was aborted") === -1 && A.toString().indexOf("The user aborted a request") === -1) throw A
+                    for await (let H of R) D.aborted || d.value.push(pn(H))
+                } catch (R) {
+                    if (R.toString().indexOf("The operation was aborted") === -1 && R.toString().indexOf("The user aborted a request") === -1) throw R
                 } finally {
-                    o.value = !1
+                    l.value = !1
                 }
             }
-            ar([s.steps, e], (O, D, G) => {
-                const A = () => {
-                    const M = new AbortController;
-                    G(() => M.abort()), h(e, s.steps.value, M)
+            vr([f.steps, e], (P, M, D) => {
+                const R = () => {
+                    const H = new AbortController;
+                    D(() => H.abort()), h(e, f.steps.value, H)
                 };
-                if (f.value.length === 0) A();
+                if (d.value.length === 0) R();
                 else {
-                    const M = setTimeout(A, l);
-                    G(() => clearTimeout(M))
+                    const H = setTimeout(R, i);
+                    D(() => clearTimeout(H))
                 }
             }, {
                 immediate: !0
             });
 
-            function p(O) {
+            function m(P) {
                 return {
-                    id: ir(),
-                    filter: O.name,
-                    language: Er({
-                        filter: O.name
+                    id: Ln(),
+                    filter: P.name,
+                    language: Rr({
+                        filter: P.name
                     }) ? c.value[0] : null,
-                    parameters: Object.fromEntries(Object.entries(O.parameters).map(([D, G]) => [D, G.default]))
+                    parameters: Object.fromEntries(Object.entries(P.parameters).map(([M, D]) => [M, hr(D)]))
                 }
             }
 
-            function g(O) {
-                const D = p(O);
-                s.update([...s.steps.value, D]), T.get(D).value = !0
+            function g(P) {
+                const M = m(P);
+                f.update([...f.steps.value, M]), j.get(M).value = !0
             }
 
-            function b(O) {
-                s.update([...s.steps.value.slice(0, O), ...s.steps.value.slice(O + 1)])
+            function y(P) {
+                f.update([...f.steps.value.slice(0, P), ...f.steps.value.slice(P + 1)])
             }
 
-            function S(O, D) {
-                s.update([...s.steps.value.slice(0, O), D, ...s.steps.value.slice(O + 1)])
+            function O(P, M) {
+                f.update([...f.steps.value.slice(0, P), M, ...f.steps.value.slice(P + 1)])
             }
 
-            function P(O, D) {
-                O.setData("text/plain", JSON.stringify(p(D.__draggable_context.element), null, 2))
+            function E(P, M) {
+                P.setData("text/plain", JSON.stringify(m(M.__draggable_context.element), null, 2))
             }
 
-            function x(O, D) {
-                O.setData("text/plain", JSON.stringify(D.__draggable_context.element, null, 2))
+            function C(P, M) {
+                P.setData("text/plain", JSON.stringify(M.__draggable_context.element, null, 2))
             }
 
-            function C(O) {
-                return f.value.length === O + 1 ? "loading" : f.value.length >= O + 1 && f.value[O + 1].stderr ? "failed" : f.value.length >= O + 1 ? "loaded" : "pending"
+            function T(P) {
+                return d.value.length < P + 1 ? "pending" : d.value.length === P + 1 ? "loading" : d.value[P + 1].returncode === 0 ? "loaded" : "failed"
             }
 
-            function I(O, D) {
-                return D.length === 0 ? O : O.filter(({
-                    name: G,
-                    description: A
-                }) => G.toLowerCase().indexOf(D.toLowerCase()) !== -1 || A && A.toLowerCase().indexOf(D.toLowerCase()) !== -1)
+            function $(P, M) {
+                return M.length === 0 ? P : P.filter(({
+                    name: D,
+                    description: R
+                }) => D.toLowerCase().indexOf(M.toLowerCase()) !== -1 || R && R.toLowerCase().indexOf(M.toLowerCase()) !== -1)
             }
-            Jt();
-            const j = Qt(() => {
-                var O, D;
+            zt();
+            const L = qt(() => {
+                var P, M;
                 return {
-                    original: f.value.length > 0 ? (O = f.value[0].stdout) == null ? void 0 : O.length : null,
-                    clean: f.value.length === s.steps.value.length + 1 ? (D = f.value[s.steps.value.length].stdout) == null ? void 0 : D.length : null,
+                    original: d.value.length > 0 ? (P = d.value[0].stdout) == null ? void 0 : P.length : null,
+                    clean: d.value.length === f.steps.value.length + 1 ? (M = d.value[f.steps.value.length].stdout) == null ? void 0 : M.length : null,
                     changes: null
                 }
             });
 
-            function L(O) {
-                (n === "Meta" ? O.metaKey : O.ctrlKey) && O.keyCode === 90 && (O.shiftKey ? s.canRedo.value && s.redo() : s.canUndo.value && s.undo(), O.preventDefault())
+            function I(P) {
+                (n === "Meta" ? P.metaKey : P.ctrlKey) && P.keyCode === 90 && (P.shiftKey ? f.canRedo.value && f.redo() : f.canUndo.value && f.undo(), P.preventDefault())
             }
-            tr(() => {
-                document.body.addEventListener("keydown", L)
-            }), er(() => {
-                document.body.removeEventListener("keydown", L)
+            jn(() => {
+                document.body.addEventListener("keydown", I)
+            }), fr(() => {
+                document.body.removeEventListener("keydown", I)
             });
-            const T = new class {
+            const j = new class {
                 constructor() {
                     this.map = new Map
                 }
-                get(O) {
-                    return this.map.has(O.id) || this.map.set(O.id, Jt(!1)), this.map.get(O.id)
+                get(P) {
+                    return this.map.has(P.id) || this.map.set(P.id, zt(!1)), this.map.get(P.id)
                 }
             };
-            return (O, D) => {
-                var G, A, M, X;
-                return K(), Y("div", Os, [Z("div", Ts, [Z("header", Is, [Mt(Bi, {
+            return (P, M) => {
+                var D, R, H, F;
+                return U(), W("div", Hl, [X("div", Wl, [X("header", Xl, [Tt(or, {
                     modelValue: r.value,
-                    "onUpdate:modelValue": D[0] || (D[0] = R => r.value = R)
+                    "onUpdate:modelValue": M[0] || (M[0] = N => r.value = N)
                 }, {
-                    default: te(() => [Zt("Display as rows")]),
+                    default: Nt(() => [Bt("Display as rows")]),
                     _: 1
-                }, 8, ["modelValue"]), Z("div", Ps, [Z("button", {
+                }, 8, ["modelValue"]), Tt(or, {
+                    modelValue: s.value,
+                    "onUpdate:modelValue": M[1] || (M[1] = N => s.value = N)
+                }, {
+                    default: Nt(() => [Bt("Display whitespace")]),
+                    _: 1
+                }, 8, ["modelValue"]), X("div", Yl, [X("button", {
                     class: "icon-button",
                     title: "Undo",
-                    onClick: D[1] || (D[1] = R => B(s).undo()),
-                    disabled: !B(s).canUndo.value
-                }, [Mt(B(ja))], 8, Cs), Z("button", {
+                    onClick: M[2] || (M[2] = N => K(f).undo()),
+                    disabled: !K(f).canUndo.value
+                }, [Tt(K(Ha))], 8, zl), X("button", {
                     class: "icon-button",
                     title: "Redo",
-                    onClick: D[2] || (D[2] = R => B(s).redo()),
-                    disabled: !B(s).canRedo.value
-                }, [Mt(B(Fa))], 8, Ds)]), Mt(Xi, {
+                    onClick: M[3] || (M[3] = N => K(f).redo()),
+                    disabled: !K(f).canRedo.value
+                }, [Tt(K(Wa))], 8, Jl)]), Tt(qi, {
                     class: "table-buttons",
-                    modelValue: t.value,
-                    "onUpdate:modelValue": D[3] || (D[3] = R => t.value = R),
-                    options: u
+                    modelValue: o.value,
+                    "onUpdate:modelValue": M[4] || (M[4] = N => o.value = N),
+                    options: t
                 }, {
-                    default: te(({
-                        option: R
-                    }) => [Zt(it(R) + " ", 1), B(j)[R] !== null ? (K(), Y("small", As, it(B(j)[R]), 1)) : ee("", !0)]),
+                    default: Nt(({
+                        option: N
+                    }) => [Bt(it(N) + " ", 1), K(L)[N] !== null ? (U(), W("small", Ql, it(K(L)[N]), 1)) : _t("", !0)]),
                     _: 1
-                }, 8, ["modelValue"])]), Z("div", Rs, [Mt(Es, {
+                }, 8, ["modelValue"])]), X("div", Zl, [Tt(Bl, {
                     class: "filter-output-table",
-                    languages: B(c),
-                    rows: t.value === "original" ? (G = B(v)) == null ? void 0 : G.stdout : (A = B(d)) == null ? void 0 : A.stdout,
-                    "ref-rows": t.value === "changes" ? (M = B(v)) == null ? void 0 : M.stdout : null,
-                    "display-as-rows": r.value
-                }, null, 8, ["languages", "rows", "ref-rows", "display-as-rows"]), (X = B(d)) != null && X.stderr ? (K(), Y("div", ws, [Z("pre", null, it(B(d).stderr), 1)])) : ee("", !0)])]), Z("div", Ms, [Z("div", Ns, [Mt(B(Ha), {
-                    filter: I,
-                    options: B(i),
+                    languages: K(c),
+                    rows: o.value === "original" ? (D = K(p)) == null ? void 0 : D.stdout : (R = K(v)) == null ? void 0 : R.stdout,
+                    "ref-rows": o.value === "changes" ? (H = K(p)) == null ? void 0 : H.stdout : null,
+                    "display-as-rows": r.value,
+                    "display-whitespace": s.value
+                }, null, 8, ["languages", "rows", "ref-rows", "display-as-rows", "display-whitespace"]), (F = K(v)) != null && F.stderr ? (U(), W("div", kl, [X("pre", null, it(K(v).stderr), 1)])) : _t("", !0)])]), X("div", ql, [X("div", _l, [Tt(K(ka), {
+                    filter: $,
+                    options: K(u),
                     label: "name",
                     placeholder: "Search filters\u2026",
                     "onOption:selected": g
                 }, {
-                    option: te(({
-                        name: R,
-                        description: F
-                    }) => [Z("div", {
+                    option: Nt(({
+                        name: N,
+                        description: k
+                    }) => [X("div", {
                         class: "filter-search-result",
-                        title: F
-                    }, [Zt(it(R), 1), Fs, Z("small", null, it(F), 1)], 8, js)]),
+                        title: k
+                    }, [Bt(it(N), 1), es, X("small", null, it(k), 1)], 8, ts)]),
                     _: 1
-                }, 8, ["options"])]), Mt(B(Jn), {
+                }, 8, ["options"])]), Tt(K(Nn), {
                     tag: "ol",
                     class: "filter-steps",
                     "item-key": "id",
-                    modelValue: B(s).steps.value,
-                    "onUpdate:modelValue": D[4] || (D[4] = R => B(s).update(R)),
+                    modelValue: K(f).steps.value,
+                    "onUpdate:modelValue": M[5] || (M[5] = N => K(f).update(N)),
                     group: {
                         name: "filters"
                     },
                     "multi-drag": !0,
-                    "set-data": x,
-                    "multi-drag-key": B(n)
+                    "set-data": C,
+                    "multi-drag-key": K(n)
                 }, {
-                    item: te(({
-                        element: R,
-                        index: F
-                    }) => [Mt(os, {
+                    item: Nt(({
+                        element: N,
+                        index: k
+                    }) => [Tt(Tl, {
                         class: "filter-step",
-                        languages: B(c),
-                        modelValue: R,
-                        "onUpdate:modelValue": _ => S(F, _),
-                        open: B(T).get(R).value,
-                        "onUpdate:open": _ => B(T).get(R).value = _
+                        languages: K(c),
+                        modelValue: N,
+                        "onUpdate:modelValue": ot => O(k, ot),
+                        open: K(j).get(N).value,
+                        "onUpdate:open": ot => K(j).get(N).value = ot
                     }, {
-                        header: te(() => {
-                            var _, at;
-                            return [Z("span", Ls, it(R.filter), 1), C(F) === "loaded" ? (K(), Y("small", $s, it((at = (_ = f.value[F + 1]) == null ? void 0 : _.stdout) == null ? void 0 : at.length), 1)) : (K(), Y("small", {
+                        header: Nt(() => {
+                            var ot, St;
+                            return [X("span", ns, it(N.filter), 1), T(k) === "loaded" ? (U(), W("small", rs, it((St = (ot = d.value[k + 1]) == null ? void 0 : ot.stdout) == null ? void 0 : St.length), 1)) : (U(), W("small", {
                                 key: 1,
-                                class: Be(["loading-state", {
-                                    [C(F)]: !0
+                                class: We(["loading-state", {
+                                    [T(k)]: !0
                                 }])
-                            }, it(C(F)), 3)), Z("button", {
-                                onClick: xt => b(F),
+                            }, it(T(k)), 3)), X("button", {
+                                onClick: ct => y(k),
                                 class: "icon-button remove-filter-btn",
                                 title: "Do not use filter"
-                            }, [Mt(B(La))], 8, Us)]
+                            }, [Tt(K(Xa))], 8, os)]
                         }),
                         _: 2
                     }, 1032, ["languages", "modelValue", "onUpdate:modelValue", "open", "onUpdate:open"])]),
                     _: 1
-                }, 8, ["modelValue", "multi-drag-key"]), Mt(B(Jn), {
+                }, 8, ["modelValue", "multi-drag-key"]), Tt(K(Nn), {
                     tag: "ul",
                     class: "available-filters",
-                    modelValue: B(i),
-                    "onUpdate:modelValue": D[5] || (D[5] = R => qn(i) ? i.value = R : null),
+                    modelValue: K(u),
+                    "onUpdate:modelValue": M[6] || (M[6] = N => lr(u) ? u.value = N : null),
                     "item-key": "name",
                     group: {
                         name: "filters",
                         pull: "clone",
                         put: !1
                     },
                     sort: !1,
-                    "set-data": P,
-                    clone: p
+                    "set-data": E,
+                    clone: m
                 }, {
-                    item: te(({
-                        element: R
-                    }) => [Z("li", Vs, [Z("details", Gs, [Z("summary", null, [Z("span", {
-                        title: R.description,
+                    item: Nt(({
+                        element: N
+                    }) => [X("li", as, [X("details", is, [X("summary", null, [X("span", {
+                        title: N.description,
                         class: "filter-name"
-                    }, it(R.name), 9, Bs), Z("button", {
-                        onClick: F => g(R),
+                    }, it(N.name), 9, ls), X("button", {
+                        onClick: k => g(N),
                         class: "icon-button add-filter-btn",
                         title: "Use filter"
-                    }, [Mt(B($a))], 8, Ks)]), Z("p", null, it(R.description), 1)])])]),
+                    }, [Tt(K(pr))], 8, ss)]), X("p", null, it(N.description), 1)])])]),
                     _: 1
                 }, 8, ["modelValue"])])])
             }
         }
     },
-    Ws = xe(Hs, [
-        ["__scopeId", "data-v-2f50d990"]
+    fs = ne(us, [
+        ["__scopeId", "data-v-d9732d88"]
     ]);
-const Xs = {
+const cs = {
         class: "filter-editor"
     },
-    Ys = {
+    ds = {
         __name: "EditFiltersView",
         setup(a) {
-            const e = Ua(),
-                n = Qt(() => Ba(e.params.datasetName));
-            return (l, r) => {
-                const u = rr("RouterLink");
-                return K(), Y("div", Xs, [Z("header", null, [Z("h2", null, [Zt("Dataset: "), Z("em", null, it(B(n).name), 1)]), Mt(Ga, {
-                    dataset: B(n)
-                }, null, 8, ["dataset"])]), B(n) ? (K(), Ke(Ws, {
+            const e = Ya(),
+                n = qt(() => Za(e.params.datasetName));
+            return (i, r) => {
+                const s = dr("RouterLink");
+                return U(), W("div", cs, [X("header", null, [X("h2", null, [Bt("Dataset: "), X("em", null, it(K(n).name), 1)]), Tt(Qa, {
+                    dataset: K(n)
+                }, null, 8, ["dataset"])]), K(n) ? (U(), ce(fs, {
                     key: 0,
-                    dataset: B(n)
-                }, null, 8, ["dataset"])) : ee("", !0), (K(), Ke(_n, {
+                    dataset: K(n)
+                }, null, 8, ["dataset"])) : _t("", !0), (U(), ce(sr, {
                     to: ".navbar"
-                }, [Mt(u, {
+                }, [Tt(s, {
                     class: "import-data-button",
                     to: {
                         name: "add-dataset"
                     }
                 }, {
-                    default: te(() => [Zt(" Import dataset "), Mt(B(Va), {
+                    default: Nt(() => [Bt(" Import dataset "), Tt(K(za), {
                         class: "import-data-icon"
                     })]),
                     _: 1
                 })]))])
             }
         }
     },
-    ks = xe(Ys, [
+    gs = ne(ds, [
         ["__scopeId", "data-v-3883cacc"]
     ]);
 export {
-    ks as
+    gs as
     default
 };
```

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/ListDatasetsView.02d1a0b3.css` & `opuscleaner-0.2/opuscleaner/frontend/assets/ListDatasetsView.79aac80d.css`

 * *Files 19% similar despite different names*

```diff
@@ -1 +1 @@
-.import-data-button[data-v-10416316]{display:flex;align-items:center;border:none;border-radius:3px;height:40px;padding:0 30px;background-color:#17223d;color:#e4960e;font-size:18px;text-decoration:none;line-height:40px}.import-data-icon[data-v-10416316]{margin-left:5px}.datasets-table[data-v-10416316]{border:2px solid #1c3948;border-collapse:collapse;width:100%}.datasets-table thead[data-v-10416316]{background-color:#17223d;color:#e4960e;font-size:20px;text-align:left}.datasets-table tbody[data-v-10416316]{color:#17223d}.datasets-table thead th[data-v-10416316]{padding:20px 0 10px 10px;min-width:150px}.datasets-table tbody tr[data-v-10416316]{border-bottom:1px solid #1c3948;border-right:2px solid #1c3948}.datasets-table tbody td[data-v-10416316]{border-right:2px solid #1c3948}.datasets-table tbody tr td[data-v-10416316]{padding:10px}.category-tags[data-v-10416316]{display:flex}.tags[data-v-10416316]{width:45%}.filter-steps[data-v-10416316]{text-align:right}.illustration-container[data-v-10416316]{text-align:center;font-size:1.2em;line-height:2}.illustration-container img[data-v-10416316]{max-width:600px;width:calc(100% - 4em);margin:2em}.illustration-container .credits[data-v-10416316]{font-size:.8em}
+.import-data-button[data-v-45560305]{display:flex;align-items:center;border:none;border-radius:3px;height:40px;padding:0 30px;background-color:#17223d;color:#e4960e;font-size:18px;text-decoration:none;line-height:40px}.import-data-icon[data-v-45560305]{margin-left:5px}.datasets-table[data-v-45560305]{border:2px solid #1c3948;border-collapse:collapse;width:100%}.datasets-table thead[data-v-45560305]{background-color:#17223d;color:#e4960e;font-size:20px;text-align:left}.datasets-table tbody[data-v-45560305]{color:#17223d}.datasets-table thead th[data-v-45560305]{padding:20px 0 10px 10px;min-width:150px}.datasets-table tbody tr[data-v-45560305]{border-bottom:1px solid #1c3948;border-right:2px solid #1c3948}.datasets-table tbody td[data-v-45560305]{border-right:2px solid #1c3948}.datasets-table tbody tr td[data-v-45560305]{padding:10px}.category-tags[data-v-45560305]{display:flex}.tags[data-v-45560305]{width:45%}.filter-steps[data-v-45560305]{text-align:right}.illustration-container[data-v-45560305]{text-align:center;font-size:1.2em;line-height:2}.illustration-container img[data-v-45560305]{max-width:600px;width:calc(100% - 4em);margin:2em}.illustration-container .credits[data-v-45560305]{font-size:.8em}
```

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/ListDatasetsView.1513f813.js` & `opuscleaner-0.2/opuscleaner/frontend/assets/ListDatasetsView.0c61d7cc.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,39 +1,38 @@
 import {
-    _ as f,
+    _ as g,
     o,
     c as n,
     a as y,
     b as s,
-    w as c,
+    w as i,
     u as e,
-    R as i,
+    R as c,
     T as b,
     d as t,
     F as k,
     r as w,
     e as I,
     f as _,
     U as v,
     t as u,
     C as N,
     g as D,
     P as S,
     p as V,
     h as x
-} from "./index.490d1368.js";
+} from "./index.6cc31f0d.js";
 import {
     g as h,
-    T as C
-} from "./TagsEditor.8b755087.js";
-import {
-    g as F
-} from "./filtersteps.2a7228ad.js";
+    T as C,
+    a as F
+} from "./TagsEditor.23cf196f.js";
+import "./hacks.1ae1ba64.js";
 const L = "/frontend/assets/data-cuate.84693c76.svg";
-const d = l => (V("data-v-10416316"), l = l(), x(), l),
+const d = l => (V("data-v-45560305"), l = l(), x(), l),
     T = {
         class: "table-container-first-screen"
     },
     B = d(() => t("h2", {
         class: "table-title"
     }, "Your datasets", -1)),
     E = {
@@ -58,79 +57,80 @@
     }, [_("Image by "), t("a", {
         href: "https://www.freepik.com/free-vector/no-data-concept-illustration_8961448.htm",
         target: "_blank"
     }, "storyset on Freepik"), _(".")], -1)),
     q = {
         __name: "ListDatasetsView",
         setup(l) {
-            function g(r) {
+            function f(r) {
                 const p = Object.keys((r == null ? void 0 : r.columns) || {}),
                     a = new Intl.DisplayNames([], {
                         type: "language"
                     });
                 return p.map(m => {
                     try {
                         return a.of(m.replace("_", "-"))
                     } catch {
                         return m
                     }
                 })
             }
             return (r, p) => (o(), n("div", T, [(o(), y(b, {
                 to: ".navbar"
-            }, [s(e(i), {
+            }, [s(e(c), {
                 class: "import-data-button",
                 to: {
                     name: "add-dataset"
                 }
             }, {
-                default: c(() => [_(" Import dataset "), s(e(v), {
+                default: i(() => [_(" Import dataset "), s(e(v), {
                     class: "import-data-icon"
                 })]),
                 _: 1
             })])), B, e(h)().length > 0 ? (o(), n("table", E, [R, t("tbody", null, [(o(!0), n(k, null, w(e(h)(), a => (o(), n("tr", {
                 key: a.id
-            }, [t("td", null, u(a.name), 1), t("td", null, u(g(a).join("\u2013")), 1), t("td", j, [s(C, {
+            }, [t("td", null, u(a.name), 1), t("td", null, u(f(a).join("\u2013")), 1), t("td", j, [s(C, {
                 dataset: a
-            }, null, 8, ["dataset"])]), t("td", P, u(e(F)(a).steps.value.length), 1), t("td", null, [s(e(i), {
+            }, null, 8, ["dataset"])]), t("td", P, u(e(F)(a).steps.value.length), 1), t("td", null, [s(e(c), {
                 class: "icon-button",
                 title: "Show filter yaml",
                 to: {
                     name: "edit-filters-yaml",
                     params: {
-                        datasetName: a.name
+                        datasetName: a.name,
+                        format: "configuration-for-opusfilter.yaml"
                     }
                 }
             }, {
-                default: c(() => [s(e(N))]),
+                default: i(() => [s(e(N))]),
                 _: 2
-            }, 1032, ["to"]), s(e(i), {
+            }, 1032, ["to"]), s(e(c), {
                 class: "icon-button",
                 title: "Edit filters",
                 to: {
                     name: "edit-filters",
                     params: {
                         datasetName: a.name
                     }
                 }
             }, {
-                default: c(() => [s(e(D))]),
+                default: i(() => [s(e(D))]),
                 _: 2
-            }, 1032, ["to"]), s(e(i), {
+            }, 1032, ["to"]), s(e(c), {
                 class: "icon-button",
                 title: "Show dataset statistics",
                 to: {}
             }, {
-                default: c(() => [s(e(S))]),
+                default: i(() => [s(e(S))]),
                 _: 1
             })])]))), 128))])])) : (o(), n("div", U, [t("img", {
                 src: e(L)
             }, null, 8, A), O, Y])), s(e(I))]))
         }
     },
-    K = f(q, [
-        ["__scopeId", "data-v-10416316"]
+    K = g(q, [
+        ["__scopeId", "data-v-45560305"]
     ]);
 export {
     K as
     default
 };
```

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css` & `opuscleaner-0.2/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/data-cuate.84693c76.svg` & `opuscleaner-0.2/opuscleaner/frontend/assets/data-cuate.84693c76.svg`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg` & `opuscleaner-0.2/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/eu.24cff2c1.png` & `opuscleaner-0.2/opuscleaner/frontend/assets/eu.24cff2c1.png`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/horizon-europe.80625b0c.png` & `opuscleaner-0.2/opuscleaner/frontend/assets/horizon-europe.80625b0c.png`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/index.490d1368.js` & `opuscleaner-0.2/opuscleaner/frontend/assets/index.6cc31f0d.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -50,22 +50,22 @@
         }
         return t
     } else {
         if (he(e)) return e;
         if (ae(e)) return e
     }
 }
-const yl = /;(?![^(]*\))/g,
-    vl = /:(.+)/;
+const vl = /;(?![^(]*\))/g,
+    yl = /:(.+)/;
 
 function bl(e) {
     const t = {};
-    return e.split(yl).forEach(n => {
+    return e.split(vl).forEach(n => {
         if (n) {
-            const s = n.split(vl);
+            const s = n.split(yl);
             s.length > 1 && (t[s[0].trim()] = s[1].trim())
         }
     }), t
 }
 
 function os(e) {
     let t = "";
@@ -84,28 +84,28 @@
     let {
         class: t,
         style: n
     } = e;
     return t && !he(t) && (e.class = os(t)), n && (e.style = is(n)), e
 }
 
-function El(e, t) {
+function xl(e, t) {
     if (e.length !== t.length) return !1;
     let n = !0;
     for (let s = 0; n && s < e.length; s++) n = gt(e[s], t[s]);
     return n
 }
 
 function gt(e, t) {
     if (e === t) return !0;
     let n = Sr(e),
         s = Sr(t);
     if (n || s) return n && s ? e.getTime() === t.getTime() : !1;
     if (n = _n(e), s = _n(t), n || s) return e === t;
-    if (n = U(e), s = U(t), n || s) return n && s ? El(e, t) : !1;
+    if (n = U(e), s = U(t), n || s) return n && s ? xl(e, t) : !1;
     if (n = ae(e), s = ae(t), n || s) {
         if (!n || !s) return !1;
         const r = Object.keys(e).length,
             i = Object.keys(t).length;
         if (r !== i) return !1;
         for (const o in e) {
             const c = e.hasOwnProperty(o),
@@ -124,15 +124,15 @@
         [`Map(${t.size})`]: [...t.entries()].reduce((n, [s, r]) => (n[`${s} =>`] = r, n), {})
     } : kt(t) ? {
         [`Set(${t.size})`]: [...t.values()]
     } : ae(t) && !U(t) && !Fi(t) ? String(t) : t,
     re = {},
     Ht = [],
     Ke = () => {},
-    xl = () => !1,
+    El = () => !1,
     Cl = /^on[^a-z]/,
     Tn = e => Cl.test(e),
     tr = e => e.startsWith("onUpdate:"),
     pe = Object.assign,
     nr = (e, t) => {
         const n = e.indexOf(t);
         n > -1 && e.splice(n, 1)
@@ -155,15 +155,15 @@
     rr = e => he(e) && e !== "NaN" && e[0] !== "-" && "" + parseInt(e, 10) === e,
     un = rs(",key,ref,ref_for,ref_key,onVnodeBeforeMount,onVnodeMounted,onVnodeBeforeUpdate,onVnodeUpdated,onVnodeBeforeUnmount,onVnodeUnmounted"),
     cs = e => {
         const t = Object.create(null);
         return n => t[n] || (t[n] = e(n))
     },
     Pl = /-(\w)/g,
-    Be = cs(e => e.replace(Pl, (t, n) => n ? n.toUpperCase() : "")),
+    He = cs(e => e.replace(Pl, (t, n) => n ? n.toUpperCase() : "")),
     Al = /\B([A-Z])/g,
     Xe = cs(e => e.replace(Al, "-$1").toLowerCase()),
     as = cs(e => e.charAt(0).toUpperCase() + e.slice(1)),
     zn = cs(e => e ? `on${as(e)}` : ""),
     qt = (e, t) => !Object.is(e, t),
     Dt = (e, t) => {
         for (let n = 0; n < e.length; n++) e[n](t)
@@ -402,15 +402,15 @@
         if (r === "__v_isReactive") return !e;
         if (r === "__v_isReadonly") return e;
         if (r === "__v_isShallow") return t;
         if (r === "__v_raw" && i === (e ? t ? Ji : Qi : t ? Yi : qi).get(s)) return s;
         const o = U(s);
         if (!e && o && ee(Mr, r)) return Reflect.get(Mr, r, i);
         const c = Reflect.get(s, r, i);
-        return (_n(r) ? zi.has(r) : Il(r)) || (e || Le(s, "get", r), t) ? c : _e(c) ? o && rr(r) ? c : c.value : ae(c) ? e ? Xi(c) : be(c) : c
+        return (_n(r) ? zi.has(r) : Il(r)) || (e || Le(s, "get", r), t) ? c : _e(c) ? o && rr(r) ? c : c.value : ae(c) ? e ? Xi(c) : ve(c) : c
     }
 }
 const Bl = Ki(),
     Hl = Ki(!0);
 
 function Ki(e = !1) {
     return function(n, s, r, i) {
@@ -467,15 +467,15 @@
 function In(e, t, n = !1, s = !1) {
     e = e.__v_raw;
     const r = te(e),
         i = te(t);
     n || (t !== i && Le(r, "get", t), Le(r, "get", i));
     const {
         has: o
-    } = ds(r), c = s ? or : n ? lr : yn;
+    } = ds(r), c = s ? or : n ? lr : vn;
     if (o.call(r, t)) return c(e.get(t));
     if (o.call(r, i)) return c(e.get(i));
     e !== r && e.get(t)
 }
 
 function Mn(e, t = !1) {
     const n = this.__v_raw,
@@ -527,28 +527,28 @@
 }
 
 function Ln(e, t) {
     return function(s, r) {
         const i = this,
             o = i.__v_raw,
             c = te(o),
-            l = t ? or : e ? lr : yn;
+            l = t ? or : e ? lr : vn;
         return !e && Le(c, "iterate", Pt), o.forEach((a, u) => s.call(r, l(a), l(u), i))
     }
 }
 
 function Fn(e, t, n) {
     return function(...s) {
         const r = this.__v_raw,
             i = te(r),
             o = jt(i),
             c = e === "entries" || e === Symbol.iterator && o,
             l = e === "keys" && o,
             a = r[e](...s),
-            u = n ? or : t ? lr : yn;
+            u = n ? or : t ? lr : vn;
         return !t && Le(i, "iterate", l ? Bs : Pt), {
             next() {
                 const {
                     value: d,
                     done: h
                 } = a.next();
                 return h ? {
@@ -675,15 +675,15 @@
     }
 }
 
 function tc(e) {
     return e.__v_skip || !Object.isExtensible(e) ? 0 : ec(Tl(e))
 }
 
-function be(e) {
+function ve(e) {
     return Yt(e) ? e : ps(e, !1, Vi, Jl, qi)
 }
 
 function nc(e) {
     return ps(e, !1, zl, Xl, Yi)
 }
 
@@ -725,15 +725,15 @@
     const t = e && e.__v_raw;
     return t ? te(t) : e
 }
 
 function Gi(e) {
     return Yn(e, "__v_skip", !0), e
 }
-const yn = e => ae(e) ? be(e) : e,
+const vn = e => ae(e) ? ve(e) : e,
     lr = e => ae(e) ? Xi(e) : e;
 
 function cr(e) {
     ht && ze && (e = te(e), Ui(e.dep || (e.dep = ir())))
 }
 
 function gs(e, t) {
@@ -753,22 +753,22 @@
 }
 
 function to(e, t) {
     return _e(e) ? e : new sc(e, t)
 }
 class sc {
     constructor(t, n) {
-        this.__v_isShallow = n, this.dep = void 0, this.__v_isRef = !0, this._rawValue = n ? t : te(t), this._value = n ? t : yn(t)
+        this.__v_isShallow = n, this.dep = void 0, this.__v_isRef = !0, this._rawValue = n ? t : te(t), this._value = n ? t : vn(t)
     }
     get value() {
         return cr(this), this._value
     }
     set value(t) {
         const n = this.__v_isShallow || Qn(t) || Yt(t);
-        t = n ? t : te(t), qt(t, this._rawValue) && (this._rawValue = t, this._value = n ? t : yn(t), gs(this))
+        t = n ? t : te(t), qt(t, this._rawValue) && (this._rawValue = t, this._value = n ? t : vn(t), gs(this))
     }
 }
 
 function zf(e) {
     gs(e)
 }
 
@@ -803,15 +803,15 @@
     }
 }
 
 function Kf(e) {
     return new ic(e)
 }
 
-function He(e) {
+function Fe(e) {
     const t = U(e) ? new Array(e.length) : {};
     for (const n in e) t[n] = lc(e, n);
     return t
 }
 class oc {
     constructor(t, n, s) {
         this._object = t, this._key = n, this._defaultValue = s, this.__v_isRef = !0
@@ -923,23 +923,23 @@
         r = s ? e(...s) : e()
     } catch (i) {
         tn(i, t, n)
     }
     return r
 }
 
-function $e(e, t, n, s) {
+function Be(e, t, n, s) {
     if (Q(e)) {
         const i = nt(e, t, n, s);
         return i && sr(i) && i.catch(o => {
             tn(o, t, n)
         }), i
     }
     const r = [];
-    for (let i = 0; i < e.length; i++) r.push($e(e[i], t, n, s));
+    for (let i = 0; i < e.length; i++) r.push(Be(e[i], t, n, s));
     return r
 }
 
 function tn(e, t, n, s = !0) {
     const r = t ? t.vnode : null;
     if (t) {
         let i = t.parent;
@@ -961,60 +961,60 @@
     }
     gc(e, n, r, s)
 }
 
 function gc(e, t, n, s = !0) {
     console.error(e)
 }
-let vn = !1,
+let yn = !1,
     js = !1;
-const xe = [];
+const Ee = [];
 let Qe = 0;
 const zt = [];
 let et = null,
     Ct = 0;
 const io = Promise.resolve();
 let ar = null;
 
 function ur(e) {
     const t = ar || io;
     return e ? t.then(this ? e.bind(this) : e) : t
 }
 
 function mc(e) {
     let t = Qe + 1,
-        n = xe.length;
+        n = Ee.length;
     for (; t < n;) {
         const s = t + n >>> 1;
-        bn(xe[s]) < e ? t = s + 1 : n = s
+        bn(Ee[s]) < e ? t = s + 1 : n = s
     }
     return t
 }
 
 function ms(e) {
-    (!xe.length || !xe.includes(e, vn && e.allowRecurse ? Qe + 1 : Qe)) && (e.id == null ? xe.push(e) : xe.splice(mc(e.id), 0, e), oo())
+    (!Ee.length || !Ee.includes(e, yn && e.allowRecurse ? Qe + 1 : Qe)) && (e.id == null ? Ee.push(e) : Ee.splice(mc(e.id), 0, e), oo())
 }
 
 function oo() {
-    !vn && !js && (js = !0, ar = io.then(co))
+    !yn && !js && (js = !0, ar = io.then(co))
 }
 
 function _c(e) {
-    const t = xe.indexOf(e);
-    t > Qe && xe.splice(t, 1)
+    const t = Ee.indexOf(e);
+    t > Qe && Ee.splice(t, 1)
 }
 
 function lo(e) {
     U(e) ? zt.push(...e) : (!et || !et.includes(e, e.allowRecurse ? Ct + 1 : Ct)) && zt.push(e), oo()
 }
 
-function Br(e, t = vn ? Qe + 1 : 0) {
-    for (; t < xe.length; t++) {
-        const n = xe[t];
-        n && n.pre && (xe.splice(t, 1), t--, n())
+function Br(e, t = yn ? Qe + 1 : 0) {
+    for (; t < Ee.length; t++) {
+        const n = Ee[t];
+        n && n.pre && (Ee.splice(t, 1), t--, n())
     }
 }
 
 function Jn(e) {
     if (zt.length) {
         const t = [...new Set(zt)];
         if (zt.length = 0, et) {
@@ -1022,44 +1022,44 @@
             return
         }
         for (et = t, et.sort((n, s) => bn(n) - bn(s)), Ct = 0; Ct < et.length; Ct++) et[Ct]();
         et = null, Ct = 0
     }
 }
 const bn = e => e.id == null ? 1 / 0 : e.id,
-    yc = (e, t) => {
+    vc = (e, t) => {
         const n = bn(e) - bn(t);
         if (n === 0) {
             if (e.pre && !t.pre) return -1;
             if (t.pre && !e.pre) return 1
         }
         return n
     };
 
 function co(e) {
-    js = !1, vn = !0, xe.sort(yc);
+    js = !1, yn = !0, Ee.sort(vc);
     const t = Ke;
     try {
-        for (Qe = 0; Qe < xe.length; Qe++) {
-            const n = xe[Qe];
+        for (Qe = 0; Qe < Ee.length; Qe++) {
+            const n = Ee[Qe];
             n && n.active !== !1 && nt(n, null, 14)
         }
     } finally {
-        Qe = 0, xe.length = 0, Jn(), vn = !1, ar = null, (xe.length || zt.length) && co()
+        Qe = 0, Ee.length = 0, Jn(), yn = !1, ar = null, (Ee.length || zt.length) && co()
     }
 }
 let sn, $n = [];
 
-function vc(e, t) {
+function yc(e, t) {
     var n, s;
     sn = e, sn ? (sn.enabled = !0, $n.forEach(({
         event: r,
         args: i
     }) => sn.emit(r, ...i)), $n = []) : typeof window < "u" && window.HTMLElement && !(!((s = (n = window.navigator) === null || n === void 0 ? void 0 : n.userAgent) === null || s === void 0) && s.includes("jsdom")) ? ((t.__VUE_DEVTOOLS_HOOK_REPLAY__ = t.__VUE_DEVTOOLS_HOOK_REPLAY__ || []).push(i => {
-        vc(i, t)
+        yc(i, t)
     }), setTimeout(() => {
         sn || (t.__VUE_DEVTOOLS_HOOK_REPLAY__ = null, $n = [])
     }, 3e3)) : $n = []
 }
 
 function bc(e, t, ...n) {
     if (e.isUnmounted) return;
@@ -1071,21 +1071,21 @@
         const u = `${o==="modelValue"?"model":o}Modifiers`,
             {
                 number: d,
                 trim: h
             } = s[u] || re;
         h && (r = n.map(_ => _.trim())), d && (r = n.map(mt))
     }
-    let c, l = s[c = zn(t)] || s[c = zn(Be(t))];
-    !l && i && (l = s[c = zn(Xe(t))]), l && $e(l, e, 6, r);
+    let c, l = s[c = zn(t)] || s[c = zn(He(t))];
+    !l && i && (l = s[c = zn(Xe(t))]), l && Be(l, e, 6, r);
     const a = s[c + "Once"];
     if (a) {
         if (!e.emitted) e.emitted = {};
         else if (e.emitted[c]) return;
-        e.emitted[c] = !0, $e(a, e, 6, r)
+        e.emitted[c] = !0, Be(a, e, 6, r)
     }
 }
 
 function ao(e, t, n = !1) {
     const s = t.emitsCache,
         r = s.get(e);
     if (r !== void 0) return r;
@@ -1102,27 +1102,27 @@
     return !i && !c ? (ae(e) && s.set(e, null), null) : (U(i) ? i.forEach(l => o[l] = null) : pe(o, i), ae(e) && s.set(e, o), o)
 }
 
 function _s(e, t) {
     return !e || !Tn(t) ? !1 : (t = t.slice(2).replace(/Once$/, ""), ee(e, t[0].toLowerCase() + t.slice(1)) || ee(e, Xe(t)) || ee(e, t))
 }
 let Ce = null,
-    ys = null;
+    vs = null;
 
 function wn(e) {
     const t = Ce;
-    return Ce = e, ys = e && e.type.__scopeId || null, t
+    return Ce = e, vs = e && e.type.__scopeId || null, t
 }
 
 function Vf(e) {
-    ys = e
+    vs = e
 }
 
 function Wf() {
-    ys = null
+    vs = null
 }
 const qf = e => fr;
 
 function fr(e, t = Ce, n) {
     if (!t || e._n) return e;
     const s = (...r) => {
         s._d && Xr(-1);
@@ -1156,57 +1156,57 @@
         ctx: b,
         inheritAttrs: P
     } = e;
     let I, m;
     const p = wn(e);
     try {
         if (n.shapeFlag & 4) {
-            const x = r || s;
-            I = Me(u.call(x, x, d, i, _, h, b)), m = l
+            const E = r || s;
+            I = Me(u.call(E, E, d, i, _, h, b)), m = l
         } else {
-            const x = t;
-            I = Me(x.length > 1 ? x(i, {
+            const E = t;
+            I = Me(E.length > 1 ? E(i, {
                 attrs: l,
                 slots: c,
                 emit: a
-            }) : x(i, null)), m = t.props ? l : Ec(l)
+            }) : E(i, null)), m = t.props ? l : xc(l)
         }
-    } catch (x) {
-        hn.length = 0, tn(x, e, 1), I = ce(Te)
+    } catch (E) {
+        hn.length = 0, tn(E, e, 1), I = ce(Pe)
     }
-    let v = I;
+    let y = I;
     if (m && P !== !1) {
-        const x = Object.keys(m),
+        const E = Object.keys(m),
             {
                 shapeFlag: k
-            } = v;
-        x.length && k & 7 && (o && x.some(tr) && (m = xc(m, o)), v = rt(v, m))
+            } = y;
+        E.length && k & 7 && (o && E.some(tr) && (m = Ec(m, o)), y = rt(y, m))
     }
-    return n.dirs && (v = rt(v), v.dirs = v.dirs ? v.dirs.concat(n.dirs) : n.dirs), n.transition && (v.transition = n.transition), I = v, wn(p), I
+    return n.dirs && (y = rt(y), y.dirs = y.dirs ? y.dirs.concat(n.dirs) : n.dirs), n.transition && (y.transition = n.transition), I = y, wn(p), I
 }
 
 function wc(e) {
     let t;
     for (let n = 0; n < e.length; n++) {
         const s = e[n];
         if (Ot(s)) {
-            if (s.type !== Te || s.children === "v-if") {
+            if (s.type !== Pe || s.children === "v-if") {
                 if (t) return;
                 t = s
             }
         } else return
     }
     return t
 }
-const Ec = e => {
+const xc = e => {
         let t;
         for (const n in e)(n === "class" || n === "style" || Tn(n)) && ((t || (t = {}))[n] = e[n]);
         return t
     },
-    xc = (e, t) => {
+    Ec = (e, t) => {
         const n = {};
         for (const s in e)(!tr(s) || !(s.slice(9) in t)) && (n[s] = e[s]);
         return n
     };
 
 function Cc(e, t, n) {
     const {
@@ -1258,27 +1258,27 @@
         },
         hydrate: Ac,
         create: hr,
         normalize: Sc
     },
     Yf = Rc;
 
-function En(e, t) {
+function xn(e, t) {
     const n = e.props && e.props[t];
     Q(n) && n()
 }
 
 function Tc(e, t, n, s, r, i, o, c, l) {
     const {
         p: a,
         o: {
             createElement: u
         }
     } = l, d = u("div"), h = e.suspense = hr(e, r, s, t, d, n, i, o, c, l);
-    a(null, h.pendingBranch = e.ssContent, d, null, s, h, i, o), h.deps > 0 ? (En(e, "onPending"), En(e, "onFallback"), a(null, e.ssFallback, t, n, s, null, i, o), Kt(h, e.ssFallback)) : h.resolve()
+    a(null, h.pendingBranch = e.ssContent, d, null, s, h, i, o), h.deps > 0 ? (xn(e, "onPending"), xn(e, "onFallback"), a(null, e.ssFallback, t, n, s, null, i, o), Kt(h, e.ssFallback)) : h.resolve()
 }
 
 function Pc(e, t, n, s, r, i, o, c, {
     p: l,
     um: a,
     o: {
         createElement: u
@@ -1292,22 +1292,22 @@
             activeBranch: b,
             pendingBranch: P,
             isInFallback: I,
             isHydrating: m
         } = d;
     if (P) d.pendingBranch = h, Je(h, P) ? (l(P, h, d.hiddenContainer, null, r, d, i, o, c), d.deps <= 0 ? d.resolve() : I && (l(b, _, n, s, r, null, i, o, c), Kt(d, _))) : (d.pendingId++, m ? (d.isHydrating = !1, d.activeBranch = P) : a(P, r, d), d.deps = 0, d.effects.length = 0, d.hiddenContainer = u("div"), I ? (l(null, h, d.hiddenContainer, null, r, d, i, o, c), d.deps <= 0 ? d.resolve() : (l(b, _, n, s, r, null, i, o, c), Kt(d, _))) : b && Je(h, b) ? (l(b, h, n, s, r, d, i, o, c), d.resolve(!0)) : (l(null, h, d.hiddenContainer, null, r, d, i, o, c), d.deps <= 0 && d.resolve()));
     else if (b && Je(h, b)) l(b, h, n, s, r, d, i, o, c), Kt(d, h);
-    else if (En(t, "onPending"), d.pendingBranch = h, d.pendingId++, l(null, h, d.hiddenContainer, null, r, d, i, o, c), d.deps <= 0) d.resolve();
+    else if (xn(t, "onPending"), d.pendingBranch = h, d.pendingId++, l(null, h, d.hiddenContainer, null, r, d, i, o, c), d.deps <= 0) d.resolve();
     else {
         const {
             timeout: p,
-            pendingId: v
+            pendingId: y
         } = d;
         p > 0 ? setTimeout(() => {
-            d.pendingId === v && d.fallback(_)
+            d.pendingId === y && d.fallback(_)
         }, p) : p === 0 && d.fallback(_)
     }
 }
 
 function hr(e, t, n, s, r, i, o, c, l, a, u = !1) {
     const {
         p: d,
@@ -1331,26 +1331,26 @@
         timeout: typeof m == "number" ? m : -1,
         activeBranch: null,
         pendingBranch: null,
         isInFallback: !0,
         isHydrating: u,
         isUnmounted: !1,
         effects: [],
-        resolve(v = !1) {
+        resolve(y = !1) {
             const {
-                vnode: x,
+                vnode: E,
                 activeBranch: k,
                 pendingBranch: L,
                 pendingId: B,
                 effects: R,
                 parentComponent: z,
                 container: j
             } = p;
             if (p.isHydrating) p.isHydrating = !1;
-            else if (!v) {
+            else if (!y) {
                 const X = k && L.transition && L.transition.mode === "out-in";
                 X && (k.transition.afterLeave = () => {
                     B === p.pendingId && h(L, j, H, 0)
                 });
                 let {
                     anchor: H
                 } = p;
@@ -1362,58 +1362,58 @@
             for (; V;) {
                 if (V.pendingBranch) {
                     V.effects.push(...R), F = !0;
                     break
                 }
                 V = V.parent
             }
-            F || lo(R), p.effects = [], En(x, "onResolve")
+            F || lo(R), p.effects = [], xn(E, "onResolve")
         },
-        fallback(v) {
+        fallback(y) {
             if (!p.pendingBranch) return;
             const {
-                vnode: x,
+                vnode: E,
                 activeBranch: k,
                 parentComponent: L,
                 container: B,
                 isSVG: R
             } = p;
-            En(x, "onFallback");
+            xn(E, "onFallback");
             const z = b(k),
                 j = () => {
-                    !p.isInFallback || (d(null, v, B, z, L, null, R, c, l), Kt(p, v))
+                    !p.isInFallback || (d(null, y, B, z, L, null, R, c, l), Kt(p, y))
                 },
-                V = v.transition && v.transition.mode === "out-in";
+                V = y.transition && y.transition.mode === "out-in";
             V && (k.transition.afterLeave = j), p.isInFallback = !0, _(k, L, null, !0), V || j()
         },
-        move(v, x, k) {
-            p.activeBranch && h(p.activeBranch, v, x, k), p.container = v
+        move(y, E, k) {
+            p.activeBranch && h(p.activeBranch, y, E, k), p.container = y
         },
         next() {
             return p.activeBranch && b(p.activeBranch)
         },
-        registerDep(v, x) {
+        registerDep(y, E) {
             const k = !!p.pendingBranch;
             k && p.deps++;
-            const L = v.vnode.el;
-            v.asyncDep.catch(B => {
-                tn(B, v, 0)
+            const L = y.vnode.el;
+            y.asyncDep.catch(B => {
+                tn(B, y, 0)
             }).then(B => {
-                if (v.isUnmounted || p.isUnmounted || p.pendingId !== v.suspenseId) return;
-                v.asyncResolved = !0;
+                if (y.isUnmounted || p.isUnmounted || p.pendingId !== y.suspenseId) return;
+                y.asyncResolved = !0;
                 const {
                     vnode: R
-                } = v;
-                qs(v, B, !1), L && (R.el = L);
-                const z = !L && v.subTree.el;
-                x(v, R, P(L || v.subTree.el), L ? null : b(v.subTree), p, o, l), z && I(z), dr(v, R.el), k && --p.deps === 0 && p.resolve()
+                } = y;
+                qs(y, B, !1), L && (R.el = L);
+                const z = !L && y.subTree.el;
+                E(y, R, P(L || y.subTree.el), L ? null : b(y.subTree), p, o, l), z && I(z), dr(y, R.el), k && --p.deps === 0 && p.resolve()
             })
         },
-        unmount(v, x) {
-            p.isUnmounted = !0, p.activeBranch && _(p.activeBranch, n, v, x), p.pendingBranch && _(p.pendingBranch, n, v, x)
+        unmount(y, E) {
+            p.isUnmounted = !0, p.activeBranch && _(p.activeBranch, n, y, E), p.pendingBranch && _(p.pendingBranch, n, y, E)
         }
     };
     return p
 }
 
 function Ac(e, t, n, s, r, i, o, c, l) {
     const a = t.suspense = hr(t, s, n, e.parentNode, document.createElement("div"), null, r, i, o, c, !0),
@@ -1422,15 +1422,15 @@
 }
 
 function Sc(e) {
     const {
         shapeFlag: t,
         children: n
     } = e, s = t & 32;
-    e.ssContent = jr(s ? n.default : n), e.ssFallback = s ? jr(n.fallback) : ce(Te)
+    e.ssContent = jr(s ? n.default : n), e.ssFallback = s ? jr(n.fallback) : ce(Pe)
 }
 
 function jr(e) {
     let t;
     if (Q(e)) {
         const n = St && e._c;
         n && (e._d = !1, Jt()), e = e(), n && (e._d = !0, t = Oe, Ao())
@@ -1500,31 +1500,31 @@
     let l, a = !1,
         u = !1;
     if (_e(e) ? (l = () => e.value, a = Qn(e)) : Ut(e) ? (l = () => e, s = !0) : U(e) ? (u = !0, a = e.some(m => Ut(m) || Qn(m)), l = () => e.map(m => {
             if (_e(m)) return m.value;
             if (Ut(m)) return Tt(m);
             if (Q(m)) return nt(m, c, 2)
         })) : Q(e) ? t ? l = () => nt(e, c, 2) : l = () => {
-            if (!(c && c.isUnmounted)) return d && d(), $e(e, c, 3, [h])
+            if (!(c && c.isUnmounted)) return d && d(), Be(e, c, 3, [h])
         } : l = Ke, t && s) {
         const m = l;
         l = () => Tt(m())
     }
     let d, h = m => {
         d = I.onStop = () => {
             nt(m, c, 4)
         }
     };
-    if (Xt) return h = Ke, t ? n && $e(t, c, 3, [l(), u ? [] : void 0, h]) : l(), Ke;
+    if (Xt) return h = Ke, t ? n && Be(t, c, 3, [l(), u ? [] : void 0, h]) : l(), Ke;
     let _ = u ? [] : Dr;
     const b = () => {
         if (!!I.active)
             if (t) {
                 const m = I.run();
-                (s || a || (u ? m.some((p, v) => qt(p, _[v])) : qt(m, _))) && (d && d(), $e(t, c, 3, [m, _ === Dr ? void 0 : _, h]), _ = m)
+                (s || a || (u ? m.some((p, y) => qt(p, _[y])) : qt(m, _))) && (d && d(), Be(t, c, 3, [m, _ === Dr ? void 0 : _, h]), _ = m)
             } else I.run()
     };
     b.allowRecurse = !!t;
     let P;
     r === "sync" ? P = b : r === "post" ? P = () => ye(b, c && c.suspense) : (b.pre = !0, c && (b.id = c.uid), P = () => ms(b));
     const I = new us(l, P);
     return t ? n ? b() : _ = I.run() : r === "post" ? ye(I.run.bind(I), c && c.suspense) : I.run(), () => {
@@ -1534,17 +1534,17 @@
 
 function kc(e, t, n) {
     const s = this.proxy,
         r = he(e) ? e.includes(".") ? ho(s, e) : () => s[e] : e.bind(s, s);
     let i;
     Q(t) ? i = t : (i = t.handler, n = t);
     const o = me;
-    yt(this);
+    vt(this);
     const c = An(r, i.bind(s), n);
-    return o ? yt(o) : pt(), c
+    return o ? vt(o) : pt(), c
 }
 
 function ho(e, t) {
     const n = t.split(".");
     return () => {
         let s = e;
         for (let r = 0; r < n.length && s; r++) s = s[n[r]];
@@ -1574,78 +1574,78 @@
     };
     return On(() => {
         e.isMounted = !0
     }), mr(() => {
         e.isUnmounting = !0
     }), e
 }
-const Fe = [Function, Array],
+const $e = [Function, Array],
     Ic = {
         name: "BaseTransition",
         props: {
             mode: String,
             appear: Boolean,
             persisted: Boolean,
-            onBeforeEnter: Fe,
-            onEnter: Fe,
-            onAfterEnter: Fe,
-            onEnterCancelled: Fe,
-            onBeforeLeave: Fe,
-            onLeave: Fe,
-            onAfterLeave: Fe,
-            onLeaveCancelled: Fe,
-            onBeforeAppear: Fe,
-            onAppear: Fe,
-            onAfterAppear: Fe,
-            onAppearCancelled: Fe
+            onBeforeEnter: $e,
+            onEnter: $e,
+            onAfterEnter: $e,
+            onEnterCancelled: $e,
+            onBeforeLeave: $e,
+            onLeave: $e,
+            onAfterLeave: $e,
+            onLeaveCancelled: $e,
+            onBeforeAppear: $e,
+            onAppear: $e,
+            onAfterAppear: $e,
+            onAppearCancelled: $e
         },
         setup(e, {
             slots: t
         }) {
             const n = Nt(),
                 s = po();
             let r;
             return () => {
                 const i = t.default && pr(t.default(), !0);
                 if (!i || !i.length) return;
                 let o = i[0];
                 if (i.length > 1) {
                     for (const P of i)
-                        if (P.type !== Te) {
+                        if (P.type !== Pe) {
                             o = P;
                             break
                         }
                 }
                 const c = te(e),
                     {
                         mode: l
                     } = c;
                 if (s.isLeaving) return Ts(o);
                 const a = Ur(o);
                 if (!a) return Ts(o);
-                const u = xn(a, c, s, n);
+                const u = En(a, c, s, n);
                 Qt(a, u);
                 const d = n.subTree,
                     h = d && Ur(d);
                 let _ = !1;
                 const {
                     getTransitionKey: b
                 } = a.type;
                 if (b) {
                     const P = b();
                     r === void 0 ? r = P : P !== r && (r = P, _ = !0)
                 }
-                if (h && h.type !== Te && (!Je(a, h) || _)) {
-                    const P = xn(h, c, s, n);
+                if (h && h.type !== Pe && (!Je(a, h) || _)) {
+                    const P = En(h, c, s, n);
                     if (Qt(h, P), l === "out-in") return s.isLeaving = !0, P.afterLeave = () => {
                         s.isLeaving = !1, n.update()
                     }, Ts(o);
-                    l === "in-out" && a.type !== Te && (P.delayLeave = (I, m, p) => {
-                        const v = mo(s, h);
-                        v[String(h.key)] = h, I._leaveCb = () => {
+                    l === "in-out" && a.type !== Pe && (P.delayLeave = (I, m, p) => {
+                        const y = mo(s, h);
+                        y[String(h.key)] = h, I._leaveCb = () => {
                             m(), I._leaveCb = void 0, delete u.delayedLeave
                         }, u.delayedLeave = p
                     })
                 }
                 return o
             }
         }
@@ -1656,15 +1656,15 @@
     const {
         leavingVNodes: n
     } = e;
     let s = n.get(t.type);
     return s || (s = Object.create(null), n.set(t.type, s)), s
 }
 
-function xn(e, t, n, s) {
+function En(e, t, n, s) {
     const {
         appear: r,
         mode: i,
         persisted: o = !1,
         onBeforeEnter: c,
         onEnter: l,
         onAfterEnter: a,
@@ -1673,29 +1673,29 @@
         onLeave: h,
         onAfterLeave: _,
         onLeaveCancelled: b,
         onBeforeAppear: P,
         onAppear: I,
         onAfterAppear: m,
         onAppearCancelled: p
-    } = t, v = String(e.key), x = mo(n, e), k = (R, z) => {
-        R && $e(R, s, 9, z)
+    } = t, y = String(e.key), E = mo(n, e), k = (R, z) => {
+        R && Be(R, s, 9, z)
     }, L = (R, z) => {
         const j = z[1];
         k(R, z), U(R) ? R.every(V => V.length <= 1) && j() : R.length <= 1 && j()
     }, B = {
         mode: i,
         persisted: o,
         beforeEnter(R) {
             let z = c;
             if (!n.isMounted)
                 if (r) z = P || c;
                 else return;
             R._leaveCb && R._leaveCb(!0);
-            const j = x[v];
+            const j = E[y];
             j && Je(e, j) && j.el._leaveCb && j.el._leaveCb(), k(z, [R])
         },
         enter(R) {
             let z = l,
                 j = a,
                 V = u;
             if (!n.isMounted)
@@ -1709,20 +1709,20 @@
         },
         leave(R, z) {
             const j = String(e.key);
             if (R._enterCb && R._enterCb(!0), n.isUnmounting) return z();
             k(d, [R]);
             let V = !1;
             const F = R._leaveCb = X => {
-                V || (V = !0, z(), X ? k(b, [R]) : k(_, [R]), R._leaveCb = void 0, x[j] === e && delete x[j])
+                V || (V = !0, z(), X ? k(b, [R]) : k(_, [R]), R._leaveCb = void 0, E[j] === e && delete E[j])
             };
-            x[j] = e, h ? L(h, [R, F]) : F()
+            E[j] = e, h ? L(h, [R, F]) : F()
         },
         clone(R) {
-            return xn(R, t, n, s)
+            return En(R, t, n, s)
         }
     };
     return B
 }
 
 function Ts(e) {
     if (Sn(e)) return e = rt(e), e.children = null, e
@@ -1738,24 +1738,24 @@
 
 function pr(e, t = !1, n) {
     let s = [],
         r = 0;
     for (let i = 0; i < e.length; i++) {
         let o = e[i];
         const c = n == null ? o.key : String(n) + String(o.key != null ? o.key : i);
-        o.type === ve ? (o.patchFlag & 128 && r++, s = s.concat(pr(o.children, t, c))) : (t || o.type !== Te) && s.push(c != null ? rt(o, {
+        o.type === be ? (o.patchFlag & 128 && r++, s = s.concat(pr(o.children, t, c))) : (t || o.type !== Pe) && s.push(c != null ? rt(o, {
             key: c
         }) : o)
     }
     if (r > 1)
         for (let i = 0; i < s.length; i++) s[i].patchFlag = -2;
     return s
 }
 
-function vs(e) {
+function ys(e) {
     return Q(e) ? {
         setup: e,
         name: e.name
     } : e
 }
 const At = e => !!e.type.__asyncLoader;
 
@@ -1780,15 +1780,15 @@
             return l || (_ = l = t().catch(b => {
                 if (b = b instanceof Error ? b : new Error(String(b)), c) return new Promise((P, I) => {
                     c(b, () => P(d()), () => I(b), u + 1)
                 });
                 throw b
             }).then(b => _ !== l && l ? l : (b && (b.__esModule || b[Symbol.toStringTag] === "Module") && (b = b.default), a = b, b)))
         };
-    return vs({
+    return ys({
         name: "AsyncComponentWrapper",
         __asyncLoader: h,
         get __asyncResolved() {
             return a
         },
         setup() {
             const _ = me;
@@ -1865,87 +1865,87 @@
                         um: u,
                         o: {
                             createElement: d
                         }
                     }
                 } = s,
                 h = d("div");
-            s.activate = (p, v, x, k, L) => {
+            s.activate = (p, y, E, k, L) => {
                 const B = p.component;
-                a(p, v, x, 0, c), l(B.vnode, p, v, x, B, c, k, p.slotScopeIds, L), ye(() => {
+                a(p, y, E, 0, c), l(B.vnode, p, y, E, B, c, k, p.slotScopeIds, L), ye(() => {
                     B.isDeactivated = !1, B.a && Dt(B.a);
                     const R = p.props && p.props.onVnodeMounted;
                     R && Se(R, B.parent, p)
                 }, c)
             }, s.deactivate = p => {
-                const v = p.component;
+                const y = p.component;
                 a(p, h, null, 1, c), ye(() => {
-                    v.da && Dt(v.da);
-                    const x = p.props && p.props.onVnodeUnmounted;
-                    x && Se(x, v.parent, p), v.isDeactivated = !0
+                    y.da && Dt(y.da);
+                    const E = p.props && p.props.onVnodeUnmounted;
+                    E && Se(E, y.parent, p), y.isDeactivated = !0
                 }, c)
             };
 
             function _(p) {
                 As(p), u(p, n, c, !0)
             }
 
             function b(p) {
-                r.forEach((v, x) => {
-                    const k = ns(v.type);
-                    k && (!p || !p(k)) && P(x)
+                r.forEach((y, E) => {
+                    const k = ns(y.type);
+                    k && (!p || !p(k)) && P(E)
                 })
             }
 
             function P(p) {
-                const v = r.get(p);
-                !o || v.type !== o.type ? _(v) : o && As(o), r.delete(p), i.delete(p)
+                const y = r.get(p);
+                !o || y.type !== o.type ? _(y) : o && As(o), r.delete(p), i.delete(p)
             }
-            Vt(() => [e.include, e.exclude], ([p, v]) => {
-                p && b(x => an(p, x)), v && b(x => !an(v, x))
+            Vt(() => [e.include, e.exclude], ([p, y]) => {
+                p && b(E => an(p, E)), y && b(E => !an(y, E))
             }, {
                 flush: "post",
                 deep: !0
             });
             let I = null;
             const m = () => {
                 I != null && r.set(I, Ss(n.subTree))
             };
             return On(m), gr(m), mr(() => {
                 r.forEach(p => {
                     const {
-                        subTree: v,
-                        suspense: x
-                    } = n, k = Ss(v);
+                        subTree: y,
+                        suspense: E
+                    } = n, k = Ss(y);
                     if (p.type === k.type) {
                         As(k);
                         const L = k.component.da;
-                        L && ye(L, x);
+                        L && ye(L, E);
                         return
                     }
                     _(p)
                 })
             }), () => {
                 if (I = null, !t.default) return null;
                 const p = t.default(),
-                    v = p[0];
+                    y = p[0];
                 if (p.length > 1) return o = null, p;
-                if (!Ot(v) || !(v.shapeFlag & 4) && !(v.shapeFlag & 128)) return o = null, v;
-                let x = Ss(v);
-                const k = x.type,
-                    L = ns(At(x) ? x.type.__asyncResolved || {} : k),
+                if (!Ot(y) || !(y.shapeFlag & 4) && !(y.shapeFlag & 128)) return o = null, y;
+                let E = Ss(y);
+                const k = E.type,
+                    L = ns(At(E) ? E.type.__asyncResolved || {} : k),
                     {
                         include: B,
                         exclude: R,
                         max: z
                     } = e;
-                if (B && (!L || !an(B, L)) || R && L && an(R, L)) return o = x, v;
-                const j = x.key == null ? k : x.key,
+                if (B && (!L || !an(B, L)) || R && L && an(R, L)) return o = E, y;
+                const j = E.key == null ? k : E.key,
                     V = r.get(j);
-                return x.el && (x = rt(x), v.shapeFlag & 128 && (v.ssContent = x)), I = j, V ? (x.el = V.el, x.component = V.component, x.transition && Qt(x, x.transition), x.shapeFlag |= 512, i.delete(j), i.add(j)) : (i.add(j), z && i.size > parseInt(z, 10) && P(i.values().next().value)), x.shapeFlag |= 256, o = x, uo(v.type) ? v : x
+                return E.el && (E = rt(E), y.shapeFlag & 128 && (y.ssContent = E)), I = j, V ? (E.el = V.el, E.component = V.component, E.transition && Qt(E, E.transition), E.shapeFlag |= 512, i.delete(j), i.add(j)) : (i.add(j), z && i.size > parseInt(z, 10) && P(i.values().next().value)), E.shapeFlag |= 256, o = E, uo(y.type) ? y : E
             }
         }
     },
     Zf = Mc;
 
 function an(e, t) {
     return U(e) ? e.some(n => an(n, t)) : he(e) ? e.split(",").includes(t) : e.test ? e.test(t) : !1
@@ -1991,16 +1991,16 @@
 }
 
 function bs(e, t, n = me, s = !1) {
     if (n) {
         const r = n[e] || (n[e] = []),
             i = t.__weh || (t.__weh = (...o) => {
                 if (n.isUnmounted) return;
-                It(), yt(n);
-                const c = $e(t, n, e, o);
+                It(), vt(n);
+                const c = Be(t, n, e, o);
                 return pt(), Mt(), c
             });
         return s ? r.unshift(i) : r.push(i), i
     }
 }
 const it = e => (t, n = me) => (!Xt || e === "sp") && bs(e, (...s) => t(...s), n),
     $c = it("bm"),
@@ -2016,15 +2016,15 @@
 function Uc(e, t = me) {
     bs("ec", e, t)
 }
 
 function Gf(e, t) {
     const n = Ce;
     if (n === null) return e;
-    const s = xs(n) || n.proxy,
+    const s = Es(n) || n.proxy,
         r = e.dirs || (e.dirs = []);
     for (let i = 0; i < t.length; i++) {
         let [o, c, l, a = re] = t[i];
         Q(o) && (o = {
             mounted: o,
             updated: o
         }), o.deep && Tt(c), r.push({
@@ -2042,48 +2042,48 @@
 function Ye(e, t, n, s) {
     const r = e.dirs,
         i = t && t.dirs;
     for (let o = 0; o < r.length; o++) {
         const c = r[o];
         i && (c.oldValue = i[o].value);
         let l = c.dir[s];
-        l && (It(), $e(l, n, 8, [e.el, c, e, t]), Mt())
+        l && (It(), Be(l, n, 8, [e.el, c, e, t]), Mt())
     }
 }
 const _r = "components",
     zc = "directives";
 
 function ed(e, t) {
-    return yr(_r, e, !0, t) || e
+    return vr(_r, e, !0, t) || e
 }
-const yo = Symbol();
+const vo = Symbol();
 
 function Kc(e) {
-    return he(e) ? yr(_r, e, !1) || e : e || yo
+    return he(e) ? vr(_r, e, !1) || e : e || vo
 }
 
 function td(e) {
-    return yr(zc, e)
+    return vr(zc, e)
 }
 
-function yr(e, t, n = !0, s = !1) {
+function vr(e, t, n = !0, s = !1) {
     const r = Ce || me;
     if (r) {
         const i = r.type;
         if (e === _r) {
             const c = ns(i, !1);
-            if (c && (c === t || c === Be(t) || c === as(Be(t)))) return i
+            if (c && (c === t || c === He(t) || c === as(He(t)))) return i
         }
         const o = zr(r[e] || i[e], t) || zr(r.appContext[e], t);
         return !o && s ? i : o
     }
 }
 
 function zr(e, t) {
-    return e && (e[t] || e[Be(t)] || e[as(Be(t))])
+    return e && (e[t] || e[He(t)] || e[as(He(t))])
 }
 
 function nd(e, t, n, s) {
     let r;
     const i = n && n[s];
     if (U(e) || he(e)) {
         r = new Array(e.length);
@@ -2120,43 +2120,43 @@
 
 function rd(e, t, n = {}, s, r) {
     if (Ce.isCE || Ce.parent && At(Ce.parent) && Ce.parent.isCE) return ce("slot", t === "default" ? null : {
         name: t
     }, s && s());
     let i = e[t];
     i && i._c && (i._d = !1), Jt();
-    const o = i && vo(i(n)),
-        c = es(ve, {
+    const o = i && yo(i(n)),
+        c = es(be, {
             key: n.key || o && o.key || `_${t}`
         }, o || (s ? s() : []), o && e._ === 1 ? 64 : -2);
     return !r && c.scopeId && (c.slotScopeIds = [c.scopeId + "-s"]), i && i._c && (i._d = !0), c
 }
 
-function vo(e) {
-    return e.some(t => Ot(t) ? !(t.type === Te || t.type === ve && !vo(t.children)) : !0) ? e : null
+function yo(e) {
+    return e.some(t => Ot(t) ? !(t.type === Pe || t.type === be && !yo(t.children)) : !0) ? e : null
 }
 
 function id(e, t) {
     const n = {};
     for (const s in e) n[t && /[A-Z]/.test(s) ? `on:${s}` : zn(s)] = e[s];
     return n
 }
-const Ds = e => e ? No(e) ? xs(e) || e.proxy : Ds(e.parent) : null,
+const Ds = e => e ? No(e) ? Es(e) || e.proxy : Ds(e.parent) : null,
     Xn = pe(Object.create(null), {
         $: e => e,
         $el: e => e.vnode.el,
         $data: e => e.data,
         $props: e => e.props,
         $attrs: e => e.attrs,
         $slots: e => e.slots,
         $refs: e => e.refs,
         $parent: e => Ds(e.parent),
         $root: e => Ds(e.root),
         $emit: e => e.emit,
-        $options: e => vr(e),
+        $options: e => yr(e),
         $forceUpdate: e => e.f || (e.f = () => ms(e.update)),
         $nextTick: e => e.n || (e.n = ur.bind(e.proxy)),
         $watch: e => kc.bind(e)
     }),
     Us = {
         get({
             _: e
@@ -2231,15 +2231,15 @@
         has(e, t) {
             return t[0] !== "_" && !gl(t)
         }
     });
 let zs = !0;
 
 function Wc(e) {
-    const t = vr(e),
+    const t = yr(e),
         n = e.proxy,
         s = e.ctx;
     zs = !1, t.beforeCreate && Kr(t.beforeCreate, e, "bc");
     const {
         data: r,
         computed: i,
         methods: o,
@@ -2251,16 +2251,16 @@
         mounted: h,
         beforeUpdate: _,
         updated: b,
         activated: P,
         deactivated: I,
         beforeDestroy: m,
         beforeUnmount: p,
-        destroyed: v,
-        unmounted: x,
+        destroyed: y,
+        unmounted: E,
         render: k,
         renderTracked: L,
         renderTriggered: B,
         errorCaptured: R,
         serverPrefetch: z,
         expose: j,
         inheritAttrs: V,
@@ -2271,15 +2271,15 @@
     if (a && qc(a, s, null, e.appContext.config.unwrapInjectedRef), o)
         for (const ue in o) {
             const oe = o[ue];
             Q(oe) && (s[ue] = oe.bind(n))
         }
     if (r) {
         const ue = r.call(n, n);
-        ae(ue) && (e.data = be(ue))
+        ae(ue) && (e.data = ve(ue))
     }
     if (zs = !0, i)
         for (const ue in i) {
             const oe = i[ue],
                 je = Q(oe) ? oe.bind(n, n) : Q(oe.get) ? oe.get.bind(n, n) : Ke,
                 bt = !Q(oe) && Q(oe.set) ? oe.set.bind(n) : Ke,
                 De = Y({
@@ -2302,15 +2302,15 @@
         })
     }
     u && Kr(u, e, "c");
 
     function ne(ue, oe) {
         U(oe) ? oe.forEach(je => ue(je.bind(n))) : oe && ue(oe.bind(n))
     }
-    if (ne($c, d), ne(On, h), ne(Bc, _), ne(gr, b), ne(Nc, P), ne(Lc, I), ne(Uc, R), ne(Dc, L), ne(jc, B), ne(mr, p), ne(ws, x), ne(Hc, z), U(j))
+    if (ne($c, d), ne(On, h), ne(Bc, _), ne(gr, b), ne(Nc, P), ne(Lc, I), ne(Uc, R), ne(Dc, L), ne(jc, B), ne(mr, p), ne(ws, E), ne(Hc, z), U(j))
         if (j.length) {
             const ue = e.exposed || (e.exposed = {});
             j.forEach(oe => {
                 Object.defineProperty(ue, oe, {
                     get: () => n[oe],
                     set: je => n[oe] = je
                 })
@@ -2330,15 +2330,15 @@
             get: () => o.value,
             set: c => o.value = c
         }) : t[r] = o
     }
 }
 
 function Kr(e, t, n) {
-    $e(U(e) ? e.map(s => s.bind(t.proxy)) : e.bind(t.proxy), t, n)
+    Be(U(e) ? e.map(s => s.bind(t.proxy)) : e.bind(t.proxy), t, n)
 }
 
 function bo(e, t, n, s) {
     const r = s.includes(".") ? ho(n, s) : () => n[s];
     if (he(e)) {
         const i = t[e];
         Q(i) && Vt(r, i)
@@ -2347,15 +2347,15 @@
         if (U(e)) e.forEach(i => bo(i, t, n, s));
         else {
             const i = Q(e.handler) ? e.handler.bind(n) : t[e.handler];
             Q(i) && Vt(r, i, e)
         }
 }
 
-function vr(e) {
+function yr(e) {
     const t = e.type,
         {
             mixins: n,
             extends: s
         } = t,
         {
             mixins: r,
@@ -2379,78 +2379,78 @@
         if (!(s && o === "expose")) {
             const c = Yc[o] || n && n[o];
             e[o] = c ? c(e[o], t[o]) : t[o]
         } return e
 }
 const Yc = {
     data: Vr,
-    props: xt,
-    emits: xt,
-    methods: xt,
-    computed: xt,
-    beforeCreate: Re,
-    created: Re,
-    beforeMount: Re,
-    mounted: Re,
-    beforeUpdate: Re,
-    updated: Re,
-    beforeDestroy: Re,
-    beforeUnmount: Re,
-    destroyed: Re,
-    unmounted: Re,
-    activated: Re,
-    deactivated: Re,
-    errorCaptured: Re,
-    serverPrefetch: Re,
-    components: xt,
-    directives: xt,
+    props: Et,
+    emits: Et,
+    methods: Et,
+    computed: Et,
+    beforeCreate: Te,
+    created: Te,
+    beforeMount: Te,
+    mounted: Te,
+    beforeUpdate: Te,
+    updated: Te,
+    beforeDestroy: Te,
+    beforeUnmount: Te,
+    destroyed: Te,
+    unmounted: Te,
+    activated: Te,
+    deactivated: Te,
+    errorCaptured: Te,
+    serverPrefetch: Te,
+    components: Et,
+    directives: Et,
     watch: Jc,
     provide: Vr,
     inject: Qc
 };
 
 function Vr(e, t) {
     return t ? e ? function() {
         return pe(Q(e) ? e.call(this, this) : e, Q(t) ? t.call(this, this) : t)
     } : t : e
 }
 
 function Qc(e, t) {
-    return xt(Ks(e), Ks(t))
+    return Et(Ks(e), Ks(t))
 }
 
 function Ks(e) {
     if (U(e)) {
         const t = {};
         for (let n = 0; n < e.length; n++) t[e[n]] = e[n];
         return t
     }
     return e
 }
 
-function Re(e, t) {
+function Te(e, t) {
     return e ? [...new Set([].concat(e, t))] : t
 }
 
-function xt(e, t) {
+function Et(e, t) {
     return e ? pe(pe(Object.create(null), e), t) : t
 }
 
 function Jc(e, t) {
     if (!e) return t;
     if (!t) return e;
     const n = pe(Object.create(null), e);
-    for (const s in t) n[s] = Re(e[s], t[s]);
+    for (const s in t) n[s] = Te(e[s], t[s]);
     return n
 }
 
 function Xc(e, t, n, s = !1) {
     const r = {},
         i = {};
-    Yn(i, Es, 1), e.propsDefaults = Object.create(null), wo(e, t, r, i);
+    Yn(i, xs, 1), e.propsDefaults = Object.create(null), wo(e, t, r, i);
     for (const o in e.propsOptions[0]) o in r || (r[o] = void 0);
     n ? e.props = s ? r : nc(r) : e.type.props ? e.props = r : e.props = i, e.attrs = i
 }
 
 function Zc(e, t, n, s) {
     const {
         props: r,
@@ -2466,15 +2466,15 @@
             for (let d = 0; d < u.length; d++) {
                 let h = u[d];
                 if (_s(e.emitsOptions, h)) continue;
                 const _ = t[h];
                 if (l)
                     if (ee(i, h)) _ !== i[h] && (i[h] = _, a = !0);
                     else {
-                        const b = Be(h);
+                        const b = He(h);
                         r[b] = Vs(l, c, b, _, e, !1)
                     }
                 else _ !== i[h] && (i[h] = _, a = !0)
             }
         }
     } else {
         wo(e, t, r, i) && (a = !0);
@@ -2491,15 +2491,15 @@
     let o = !1,
         c;
     if (t)
         for (let l in t) {
             if (un(l)) continue;
             const a = t[l];
             let u;
-            r && ee(r, u = Be(l)) ? !i || !i.includes(u) ? n[u] = a : (c || (c = {}))[u] = a : _s(e.emitsOptions, l) || (!(l in s) || a !== s[l]) && (s[l] = a, o = !0)
+            r && ee(r, u = He(l)) ? !i || !i.includes(u) ? n[u] = a : (c || (c = {}))[u] = a : _s(e.emitsOptions, l) || (!(l in s) || a !== s[l]) && (s[l] = a, o = !0)
         }
     if (i) {
         const l = te(n),
             a = c || re;
         for (let u = 0; u < i.length; u++) {
             const d = i[u];
             n[d] = Vs(r, l, d, a[d], e, !ee(a, d))
@@ -2514,46 +2514,46 @@
         const c = ee(o, "default");
         if (c && s === void 0) {
             const l = o.default;
             if (o.type !== Function && Q(l)) {
                 const {
                     propsDefaults: a
                 } = r;
-                n in a ? s = a[n] : (yt(r), s = a[n] = l.call(null, t), pt())
+                n in a ? s = a[n] : (vt(r), s = a[n] = l.call(null, t), pt())
             } else s = l
         }
         o[0] && (i && !c ? s = !1 : o[1] && (s === "" || s === Xe(n)) && (s = !0))
     }
     return s
 }
 
-function Eo(e, t, n = !1) {
+function xo(e, t, n = !1) {
     const s = t.propsCache,
         r = s.get(e);
     if (r) return r;
     const i = e.props,
         o = {},
         c = [];
     let l = !1;
     if (!Q(e)) {
         const u = d => {
             l = !0;
-            const [h, _] = Eo(d, t, !0);
+            const [h, _] = xo(d, t, !0);
             pe(o, h), _ && c.push(..._)
         };
         !n && t.mixins.length && t.mixins.forEach(u), e.extends && u(e.extends), e.mixins && e.mixins.forEach(u)
     }
     if (!i && !l) return ae(e) && s.set(e, Ht), Ht;
     if (U(i))
         for (let u = 0; u < i.length; u++) {
-            const d = Be(i[u]);
+            const d = He(i[u]);
             Wr(d) && (o[d] = re)
         } else if (i)
             for (const u in i) {
-                const d = Be(u);
+                const d = He(u);
                 if (Wr(d)) {
                     const h = i[u],
                         _ = o[d] = U(h) || Q(h) ? {
                             type: h
                         } : h;
                     if (_) {
                         const b = Qr(Boolean, _.type),
@@ -2578,25 +2578,25 @@
 function Yr(e, t) {
     return qr(e) === qr(t)
 }
 
 function Qr(e, t) {
     return U(t) ? t.findIndex(n => Yr(n, e)) : Q(t) && Yr(t, e) ? 0 : -1
 }
-const xo = e => e[0] === "_" || e === "$stable",
+const Eo = e => e[0] === "_" || e === "$stable",
     br = e => U(e) ? e.map(Me) : [Me(e)],
     Gc = (e, t, n) => {
         if (t._n) return t;
         const s = fr((...r) => br(t(...r)), n);
         return s._c = !1, s
     },
     Co = (e, t, n) => {
         const s = e._ctx;
         for (const r in e) {
-            if (xo(r)) continue;
+            if (Eo(r)) continue;
             const i = e[r];
             if (Q(i)) t[r] = Gc(r, i, s);
             else if (i != null) {
                 const o = br(i);
                 t[r] = () => o
             }
         }
@@ -2606,15 +2606,15 @@
         e.slots.default = () => n
     },
     ea = (e, t) => {
         if (e.vnode.shapeFlag & 32) {
             const n = t._;
             n ? (e.slots = te(t), Yn(t, "_", n)) : Co(t, e.slots = {})
         } else e.slots = {}, t && Ro(e, t);
-        Yn(e.slots, Es, 1)
+        Yn(e.slots, xs, 1)
     },
     ta = (e, t, n) => {
         const {
             vnode: s,
             slots: r
         } = e;
         let i = !0,
@@ -2622,22 +2622,22 @@
         if (s.shapeFlag & 32) {
             const c = t._;
             c ? n && c === 1 ? i = !1 : (pe(r, t), !n && c === 1 && delete r._) : (i = !t.$stable, Co(t, r)), o = t
         } else t && (Ro(e, t), o = {
             default: 1
         });
         if (i)
-            for (const c in r) !xo(c) && !(c in o) && delete r[c]
+            for (const c in r) !Eo(c) && !(c in o) && delete r[c]
     };
 
 function To() {
     return {
         app: null,
         config: {
-            isNativeTag: xl,
+            isNativeTag: El,
             performance: !1,
             globalProperties: {},
             optionMergeStrategies: {},
             errorHandler: void 0,
             warnHandler: void 0,
             compilerOptions: {}
         },
@@ -2681,15 +2681,15 @@
             },
             directive(a, u) {
                 return u ? (i.directives[a] = u, l) : i.directives[a]
             },
             mount(a, u, d) {
                 if (!c) {
                     const h = ce(s, r);
-                    return h.appContext = i, u && t ? t(h, a) : e(h, a, d), c = !0, l._container = a, a.__vue_app__ = l, xs(h.component) || h.component.proxy
+                    return h.appContext = i, u && t ? t(h, a) : e(h, a, d), c = !0, l._container = a, a.__vue_app__ = l, Es(h.component) || h.component.proxy
                 }
             },
             unmount() {
                 c && (e(null, l._container), delete l._container.__vue_app__)
             },
             provide(a, u) {
                 return i.provides[a] = u, l
@@ -2701,15 +2701,15 @@
 
 function Gn(e, t, n, s, r = !1) {
     if (U(e)) {
         e.forEach((h, _) => Gn(h, t && (U(t) ? t[_] : t), n, s, r));
         return
     }
     if (At(s) && !r) return;
-    const i = s.shapeFlag & 4 ? xs(s.component) || s.component.proxy : s.el,
+    const i = s.shapeFlag & 4 ? Es(s.component) || s.component.proxy : s.el,
         o = r ? null : i,
         {
             i: c,
             r: l
         } = e,
         a = t && t.r,
         u = c.refs === re ? c.refs = {} : c.refs,
@@ -2748,116 +2748,116 @@
         }
     } = e, u = (m, p) => {
         if (!p.hasChildNodes()) {
             n(null, m, p), Jn(), p._vnode = m;
             return
         }
         lt = !1, d(p.firstChild, m, null, null, null), Jn(), p._vnode = m, lt && console.error("Hydration completed but contains mismatches.")
-    }, d = (m, p, v, x, k, L = !1) => {
+    }, d = (m, p, y, E, k, L = !1) => {
         const B = Hn(m) && m.data === "[",
-            R = () => P(m, p, v, x, k, B),
+            R = () => P(m, p, y, E, k, B),
             {
                 type: z,
                 ref: j,
                 shapeFlag: V,
                 patchFlag: F
             } = p;
         let X = m.nodeType;
         p.el = m, F === -2 && (L = !1, p.dynamicChildren = null);
         let H = null;
         switch (z) {
             case Cn:
                 X !== 3 ? p.children === "" ? (l(p.el = r(""), o(m), m), H = m) : H = R() : (m.data !== p.children && (lt = !0, m.data = p.children), H = i(m));
                 break;
-            case Te:
+            case Pe:
                 X !== 8 || B ? H = R() : H = i(m);
                 break;
             case Wt:
                 if (B && (m = i(m), X = m.nodeType), X === 1 || X === 3) {
                     H = m;
                     const we = !p.children.length;
                     for (let ne = 0; ne < p.staticCount; ne++) we && (p.children += H.nodeType === 1 ? H.outerHTML : H.data), ne === p.staticCount - 1 && (p.anchor = H), H = i(H);
                     return B ? i(H) : H
                 } else R();
                 break;
-            case ve:
-                B ? H = b(m, p, v, x, k, L) : H = R();
+            case be:
+                B ? H = b(m, p, y, E, k, L) : H = R();
                 break;
             default:
-                if (V & 1) X !== 1 || p.type.toLowerCase() !== m.tagName.toLowerCase() ? H = R() : H = h(m, p, v, x, k, L);
+                if (V & 1) X !== 1 || p.type.toLowerCase() !== m.tagName.toLowerCase() ? H = R() : H = h(m, p, y, E, k, L);
                 else if (V & 6) {
                     p.slotScopeIds = k;
                     const we = o(m);
-                    if (t(p, we, null, v, x, Bn(we), L), H = B ? I(m) : i(m), H && Hn(H) && H.data === "teleport end" && (H = i(H)), At(p)) {
+                    if (t(p, we, null, y, E, Bn(we), L), H = B ? I(m) : i(m), H && Hn(H) && H.data === "teleport end" && (H = i(H)), At(p)) {
                         let ne;
-                        B ? (ne = ce(ve), ne.anchor = H ? H.previousSibling : we.lastChild) : ne = m.nodeType === 3 ? Io("") : ce("div"), ne.el = m, p.component.subTree = ne
+                        B ? (ne = ce(be), ne.anchor = H ? H.previousSibling : we.lastChild) : ne = m.nodeType === 3 ? Io("") : ce("div"), ne.el = m, p.component.subTree = ne
                     }
-                } else V & 64 ? X !== 8 ? H = R() : H = p.type.hydrate(m, p, v, x, k, L, e, _) : V & 128 && (H = p.type.hydrate(m, p, v, x, Bn(o(m)), k, L, e, d))
+                } else V & 64 ? X !== 8 ? H = R() : H = p.type.hydrate(m, p, y, E, k, L, e, _) : V & 128 && (H = p.type.hydrate(m, p, y, E, Bn(o(m)), k, L, e, d))
         }
-        return j != null && Gn(j, null, x, p), H
-    }, h = (m, p, v, x, k, L) => {
+        return j != null && Gn(j, null, E, p), H
+    }, h = (m, p, y, E, k, L) => {
         L = L || !!p.dynamicChildren;
         const {
             type: B,
             props: R,
             patchFlag: z,
             shapeFlag: j,
             dirs: V
         } = p, F = B === "input" && V || B === "option";
         if (F || z !== -1) {
-            if (V && Ye(p, null, v, "created"), R)
+            if (V && Ye(p, null, y, "created"), R)
                 if (F || !L || z & 48)
-                    for (const H in R)(F && H.endsWith("value") || Tn(H) && !un(H)) && s(m, H, null, R[H], !1, void 0, v);
-                else R.onClick && s(m, "onClick", null, R.onClick, !1, void 0, v);
+                    for (const H in R)(F && H.endsWith("value") || Tn(H) && !un(H)) && s(m, H, null, R[H], !1, void 0, y);
+                else R.onClick && s(m, "onClick", null, R.onClick, !1, void 0, y);
             let X;
-            if ((X = R && R.onVnodeBeforeMount) && Se(X, v, p), V && Ye(p, null, v, "beforeMount"), ((X = R && R.onVnodeMounted) || V) && fo(() => {
-                    X && Se(X, v, p), V && Ye(p, null, v, "mounted")
-                }, x), j & 16 && !(R && (R.innerHTML || R.textContent))) {
-                let H = _(m.firstChild, p, m, v, x, k, L);
+            if ((X = R && R.onVnodeBeforeMount) && Se(X, y, p), V && Ye(p, null, y, "beforeMount"), ((X = R && R.onVnodeMounted) || V) && fo(() => {
+                    X && Se(X, y, p), V && Ye(p, null, y, "mounted")
+                }, E), j & 16 && !(R && (R.innerHTML || R.textContent))) {
+                let H = _(m.firstChild, p, m, y, E, k, L);
                 for (; H;) {
                     lt = !0;
                     const we = H;
                     H = H.nextSibling, c(we)
                 }
             } else j & 8 && m.textContent !== p.children && (lt = !0, m.textContent = p.children)
         }
         return m.nextSibling
-    }, _ = (m, p, v, x, k, L, B) => {
+    }, _ = (m, p, y, E, k, L, B) => {
         B = B || !!p.dynamicChildren;
         const R = p.children,
             z = R.length;
         for (let j = 0; j < z; j++) {
             const V = B ? R[j] : R[j] = Me(R[j]);
-            if (m) m = d(m, V, x, k, L, B);
+            if (m) m = d(m, V, E, k, L, B);
             else {
                 if (V.type === Cn && !V.children) continue;
-                lt = !0, n(null, V, v, null, x, k, Bn(v), L)
+                lt = !0, n(null, V, y, null, E, k, Bn(y), L)
             }
         }
         return m
-    }, b = (m, p, v, x, k, L) => {
+    }, b = (m, p, y, E, k, L) => {
         const {
             slotScopeIds: B
         } = p;
         B && (k = k ? k.concat(B) : B);
         const R = o(m),
-            z = _(i(m), p, R, v, x, k, L);
+            z = _(i(m), p, R, y, E, k, L);
         return z && Hn(z) && z.data === "]" ? i(p.anchor = z) : (lt = !0, l(p.anchor = a("]"), R, z), z)
-    }, P = (m, p, v, x, k, L) => {
+    }, P = (m, p, y, E, k, L) => {
         if (lt = !0, p.el = null, L) {
             const z = I(m);
             for (;;) {
                 const j = i(m);
                 if (j && j !== z) c(j);
                 else break
             }
         }
         const B = i(m),
             R = o(m);
-        return c(m), n(null, p, R, B, v, x, Bn(R), k), B
+        return c(m), n(null, p, R, B, y, E, Bn(R), k), B
     }, I = m => {
         let p = 0;
         for (; m;)
             if (m = i(m), m && Hn(m) && (m.data === "[" && p++, m.data === "]")) {
                 if (p === 0) return i(m);
                 p--
             } return m
@@ -2886,176 +2886,176 @@
         createComment: l,
         setText: a,
         setElementText: u,
         parentNode: d,
         nextSibling: h,
         setScopeId: _ = Ke,
         insertStaticContent: b
-    } = e, P = (f, g, y, w = null, C = null, S = null, N = !1, A = null, O = !!g.dynamicChildren) => {
+    } = e, P = (f, g, v, w = null, C = null, S = null, N = !1, A = null, O = !!g.dynamicChildren) => {
         if (f === g) return;
         f && !Je(f, g) && (w = M(f), Ae(f, C, S, !0), f = null), g.patchFlag === -2 && (O = !1, g.dynamicChildren = null);
         const {
             type: T,
             ref: W,
             shapeFlag: D
         } = g;
         switch (T) {
             case Cn:
-                I(f, g, y, w);
+                I(f, g, v, w);
                 break;
-            case Te:
-                m(f, g, y, w);
+            case Pe:
+                m(f, g, v, w);
                 break;
             case Wt:
-                f == null && p(g, y, w, N);
+                f == null && p(g, v, w, N);
                 break;
-            case ve:
-                F(f, g, y, w, C, S, N, A, O);
+            case be:
+                F(f, g, v, w, C, S, N, A, O);
                 break;
             default:
-                D & 1 ? k(f, g, y, w, C, S, N, A, O) : D & 6 ? X(f, g, y, w, C, S, N, A, O) : (D & 64 || D & 128) && T.process(f, g, y, w, C, S, N, A, O, se)
+                D & 1 ? k(f, g, v, w, C, S, N, A, O) : D & 6 ? X(f, g, v, w, C, S, N, A, O) : (D & 64 || D & 128) && T.process(f, g, v, w, C, S, N, A, O, se)
         }
         W != null && C && Gn(W, f && f.ref, S, g || f, !g)
-    }, I = (f, g, y, w) => {
-        if (f == null) s(g.el = c(g.children), y, w);
+    }, I = (f, g, v, w) => {
+        if (f == null) s(g.el = c(g.children), v, w);
         else {
             const C = g.el = f.el;
             g.children !== f.children && a(C, g.children)
         }
-    }, m = (f, g, y, w) => {
-        f == null ? s(g.el = l(g.children || ""), y, w) : g.el = f.el
-    }, p = (f, g, y, w) => {
-        [f.el, f.anchor] = b(f.children, g, y, w, f.el, f.anchor)
-    }, v = ({
+    }, m = (f, g, v, w) => {
+        f == null ? s(g.el = l(g.children || ""), v, w) : g.el = f.el
+    }, p = (f, g, v, w) => {
+        [f.el, f.anchor] = b(f.children, g, v, w, f.el, f.anchor)
+    }, y = ({
         el: f,
         anchor: g
-    }, y, w) => {
+    }, v, w) => {
         let C;
-        for (; f && f !== g;) C = h(f), s(f, y, w), f = C;
-        s(g, y, w)
-    }, x = ({
+        for (; f && f !== g;) C = h(f), s(f, v, w), f = C;
+        s(g, v, w)
+    }, E = ({
         el: f,
         anchor: g
     }) => {
-        let y;
-        for (; f && f !== g;) y = h(f), r(f), f = y;
+        let v;
+        for (; f && f !== g;) v = h(f), r(f), f = v;
         r(g)
-    }, k = (f, g, y, w, C, S, N, A, O) => {
-        N = N || g.type === "svg", f == null ? L(g, y, w, C, S, N, A, O) : z(f, g, C, S, N, A, O)
-    }, L = (f, g, y, w, C, S, N, A) => {
+    }, k = (f, g, v, w, C, S, N, A, O) => {
+        N = N || g.type === "svg", f == null ? L(g, v, w, C, S, N, A, O) : z(f, g, C, S, N, A, O)
+    }, L = (f, g, v, w, C, S, N, A) => {
         let O, T;
         const {
             type: W,
             props: D,
             shapeFlag: q,
             transition: J,
             dirs: G
         } = f;
         if (O = f.el = o(f.type, S, D && D.is, D), q & 8 ? u(O, f.children) : q & 16 && R(f.children, O, null, w, C, S && W !== "foreignObject", N, A), G && Ye(f, null, w, "created"), D) {
             for (const le in D) le !== "value" && !un(le) && i(O, le, null, D[le], S, f.children, w, C, $);
             "value" in D && i(O, "value", null, D.value), (T = D.onVnodeBeforeMount) && Se(T, w, f)
         }
         B(O, f, f.scopeId, N, w), G && Ye(f, null, w, "beforeMount");
         const fe = (!C || C && !C.pendingBranch) && J && !J.persisted;
-        fe && J.beforeEnter(O), s(O, g, y), ((T = D && D.onVnodeMounted) || fe || G) && ye(() => {
+        fe && J.beforeEnter(O), s(O, g, v), ((T = D && D.onVnodeMounted) || fe || G) && ye(() => {
             T && Se(T, w, f), fe && J.enter(O), G && Ye(f, null, w, "mounted")
         }, C)
-    }, B = (f, g, y, w, C) => {
-        if (y && _(f, y), w)
+    }, B = (f, g, v, w, C) => {
+        if (v && _(f, v), w)
             for (let S = 0; S < w.length; S++) _(f, w[S]);
         if (C) {
             let S = C.subTree;
             if (g === S) {
                 const N = C.vnode;
                 B(f, N, N.scopeId, N.slotScopeIds, C.parent)
             }
         }
-    }, R = (f, g, y, w, C, S, N, A, O = 0) => {
+    }, R = (f, g, v, w, C, S, N, A, O = 0) => {
         for (let T = O; T < f.length; T++) {
             const W = f[T] = A ? ft(f[T]) : Me(f[T]);
-            P(null, W, g, y, w, C, S, N, A)
+            P(null, W, g, v, w, C, S, N, A)
         }
-    }, z = (f, g, y, w, C, S, N) => {
+    }, z = (f, g, v, w, C, S, N) => {
         const A = g.el = f.el;
         let {
             patchFlag: O,
             dynamicChildren: T,
             dirs: W
         } = g;
         O |= f.patchFlag & 16;
         const D = f.props || re,
             q = g.props || re;
         let J;
-        y && wt(y, !1), (J = q.onVnodeBeforeUpdate) && Se(J, y, g, f), W && Ye(g, f, y, "beforeUpdate"), y && wt(y, !0);
+        v && wt(v, !1), (J = q.onVnodeBeforeUpdate) && Se(J, v, g, f), W && Ye(g, f, v, "beforeUpdate"), v && wt(v, !0);
         const G = C && g.type !== "foreignObject";
-        if (T ? j(f.dynamicChildren, T, A, y, w, G, S) : N || oe(f, g, A, null, y, w, G, S, !1), O > 0) {
-            if (O & 16) V(A, g, D, q, y, w, C);
+        if (T ? j(f.dynamicChildren, T, A, v, w, G, S) : N || oe(f, g, A, null, v, w, G, S, !1), O > 0) {
+            if (O & 16) V(A, g, D, q, v, w, C);
             else if (O & 2 && D.class !== q.class && i(A, "class", null, q.class, C), O & 4 && i(A, "style", D.style, q.style, C), O & 8) {
                 const fe = g.dynamicProps;
                 for (let le = 0; le < fe.length; le++) {
                     const ge = fe[le],
                         Ue = D[ge],
                         Ft = q[ge];
-                    (Ft !== Ue || ge === "value") && i(A, ge, Ue, Ft, C, f.children, y, w, $)
+                    (Ft !== Ue || ge === "value") && i(A, ge, Ue, Ft, C, f.children, v, w, $)
                 }
             }
             O & 1 && f.children !== g.children && u(A, g.children)
-        } else !N && T == null && V(A, g, D, q, y, w, C);
+        } else !N && T == null && V(A, g, D, q, v, w, C);
         ((J = q.onVnodeUpdated) || W) && ye(() => {
-            J && Se(J, y, g, f), W && Ye(g, f, y, "updated")
+            J && Se(J, v, g, f), W && Ye(g, f, v, "updated")
         }, w)
-    }, j = (f, g, y, w, C, S, N) => {
+    }, j = (f, g, v, w, C, S, N) => {
         for (let A = 0; A < g.length; A++) {
             const O = f[A],
                 T = g[A],
-                W = O.el && (O.type === ve || !Je(O, T) || O.shapeFlag & 70) ? d(O.el) : y;
+                W = O.el && (O.type === be || !Je(O, T) || O.shapeFlag & 70) ? d(O.el) : v;
             P(O, T, W, null, w, C, S, N, !0)
         }
-    }, V = (f, g, y, w, C, S, N) => {
-        if (y !== w) {
-            if (y !== re)
-                for (const A in y) !un(A) && !(A in w) && i(f, A, y[A], null, N, g.children, C, S, $);
+    }, V = (f, g, v, w, C, S, N) => {
+        if (v !== w) {
+            if (v !== re)
+                for (const A in v) !un(A) && !(A in w) && i(f, A, v[A], null, N, g.children, C, S, $);
             for (const A in w) {
                 if (un(A)) continue;
                 const O = w[A],
-                    T = y[A];
+                    T = v[A];
                 O !== T && A !== "value" && i(f, A, T, O, N, g.children, C, S, $)
             }
-            "value" in w && i(f, "value", y.value, w.value)
+            "value" in w && i(f, "value", v.value, w.value)
         }
-    }, F = (f, g, y, w, C, S, N, A, O) => {
+    }, F = (f, g, v, w, C, S, N, A, O) => {
         const T = g.el = f ? f.el : c(""),
             W = g.anchor = f ? f.anchor : c("");
         let {
             patchFlag: D,
             dynamicChildren: q,
             slotScopeIds: J
         } = g;
-        J && (A = A ? A.concat(J) : J), f == null ? (s(T, y, w), s(W, y, w), R(g.children, y, W, C, S, N, A, O)) : D > 0 && D & 64 && q && f.dynamicChildren ? (j(f.dynamicChildren, q, y, C, S, N, A), (g.key != null || C && g === C.subTree) && wr(f, g, !0)) : oe(f, g, y, W, C, S, N, A, O)
-    }, X = (f, g, y, w, C, S, N, A, O) => {
-        g.slotScopeIds = A, f == null ? g.shapeFlag & 512 ? C.ctx.activate(g, y, w, N, O) : H(g, y, w, C, S, N, O) : we(f, g, O)
-    }, H = (f, g, y, w, C, S, N) => {
+        J && (A = A ? A.concat(J) : J), f == null ? (s(T, v, w), s(W, v, w), R(g.children, v, W, C, S, N, A, O)) : D > 0 && D & 64 && q && f.dynamicChildren ? (j(f.dynamicChildren, q, v, C, S, N, A), (g.key != null || C && g === C.subTree) && wr(f, g, !0)) : oe(f, g, v, W, C, S, N, A, O)
+    }, X = (f, g, v, w, C, S, N, A, O) => {
+        g.slotScopeIds = A, f == null ? g.shapeFlag & 512 ? C.ctx.activate(g, v, w, N, O) : H(g, v, w, C, S, N, O) : we(f, g, O)
+    }, H = (f, g, v, w, C, S, N) => {
         const A = f.component = Mo(f, w, C);
         if (Sn(f) && (A.ctx.renderer = se), Lo(A), A.asyncDep) {
             if (C && C.registerDep(A, ne), !f.el) {
-                const O = A.subTree = ce(Te);
-                m(null, O, g, y)
+                const O = A.subTree = ce(Pe);
+                m(null, O, g, v)
             }
             return
         }
-        ne(A, f, g, y, C, S, N)
-    }, we = (f, g, y) => {
+        ne(A, f, g, v, C, S, N)
+    }, we = (f, g, v) => {
         const w = g.component = f.component;
-        if (Cc(f, g, y))
+        if (Cc(f, g, v))
             if (w.asyncDep && !w.asyncResolved) {
-                ue(w, g, y);
+                ue(w, g, v);
                 return
             } else w.next = g, _c(w.update), w.update();
         else g.el = f.el, w.vnode = g
-    }, ne = (f, g, y, w, C, S, N) => {
+    }, ne = (f, g, v, w, C, S, N) => {
         const A = () => {
                 if (f.isMounted) {
                     let {
                         next: W,
                         bu: D,
                         u: q,
                         parent: J,
@@ -3078,82 +3078,82 @@
                     if (wt(f, !1), J && Dt(J), !le && (W = q && q.onVnodeBeforeMount) && Se(W, fe, g), wt(f, !0), D && Z) {
                         const ge = () => {
                             f.subTree = Vn(f), Z(D, f.subTree, f, C, null)
                         };
                         le ? g.type.__asyncLoader().then(() => !f.isUnmounted && ge()) : ge()
                     } else {
                         const ge = f.subTree = Vn(f);
-                        P(null, ge, y, w, f, C, S), g.el = ge.el
+                        P(null, ge, v, w, f, C, S), g.el = ge.el
                     }
                     if (G && ye(G, C), !le && (W = q && q.onVnodeMounted)) {
                         const ge = g;
                         ye(() => Se(W, fe, ge), C)
-                    }(g.shapeFlag & 256 || fe && At(fe.vnode) && fe.vnode.shapeFlag & 256) && f.a && ye(f.a, C), f.isMounted = !0, g = y = w = null
+                    }(g.shapeFlag & 256 || fe && At(fe.vnode) && fe.vnode.shapeFlag & 256) && f.a && ye(f.a, C), f.isMounted = !0, g = v = w = null
                 }
             },
             O = f.effect = new us(A, () => ms(T), f.scope),
             T = f.update = () => O.run();
         T.id = f.uid, wt(f, !0), T()
-    }, ue = (f, g, y) => {
+    }, ue = (f, g, v) => {
         g.component = f;
         const w = f.vnode.props;
-        f.vnode = g, f.next = null, Zc(f, g.props, w, y), ta(f, g.children, y), It(), Br(), Mt()
-    }, oe = (f, g, y, w, C, S, N, A, O = !1) => {
+        f.vnode = g, f.next = null, Zc(f, g.props, w, v), ta(f, g.children, v), It(), Br(), Mt()
+    }, oe = (f, g, v, w, C, S, N, A, O = !1) => {
         const T = f && f.children,
             W = f ? f.shapeFlag : 0,
             D = g.children,
             {
                 patchFlag: q,
                 shapeFlag: J
             } = g;
         if (q > 0) {
             if (q & 128) {
-                bt(T, D, y, w, C, S, N, A, O);
+                bt(T, D, v, w, C, S, N, A, O);
                 return
             } else if (q & 256) {
-                je(T, D, y, w, C, S, N, A, O);
+                je(T, D, v, w, C, S, N, A, O);
                 return
             }
         }
-        J & 8 ? (W & 16 && $(T, C, S), D !== T && u(y, D)) : W & 16 ? J & 16 ? bt(T, D, y, w, C, S, N, A, O) : $(T, C, S, !0) : (W & 8 && u(y, ""), J & 16 && R(D, y, w, C, S, N, A, O))
-    }, je = (f, g, y, w, C, S, N, A, O) => {
+        J & 8 ? (W & 16 && $(T, C, S), D !== T && u(v, D)) : W & 16 ? J & 16 ? bt(T, D, v, w, C, S, N, A, O) : $(T, C, S, !0) : (W & 8 && u(v, ""), J & 16 && R(D, v, w, C, S, N, A, O))
+    }, je = (f, g, v, w, C, S, N, A, O) => {
         f = f || Ht, g = g || Ht;
         const T = f.length,
             W = g.length,
             D = Math.min(T, W);
         let q;
         for (q = 0; q < D; q++) {
             const J = g[q] = O ? ft(g[q]) : Me(g[q]);
-            P(f[q], J, y, null, C, S, N, A, O)
+            P(f[q], J, v, null, C, S, N, A, O)
         }
-        T > W ? $(f, C, S, !0, !1, D) : R(g, y, w, C, S, N, A, O, D)
-    }, bt = (f, g, y, w, C, S, N, A, O) => {
+        T > W ? $(f, C, S, !0, !1, D) : R(g, v, w, C, S, N, A, O, D)
+    }, bt = (f, g, v, w, C, S, N, A, O) => {
         let T = 0;
         const W = g.length;
         let D = f.length - 1,
             q = W - 1;
         for (; T <= D && T <= q;) {
             const J = f[T],
                 G = g[T] = O ? ft(g[T]) : Me(g[T]);
-            if (Je(J, G)) P(J, G, y, null, C, S, N, A, O);
+            if (Je(J, G)) P(J, G, v, null, C, S, N, A, O);
             else break;
             T++
         }
         for (; T <= D && T <= q;) {
             const J = f[D],
                 G = g[q] = O ? ft(g[q]) : Me(g[q]);
-            if (Je(J, G)) P(J, G, y, null, C, S, N, A, O);
+            if (Je(J, G)) P(J, G, v, null, C, S, N, A, O);
             else break;
             D--, q--
         }
         if (T > D) {
             if (T <= q) {
                 const J = q + 1,
                     G = J < W ? g[J].el : w;
-                for (; T <= q;) P(null, g[T] = O ? ft(g[T]) : Me(g[T]), y, G, C, S, N, A, O), T++
+                for (; T <= q;) P(null, g[T] = O ? ft(g[T]) : Me(g[T]), v, G, C, S, N, A, O), T++
             }
         } else if (T > q)
             for (; T <= D;) Ae(f[T], C, S, !0), T++;
         else {
             const J = T,
                 G = T,
                 fe = new Map;
@@ -3176,141 +3176,141 @@
                 let qe;
                 if (ke.key != null) qe = fe.get(ke.key);
                 else
                     for (le = G; le <= q; le++)
                         if (nn[le - G] === 0 && Je(ke, g[le])) {
                             qe = le;
                             break
-                        } qe === void 0 ? Ae(ke, C, S, !0) : (nn[qe - G] = T + 1, qe >= Tr ? Tr = qe : Ft = !0, P(ke, g[qe], y, null, C, S, N, A, O), ge++)
+                        } qe === void 0 ? Ae(ke, C, S, !0) : (nn[qe - G] = T + 1, qe >= Tr ? Tr = qe : Ft = !0, P(ke, g[qe], v, null, C, S, N, A, O), ge++)
             }
             const Pr = Ft ? la(nn) : Ht;
             for (le = Pr.length - 1, T = Ue - 1; T >= 0; T--) {
                 const ke = G + T,
                     qe = g[ke],
                     Ar = ke + 1 < W ? g[ke + 1].el : w;
-                nn[T] === 0 ? P(null, qe, y, Ar, C, S, N, A, O) : Ft && (le < 0 || T !== Pr[le] ? De(qe, y, Ar, 2) : le--)
+                nn[T] === 0 ? P(null, qe, v, Ar, C, S, N, A, O) : Ft && (le < 0 || T !== Pr[le] ? De(qe, v, Ar, 2) : le--)
             }
         }
-    }, De = (f, g, y, w, C = null) => {
+    }, De = (f, g, v, w, C = null) => {
         const {
             el: S,
             type: N,
             transition: A,
             children: O,
             shapeFlag: T
         } = f;
         if (T & 6) {
-            De(f.component.subTree, g, y, w);
+            De(f.component.subTree, g, v, w);
             return
         }
         if (T & 128) {
-            f.suspense.move(g, y, w);
+            f.suspense.move(g, v, w);
             return
         }
         if (T & 64) {
-            N.move(f, g, y, se);
+            N.move(f, g, v, se);
             return
         }
-        if (N === ve) {
-            s(S, g, y);
-            for (let D = 0; D < O.length; D++) De(O[D], g, y, w);
-            s(f.anchor, g, y);
+        if (N === be) {
+            s(S, g, v);
+            for (let D = 0; D < O.length; D++) De(O[D], g, v, w);
+            s(f.anchor, g, v);
             return
         }
         if (N === Wt) {
-            v(f, g, y);
+            y(f, g, v);
             return
         }
         if (w !== 2 && T & 1 && A)
-            if (w === 0) A.beforeEnter(S), s(S, g, y), ye(() => A.enter(S), C);
+            if (w === 0) A.beforeEnter(S), s(S, g, v), ye(() => A.enter(S), C);
             else {
                 const {
                     leave: D,
                     delayLeave: q,
                     afterLeave: J
-                } = A, G = () => s(S, g, y), fe = () => {
+                } = A, G = () => s(S, g, v), fe = () => {
                     D(S, () => {
                         G(), J && J()
                     })
                 };
                 q ? q(S, G, fe) : fe()
             }
-        else s(S, g, y)
-    }, Ae = (f, g, y, w = !1, C = !1) => {
+        else s(S, g, v)
+    }, Ae = (f, g, v, w = !1, C = !1) => {
         const {
             type: S,
             props: N,
             ref: A,
             children: O,
             dynamicChildren: T,
             shapeFlag: W,
             patchFlag: D,
             dirs: q
         } = f;
-        if (A != null && Gn(A, null, y, f, !0), W & 256) {
+        if (A != null && Gn(A, null, v, f, !0), W & 256) {
             g.ctx.deactivate(f);
             return
         }
         const J = W & 1 && q,
             G = !At(f);
         let fe;
-        if (G && (fe = N && N.onVnodeBeforeUnmount) && Se(fe, g, f), W & 6) E(f.component, y, w);
+        if (G && (fe = N && N.onVnodeBeforeUnmount) && Se(fe, g, f), W & 6) x(f.component, v, w);
         else {
             if (W & 128) {
-                f.suspense.unmount(y, w);
+                f.suspense.unmount(v, w);
                 return
             }
-            J && Ye(f, null, g, "beforeUnmount"), W & 64 ? f.type.remove(f, g, y, C, se, w) : T && (S !== ve || D > 0 && D & 64) ? $(T, g, y, !1, !0) : (S === ve && D & 384 || !C && W & 16) && $(O, g, y), w && Lt(f)
+            J && Ye(f, null, g, "beforeUnmount"), W & 64 ? f.type.remove(f, g, v, C, se, w) : T && (S !== be || D > 0 && D & 64) ? $(T, g, v, !1, !0) : (S === be && D & 384 || !C && W & 16) && $(O, g, v), w && Lt(f)
         }(G && (fe = N && N.onVnodeUnmounted) || J) && ye(() => {
             fe && Se(fe, g, f), J && Ye(f, null, g, "unmounted")
-        }, y)
+        }, v)
     }, Lt = f => {
         const {
             type: g,
-            el: y,
+            el: v,
             anchor: w,
             transition: C
         } = f;
-        if (g === ve) {
-            kn(y, w);
+        if (g === be) {
+            kn(v, w);
             return
         }
         if (g === Wt) {
-            x(f);
+            E(f);
             return
         }
         const S = () => {
-            r(y), C && !C.persisted && C.afterLeave && C.afterLeave()
+            r(v), C && !C.persisted && C.afterLeave && C.afterLeave()
         };
         if (f.shapeFlag & 1 && C && !C.persisted) {
             const {
                 leave: N,
                 delayLeave: A
-            } = C, O = () => N(y, S);
+            } = C, O = () => N(v, S);
             A ? A(f.el, S, O) : O()
         } else S()
     }, kn = (f, g) => {
-        let y;
-        for (; f !== g;) y = h(f), r(f), f = y;
+        let v;
+        for (; f !== g;) v = h(f), r(f), f = v;
         r(g)
-    }, E = (f, g, y) => {
+    }, x = (f, g, v) => {
         const {
             bum: w,
             scope: C,
             update: S,
             subTree: N,
             um: A
         } = f;
-        w && Dt(w), C.stop(), S && (S.active = !1, Ae(N, f, g, y)), A && ye(A, g), ye(() => {
+        w && Dt(w), C.stop(), S && (S.active = !1, Ae(N, f, g, v)), A && ye(A, g), ye(() => {
             f.isUnmounted = !0
         }, g), g && g.pendingBranch && !g.isUnmounted && f.asyncDep && !f.asyncResolved && f.suspenseId === g.pendingId && (g.deps--, g.deps === 0 && g.resolve())
-    }, $ = (f, g, y, w = !1, C = !1, S = 0) => {
-        for (let N = S; N < f.length; N++) Ae(f[N], g, y, w, C)
-    }, M = f => f.shapeFlag & 6 ? M(f.component.subTree) : f.shapeFlag & 128 ? f.suspense.next() : h(f.anchor || f.el), K = (f, g, y) => {
-        f == null ? g._vnode && Ae(g._vnode, null, null, !0) : P(g._vnode || null, f, g, null, null, null, y), Br(), Jn(), g._vnode = f
+    }, $ = (f, g, v, w = !1, C = !1, S = 0) => {
+        for (let N = S; N < f.length; N++) Ae(f[N], g, v, w, C)
+    }, M = f => f.shapeFlag & 6 ? M(f.component.subTree) : f.shapeFlag & 128 ? f.suspense.next() : h(f.anchor || f.el), K = (f, g, v) => {
+        f == null ? g._vnode && Ae(g._vnode, null, null, !0) : P(g._vnode || null, f, g, null, null, null, v), Br(), Jn(), g._vnode = f
     }, se = {
         p: P,
         um: Ae,
         m: De,
         r: Lt,
         mt: H,
         mc: R,
@@ -3383,37 +3383,37 @@
                     querySelector: b,
                     createText: P,
                     createComment: I
                 }
             } = a, m = dn(t.props);
             let {
                 shapeFlag: p,
-                children: v,
-                dynamicChildren: x
+                children: y,
+                dynamicChildren: E
             } = t;
             if (e == null) {
                 const k = t.el = P(""),
                     L = t.anchor = P("");
                 _(k, n, s), _(L, n, s);
                 const B = t.target = Ws(t.props, b),
                     R = t.targetAnchor = P("");
                 B && (_(R, B), o = o || Jr(B));
                 const z = (j, V) => {
-                    p & 16 && u(v, j, V, r, i, o, c, l)
+                    p & 16 && u(y, j, V, r, i, o, c, l)
                 };
                 m ? z(n, L) : B && z(B, R)
             } else {
                 t.el = e.el;
                 const k = t.anchor = e.anchor,
                     L = t.target = e.target,
                     B = t.targetAnchor = e.targetAnchor,
                     R = dn(e.props),
                     z = R ? n : L,
                     j = R ? k : B;
-                if (o = o || Jr(L), x ? (h(e.dynamicChildren, x, z, r, i, o, c), wr(e, t, !0)) : l || d(e, t, z, j, r, i, o, c, !1), m) R || jn(t, n, k, a, 1);
+                if (o = o || Jr(L), E ? (h(e.dynamicChildren, E, z, r, i, o, c), wr(e, t, !0)) : l || d(e, t, z, j, r, i, o, c, !1), m) R || jn(t, n, k, a, 1);
                 else if ((t.props && t.props.to) !== (e.props && e.props.to)) {
                     const V = t.target = Ws(t.props, b);
                     V && jn(t, V, null, a, 0)
                 } else R && jn(t, L, B, a, 1)
             }
         },
         remove(e, t, n, s, {
@@ -3480,17 +3480,17 @@
                         break
                     } a(d, t, u, n, s, r, i)
             }
     }
     return t.anchor && o(t.anchor)
 }
 const fa = aa,
-    ve = Symbol(void 0),
+    be = Symbol(void 0),
     Cn = Symbol(void 0),
-    Te = Symbol(void 0),
+    Pe = Symbol(void 0),
     Wt = Symbol(void 0),
     hn = [];
 let Oe = null;
 
 function Jt(e = !1) {
     hn.push(Oe = e ? null : [])
 }
@@ -3505,15 +3505,15 @@
 }
 
 function So(e) {
     return e.dynamicChildren = St > 0 ? Oe || Ht : null, Ao(), St > 0 && Oe && Oe.push(e), e
 }
 
 function da(e, t, n, s, r, i) {
-    return So(Ee(e, t, n, s, r, i, !0))
+    return So(xe(e, t, n, s, r, i, !0))
 }
 
 function es(e, t, n, s, r) {
     return So(ce(e, t, n, s, r, !0))
 }
 
 function Ot(e) {
@@ -3521,38 +3521,38 @@
 }
 
 function Je(e, t) {
     return e.type === t.type && e.key === t.key
 }
 
 function od(e) {}
-const Es = "__vInternal",
+const xs = "__vInternal",
     Oo = ({
         key: e
     }) => e != null ? e : null,
     qn = ({
         ref: e,
         ref_key: t,
         ref_for: n
     }) => e != null ? he(e) || _e(e) || Q(e) ? {
         i: Ce,
         r: e,
         k: t,
         f: !!n
     } : e : null;
 
-function Ee(e, t = null, n = null, s = 0, r = null, i = e === ve ? 0 : 1, o = !1, c = !1) {
+function xe(e, t = null, n = null, s = 0, r = null, i = e === be ? 0 : 1, o = !1, c = !1) {
     const l = {
         __v_isVNode: !0,
         __v_skip: !0,
         type: e,
         props: t,
         key: t && Oo(t),
         ref: t && qn(t),
-        scopeId: ys,
+        scopeId: vs,
         slotScopeIds: null,
         children: n,
         component: null,
         suspense: null,
         ssContent: null,
         ssFallback: null,
         dirs: null,
@@ -3564,37 +3564,37 @@
         staticCount: 0,
         shapeFlag: i,
         patchFlag: s,
         dynamicProps: r,
         dynamicChildren: null,
         appContext: null
     };
-    return c ? (Er(l, n), i & 128 && e.normalize(l)) : n && (l.shapeFlag |= he(n) ? 8 : 16), St > 0 && !o && Oe && (l.patchFlag > 0 || i & 6) && l.patchFlag !== 32 && Oe.push(l), l
+    return c ? (xr(l, n), i & 128 && e.normalize(l)) : n && (l.shapeFlag |= he(n) ? 8 : 16), St > 0 && !o && Oe && (l.patchFlag > 0 || i & 6) && l.patchFlag !== 32 && Oe.push(l), l
 }
 const ce = ha;
 
 function ha(e, t = null, n = null, s = 0, r = null, i = !1) {
-    if ((!e || e === yo) && (e = Te), Ot(e)) {
+    if ((!e || e === vo) && (e = Pe), Ot(e)) {
         const c = rt(e, t, !0);
-        return n && Er(c, n), St > 0 && !i && Oe && (c.shapeFlag & 6 ? Oe[Oe.indexOf(e)] = c : Oe.push(c)), c.patchFlag |= -2, c
+        return n && xr(c, n), St > 0 && !i && Oe && (c.shapeFlag & 6 ? Oe[Oe.indexOf(e)] = c : Oe.push(c)), c.patchFlag |= -2, c
     }
     if (wa(e) && (e = e.__vccOpts), t) {
         t = ko(t);
         let {
             class: c,
             style: l
         } = t;
         c && !he(c) && (t.class = os(c)), ae(l) && (Zi(l) && !U(l) && (l = pe({}, l)), t.style = is(l))
     }
     const o = he(e) ? 1 : uo(e) ? 128 : ca(e) ? 64 : ae(e) ? 4 : Q(e) ? 2 : 0;
-    return Ee(e, t, n, s, r, o, i, !0)
+    return xe(e, t, n, s, r, o, i, !0)
 }
 
 function ko(e) {
-    return e ? Zi(e) || Es in e ? pe({}, e) : e : null
+    return e ? Zi(e) || xs in e ? pe({}, e) : e : null
 }
 
 function rt(e, t, n = !1) {
     const {
         props: s,
         ref: r,
         patchFlag: i,
@@ -3610,15 +3610,15 @@
         scopeId: e.scopeId,
         slotScopeIds: e.slotScopeIds,
         children: o,
         target: e.target,
         targetAnchor: e.targetAnchor,
         staticCount: e.staticCount,
         shapeFlag: e.shapeFlag,
-        patchFlag: t && e.type !== ve ? i === -1 ? 16 : i | 16 : i,
+        patchFlag: t && e.type !== be ? i === -1 ? 16 : i | 16 : i,
         dynamicProps: e.dynamicProps,
         dynamicChildren: e.dynamicChildren,
         appContext: e.appContext,
         dirs: e.dirs,
         transition: e.transition,
         component: e.component,
         suspense: e.suspense,
@@ -3635,41 +3635,41 @@
 
 function ld(e, t) {
     const n = ce(Wt, null, e);
     return n.staticCount = t, n
 }
 
 function cd(e = "", t = !1) {
-    return t ? (Jt(), es(Te, null, e)) : ce(Te, null, e)
+    return t ? (Jt(), es(Pe, null, e)) : ce(Pe, null, e)
 }
 
 function Me(e) {
-    return e == null || typeof e == "boolean" ? ce(Te) : U(e) ? ce(ve, null, e.slice()) : typeof e == "object" ? ft(e) : ce(Cn, null, String(e))
+    return e == null || typeof e == "boolean" ? ce(Pe) : U(e) ? ce(be, null, e.slice()) : typeof e == "object" ? ft(e) : ce(Cn, null, String(e))
 }
 
 function ft(e) {
     return e.el === null && e.patchFlag !== -1 || e.memo ? e : rt(e)
 }
 
-function Er(e, t) {
+function xr(e, t) {
     let n = 0;
     const {
         shapeFlag: s
     } = e;
     if (t == null) t = null;
     else if (U(t)) n = 16;
     else if (typeof t == "object")
         if (s & 65) {
             const r = t.default;
-            r && (r._c && (r._d = !1), Er(e, r()), r._c && (r._d = !0));
+            r && (r._c && (r._d = !1), xr(e, r()), r._c && (r._d = !0));
             return
         } else {
             n = 32;
             const r = t._;
-            !r && !(Es in t) ? t._ctx = Ce : r === 3 && Ce && (Ce.slots._ === 1 ? t._ = 1 : (t._ = 2, e.patchFlag |= 1024))
+            !r && !(xs in t) ? t._ctx = Ce : r === 3 && Ce && (Ce.slots._ === 1 ? t._ = 1 : (t._ = 2, e.patchFlag |= 1024))
         }
     else Q(t) ? (t = {
         default: t,
         _ctx: Ce
     }, n = 32) : (t = String(t), s & 64 ? (n = 16, t = [Io(t)]) : n = 8);
     e.children = t, e.shapeFlag |= n
 }
@@ -3687,15 +3687,15 @@
             o && i !== o && !(U(i) && i.includes(o)) && (t[r] = i ? [].concat(i, o) : o)
         } else r !== "" && (t[r] = s[r])
     }
     return t
 }
 
 function Se(e, t, n, s = null) {
-    $e(e, t, 7, [n, s])
+    Be(e, t, 7, [n, s])
 }
 const ga = To();
 let ma = 0;
 
 function Mo(e, t, n) {
     const s = e.type,
         r = (t ? t.appContext : e.appContext) || ga,
@@ -3717,15 +3717,15 @@
             exposeProxy: null,
             withProxy: null,
             provides: t ? t.provides : Object.create(r.provides),
             accessCache: null,
             renderCache: [],
             components: null,
             directives: null,
-            propsOptions: Eo(s, r),
+            propsOptions: xo(s, r),
             emitsOptions: ao(s, r),
             emit: null,
             emitted: null,
             propsDefaults: re,
             inheritAttrs: s.inheritAttrs,
             ctx: re,
             data: re,
@@ -3759,15 +3759,15 @@
         };
     return i.ctx = {
         _: i
     }, i.root = t ? t.root : i, i.emit = bc.bind(null, i), e.ce && e.ce(i), i
 }
 let me = null;
 const Nt = () => me || Ce,
-    yt = e => {
+    vt = e => {
         me = e, e.scope.on()
     },
     pt = () => {
         me && me.scope.off(), me = null
     };
 
 function No(e) {
@@ -3790,15 +3790,15 @@
     const n = e.type;
     e.accessCache = Object.create(null), e.proxy = Gi(new Proxy(e.ctx, Us));
     const {
         setup: s
     } = n;
     if (s) {
         const r = e.setupContext = s.length > 1 ? $o(e) : null;
-        yt(e), It();
+        vt(e), It();
         const i = nt(s, e, 0, [e.props, r]);
         if (Mt(), pt(), sr(i)) {
             if (i.then(pt, pt), t) return i.then(o => {
                 qs(e, o, t)
             }).catch(o => {
                 tn(o, e, 0)
             });
@@ -3819,15 +3819,15 @@
 }
 const ud = () => !ts;
 
 function Fo(e, t, n) {
     const s = e.type;
     if (!e.render) {
         if (!t && ts && !s.render) {
-            const r = s.template || vr(e).template;
+            const r = s.template || yr(e).template;
             if (r) {
                 const {
                     isCustomElement: i,
                     compilerOptions: o
                 } = e.appContext.config, {
                     delimiters: c,
                     compilerOptions: l
@@ -3836,50 +3836,50 @@
                     delimiters: c
                 }, o), l);
                 s.render = ts(r, a)
             }
         }
         e.render = s.render || Ke, Ys && Ys(e)
     }
-    yt(e), It(), Wc(e), Mt(), pt()
+    vt(e), It(), Wc(e), Mt(), pt()
 }
 
-function ya(e) {
+function va(e) {
     return new Proxy(e.attrs, {
         get(t, n) {
             return Le(e, "get", "$attrs"), t[n]
         }
     })
 }
 
 function $o(e) {
     const t = s => {
         e.exposed = s || {}
     };
     let n;
     return {
         get attrs() {
-            return n || (n = ya(e))
+            return n || (n = va(e))
         },
         slots: e.slots,
         emit: e.emit,
         expose: t
     }
 }
 
-function xs(e) {
+function Es(e) {
     if (e.exposed) return e.exposeProxy || (e.exposeProxy = new Proxy(no(Gi(e.exposed)), {
         get(t, n) {
             if (n in t) return t[n];
             if (n in Xn) return Xn[n](e)
         }
     }))
 }
-const va = /(?:^|[-_])(\w)/g,
-    ba = e => e.replace(va, t => t.toUpperCase()).replace(/[-_]/g, "");
+const ya = /(?:^|[-_])(\w)/g,
+    ba = e => e.replace(ya, t => t.toUpperCase()).replace(/[-_]/g, "");
 
 function ns(e, t = !0) {
     return Q(e) ? e.displayName || e.name : e.name || t && e.__name
 }
 
 function Bo(e, t, n = !1) {
     let s = ns(t);
@@ -3939,53 +3939,53 @@
         } : r.default = t[s] : r === null && (n[s] = {
             default: t[s]
         })
     }
     return n
 }
 
-function yd(e, t) {
+function vd(e, t) {
     const n = {};
     for (const s in e) t.includes(s) || Object.defineProperty(n, s, {
         enumerable: !0,
         get: () => e[s]
     });
     return n
 }
 
-function vd(e) {
+function yd(e) {
     const t = Nt();
     let n = e();
     return pt(), sr(n) && (n = n.catch(s => {
-        throw yt(t), s
-    })), [n, () => yt(t)]
+        throw vt(t), s
+    })), [n, () => vt(t)]
 }
 
-function Pe(e, t, n) {
+function Re(e, t, n) {
     const s = arguments.length;
     return s === 2 ? ae(t) && !U(t) ? Ot(t) ? ce(e, null, [t]) : ce(e, t) : ce(e, null, t) : (s > 3 ? n = Array.prototype.slice.call(arguments, 2) : s === 3 && Ot(n) && (n = [n]), ce(e, t, n))
 }
-const Ea = Symbol(""),
+const xa = Symbol(""),
     bd = () => {
         {
-            const e = Ve(Ea);
+            const e = Ve(xa);
             return e || uc("Server rendering context not provided. Make sure to only call useSSRContext() conditionally in the server build."), e
         }
     };
 
 function wd() {}
 
-function Ed(e, t, n, s) {
+function xd(e, t, n, s) {
     const r = n[s];
-    if (r && xa(r, e)) return r;
+    if (r && Ea(r, e)) return r;
     const i = t();
     return i.memo = e.slice(), n[s] = i
 }
 
-function xa(e, t) {
+function Ea(e, t) {
     const n = e.memo;
     if (n.length != t.length) return !1;
     for (let s = 0; s < n.length; s++)
         if (qt(n[s], t[s])) return !1;
     return St > 0 && Oe && Oe.push(e), !0
 }
 const Ca = "3.2.41",
@@ -3993,15 +3993,15 @@
         createComponentInstance: Mo,
         setupComponent: Lo,
         renderComponentRoot: Vn,
         setCurrentRenderingInstance: wn,
         isVNode: Ot,
         normalizeVNode: Me
     },
-    xd = Ra,
+    Ed = Ra,
     Cd = null,
     Rd = null,
     Ta = "http://www.w3.org/2000/svg",
     Rt = typeof document < "u" ? document : null,
     Zr = Rt && Rt.createElement("template"),
     Pa = {
         insert: (e, t, n) => {
@@ -4078,15 +4078,15 @@
 }
 const ei = ["Webkit", "Moz", "ms"],
     Os = {};
 
 function Oa(e, t) {
     const n = Os[t];
     if (n) return n;
-    let s = Be(t);
+    let s = He(t);
     if (s !== "filter" && s in e) return Os[t] = s;
     s = as(s);
     for (let r = 0; r < ei.length; r++) {
         const i = ei[r] + s;
         if (i in e) return Os[t] = i
     }
     return t
@@ -4158,15 +4158,15 @@
 const Fa = Promise.resolve(),
     $a = () => ks || (Fa.then(() => ks = 0), ks = Date.now());
 
 function Ba(e, t) {
     const n = s => {
         if (!s._vts) s._vts = Date.now();
         else if (s._vts <= n.attached) return;
-        $e(Ha(s, n.value), t, 5, [s])
+        Be(Ha(s, n.value), t, 5, [s])
     };
     return n.value = e, n.attached = $a(), n
 }
 
 function Ha(e, t) {
     if (U(t)) {
         const n = e.stopImmediatePropagation;
@@ -4181,25 +4181,25 @@
     };
 
 function Da(e, t, n, s) {
     return s ? !!(t === "innerHTML" || t === "textContent" || t in e && si.test(t) && Q(n)) : t === "spellcheck" || t === "draggable" || t === "translate" || t === "form" || t === "list" && e.tagName === "INPUT" || t === "type" && e.tagName === "TEXTAREA" || si.test(t) && he(n) ? !1 : t in e
 }
 
 function Ua(e, t) {
-    const n = vs(e);
-    class s extends xr {
+    const n = ys(e);
+    class s extends Er {
         constructor(i) {
             super(n, i, t)
         }
     }
     return s.def = n, s
 }
 const Td = e => Ua(e, lu),
     za = typeof HTMLElement < "u" ? HTMLElement : class {};
-class xr extends za {
+class Er extends za {
     constructor(t, n = {}, s) {
         super(), this._def = t, this._props = n, this._instance = null, this._connected = !1, this._resolved = !1, this._numberProps = null, this.shadowRoot && s ? s(this._createVNode(), this.shadowRoot) : this.attachShadow({
             mode: "open"
         })
     }
     connectedCallback() {
         this._connected = !0, this._instance || this._resolveDef()
@@ -4227,30 +4227,30 @@
                 if (o)
                     for (const a in this._props) {
                         const u = r[a];
                         (u === Number || u && u.type === Number) && (this._props[a] = mt(this._props[a]), (l || (l = Object.create(null)))[a] = !0)
                     }
                 this._numberProps = l;
                 for (const a of Object.keys(this)) a[0] !== "_" && this._setProp(a, this[a], !0, !1);
-                for (const a of c.map(Be)) Object.defineProperty(this, a, {
+                for (const a of c.map(He)) Object.defineProperty(this, a, {
                     get() {
                         return this._getProp(a)
                     },
                     set(u) {
                         this._setProp(a, u)
                     }
                 });
                 this._applyStyles(i), this._update()
             },
             n = this._def.__asyncLoader;
         n ? n().then(t) : t(this._def)
     }
     _setAttr(t) {
         let n = this.getAttribute(t);
-        this._numberProps && this._numberProps[t] && (n = mt(n)), this._setProp(Be(t), n, !1)
+        this._numberProps && this._numberProps[t] && (n = mt(n)), this._setProp(He(t), n, !1)
     }
     _getProp(t) {
         return this._props[t]
     }
     _setProp(t, n, s = !0, r = !0) {
         n !== this._props[t] && (this._props[t] = n, r && this._instance && this._update(), s && (n === !0 ? this.setAttribute(Xe(t), "") : typeof n == "string" || typeof n == "number" ? this.setAttribute(Xe(t), n + "") : n || this.removeAttribute(Xe(t))))
     }
@@ -4263,15 +4263,15 @@
             this._instance = n, n.isCE = !0, n.emit = (r, ...i) => {
                 this.dispatchEvent(new CustomEvent(r, {
                     detail: i
                 }))
             };
             let s = this;
             for (; s = s && (s.parentNode || s.host);)
-                if (s instanceof xr) {
+                if (s instanceof Er) {
                     n.parent = s._instance;
                     break
                 }
         }), t
     }
     _applyStyles(t) {
         t && t.forEach(n => {
@@ -4309,15 +4309,15 @@
         const n = e.suspense;
         e = n.activeBranch, n.pendingBranch && !n.isHydrating && n.effects.push(() => {
             Js(n.activeBranch, t)
         })
     }
     for (; e.component;) e = e.component.subTree;
     if (e.shapeFlag & 1 && e.el) ri(e.el, t);
-    else if (e.type === ve) e.children.forEach(n => Js(n, t));
+    else if (e.type === be) e.children.forEach(n => Js(n, t));
     else if (e.type === Wt) {
         let {
             el: n,
             anchor: s
         } = e;
         for (; n && (ri(n, t), n !== s);) n = n.nextSibling
     }
@@ -4329,15 +4329,15 @@
         for (const s in t) n.setProperty(`--${s}`, t[s])
     }
 }
 const ct = "transition",
     rn = "animation",
     jo = (e, {
         slots: t
-    }) => Pe(go, Uo(e), t);
+    }) => Re(go, Uo(e), t);
 jo.displayName = "Transition";
 const Do = {
         name: String,
         type: String,
         css: {
             type: Boolean,
             default: !0
@@ -4350,15 +4350,15 @@
         appearActiveClass: String,
         appearToClass: String,
         leaveFromClass: String,
         leaveActiveClass: String,
         leaveToClass: String
     },
     Ka = jo.props = pe({}, go.props, Do),
-    Et = (e, t = []) => {
+    xt = (e, t = []) => {
         U(e) ? e.forEach(n => n(...t)) : e && e(...t)
     },
     ii = e => e ? U(e) ? e.some(t => t.length > 1) : e.length > 1 : !1;
 
 function Uo(e) {
     const t = {};
     for (const F in e) F in Do || (t[F] = e[F]);
@@ -4375,55 +4375,55 @@
         appearToClass: u = c,
         leaveFromClass: d = `${n}-leave-from`,
         leaveActiveClass: h = `${n}-leave-active`,
         leaveToClass: _ = `${n}-leave-to`
     } = e, b = Va(r), P = b && b[0], I = b && b[1], {
         onBeforeEnter: m,
         onEnter: p,
-        onEnterCancelled: v,
-        onLeave: x,
+        onEnterCancelled: y,
+        onLeave: E,
         onLeaveCancelled: k,
         onBeforeAppear: L = m,
         onAppear: B = p,
-        onAppearCancelled: R = v
+        onAppearCancelled: R = y
     } = t, z = (F, X, H) => {
         ut(F, X ? u : c), ut(F, X ? a : o), H && H()
     }, j = (F, X) => {
         F._isLeaving = !1, ut(F, d), ut(F, _), ut(F, h), X && X()
     }, V = F => (X, H) => {
         const we = F ? B : p,
             ne = () => z(X, F, H);
-        Et(we, [X, ne]), oi(() => {
+        xt(we, [X, ne]), oi(() => {
             ut(X, F ? l : i), Ge(X, F ? u : c), ii(we) || li(X, s, P, ne)
         })
     };
     return pe(t, {
         onBeforeEnter(F) {
-            Et(m, [F]), Ge(F, i), Ge(F, o)
+            xt(m, [F]), Ge(F, i), Ge(F, o)
         },
         onBeforeAppear(F) {
-            Et(L, [F]), Ge(F, l), Ge(F, a)
+            xt(L, [F]), Ge(F, l), Ge(F, a)
         },
         onEnter: V(!1),
         onAppear: V(!0),
         onLeave(F, X) {
             F._isLeaving = !0;
             const H = () => j(F, X);
             Ge(F, d), Ko(), Ge(F, h), oi(() => {
-                !F._isLeaving || (ut(F, d), Ge(F, _), ii(x) || li(F, s, I, H))
-            }), Et(x, [F, H])
+                !F._isLeaving || (ut(F, d), Ge(F, _), ii(E) || li(F, s, I, H))
+            }), xt(E, [F, H])
         },
         onEnterCancelled(F) {
-            z(F, !1), Et(v, [F])
+            z(F, !1), xt(y, [F])
         },
         onAppearCancelled(F) {
-            z(F, !0), Et(R, [F])
+            z(F, !0), xt(R, [F])
         },
         onLeaveCancelled(F) {
-            j(F), Et(k, [F])
+            j(F), xt(k, [F])
         }
     })
 }
 
 function Va(e) {
     if (e == null) return null;
     if (ae(e)) return [Is(e.enter), Is(e.leave)]; {
@@ -4542,24 +4542,24 @@
                         h && h.target !== a || (!h || /transform$/.test(h.propertyName)) && (a.removeEventListener("transitionend", d), a._moveCb = null, ut(a, o))
                     };
                     a.addEventListener("transitionend", d)
                 })
             }), () => {
                 const o = te(e),
                     c = Uo(o);
-                let l = o.tag || ve;
+                let l = o.tag || be;
                 r = i, i = t.default ? pr(t.default()) : [];
                 for (let a = 0; a < i.length; a++) {
                     const u = i[a];
-                    u.key != null && Qt(u, xn(u, c, s, n))
+                    u.key != null && Qt(u, En(u, c, s, n))
                 }
                 if (r)
                     for (let a = 0; a < r.length; a++) {
                         const u = r[a];
-                        Qt(u, xn(u, c, s, n)), Vo.set(u, u.el.getBoundingClientRect())
+                        Qt(u, En(u, c, s, n)), Vo.set(u, u.el.getBoundingClientRect())
                     }
                 return ce(l, null, i)
             }
         }
     },
     Sd = qa;
 
@@ -4591,15 +4591,15 @@
     const r = t.nodeType === 1 ? t : t.parentNode;
     r.appendChild(s);
     const {
         hasTransform: i
     } = zo(s);
     return r.removeChild(s), i
 }
-const vt = e => {
+const yt = e => {
     const t = e.props["onUpdate:modelValue"] || !1;
     return U(t) ? n => Dt(t, n) : t
 };
 
 function Za(e) {
     e.target.composing = !0
 }
@@ -4612,15 +4612,15 @@
         created(e, {
             modifiers: {
                 lazy: t,
                 trim: n,
                 number: s
             }
         }, r) {
-            e._assign = vt(r);
+            e._assign = yt(r);
             const i = s || r.props && r.props.type === "number";
             tt(e, t ? "change" : "input", o => {
                 if (o.target.composing) return;
                 let c = e.value;
                 n && (c = c.trim()), i && (c = mt(c)), e._assign(c)
             }), n && tt(e, "change", () => {
                 e.value = e.value.trim()
@@ -4635,23 +4635,23 @@
             value: t,
             modifiers: {
                 lazy: n,
                 trim: s,
                 number: r
             }
         }, i) {
-            if (e._assign = vt(i), e.composing || document.activeElement === e && e.type !== "range" && (n || s && e.value.trim() === t || (r || e.type === "number") && mt(e.value) === t)) return;
+            if (e._assign = yt(i), e.composing || document.activeElement === e && e.type !== "range" && (n || s && e.value.trim() === t || (r || e.type === "number") && mt(e.value) === t)) return;
             const o = t == null ? "" : t;
             e.value !== o && (e.value = o)
         }
     },
     qo = {
         deep: !0,
         created(e, t, n) {
-            e._assign = vt(n), tt(e, "change", () => {
+            e._assign = yt(n), tt(e, "change", () => {
                 const s = e._modelValue,
                     r = Zt(e),
                     i = e.checked,
                     o = e._assign;
                 if (U(s)) {
                     const c = ls(s, r),
                         l = c !== -1;
@@ -4664,60 +4664,60 @@
                     const c = new Set(s);
                     i ? c.add(r) : c.delete(r), o(c)
                 } else o(Qo(e, i))
             })
         },
         mounted: fi,
         beforeUpdate(e, t, n) {
-            e._assign = vt(n), fi(e, t, n)
+            e._assign = yt(n), fi(e, t, n)
         }
     };
 
 function fi(e, {
     value: t,
     oldValue: n
 }, s) {
     e._modelValue = t, U(t) ? e.checked = ls(t, s.props.value) > -1 : kt(t) ? e.checked = t.has(s.props.value) : t !== n && (e.checked = gt(t, Qo(e, !0)))
 }
 const Yo = {
         created(e, {
             value: t
         }, n) {
-            e.checked = gt(t, n.props.value), e._assign = vt(n), tt(e, "change", () => {
+            e.checked = gt(t, n.props.value), e._assign = yt(n), tt(e, "change", () => {
                 e._assign(Zt(e))
             })
         },
         beforeUpdate(e, {
             value: t,
             oldValue: n
         }, s) {
-            e._assign = vt(s), t !== n && (e.checked = gt(t, s.props.value))
+            e._assign = yt(s), t !== n && (e.checked = gt(t, s.props.value))
         }
     },
     Ga = {
         deep: !0,
         created(e, {
             value: t,
             modifiers: {
                 number: n
             }
         }, s) {
             const r = kt(t);
             tt(e, "change", () => {
                 const i = Array.prototype.filter.call(e.options, o => o.selected).map(o => n ? mt(Zt(o)) : Zt(o));
                 e._assign(e.multiple ? r ? new Set(i) : i : i[0])
-            }), e._assign = vt(s)
+            }), e._assign = yt(s)
         },
         mounted(e, {
             value: t
         }) {
             di(e, t)
         },
         beforeUpdate(e, t, n) {
-            e._assign = vt(n)
+            e._assign = yt(n)
         },
         updated(e, {
             value: t
         }) {
             di(e, t)
         }
     };
@@ -5047,19 +5047,19 @@
             const t = document.querySelector("base");
             e = t && t.getAttribute("href") || "/", e = e.replace(/^\w+:\/\/[^\/]+/, "")
         } else e = "/";
     return e[0] !== "/" && e[0] !== "#" && (e = "/" + e), fu(e)
 }
 const _u = /^[^#]+#/;
 
-function yu(e, t) {
+function vu(e, t) {
     return e.replace(_u, "#") + t
 }
 
-function vu(e, t) {
+function yu(e, t) {
     const n = document.documentElement.getBoundingClientRect(),
         s = e.getBoundingClientRect();
     return {
         behavior: t.behavior,
         left: s.left - n.left - (t.left || 0),
         top: s.top - n.top - (t.top || 0)
     }
@@ -5072,33 +5072,33 @@
 function bu(e) {
     let t;
     if ("el" in e) {
         const n = e.el,
             s = typeof n == "string" && n.startsWith("#"),
             r = typeof n == "string" ? s ? document.getElementById(n.slice(1)) : document.querySelector(n) : n;
         if (!r) return;
-        t = vu(r, e)
+        t = yu(r, e)
     } else t = e;
     "scrollBehavior" in document.documentElement.style ? window.scrollTo(t) : window.scrollTo(t.left != null ? t.left : window.pageXOffset, t.top != null ? t.top : window.pageYOffset)
 }
 
-function yi(e, t) {
+function vi(e, t) {
     return (history.state ? history.state.position - t : -1) + e
 }
 const Zs = new Map;
 
 function wu(e, t) {
     Zs.set(e, t)
 }
 
-function Eu(e) {
+function xu(e) {
     const t = Zs.get(e);
     return Zs.delete(e), t
 }
-let xu = () => location.protocol + "//" + location.host;
+let Eu = () => location.protocol + "//" + location.host;
 
 function nl(e, t) {
     const {
         pathname: n,
         search: s,
         hash: r
     } = t, i = e.indexOf("#");
@@ -5166,15 +5166,15 @@
     return window.addEventListener("popstate", c), window.addEventListener("beforeunload", u), {
         pauseListeners: l,
         listen: a,
         destroy: d
     }
 }
 
-function vi(e, t, n, s = !1, r = !1) {
+function yi(e, t, n, s = !1, r = !1) {
     return {
         back: e,
         current: t,
         forward: n,
         replaced: s,
         position: window.history.length,
         scroll: r ? Cs() : null
@@ -5197,36 +5197,36 @@
         position: t.length - 1,
         replaced: !0,
         scroll: null
     }, !0);
 
     function i(l, a, u) {
         const d = e.indexOf("#"),
-            h = d > -1 ? (n.host && document.querySelector("base") ? e : e.slice(d)) + l : xu() + e + l;
+            h = d > -1 ? (n.host && document.querySelector("base") ? e : e.slice(d)) + l : Eu() + e + l;
         try {
             t[u ? "replaceState" : "pushState"](a, "", h), r.value = a
         } catch (_) {
             console.error(_), n[u ? "replace" : "assign"](h)
         }
     }
 
     function o(l, a) {
-        const u = ie({}, t.state, vi(r.value.back, l, r.value.forward, !0), a, {
+        const u = ie({}, t.state, yi(r.value.back, l, r.value.forward, !0), a, {
             position: r.value.position
         });
         i(l, u, !0), s.value = l
     }
 
     function c(l, a) {
         const u = ie({}, r.value, t.state, {
             forward: l,
             scroll: Cs()
         });
         i(u.current, u, !0);
-        const d = ie({}, vi(s.value, l, null), {
+        const d = ie({}, yi(s.value, l, null), {
             position: u.position + 1
         }, a);
         i(l, d, !1), s.value = l
     }
     return {
         location: s,
         state: r,
@@ -5243,15 +5243,15 @@
     function s(i, o = !0) {
         o || n.pauseListeners(), history.go(i)
     }
     const r = ie({
         location: "",
         base: e,
         go: s,
-        createHref: yu.bind(null, e)
+        createHref: vu.bind(null, e)
     }, t, n);
     return Object.defineProperty(r, "location", {
         enumerable: !0,
         get: () => t.location.value
     }), Object.defineProperty(r, "state", {
         enumerable: !0,
         get: () => t.state.value
@@ -5330,20 +5330,20 @@
                     optional: I
                 });
                 const p = m || wi;
                 if (p !== wi) {
                     _ += 10;
                     try {
                         new RegExp(`(${p})`)
-                    } catch (x) {
-                        throw new Error(`Invalid custom RegExp for param "${b}" (${p}): ` + x.message)
+                    } catch (E) {
+                        throw new Error(`Invalid custom RegExp for param "${b}" (${p}): ` + E.message)
                     }
                 }
-                let v = P ? `((?:${p})(?:/(?:${p}))*)` : `(${p})`;
-                d || (v = I && a.length < 2 ? `(?:/${v})` : "/" + v), I && (v += "?"), r += v, _ += 20, I && (_ += -8), P && (_ += -20), p === ".*" && (_ += -50)
+                let y = P ? `((?:${p})(?:/(?:${p}))*)` : `(${p})`;
+                d || (y = I && a.length < 2 ? `(?:/${y})` : "/" + y), I && (y += "?"), r += y, _ += 20, I && (_ += -8), P && (_ += -20), p === ".*" && (_ += -50)
             }
             u.push(_)
         }
         s.push(u)
     }
     if (n.strict && n.end) {
         const a = s.length - 1;
@@ -5412,21 +5412,21 @@
         r = t.score;
     for (; n < s.length && n < r.length;) {
         const i = Iu(s[n], r[n]);
         if (i) return i;
         n++
     }
     if (Math.abs(r.length - s.length) === 1) {
-        if (Ei(s)) return 1;
-        if (Ei(r)) return -1
+        if (xi(s)) return 1;
+        if (xi(r)) return -1
     }
     return r.length - s.length
 }
 
-function Ei(e) {
+function xi(e) {
     const t = e[e.length - 1];
     return e.length > 0 && t[t.length - 1] < 0
 }
 const Nu = {
         type: 0,
         value: ""
     },
@@ -5528,32 +5528,32 @@
     function i(u, d, h) {
         const _ = !h,
             b = Hu(u);
         b.aliasOf = h && h.record;
         const P = Ri(t, u),
             I = [b];
         if ("alias" in u) {
-            const v = typeof u.alias == "string" ? [u.alias] : u.alias;
-            for (const x of v) I.push(ie({}, b, {
+            const y = typeof u.alias == "string" ? [u.alias] : u.alias;
+            for (const E of y) I.push(ie({}, b, {
                 components: h ? h.record.components : b.components,
-                path: x,
+                path: E,
                 aliasOf: h ? h.record : b
             }))
         }
         let m, p;
-        for (const v of I) {
+        for (const y of I) {
             const {
-                path: x
-            } = v;
-            if (d && x[0] !== "/") {
+                path: E
+            } = y;
+            if (d && E[0] !== "/") {
                 const k = d.record.path,
                     L = k[k.length - 1] === "/" ? "" : "/";
-                v.path = d.record.path + (x && L + x)
+                y.path = d.record.path + (E && L + E)
             }
-            if (m = $u(v, d, P), h ? h.alias.push(m) : (p = p || m, p !== m && p.alias.push(m), _ && u.name && !Ci(m) && o(u.name)), b.children) {
+            if (m = $u(y, d, P), h ? h.alias.push(m) : (p = p || m, p !== m && p.alias.push(m), _ && u.name && !Ci(m) && o(u.name)), b.children) {
                 const k = b.children;
                 for (let L = 0; L < k.length; L++) i(k[L], m, h && h.children[L])
             }
             h = h || m, l(m)
         }
         return p ? () => {
             o(p)
@@ -5583,15 +5583,15 @@
     function a(u, d) {
         let h, _ = {},
             b, P;
         if ("name" in u && u.name) {
             if (h = s.get(u.name), !h) throw en(1, {
                 location: u
             });
-            P = h.record.name, _ = ie(xi(d.params, h.keys.filter(p => !p.optional).map(p => p.name)), u.params && xi(u.params, h.keys.map(p => p.name))), b = h.stringify(_)
+            P = h.record.name, _ = ie(Ei(d.params, h.keys.filter(p => !p.optional).map(p => p.name)), u.params && Ei(u.params, h.keys.map(p => p.name))), b = h.stringify(_)
         } else if ("path" in u) b = u.path, h = n.find(p => p.re.test(b)), h && (_ = h.parse(b), P = h.record.name);
         else {
             if (h = d.name ? s.get(d.name) : n.find(p => p.re.test(d.path)), !h) throw en(1, {
                 location: u,
                 currentLocation: d
             });
             P = h.record.name, _ = ie({}, d.params, u.params), b = h.stringify(_)
@@ -5612,15 +5612,15 @@
         resolve: a,
         removeRoute: o,
         getRoutes: c,
         getRecordMatcher: r
     }
 }
 
-function xi(e, t) {
+function Ei(e, t) {
     const n = {};
     for (const s of t) s in e && (n[s] = e[s]);
     return n
 }
 
 function Hu(e) {
     return {
@@ -5854,15 +5854,15 @@
         route: s,
         href: Y(() => s.value.href),
         isActive: i,
         isExactActive: o,
         navigate: c
     }
 }
-const of = vs({
+const of = ys({
     name: "RouterLink",
     compatConfig: {
         MODE: 3
     },
     props: {
         to: {
             type: [String, Object],
@@ -5877,25 +5877,25 @@
             default: "page"
         }
     },
     useLink: Ai,
     setup(e, {
         slots: t
     }) {
-        const n = be(Ai(e)),
+        const n = ve(Ai(e)),
             {
                 options: s
             } = Ve(Rs),
             r = Y(() => ({
                 [Oi(e.activeClass, s.linkActiveClass, "router-link-active")]: n.isActive,
                 [Oi(e.exactActiveClass, s.linkExactActiveClass, "router-link-exact-active")]: n.isExactActive
             }));
         return () => {
             const i = t.default && t.default(n);
-            return e.custom ? i : Pe("a", {
+            return e.custom ? i : Re("a", {
                 "aria-current": n.isExactActive ? e.ariaCurrentValue : null,
                 href: n.href,
                 onClick: n.navigate,
                 class: r.value
             }, i)
         }
     }
@@ -5922,15 +5922,15 @@
     return !0
 }
 
 function Si(e) {
     return e ? e.aliasOf ? e.aliasOf.path : e.path : ""
 }
 const Oi = (e, t, n) => e != null ? e : t != null ? t : n,
-    af = vs({
+    af = ys({
         name: "RouterView",
         inheritAttrs: !1,
         props: {
             name: {
                 type: String,
                 default: "default"
             },
@@ -5970,15 +5970,15 @@
                     h = d && d.components[u];
                 if (!h) return ki(n.default, {
                     Component: h,
                     route: a
                 });
                 const _ = d.props[u],
                     b = _ ? _ === !0 ? a.params : typeof _ == "function" ? _(a) : _ : null,
-                    I = Pe(h, ie({}, b, t, {
+                    I = Re(h, ie({}, b, t, {
                         onVnodeUnmounted: m => {
                             m.component.isUnmounted && (d.instances[u] = null)
                         },
                         ref: l
                     }));
                 return ki(n.default, {
                     Component: I,
@@ -6002,283 +6002,283 @@
         r = e.history,
         i = ln(),
         o = ln(),
         c = ln(),
         l = eo(at);
     let a = at;
     Bt && e.scrollBehavior && "scrollRestoration" in history && (history.scrollRestoration = "manual");
-    const u = Ms.bind(null, E => "" + E),
+    const u = Ms.bind(null, x => "" + x),
         d = Ms.bind(null, ef),
         h = Ms.bind(null, ss);
 
-    function _(E, $) {
+    function _(x, $) {
         let M, K;
-        return sl(E) ? (M = t.getRecordMatcher(E), K = $) : K = E, t.addRoute(K, M)
+        return sl(x) ? (M = t.getRecordMatcher(x), K = $) : K = x, t.addRoute(K, M)
     }
 
-    function b(E) {
-        const $ = t.getRecordMatcher(E);
+    function b(x) {
+        const $ = t.getRecordMatcher(x);
         $ && t.removeRoute($)
     }
 
     function P() {
-        return t.getRoutes().map(E => E.record)
+        return t.getRoutes().map(x => x.record)
     }
 
-    function I(E) {
-        return !!t.getRecordMatcher(E)
+    function I(x) {
+        return !!t.getRecordMatcher(x)
     }
 
-    function m(E, $) {
-        if ($ = ie({}, $ || l.value), typeof E == "string") {
-            const f = Ns(n, E, $.path),
+    function m(x, $) {
+        if ($ = ie({}, $ || l.value), typeof x == "string") {
+            const f = Ns(n, x, $.path),
                 g = t.resolve({
                     path: f.path
                 }, $),
-                y = r.createHref(f.fullPath);
+                v = r.createHref(f.fullPath);
             return ie(f, g, {
                 params: h(g.params),
                 hash: ss(f.hash),
                 redirectedFrom: void 0,
-                href: y
+                href: v
             })
         }
         let M;
-        if ("path" in E) M = ie({}, E, {
-            path: Ns(n, E.path, $.path).path
+        if ("path" in x) M = ie({}, x, {
+            path: Ns(n, x.path, $.path).path
         });
         else {
-            const f = ie({}, E.params);
+            const f = ie({}, x.params);
             for (const g in f) f[g] == null && delete f[g];
-            M = ie({}, E, {
-                params: d(E.params)
+            M = ie({}, x, {
+                params: d(x.params)
             }), $.params = d($.params)
         }
         const K = t.resolve(M, $),
-            se = E.hash || "";
+            se = x.hash || "";
         K.params = u(h(K.params));
-        const de = du(s, ie({}, E, {
+        const de = du(s, ie({}, x, {
                 hash: Xu(se),
                 path: K.path
             })),
             Z = r.createHref(de);
         return ie({
             fullPath: de,
             hash: se,
-            query: s === Ti ? nf(E.query) : E.query || {}
+            query: s === Ti ? nf(x.query) : x.query || {}
         }, K, {
             redirectedFrom: void 0,
             href: Z
         })
     }
 
-    function p(E) {
-        return typeof E == "string" ? Ns(n, E, l.value.path) : ie({}, E)
+    function p(x) {
+        return typeof x == "string" ? Ns(n, x, l.value.path) : ie({}, x)
     }
 
-    function v(E, $) {
-        if (a !== E) return en(8, {
+    function y(x, $) {
+        if (a !== x) return en(8, {
             from: $,
-            to: E
+            to: x
         })
     }
 
-    function x(E) {
-        return B(E)
+    function E(x) {
+        return B(x)
     }
 
-    function k(E) {
-        return x(ie(p(E), {
+    function k(x) {
+        return E(ie(p(x), {
             replace: !0
         }))
     }
 
-    function L(E) {
-        const $ = E.matched[E.matched.length - 1];
+    function L(x) {
+        const $ = x.matched[x.matched.length - 1];
         if ($ && $.redirect) {
             const {
                 redirect: M
             } = $;
-            let K = typeof M == "function" ? M(E) : M;
+            let K = typeof M == "function" ? M(x) : M;
             return typeof K == "string" && (K = K.includes("?") || K.includes("#") ? K = p(K) : {
                 path: K
             }, K.params = {}), ie({
-                query: E.query,
-                hash: E.hash,
-                params: "path" in K ? {} : E.params
+                query: x.query,
+                hash: x.hash,
+                params: "path" in K ? {} : x.params
             }, K)
         }
     }
 
-    function B(E, $) {
-        const M = a = m(E),
+    function B(x, $) {
+        const M = a = m(x),
             K = l.value,
-            se = E.state,
-            de = E.force,
-            Z = E.replace === !0,
+            se = x.state,
+            de = x.force,
+            Z = x.replace === !0,
             f = L(M);
         if (f) return B(ie(p(f), {
             state: typeof f == "object" ? ie({}, se, f.state) : se,
             force: de,
             replace: Z
         }), $ || M);
         const g = M;
         g.redirectedFrom = $;
-        let y;
-        return !de && hu(s, K, M) && (y = en(16, {
+        let v;
+        return !de && hu(s, K, M) && (v = en(16, {
             to: g,
             from: K
-        }), bt(K, K, !0, !1)), (y ? Promise.resolve(y) : z(g, K)).catch(w => Ze(w) ? Ze(w, 2) ? w : je(w) : ue(w, g, K)).then(w => {
+        }), bt(K, K, !0, !1)), (v ? Promise.resolve(v) : z(g, K)).catch(w => Ze(w) ? Ze(w, 2) ? w : je(w) : ue(w, g, K)).then(w => {
             if (w) {
                 if (Ze(w, 2)) return B(ie({
                     replace: Z
                 }, p(w.to), {
                     state: typeof w.to == "object" ? ie({}, se, w.to.state) : se,
                     force: de
                 }), $ || g)
             } else w = V(g, K, !0, Z, se);
             return j(g, K, w), w
         })
     }
 
-    function R(E, $) {
-        const M = v(E, $);
+    function R(x, $) {
+        const M = y(x, $);
         return M ? Promise.reject(M) : Promise.resolve()
     }
 
-    function z(E, $) {
+    function z(x, $) {
         let M;
-        const [K, se, de] = ff(E, $);
-        M = Ls(K.reverse(), "beforeRouteLeave", E, $);
+        const [K, se, de] = ff(x, $);
+        M = Ls(K.reverse(), "beforeRouteLeave", x, $);
         for (const f of K) f.leaveGuards.forEach(g => {
-            M.push(dt(g, E, $))
+            M.push(dt(g, x, $))
         });
-        const Z = R.bind(null, E, $);
+        const Z = R.bind(null, x, $);
         return M.push(Z), $t(M).then(() => {
             M = [];
-            for (const f of i.list()) M.push(dt(f, E, $));
+            for (const f of i.list()) M.push(dt(f, x, $));
             return M.push(Z), $t(M)
         }).then(() => {
-            M = Ls(se, "beforeRouteUpdate", E, $);
+            M = Ls(se, "beforeRouteUpdate", x, $);
             for (const f of se) f.updateGuards.forEach(g => {
-                M.push(dt(g, E, $))
+                M.push(dt(g, x, $))
             });
             return M.push(Z), $t(M)
         }).then(() => {
             M = [];
-            for (const f of E.matched)
+            for (const f of x.matched)
                 if (f.beforeEnter && !$.matched.includes(f))
                     if (We(f.beforeEnter))
-                        for (const g of f.beforeEnter) M.push(dt(g, E, $));
-                    else M.push(dt(f.beforeEnter, E, $));
+                        for (const g of f.beforeEnter) M.push(dt(g, x, $));
+                    else M.push(dt(f.beforeEnter, x, $));
             return M.push(Z), $t(M)
-        }).then(() => (E.matched.forEach(f => f.enterCallbacks = {}), M = Ls(de, "beforeRouteEnter", E, $), M.push(Z), $t(M))).then(() => {
+        }).then(() => (x.matched.forEach(f => f.enterCallbacks = {}), M = Ls(de, "beforeRouteEnter", x, $), M.push(Z), $t(M))).then(() => {
             M = [];
-            for (const f of o.list()) M.push(dt(f, E, $));
+            for (const f of o.list()) M.push(dt(f, x, $));
             return M.push(Z), $t(M)
         }).catch(f => Ze(f, 8) ? f : Promise.reject(f))
     }
 
-    function j(E, $, M) {
-        for (const K of c.list()) K(E, $, M)
+    function j(x, $, M) {
+        for (const K of c.list()) K(x, $, M)
     }
 
-    function V(E, $, M, K, se) {
-        const de = v(E, $);
+    function V(x, $, M, K, se) {
+        const de = y(x, $);
         if (de) return de;
         const Z = $ === at,
             f = Bt ? history.state : {};
-        M && (K || Z ? r.replace(E.fullPath, ie({
+        M && (K || Z ? r.replace(x.fullPath, ie({
             scroll: Z && f && f.scroll
-        }, se)) : r.push(E.fullPath, se)), l.value = E, bt(E, $, M, Z), je()
+        }, se)) : r.push(x.fullPath, se)), l.value = x, bt(x, $, M, Z), je()
     }
     let F;
 
     function X() {
-        F || (F = r.listen((E, $, M) => {
+        F || (F = r.listen((x, $, M) => {
             if (!kn.listening) return;
-            const K = m(E),
+            const K = m(x),
                 se = L(K);
             if (se) {
                 B(ie(se, {
                     replace: !0
                 }), K).catch(gn);
                 return
             }
             a = K;
             const de = l.value;
-            Bt && wu(yi(de.fullPath, M.delta), Cs()), z(K, de).catch(Z => Ze(Z, 12) ? Z : Ze(Z, 2) ? (B(Z.to, K).then(f => {
+            Bt && wu(vi(de.fullPath, M.delta), Cs()), z(K, de).catch(Z => Ze(Z, 12) ? Z : Ze(Z, 2) ? (B(Z.to, K).then(f => {
                 Ze(f, 20) && !M.delta && M.type === Rn.pop && r.go(-1, !1)
             }).catch(gn), Promise.reject()) : (M.delta && r.go(-M.delta, !1), ue(Z, K, de))).then(Z => {
                 Z = Z || V(K, de, !1), Z && (M.delta && !Ze(Z, 8) ? r.go(-M.delta, !1) : M.type === Rn.pop && Ze(Z, 20) && r.go(-1, !1)), j(K, de, Z)
             }).catch(gn)
         }))
     }
     let H = ln(),
         we = ln(),
         ne;
 
-    function ue(E, $, M) {
-        je(E);
+    function ue(x, $, M) {
+        je(x);
         const K = we.list();
-        return K.length ? K.forEach(se => se(E, $, M)) : console.error(E), Promise.reject(E)
+        return K.length ? K.forEach(se => se(x, $, M)) : console.error(x), Promise.reject(x)
     }
 
     function oe() {
-        return ne && l.value !== at ? Promise.resolve() : new Promise((E, $) => {
-            H.add([E, $])
+        return ne && l.value !== at ? Promise.resolve() : new Promise((x, $) => {
+            H.add([x, $])
         })
     }
 
-    function je(E) {
-        return ne || (ne = !E, X(), H.list().forEach(([$, M]) => E ? M(E) : $()), H.reset()), E
+    function je(x) {
+        return ne || (ne = !x, X(), H.list().forEach(([$, M]) => x ? M(x) : $()), H.reset()), x
     }
 
-    function bt(E, $, M, K) {
+    function bt(x, $, M, K) {
         const {
             scrollBehavior: se
         } = e;
         if (!Bt || !se) return Promise.resolve();
-        const de = !M && Eu(yi(E.fullPath, 0)) || (K || !M) && history.state && history.state.scroll || null;
-        return ur().then(() => se(E, $, de)).then(Z => Z && bu(Z)).catch(Z => ue(Z, E, $))
+        const de = !M && xu(vi(x.fullPath, 0)) || (K || !M) && history.state && history.state.scroll || null;
+        return ur().then(() => se(x, $, de)).then(Z => Z && bu(Z)).catch(Z => ue(Z, x, $))
     }
-    const De = E => r.go(E);
+    const De = x => r.go(x);
     let Ae;
     const Lt = new Set,
         kn = {
             currentRoute: l,
             listening: !0,
             addRoute: _,
             removeRoute: b,
             hasRoute: I,
             getRoutes: P,
             resolve: m,
             options: e,
-            push: x,
+            push: E,
             replace: k,
             go: De,
             back: () => De(-1),
             forward: () => De(1),
             beforeEach: i.add,
             beforeResolve: o.add,
             afterEach: c.add,
             onError: we.add,
             isReady: oe,
-            install(E) {
+            install(x) {
                 const $ = this;
-                E.component("RouterLink", fl), E.component("RouterView", dl), E.config.globalProperties.$router = $, Object.defineProperty(E.config.globalProperties, "$route", {
+                x.component("RouterLink", fl), x.component("RouterView", dl), x.config.globalProperties.$router = $, Object.defineProperty(x.config.globalProperties, "$route", {
                     enumerable: !0,
                     get: () => Ne(l)
-                }), Bt && !Ae && l.value === at && (Ae = !0, x(r.location).catch(se => {}));
+                }), Bt && !Ae && l.value === at && (Ae = !0, E(r.location).catch(se => {}));
                 const M = {};
                 for (const se in at) M[se] = Y(() => l.value[se]);
-                E.provide(Rs, $), E.provide(Rr, be(M)), E.provide(er, l);
-                const K = E.unmount;
-                Lt.add(E), E.unmount = function() {
-                    Lt.delete(E), Lt.size < 1 && (a = at, F && F(), F = null, l.value = at, Ae = !1, ne = !1), K()
+                x.provide(Rs, $), x.provide(Rr, ve(M)), x.provide(er, l);
+                const K = x.unmount;
+                Lt.add(x), x.unmount = function() {
+                    Lt.delete(x), Lt.size < 1 && (a = at, F && F(), F = null, l.value = at, Ae = !1, ne = !1), K()
                 }
             }
         };
     return kn
 }
 
 function $t(e) {
@@ -6309,50 +6309,50 @@
 const hf = "/frontend/assets/datailor-logo.fbfa6008.svg",
     pf = "/frontend/assets/eu.24cff2c1.png",
     gf = "/frontend/assets/horizon-europe.80625b0c.png";
 const mf = {
         class: "navbar"
     },
     _f = ["src"],
-    yf = {
+    vf = {
         class: "footer"
     },
-    vf = {
+    yf = {
         class: "thanking"
     },
     bf = ["src"],
-    wf = Ee("p", null, " This project has received funding from the European Union\u2019s Horizon Europe research and innovation programme under grant agreement No 101070350 ", -1),
-    Ef = {
+    wf = xe("p", null, " This project has received funding from the European Union\u2019s Horizon Europe research and innovation programme under grant agreement No 101070350 ", -1),
+    xf = {
         class: "thanking"
     },
-    xf = ["src"],
-    Cf = Ee("p", null, " The contents of this publication are the sole responsibility of the HPLT consortium and do not necessarily reflect the opinion of the European Union. ", -1),
+    Ef = ["src"],
+    Cf = xe("p", null, " The contents of this publication are the sole responsibility of the HPLT consortium and do not necessarily reflect the opinion of the European Union. ", -1),
     Rf = {
         __name: "App",
         setup(e) {
-            return (t, n) => (Jt(), da(ve, null, [Ee("div", mf, [ce(Ne(fl), {
+            return (t, n) => (Jt(), da(be, null, [xe("div", mf, [ce(Ne(fl), {
                 to: {
                     name: "list-datasets"
                 }
             }, {
-                default: fr(() => [Ee("img", {
+                default: fr(() => [xe("img", {
                     class: "logo-datailor",
                     src: Ne(hf),
                     alt: "Datailor logo"
                 }, null, 8, _f)]),
                 _: 1
-            })]), ce(Ne(dl)), Ee("div", yf, [Ee("div", vf, [Ee("img", {
+            })]), ce(Ne(dl)), xe("div", vf, [xe("div", yf, [xe("img", {
                 src: Ne(pf),
                 alt: "EU logo",
                 class: "eu-flag"
-            }, null, 8, bf), wf]), Ee("div", Ef, [Ee("img", {
+            }, null, 8, bf), wf]), xe("div", xf, [xe("img", {
                 src: Ne(gf),
                 alt: "Horizon Europe logo",
                 class: "horizon-flag"
-            }, null, 8, xf), Cf])])], 64))
+            }, null, 8, Ef), Cf])])], 64))
         }
     },
     Tf = "modulepreload",
     Pf = function(e) {
         return "/frontend/" + e
     },
     Ii = {},
@@ -6379,31 +6379,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<polyline points="16 18 22 12 16 6"></polyline><polyline points="8 6 2 12 8 18"></polyline>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6426,31 +6426,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<polyline points="8 17 12 21 16 17"></polyline><line x1="12" y1="12" x2="12" y2="21"></line><path d="M20.88 18.09A5 5 0 0 0 18 9h-1.26A8 8 0 1 0 3 16.29"></path>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6473,31 +6473,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<path d="M12 20h9"></path><path d="M16.5 3.5a2.121 2.121 0 0 1 3 3L7 19l-4 1 1-4L16.5 3.5z"></path>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6520,31 +6520,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<polygon points="22 3 2 3 10 12.46 10 19 14 21 14 12.46 22 3"></polygon>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6567,31 +6567,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<line x1="5" y1="12" x2="19" y2="12"></line>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6614,31 +6614,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<path d="M21.21 15.89A10 10 0 1 1 8 2.83"></path><path d="M22 12A10 10 0 0 0 12 2v10z"></path>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6661,31 +6661,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<line x1="12" y1="5" x2="12" y2="19"></line><line x1="5" y1="12" x2="19" y2="12"></line>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6708,31 +6708,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<polyline points="1 4 1 10 7 10"></polyline><path d="M3.51 15a9 9 0 1 0 2.13-9.36L1 10"></path>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6755,31 +6755,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6802,31 +6802,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<path d="M20.59 13.41l-7.17 7.17a2 2 0 0 1-2.83 0L2 12V2h10l8.59 8.59a2 2 0 0 1 0 2.82z"></path><line x1="7" y1="7" x2="7.01" y2="7"></line>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6836,44 +6836,91 @@
                     "stroke-linejoin": "round",
                     class: "feather feather-tag"
                 }, c))
             }
         }
     },
     Vd = {
+        name: "TrashIcon",
+        props: {
+            size: {
+                type: String,
+                default: "24",
+                validator: function(t) {
+                    return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
+                }
+            }
+        },
+        functional: !0,
+        setup: function(t, n) {
+            var s = n.attrs,
+                r = Fe(t),
+                i = r.size,
+                o = Y(function() {
+                    return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
+                }),
+                c = ve(Object.assign({}, s, {
+                    width: Y(function() {
+                        var l;
+                        return (l = s.width) !== null && l !== void 0 ? l : o.value
+                    }),
+                    height: Y(function() {
+                        var l;
+                        return (l = s.height) !== null && l !== void 0 ? l : o.value
+                    })
+                }));
+            return function() {
+                return Re("svg", Object.assign({
+                    innerHTML: '<polyline points="3 6 5 6 21 6"></polyline><path d="M19 6v14a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2V6m3 0V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v2"></path>'
+                }, {
+                    xmlns: "http://www.w3.org/2000/svg",
+                    width: 24,
+                    height: 24,
+                    viewBox: "0 0 24 24",
+                    fill: "none",
+                    stroke: "currentColor",
+                    "stroke-width": 2,
+                    "stroke-linecap": "round",
+                    "stroke-linejoin": "round",
+                    class: "feather feather-trash"
+                }, c))
+            }
+        }
+    },
+    Wd = {
         name: "UploadIcon",
         props: {
             size: {
                 type: String,
                 default: "24",
                 validator: function(t) {
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path><polyline points="17 8 12 3 7 8"></polyline><line x1="12" y1="3" x2="12" y2="15"></line>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6896,31 +6943,31 @@
                     return !isNaN(t) || t.length >= 2 && !isNaN(t.slice(0, t.length - 1)) && t.slice(-1) === "x"
                 }
             }
         },
         functional: !0,
         setup: function(t, n) {
             var s = n.attrs,
-                r = He(t),
+                r = Fe(t),
                 i = r.size,
                 o = Y(function() {
                     return i.value.slice(-1) === "x" ? i.value.slice(0, i.value.length - 1) + "em" : parseInt(i.value) + "px"
                 }),
-                c = be(Object.assign({}, s, {
+                c = ve(Object.assign({}, s, {
                     width: Y(function() {
                         var l;
                         return (l = s.width) !== null && l !== void 0 ? l : o.value
                     }),
                     height: Y(function() {
                         var l;
                         return (l = s.height) !== null && l !== void 0 ? l : o.value
                     })
                 }));
             return function() {
-                return Pe("svg", Object.assign({
+                return Re("svg", Object.assign({
                     innerHTML: '<line x1="18" y1="6" x2="6" y2="18"></line><line x1="6" y1="6" x2="18" y2="18"></line>'
                 }, {
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 24,
                     height: 24,
                     viewBox: "0 0 24 24",
                     fill: "none",
@@ -6978,50 +7025,51 @@
             }
             return On(() => {
                 document.body.addEventListener("keyup", o), document.body.style.overflow = "hidden"
             }), ws(() => {
                 document.body.removeEventListener("keyup", o), document.body.style.overflow = ""
             }), (c, l) => (Jt(), es(fa, {
                 to: "body"
-            }, [Ee("div", Of, [Ee("div", {
+            }, [xe("div", Of, [xe("div", {
                 class: "overlay",
                 onClick: l[0] || (l[0] = a => i())
-            }), Ee("div", kf, [Ee("button", {
+            }), xe("div", kf, [xe("button", {
                 class: "close-button icon-button",
                 title: "Close",
                 onClick: l[1] || (l[1] = a => i())
-            }, [ce(Ne(Af))]), Ee("div", If, [(Jt(), es(Kc(Ne(s)), wl(ko(c.$attrs)), null, 16))])])])]))
+            }, [ce(Ne(Af))]), xe("div", If, [(Jt(), es(Kc(Ne(s)), wl(ko(c.$attrs)), null, 16))])])])]))
         }
     },
     Nf = Sf(Mf, [
         ["__scopeId", "data-v-1e8f5c6b"]
     ]),
     Lf = uf({
         history: Pu("/frontend/"),
         routes: [{
             path: "/",
             name: "list-datasets",
-            component: () => Un(() => import("./ListDatasetsView.1513f813.js"), ["assets/ListDatasetsView.1513f813.js", "assets/ListDatasetsView.02d1a0b3.css", "assets/TagsEditor.8b755087.js", "assets/TagsEditor.ccc03a15.css", "assets/filtersteps.2a7228ad.js"]),
+            component: () => Un(() => import("./ListDatasetsView.0c61d7cc.js"), ["assets/ListDatasetsView.0c61d7cc.js", "assets/ListDatasetsView.79aac80d.css", "assets/TagsEditor.23cf196f.js", "assets/TagsEditor.ccc03a15.css", "assets/hacks.1ae1ba64.js"]),
             children: [{
                 name: "edit-filters-yaml",
-                path: "/datasets/:datasetName/configuration.yaml",
+                path: "/datasets/:datasetName/:format",
                 component: Nf,
                 props: {
-                    component: () => Un(() => import("./EditFiltersYamlView.45bdcb50.js"), ["assets/EditFiltersYamlView.45bdcb50.js", "assets/filtersteps.2a7228ad.js"])
+                    component: () => Un(() => import("./EditFiltersYamlView.28a1a7c9.js"), ["assets/EditFiltersYamlView.28a1a7c9.js", "assets/hacks.1ae1ba64.js"]),
+                    format: "configuration-for-opusfilter.yaml"
                 }
             }]
         }, {
             path: "/datasets/:datasetName/configuration",
             name: "edit-filters",
-            component: () => Un(() => import("./EditFiltersView.272e0d14.js"), ["assets/EditFiltersView.272e0d14.js", "assets/EditFiltersView.4490d98b.css", "assets/TagsEditor.8b755087.js", "assets/TagsEditor.ccc03a15.css", "assets/filtersteps.2a7228ad.js", "assets/vue-select.6aaeaff8.js", "assets/vue-select.b0fac2a1.css"])
+            component: () => Un(() => import("./EditFiltersView.bc0dd7c3.js"), ["assets/EditFiltersView.bc0dd7c3.js", "assets/EditFiltersView.a7795492.css", "assets/TagsEditor.23cf196f.js", "assets/TagsEditor.ccc03a15.css", "assets/hacks.1ae1ba64.js", "assets/vue-select.9ddbca8a.js", "assets/vue-select.b0fac2a1.css"])
         }, {
             path: "/download/",
             name: "add-dataset",
-            component: () => Un(() => import("./AddDatasetView.5dcf722c.js"), ["assets/AddDatasetView.5dcf722c.js", "assets/AddDatasetView.4182f0f7.css", "assets/vue-select.6aaeaff8.js", "assets/vue-select.b0fac2a1.css"])
+            component: () => Un(() => import("./AddDatasetView.ff526466.js"), ["assets/AddDatasetView.ff526466.js", "assets/AddDatasetView.4182f0f7.css", "assets/vue-select.9ddbca8a.js", "assets/vue-select.b0fac2a1.css"])
         }]
     });
 const hl = cu(Rf);
 hl.use(Lf);
 hl.mount("#app");
 export {
-    He as $, Nd as A, $i as B, Ld as C, us as D, $d as E, ve as F, Kf as G, jf as H, $f as I, Bf as J, Zi as K, Ut as L, Yt as M, Qn as N, Gi as O, jd as P, Hf as Q, fl as R, no as S, fa as T, Vd as U, Uf as V, eo as W, Df as X, te as Y, lc as Z, Sf as _, es as a, Qt as a$, zf as a0, Be as a1, as as a2, os as a3, wl as a4, zn as a5, go as a6, Te as a7, Zf as a8, Wt as a9, Ot as aA, _d as aB, pa as aC, ur as aD, Nc as aE, $c as aF, mr as aG, Bc as aH, Lc as aI, Uc as aJ, On as aK, Dc as aL, jc as aM, Hc as aN, ws as aO, gr as aP, Wn as aQ, lo as aR, ad as aS, rd as aT, ed as aU, td as aV, Kc as aW, Cd as aX, xn as aY, Xr as aZ, vc as a_, Yf as aa, Cn as ab, $e as ac, nt as ad, rt as ae, Rd as af, oa as ag, yd as ah, ia as ai, sd as aj, ld as ak, Xf as al, vs as am, dd as an, hd as ao, fd as ap, sn as aq, Nt as ar, pr as as, ko as at, Pe as au, tn as av, wd as aw, Ve as ax, xa as ay, ud as az, ce as b, Ea as b0, xd as b1, id as b2, od as b3, md as b4, bd as b5, gd as b6, po as b7, Ca as b8, uc as b9, Ud as bA, zd as bB, Hd as bC, Dd as bD, Fd as bE, Qf as ba, Oc as bb, Jf as bc, vd as bd, pd as be, Ed as bf, qf as bg, jo as bh, Sd as bi, xr as bj, cu as bk, Id as bl, Ua as bm, Td as bn, lu as bo, Md as bp, pi as bq, Pd as br, Ad as bs, eu as bt, Yo as bu, Ga as bv, Xs as bw, iu as bx, kd as by, Od as bz, da as c, Ee as d, dl as e, Io as f, Bd as g, Wf as h, Kn as i, be as j, Y as k, Vt as l, Gf as m, _e as n, Jt as o, Vf as p, is as q, nd as r, cd as s, Ff as t, Ne as u, qo as v, fr as w, Kd as x, nc as y, Xi as z
+    lc as $, Qf as A, Nd as B, Ld as C, $i as D, $d as E, be as F, us as G, Kf as H, jf as I, $f as J, Bf as K, Zi as L, Ut as M, Yt as N, Qn as O, jd as P, Gi as Q, fl as R, Hf as S, fa as T, Wd as U, no as V, Uf as W, eo as X, Df as Y, te as Z, Sf as _, es as a, yc as a$, Fe as a0, zf as a1, He as a2, as as a3, os as a4, wl as a5, zn as a6, go as a7, Pe as a8, Zf as a9, ud as aA, Ot as aB, _d as aC, pa as aD, ur as aE, Nc as aF, $c as aG, mr as aH, Bc as aI, Lc as aJ, Uc as aK, On as aL, Dc as aM, jc as aN, Hc as aO, ws as aP, gr as aQ, Wn as aR, lo as aS, ad as aT, rd as aU, ed as aV, td as aW, Kc as aX, Cd as aY, En as aZ, Xr as a_, Wt as aa, Yf as ab, Cn as ac, Be as ad, nt as ae, rt as af, Rd as ag, oa as ah, vd as ai, ia as aj, sd as ak, ld as al, Xf as am, ys as an, dd as ao, hd as ap, fd as aq, sn as ar, Nt as as, pr as at, ko as au, Re as av, tn as aw, wd as ax, Ve as ay, Ea as az, ce as b, Qt as b0, xa as b1, Ed as b2, id as b3, od as b4, md as b5, bd as b6, gd as b7, po as b8, Ca as b9, Vd as bA, Dd as bB, Ud as bC, zd as bD, Hd as bE, Fd as bF, uc as ba, Oc as bb, Jf as bc, yd as bd, pd as be, xd as bf, qf as bg, jo as bh, Sd as bi, Er as bj, cu as bk, Id as bl, Ua as bm, Td as bn, lu as bo, Md as bp, pi as bq, Pd as br, Ad as bs, eu as bt, Yo as bu, Ga as bv, Xs as bw, iu as bx, kd as by, Od as bz, da as c, xe as d, dl as e, Io as f, Bd as g, Wf as h, Kn as i, ve as j, Vt as k, Xi as l, Y as m, Gf as n, Jt as o, Vf as p, _e as q, nd as r, nc as s, Ff as t, Ne as u, qo as v, fr as w, is as x, cd as y, Kd as z
 };
```

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/vue-select.6aaeaff8.js` & `opuscleaner-0.2/opuscleaner/frontend/assets/vue-select.9ddbca8a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,32 +1,32 @@
 import {
     o as a,
     c as h,
-    aV as T,
-    aT as r,
-    a4 as d,
-    at as c,
+    aW as F,
+    aU as r,
+    a5 as d,
+    au as c,
     d as p,
     F as _,
     r as V,
     f as w,
     t as $,
     a as b,
-    aW as m,
-    s as O,
-    aC as C,
-    b2 as F,
-    m as v,
+    aX as m,
+    y as O,
+    aD as C,
+    b3 as T,
+    n as v,
     bx as L,
     b as E,
     w as M,
     bz as B,
-    a3 as A,
+    a4 as A,
     bh as j
-} from "./index.490d1368.js";
+} from "./index.6cc31f0d.js";
 var I = Object.defineProperty,
     N = Object.defineProperties,
     K = Object.getOwnPropertyDescriptors,
     D = Object.getOwnPropertySymbols,
     z = Object.prototype.hasOwnProperty,
     R = Object.prototype.propertyIsEnumerable,
     P = (e, t, s) => t in e ? I(e, t, {
@@ -154,26 +154,26 @@
     },
     S = (e, t) => {
         const s = e.__vccOpts || e;
         for (const [n, l] of t) s[n] = l;
         return s
     },
     H = {},
-    Q = {
+    X = {
         xmlns: "http://www.w3.org/2000/svg",
         width: "10",
         height: "10"
     },
-    X = p("path", {
+    Q = p("path", {
         d: "M6.895455 5l2.842897-2.842898c.348864-.348863.348864-.914488 0-1.263636L9.106534.261648c-.348864-.348864-.914489-.348864-1.263636 0L5 3.104545 2.157102.261648c-.348863-.348864-.914488-.348864-1.263636 0L.261648.893466c-.348864.348864-.348864.914489 0 1.263636L3.104545 5 .261648 7.842898c-.348864.348863-.348864.914488 0 1.263636l.631818.631818c.348864.348864.914773.348864 1.263636 0L5 6.895455l2.842898 2.842897c.348863.348864.914772.348864 1.263636 0l.631818-.631818c.348864-.348864.348864-.914489 0-1.263636L6.895455 5z"
     }, null, -1),
-    Y = [X];
+    Y = [Q];
 
 function W(e, t) {
-    return a(), h("svg", Q, Y)
+    return a(), h("svg", X, Y)
 }
 const G = S(H, [
         ["render", W]
     ]),
     Z = {},
     ee = {
         xmlns: "http://www.w3.org/2000/svg",
@@ -717,15 +717,15 @@
         key: 0,
         class: "vs__no-options"
     },
     ve = w(" Sorry, no matching options. "),
     we = ["id"];
 
 function Se(e, t, s, n, l, o) {
-    const y = T("append-to-body");
+    const y = F("append-to-body");
     return a(), h("div", {
         dir: s.dir,
         class: A(["v-select", o.stateClasses])
     }, [r(e.$slots, "header", d(c(o.scope.header))), p("div", {
         id: `vs${s.uid}__combobox`,
         ref: "toggle",
         class: "vs__dropdown-toggle",
@@ -750,15 +750,15 @@
         type: "button",
         class: "vs__deselect",
         title: `Deselect ${s.getOptionLabel(i)}`,
         "aria-label": `Deselect ${s.getOptionLabel(i)}`,
         onClick: g => o.deselect(i)
     }, [(a(), b(m(o.childComponents.Deselect)))], 8, ue)) : O("", !0)]))])), 256)), r(e.$slots, "search", d(c(o.scope.search)), () => [p("input", C({
         class: "vs__search"
-    }, o.scope.search.attributes, F(o.scope.search.events)), null, 16)])], 512), p("div", fe, [v(p("button", {
+    }, o.scope.search.attributes, T(o.scope.search.events)), null, 16)])], 512), p("div", fe, [v(p("button", {
         ref: "clearButton",
         disabled: s.disabled,
         type: "button",
         class: "vs__clear",
         title: "Clear Selected",
         "aria-label": "Clear Selected",
         onClick: t[0] || (t[0] = (...i) => o.clearSelection && o.clearSelection(...i))
```

### Comparing `opuscleaner-0.1/opuscleaner/frontend/assets/vue-select.b0fac2a1.css` & `opuscleaner-0.2/opuscleaner/frontend/assets/vue-select.b0fac2a1.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.1/PKG-INFO` & `opuscleaner-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opuscleaner
-Version: 0.1
+Version: 0.2
 Project-URL: Documentation, https://github.com/unknown/opuscleaner#readme
 Project-URL: Issues, https://github.com/unknown/opuscleaner/issues
 Project-URL: Source, https://github.com/unknown/opuscleaner
 Author-email: Jelmer van der Linde <jelmer@ikhoefgeen.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -15,35 +15,48 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: fastapi==0.78.0
 Requires-Dist: pyyaml==6.0
 Requires-Dist: uvicorn==0.20.0
-Requires-Dist: xxhash==3.0.0
+Requires-Dist: xxhash==3.2.0
 Provides-Extra: all
 Requires-Dist: bicleaner; extra == 'all'
 Requires-Dist: bifixer; extra == 'all'
 Requires-Dist: fasttext; extra == 'all'
 Requires-Dist: fugashi[unidic-lite]==1.1.2; extra == 'all'
 Requires-Dist: hanziconv==0.3.2; extra == 'all'
 Requires-Dist: laserembeddings[ja,zh]==1.1.2; extra == 'all'
 Requires-Dist: more-itertools; extra == 'all'
+Requires-Dist: opusfilter==2.6.0; extra == 'all'
 Requires-Dist: pycld2==0.41; extra == 'all'
 Requires-Dist: requests; extra == 'all'
 Requires-Dist: sacremoses; extra == 'all'
 Requires-Dist: spacy-pkuseg; extra == 'all'
 Description-Content-Type: text/markdown
 
 # OpusCleaner
-OpusCleaner is a machine translation/language model data cleaner and training scheduler. The Training scheduler has moved to [empty-trainer](https://github.com/hplt-project/empty-trainer).
+OpusCleaner is a machine translation/language model data cleaner and training scheduler. The Training scheduler has moved to [OpusTrainer](https://github.com/hplt-project/OpusTrainer).
 
 ## Cleaner
 The cleaner bit takes care of downloading and cleaning multiple different datasets and preparing them for translation.
 
+### Installation for cleaning
+If you just want to use OpusCleaner for cleaning, you can install it from PyPI, and then run it
+
+```sh
+pip3 install opuscleaner
+opuscleaner-server serve
+```
+
+Then you can go to http://127.0.0.1:8000/ to show the interface.
+
+You can also install and run OpusCleaner on a remote machine, and use [SSH local forwarding](https://www.ssh.com/academy/ssh/tunneling-example) (e.g. `ssh -L 8000:localhost:8000 you@remote.machine`) to access the interface on your local machine.
+
 ### Dependencies
 (Mainly listed as shortcuts to documentation)
 
 - [FastAPI](https://fastapi.tiangolo.com) as the base for the backend part.
 - [Pydantic](https://pydantic-docs.helpmanual.io/) for conversion of untyped JSON to typed objects. And because FastAPI automatically supports it and gives you useful error messages if you mess up things.
 - [Vue](https://vuejs.org/guide/introduction.html) for frontend
 
@@ -59,39 +72,33 @@
 [<img src=".github/screenshots/filter-datasets.png" width="100%">](.github/screenshots/filter-datasets.png)
 
 Compare the dataset at different stages of filtering to see what the impact is of each filter.
 [<img src=".github/screenshots/diff-filter-output.png" width="100%">](.github/screenshots/diff-filter-output.png)
 
 
 ### Paths
-- `data/train-parts` is scanned for datasets
-- `filters` should contain filter json (but that's not implemented yet, right now it just has a hard-coded `FILTERS` dict in code)
+- `data/train-parts` is scanned for datasets. You can change this by setting the `DATA_PATH` environment variable, the default is `data/train-parts/*.*.gz`.
+- `filters` should contain filter json files. You can change the `FILTER_PATH` environment variable, the default is `<PYTHON_PACKAGE>/filters/*.json`.
 
 ### Installation for development
 ```sh
-python3 -m venv .env
-bash --init-file .env/bin/activate
-pip install -e .
-
 cd frontend
 npm clean-install
 npm run build
 cd ..
-```
-
-Link the frontend build folder into opuscleaner. Normally this is done during packaging but when opuscleaner is installed as an editable package, this doesn't happen.
 
-```sh
-ln -s ../frontend/dist opuscleaner/frontend
+python3 -m venv .env
+bash --init-file .env/bin/activate
+pip install -e .
 ```
 
 Finally you can run `opuscleaner-server` as normal. The `--reload` option will cause it to restart when any of the python files change.
 
 ```sh
-opuscleaner-server --reload
+opuscleaner-server serve --reload
 ```
 
 Then go to http://127.0.0.1:8000/ for the "interface" or http://127.0.0.1:8000/docs for the API.
 
 ### Frontend development
 
 If you're doing frontend development, try also running:
@@ -111,13 +118,13 @@
 
 ```sh
 python -m laserembeddings download-models
 ```
 
 ## Packaging
 
-Run `pip wheel .` to build & package OpusCleaner. Packaging is done through hatch, see the `pyproject.toml` and `build_frontend.py` files for details. You'll need to have a recent version of `node` and `npm` in your `PATH` for this to work.
+Run `npm build` in the `frontend/` directory first, and then run `hatch build .` in the project directory to build the wheel and source distribution.
 
 # Acknowledgements
 
 This project has received funding from the European Union’s Horizon Europe research and innovation programme under grant agreement No 101070350 and from UK Research and Innovation (UKRI) under the UK government’s Horizon Europe funding guarantee [grant number 10052546]
```

