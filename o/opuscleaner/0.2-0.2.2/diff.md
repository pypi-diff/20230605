# Comparing `tmp/opuscleaner-0.2.tar.gz` & `tmp/opuscleaner-0.2.2.tar.gz`

## Comparing `opuscleaner-0.2.tar` & `opuscleaner-0.2.2.tar`

### file list

```diff
@@ -1,107 +1,100 @@
--rwxr-xr-x   0        0        0     2689 2020-02-02 00:00:00.000000 opuscleaner-0.2/dump-parameter-schema.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 opuscleaner-0.2/requirements-all.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 opuscleaner-0.2/requirements.txt
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/index.html
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/AddDatasetView.4182f0f7.css
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/AddDatasetView.ff526466.js
--rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/EditFiltersView.a7795492.css
--rw-r--r--   0        0        0   121398 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/EditFiltersView.bc0dd7c3.js
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/EditFiltersYamlView.28a1a7c9.js
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/ListDatasetsView.0c61d7cc.js
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/ListDatasetsView.79aac80d.css
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/TagsEditor.23cf196f.js
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css
--rw-r--r--   0        0        0    38943 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/data-cuate.84693c76.svg
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg
--rw-r--r--   0        0        0    22166 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/eu.24cff2c1.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/hacks.1ae1ba64.js
--rw-r--r--   0        0        0   101750 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/horizon-europe.80625b0c.png
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/index.47848488.css
--rw-r--r--   0        0        0   124624 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/index.6cc31f0d.js
--rw-r--r--   0        0        0    17440 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/vue-select.9ddbca8a.js
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/frontend/assets/vue-select.b0fac2a1.css
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/_util.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/categories.py
--rwxr-xr-x   0        0        0    21105 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/clean.py
--rwxr-xr-x   0        0        0     2015 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/col.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/config.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/datasets.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/download.py
--rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters.py
--rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/opusfilter_compat.py
--rwxr-xr-x   0        0        0     4581 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/sample.py
--rw-r--r--   0        0        0    16891 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/server.py
--rwxr-xr-x   0        0        0     8153 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/threshold.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/alpha_ratio.json
--rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/alpha_ratio.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/bicleaner_hardrules.json
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/bifixer.json
--rwxr-xr-x   0        0        0      454 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/bifixer_dedupe.py
--rwxr-xr-x   0        0        0     2440 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/clean_common.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/deescape-special-chars.json
--rwxr-xr-x   0        0        0      631 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/deescape-special-chars.perl
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/deescape_tsv.json
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/deescape_tsv.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/detokenizer.json
--rwxr-xr-x   0        0        0    12473 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/detokenizer.perl
--rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fasttext_filter.json
--rwxr-xr-x   0        0        0     3173 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fasttext_filter.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_elitr_eca.json
--rwxr-xr-x   0        0        0     1473 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_elitr_eca.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_quotes.json
--rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_quotes.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_un_chinese.json
--rwxr-xr-x   0        0        0      354 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_un_chinese.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_wiki.json
--rwxr-xr-x   0        0        0     3569 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/fix_wiki.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/langid.json
--rwxr-xr-x   0        0        0     3019 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/langid.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/laser_similarity.json
--rwxr-xr-x   0        0        0     4525 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/laser_similarity.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/max_length.json
--rwxr-xr-x   0        0        0     1545 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/max_length.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/max_word_length.json
--rwxr-xr-x   0        0        0      869 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/max_word_length.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/num_mismatch.json
--rwxr-xr-x   0        0        0     1248 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/num_mismatch.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/regexp.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/remove_empty_lines.json
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/remove_frequent_patterns.json
--rwxr-xr-x   0        0        0     2700 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/remove_frequent_patterns.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/remove_frequent_patterns.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/sed.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/segment_chinese.json
--rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/segment_chinese.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/segment_japanese.json
--rwxr-xr-x   0        0        0      588 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/segment_japanese.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/simplify_chinese.json
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/split_sentences.json
--rwxr-xr-x   0        0        0     1059 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/split_sentences.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/src_trg_ratio.json
--rwxr-xr-x   0        0        0     2298 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/src_trg_ratio.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/strip_suffix.json
--rwxr-xr-x   0        0        0     2271 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/strip_suffix.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/traditionalise_chinese.json
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/AlphabetRatioFilter.json
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/AverageWordLengthFilter.json
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/CharacterScoreFilter.json
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/Detokenizer.json
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/HtmlTagFilter.json
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/LengthFilter.json
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/LengthRatioFilter.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/LongWordFilter.json
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/RegExpFilter.json
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/RegExpSub.json
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/Tokenizer.json
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/WhitespaceNormalizer.json
--rwxr-xr-x   0        0        0     1808 2020-02-02 00:00:00.000000 opuscleaner-0.2/opuscleaner/filters/opusfilter/opusfilter-ersatz.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 opuscleaner-0.2/utils/dedup/README.md
--rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 opuscleaner-0.2/utils/dedup/dedup.sh
--rwxr-xr-x   0        0        0     1046 2020-02-02 00:00:00.000000 opuscleaner-0.2/utils/dedup/hash-seg.py
--rwxr-xr-x   0        0        0      906 2020-02-02 00:00:00.000000 opuscleaner-0.2/utils/dedup/superdedup.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 opuscleaner-0.2/.gitignore
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 opuscleaner-0.2/README.md
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 opuscleaner-0.2/pyproject.toml
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 opuscleaner-0.2/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/_util.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/categories.py
+-rwxr-xr-x   0        0        0    21105 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/clean.py
+-rwxr-xr-x   0        0        0     2015 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/col.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/config.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/datasets.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/download.py
+-rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters.py
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/opusfilter_compat.py
+-rwxr-xr-x   0        0        0     4581 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/sample.py
+-rw-r--r--   0        0        0    16891 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/server.py
+-rwxr-xr-x   0        0        0     8153 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/threshold.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/alpha_ratio.json
+-rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/alpha_ratio.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/bicleaner_hardrules.json
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/bifixer.json
+-rwxr-xr-x   0        0        0      454 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/bifixer_dedupe.py
+-rwxr-xr-x   0        0        0     2440 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/clean_common.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/deescape-special-chars.json
+-rwxr-xr-x   0        0        0      631 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/deescape-special-chars.perl
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/deescape_tsv.json
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/deescape_tsv.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/detokenizer.json
+-rwxr-xr-x   0        0        0    12473 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/detokenizer.perl
+-rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fasttext_filter.json
+-rwxr-xr-x   0        0        0     3173 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fasttext_filter.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_elitr_eca.json
+-rwxr-xr-x   0        0        0     1473 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_elitr_eca.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_quotes.json
+-rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_quotes.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_un_chinese.json
+-rwxr-xr-x   0        0        0      354 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_un_chinese.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_wiki.json
+-rwxr-xr-x   0        0        0     3569 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_wiki.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/langid.json
+-rwxr-xr-x   0        0        0     3019 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/langid.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/laser_similarity.json
+-rwxr-xr-x   0        0        0     4525 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/laser_similarity.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/max_length.json
+-rwxr-xr-x   0        0        0     1545 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/max_length.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/max_word_length.json
+-rwxr-xr-x   0        0        0      869 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/max_word_length.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/num_mismatch.json
+-rwxr-xr-x   0        0        0     1248 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/num_mismatch.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/regexp.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/remove_empty_lines.json
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/remove_frequent_patterns.json
+-rwxr-xr-x   0        0        0     2700 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/remove_frequent_patterns.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/remove_frequent_patterns.txt
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/sed.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/segment_chinese.json
+-rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/segment_chinese.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/segment_japanese.json
+-rwxr-xr-x   0        0        0      588 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/segment_japanese.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/simplify_chinese.json
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/split_sentences.json
+-rwxr-xr-x   0        0        0     1059 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/split_sentences.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/src_trg_ratio.json
+-rwxr-xr-x   0        0        0     2298 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/src_trg_ratio.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/strip_suffix.json
+-rwxr-xr-x   0        0        0     2271 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/strip_suffix.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/traditionalise_chinese.json
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/AlphabetRatioFilter.json
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/AverageWordLengthFilter.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/CharacterScoreFilter.json
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/Detokenizer.json
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/HtmlTagFilter.json
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/LengthFilter.json
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/LengthRatioFilter.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/LongWordFilter.json
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/RegExpFilter.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/RegExpSub.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/Tokenizer.json
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/WhitespaceNormalizer.json
+-rwxr-xr-x   0        0        0     1808 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/opusfilter-ersatz.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/index.html
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/AddDatasetView.4182f0f7.css
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/AddDatasetView.ff526466.js
+-rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/EditFiltersView.a7795492.css
+-rw-r--r--   0        0        0   121398 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/EditFiltersView.bc0dd7c3.js
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/EditFiltersYamlView.28a1a7c9.js
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/ListDatasetsView.0c61d7cc.js
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/ListDatasetsView.79aac80d.css
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/TagsEditor.23cf196f.js
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css
+-rw-r--r--   0        0        0    38943 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/data-cuate.84693c76.svg
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg
+-rw-r--r--   0        0        0    22166 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/eu.24cff2c1.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/hacks.1ae1ba64.js
+-rw-r--r--   0        0        0   101750 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/horizon-europe.80625b0c.png
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/index.47848488.css
+-rw-r--r--   0        0        0   124624 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/index.6cc31f0d.js
+-rw-r--r--   0        0        0    17440 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/vue-select.9ddbca8a.js
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/vue-select.b0fac2a1.css
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/.gitignore
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/README.md
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/PKG-INFO
```

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/AddDatasetView.4182f0f7.css` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/AddDatasetView.4182f0f7.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/AddDatasetView.ff526466.js` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/AddDatasetView.ff526466.js`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/EditFiltersView.a7795492.css` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/EditFiltersView.a7795492.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/EditFiltersView.bc0dd7c3.js` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/EditFiltersView.bc0dd7c3.js`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/ListDatasetsView.0c61d7cc.js` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/ListDatasetsView.0c61d7cc.js`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/ListDatasetsView.79aac80d.css` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/ListDatasetsView.79aac80d.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/TagsEditor.23cf196f.js` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/TagsEditor.23cf196f.js`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/data-cuate.84693c76.svg` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/data-cuate.84693c76.svg`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/eu.24cff2c1.png` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/eu.24cff2c1.png`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/horizon-europe.80625b0c.png` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/horizon-europe.80625b0c.png`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/index.47848488.css` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/index.47848488.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/index.6cc31f0d.js` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/index.6cc31f0d.js`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/vue-select.9ddbca8a.js` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/vue-select.9ddbca8a.js`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/frontend/assets/vue-select.b0fac2a1.css` & `opuscleaner-0.2.2/opuscleaner/frontend/assets/vue-select.b0fac2a1.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/categories.py` & `opuscleaner-0.2.2/opuscleaner/categories.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/clean.py` & `opuscleaner-0.2.2/opuscleaner/clean.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/col.py` & `opuscleaner-0.2.2/opuscleaner/col.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/config.py` & `opuscleaner-0.2.2/opuscleaner/config.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/datasets.py` & `opuscleaner-0.2.2/opuscleaner/datasets.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/download.py` & `opuscleaner-0.2.2/opuscleaner/download.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters.py` & `opuscleaner-0.2.2/opuscleaner/filters.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/opusfilter_compat.py` & `opuscleaner-0.2.2/opuscleaner/opusfilter_compat.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/sample.py` & `opuscleaner-0.2.2/opuscleaner/sample.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/server.py` & `opuscleaner-0.2.2/opuscleaner/server.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/threshold.py` & `opuscleaner-0.2.2/opuscleaner/threshold.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/alpha_ratio.json` & `opuscleaner-0.2.2/opuscleaner/filters/alpha_ratio.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/alpha_ratio.py` & `opuscleaner-0.2.2/opuscleaner/filters/alpha_ratio.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/bicleaner_hardrules.json` & `opuscleaner-0.2.2/opuscleaner/filters/bicleaner_hardrules.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/bifixer.json` & `opuscleaner-0.2.2/opuscleaner/filters/bifixer.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/clean_common.py` & `opuscleaner-0.2.2/opuscleaner/filters/clean_common.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/deescape-special-chars.perl` & `opuscleaner-0.2.2/opuscleaner/filters/deescape-special-chars.perl`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/detokenizer.json` & `opuscleaner-0.2.2/opuscleaner/filters/detokenizer.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/detokenizer.perl` & `opuscleaner-0.2.2/opuscleaner/filters/detokenizer.perl`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/fasttext_filter.json` & `opuscleaner-0.2.2/opuscleaner/filters/fasttext_filter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/fasttext_filter.py` & `opuscleaner-0.2.2/opuscleaner/filters/fasttext_filter.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/fix_elitr_eca.py` & `opuscleaner-0.2.2/opuscleaner/filters/fix_elitr_eca.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/fix_wiki.json` & `opuscleaner-0.2.2/opuscleaner/filters/fix_wiki.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/fix_wiki.py` & `opuscleaner-0.2.2/opuscleaner/filters/fix_wiki.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/langid.json` & `opuscleaner-0.2.2/opuscleaner/filters/langid.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/langid.py` & `opuscleaner-0.2.2/opuscleaner/filters/langid.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/laser_similarity.json` & `opuscleaner-0.2.2/opuscleaner/filters/laser_similarity.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/laser_similarity.py` & `opuscleaner-0.2.2/opuscleaner/filters/laser_similarity.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/max_length.py` & `opuscleaner-0.2.2/opuscleaner/filters/max_length.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/max_word_length.py` & `opuscleaner-0.2.2/opuscleaner/filters/max_word_length.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/num_mismatch.py` & `opuscleaner-0.2.2/opuscleaner/filters/num_mismatch.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/remove_frequent_patterns.py` & `opuscleaner-0.2.2/opuscleaner/filters/remove_frequent_patterns.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/segment_japanese.py` & `opuscleaner-0.2.2/opuscleaner/filters/segment_japanese.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/split_sentences.json` & `opuscleaner-0.2.2/opuscleaner/filters/split_sentences.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/split_sentences.py` & `opuscleaner-0.2.2/opuscleaner/filters/split_sentences.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/src_trg_ratio.py` & `opuscleaner-0.2.2/opuscleaner/filters/src_trg_ratio.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/strip_suffix.json` & `opuscleaner-0.2.2/opuscleaner/filters/strip_suffix.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/strip_suffix.py` & `opuscleaner-0.2.2/opuscleaner/filters/strip_suffix.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/opusfilter/AverageWordLengthFilter.json` & `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/AverageWordLengthFilter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/opusfilter/CharacterScoreFilter.json` & `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/CharacterScoreFilter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/opusfilter/Detokenizer.json` & `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/Detokenizer.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/opusfilter/LengthFilter.json` & `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/LengthFilter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/opusfilter/RegExpFilter.json` & `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/RegExpFilter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/opusfilter/RegExpSub.json` & `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/RegExpSub.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/opusfilter/Tokenizer.json` & `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/Tokenizer.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/opuscleaner/filters/opusfilter/opusfilter-ersatz.py` & `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/opusfilter-ersatz.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/README.md` & `opuscleaner-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2/pyproject.toml` & `opuscleaner-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 opuscleaner-server = "opuscleaner.server:main"
 opuscleaner-clean = "opuscleaner.clean:main"
 opuscleaner-col = "opuscleaner.col:main"
 opuscleaner-threshold = "opuscleaner.threshold:main"
 opuscleaner-sample = "opuscleaner.sample:main"
 
 [project.urls]
-Documentation = "https://github.com/unknown/opuscleaner#readme"
-Issues = "https://github.com/unknown/opuscleaner/issues"
-Source = "https://github.com/unknown/opuscleaner"
+Documentation = "https://github.com/hplt-project/opuscleaner#readme"
+Issues = "https://github.com/hplt-project/opuscleaner/issues"
+Source = "https://github.com/hplt-project/opuscleaner"
 
 [tool.hatch.version]
 path = "opuscleaner/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
@@ -53,27 +53,20 @@
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=opuscleaner --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311"]
 
 [tool.hatch.build]
-exclude = [
-  "/.github",
-  "/.gitignore",
-  "/frontend",
-  "/placeholders",
-  "/build_frontend.py"
-]
-artifacts = [
-  "/frontend/dist/*"
+include = [
+  "/opuscleaner",
 ]
 
-[tool.hatch.build.sources]
-"/frontend/dist" = "/opuscleaner/frontend"
+[tool.hatch.build.force-include]
+"frontend/dist" = "/opuscleaner/frontend"
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
 
 [tool.hatch.metadata.hooks.requirements_txt.optional-dependencies]
 all = ["requirements-all.txt"]
```

### Comparing `opuscleaner-0.2/PKG-INFO` & `opuscleaner-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: opuscleaner
-Version: 0.2
-Project-URL: Documentation, https://github.com/unknown/opuscleaner#readme
-Project-URL: Issues, https://github.com/unknown/opuscleaner/issues
-Project-URL: Source, https://github.com/unknown/opuscleaner
+Version: 0.2.2
+Project-URL: Documentation, https://github.com/hplt-project/opuscleaner#readme
+Project-URL: Issues, https://github.com/hplt-project/opuscleaner/issues
+Project-URL: Source, https://github.com/hplt-project/opuscleaner
 Author-email: Jelmer van der Linde <jelmer@ikhoefgeen.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

